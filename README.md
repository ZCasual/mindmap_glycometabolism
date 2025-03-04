# 糖代谢路径图

## 简介

**代谢路径图** 是一个基于 D3.js 构建的交互式可视化工具，用于展示和探索各种关键的代谢途径，包括糖酵解途径（EMP）、磷酸戊糖途径（PPP）、三羧酸循环（TCA）、糖原合成（GS）、糖异生（GNG）、乙醛酸循环（GC）等。该工具旨在帮助学生、研究人员和生物学爱好者更直观地理解复杂的代谢网络及其相互关系。

## 功能

- **多通路支持**：展示多个关键代谢途径，并支持在不同通路之间进行切换和比较。
- **交互操作**：
  - **缩放和平移**：通过鼠标滚轮缩放视图，拖动图表进行平移。
  - **节点拖拽**：点击并拖动节点以重新布局图表。
  - **路径点击**：点击主要通路节点（如 EMP、TCA 等）以高亮显示相关代谢反应和酶。
- **信息面板**：点击通路节点后，右侧信息面板将显示详细的途径说明、关键酶、能量计算及其生理意义。
- **控制面板**：
  - **路径选择**：通过控制按钮快速切换不同的代谢通路显示。
  - **高亮选项**：启用单向箭头高亮和高能分子高亮，以突出显示关键反应。
  - **参数调节**：调整力导向图的聚拢程度和连线长度，以优化视图布局。
  - **左侧面板收起/展开**：通过按钮控制左侧控制面板的显示与隐藏，保持界面整洁。

## 使用方法

1. **克隆仓库**：
    ```bash
    git clone https://github.com/ZCasual/mindmap_glycometabolism.git
    ```

2. **打开 `index.html`**：
直接在浏览器中打开 `index.html` 文件，即可访问代谢路径图。

3. **打开 `index.html`**：
点击下方按钮聚焦对应板块知识，点击思维导图中的中文节点可以恢复全局视野（英文节点为主节点，效果视同按钮）。

![样例-TCA循环](https://gitee.com/casual_pleat/mindmap_glycometabolism/raw/master/test.png "样例-TCA循环")

