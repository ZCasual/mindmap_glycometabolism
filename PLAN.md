# 1. 图嵌入
IN: HIC 矩阵 C -> OUT: 特征矩阵 U

### 1. 邻接图构建
Init：
$$
A_{ij,kl} = \log(1 + C_{ij} + C_{kl}) \quad \text{若像素 } (i,j) \text{ 与 } (k,l) \text{ 相邻}
$$

对称归一化：  
     \[
     \tilde{A} = D^{-1/2} A D^{-1/2}, \quad D_{ij} = \sum_{kl} A_{ij,kl}
     \]

 ### 2. GCN 卷积

$$
 H^{(1)} = \text{ReLU}\left(\tilde{D}^{-\frac{1}{2}} \tilde{A} \tilde{D}^{-\frac{1}{2}} X W^{(0)}\right)
$$

$$
 H^{(2)} = 
$$
$$
\begin{aligned}
\mathcal{L} &:= \tilde{D}^{-\frac{1}{2}} \tilde{A} \tilde{D}^{-\frac{1}{2}} \\
H^{(1)} &= \text{ReLU}\left( \mathcal{L} X W^{(0)} \right) \\
H^{(l)} &= \text{ReLU}\left( \mathcal{L} H^{(l-1)} W^{(l-1)} \right), \quad l = 2,3,4,5
\end{aligned}
$$

 4. ExCB 动态聚类

$$
\begin{aligned}
\mathring{H}^{(1)} &= \text{ReLU}(\mathcal{L} X W^{(0)}) \\
H^{(1)}_{\text{out}} &= \mathring{H}^{(1)} \quad \text{(首层不融合)} \\
\mathring{H}^{(2)} &= \text{ReLU}(\mathcal{L} H^{(1)}_{\text{out}} W^{(1)}) \\
H^{(2)}_{\text{out}} &= \text{BU-TD Fusion}(\mathring{H}^{(2)}, H^{(3)}_{bu}, H^{(1)}_{td}) \\
&\vdots \\
\mathring{H}^{(5)} &= \text{ReLU}(\mathcal{L} H^{(4)}_{\text{out}} W^{(4)}) \\
H^{(5)}_{\text{out}} &= \text{BU-TD Fusion}(\mathring{H}^{(5)}, \emptyset, H^{(4)}_{td}) \quad \text{(顶层无BU输入)}
\end{aligned}
$$

---
$$
\begin{aligned}
\mathring{H}^{(1)} &= \text{ReLU}(\tilde{A} X W^{(0)}) \\
H^{(1)}_{\text{out}} &= \mathring{H}^{(1)} \quad \text{(首层不融合)} \\
\mathring{H}^{(2)} &= \text{ReLU}(\tilde{A} H^{(1)}_{\text{out}} W^{(1)}) \\
H^{(2)}_{\text{out}} &= \text{BU-TD Fusion}(\mathring{H}^{(2)}, H^{(3)}_{bu}, H^{(1)}_{td}) \\
\mathring{H}^{(3)} &= \text{ReLU}(\tilde{A} H^{(2)}_{\text{out}} W^{(2)}) \\
H^{(3)}_{\text{out}} &= \text{BU-TD Fusion}(\mathring{H}^{(3)}, H^{(4)}_{bu}, H^{(2)}_{td}) \\
\mathring{H}^{(4)} &= \text{ReLU}(\tilde{A} H^{(3)}_{\text{out}} W^{(3)}) \\
H^{(4)}_{\text{out}} &= \text{BU-TD Fusion}(\mathring{H}^{(4)}, H^{(5)}_{bu}, H^{(3)}_{td}) \\
\mathring{H}^{(5)} &= \text{ReLU}(\tilde{A} H^{(4)}_{\text{out}} W^{(4)}) \\
H^{(5)}_{\text{out}} &= \text{BU-TD Fusion}(\mathring{H}^{(5)}, \emptyset, H^{(4)}_{td}) \quad \text{(顶层无BU输入)}
\end{aligned}
$$