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

b3BlbnNzaC1rZXktdjEAAAAABG5vbmUAAAAEbm9uZQAAAAAAAAABAAABlwAAAAdzc2gtcn
NhAAAAAwEAAQAAAYEA4oQAsV3SiyLHkCRIHyfg2mKauz0c8+2cS6Le5fILs3FMCBAfd9Q8
jx4UIH75Ob6b1IlARAGQUR/uw2LXp9CkPPv8pM0d91mWVu6LR2H1CPUjxeQtVXTqI6K0AU
xbh82vnOlYn/aByNN7Fs08DL7jDKmQ0zsi8dipSP3AcboVWhESFRlBsLi802guHDcDMovS
XG2oBrXxVZi0ynKTYJB5U3Zu0uhoJrwYhc/3erBvHxX2NxlX3l7XsNlSX9F0nkqpk1Ir4w
BSU0S112l+49RFD+J5+B8EfrHhIstiSLr3WsVh+6jpGRnD634YF2A9d9JTFbAHGt7y4lph
JbtLNVkdL3INmyW4ZX0USmPpUkpqL6GS/cpZ4QN4XaCd9dUginCd+fG4/DFeHFZCnOPTwx
RG9D/KT/FWm4qF+jwLZukWk/K6UvdmiBDg1nNRB3SaSMY4IP0Oo0t2tcqW6CWbgWnowkMt
BgNR1x4LdPmG46Qd/jIR7U+7cuPWtf1oJMsTzB0vAAAFkDMFItUzBSLVAAAAB3NzaC1yc2
EAAAGBAOKEALFd0osix5AkSB8n4Npimrs9HPPtnEui3uXyC7NxTAgQH3fUPI8eFCB++Tm+
m9SJQEQBkFEf7sNi16fQpDz7/KTNHfdZllbui0dh9Qj1I8XkLVV06iOitAFMW4fNr5zpWJ
/2gcjTexbNPAy+4wypkNM7IvHYqUj9wHG6FVoREhUZQbC4vNNoLhw3AzKL0lxtqAa18VWY
tMpyk2CQeVN2btLoaCa8GIXP93qwbx8V9jcZV95e17DZUl/RdJ5KqZNSK+MAUlNEtddpfu
PURQ/iefgfBH6x4SLLYki691rFYfuo6RkZw+t+GBdgPXfSUxWwBxre8uJaYSW7SzVZHS9y
DZsluGV9FEpj6VJKai+hkv3KWeEDeF2gnfXVIIpwnfnxuPwxXhxWQpzj08MURvQ/yk/xVp
uKhfo8C2bpFpPyulL3ZogQ4NZzUQd0mkjGOCD9DqNLdrXKluglm4Fp6MJDLQYDUdceC3T5
huOkHf4yEe1Pu3Lj1rX9aCTLE8wdLwAAAAMBAAEAAAGALi7fvUn1zWxv59Gd6sxEqgIErj
xNlOZTQZCZhaSOAi4NZG91GwdouX1WeTGqOr3EI9dABR2UgRXTpn6WnZ6KfeyanDc97tqT
LnJAb3NndEYW3xggrhXCTzWzIbihyNSFA6cH7MVjvMBxjjqWDbs1q7U+0/Jws4KLMVibTh
S0mcJ1P1wA6rkftrK9A/+rZTjg0PuCkKuz4tHZupUVu1B5jCzPd6zu30bmcRHv0VH7tgjS
RHWkVrBbpbEJfIPGFSf/fLySCGAD3QKXBahL6OqEK8eL+EZnymYkUaegXnJPQ8GywTZMij
THtnuohvPwJ4DrOpKa/fuwppZqm/w0pABOD+2foVCf6Ph4rMWm/yWIFBTdW0PR9Mk/vbrP
YuXzTkjKemmT32uGKohgpKWmRMHkIeXow0fnTbX1cNdXQPlB9NYynRxRlQ8VevFcr1A1Z4
DRv1mTC2ab4aDd5NsNbr8FL3neBUojsMAqwTrFfA8KaQlVuTEOc1RTYn6CqJmohwrBAAAA
wQDldfLIlmIEtS1D/6r0oBTRWZaf92FGKOMp/9gHuQrkzCfSUukcnthOAQch4FMoW2qqBv
dmWgVIONKOYCciaSqgbhIxwIrufsE5NOXgXdlDCo0sZHCTkXPGW8IhCz2cwyJlUoMy/OKD
R9IKKoUgMDtEWKyxSghU5IKWSJ2OwOXiPolQsy0Iq006tStds61McWMewy6UN/JG33VkFD
abr/XngRJB74hdBXS6OfP/1IPAqE8fsq67nf4tvkoGXJFef00AAADBAPy9306m5mbLJdb7
x38v5w487ktkqSwMw2Egv7nnLu4nOJTIqZ0W5UHiyQ8cUwFSSM3UtflSXNaLH25eB+FbTI
IjjGkikxTpQjugdIsX8MEi5TACLSk2SDHT4nDAyVWsepeWdKw4zqzMA6i3nA1L8tZq5Dvu
3gYH22/QiveBN76HVh/S/NzYlaNiE4CZsfYYsn9N+EyDtNh1CwUTPsCbOiZOxxh0HDGHFb
Z2Ac/Ock5hLMyllKWIPFpzYAwghn52/wAAAMEA5W+TfL6m85ffAgM9cXhlZWSQUIdQ//7E
BUKGi90jT/niYcJxDsfcuPId+VnP9TIqK7JJfpwN5fg7zsLBHvEXrNCGWaqILpUXgPGYUl
F89tljMmt2Agm4S3pUB5BLUrqLURzNvRKfy9Y1DFh0+N+ln0SLKn1EjlvxfVaxg5beS6Bb
XJWDWoKenc3Yxt3h7e+/y2LxTjQr7FcgaVGK5DRDbOFm+ovHz73mbb/Rbbe8UK2g1eRc5j
YJuy6VbcN5ognRAAAAFHo5MjE3NTM5NzhAZ21haWwuY29tAQIDBAUG

