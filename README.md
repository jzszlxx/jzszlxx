<div align="center">

<img src="./banner.svg" alt="昱满天下 · jzszlxx" width="100%" />

</div>

### 你好，我是昱满天下

一个喜欢把想法做成**能双击运行的东西**的人。写桌面应用，也折腾 AI Agent——不太喜欢让东西停在文档和演示里。

现在主要在写 **C# / WinForms** 的桌面程序，用 **Python** 做脚本和数据处理，偶尔碰一点 TypeScript。

<br />

<img src="./tech.svg" alt="技术栈" width="100%" />

<br />

### 在做的项目

| 项目 | 是什么 | 状态 |
| --- | --- | :---: |
| **[FlatCat](https://github.com/jzszlxx/-)** | 2D 扁平桌面宠物：透明置顶、点击穿透、全局键鼠响应、摸头呼噜；番茄钟 / 喝水 / 倒计时 / 多组闹钟（按星期、贪睡、三种铃声）；四页设置窗口。C# + WinForms，单文件 exe 约 190 KB，MIT | `v1.3.0` 已发布 |

FlatCat 的几个技术点，做桌面端的朋友可能用得上：

- **透明窗口**用 `UpdateLayeredWindow` + 32bpp 预乘 ARGB，而不是 `TransparencyKey`——后者不支持半透明抗锯齿
- **点击穿透**靠每帧按渲染 alpha 生成命中掩码，光标落在猫身才摘掉 `WS_EX_TRANSPARENT`
- **全局键盘响应**用 `WH_KEYBOARD_LL` 装在专用线程，只读虚拟键码，不记录字符、不落盘、不联网
- **闹钟不重复响**用「年月日时分 + 时间 + 标签」做指纹，星期重复用位掩码 `bit0=周一 … bit6=周日`

<br />

### 几条我自己信的东西

- 工具要能上手用，才算真的做完
- 先让它跑起来，再让它好看
- 能算清楚的钱和能复现的结论，都别只凭感觉

<br />

### 联系我

|  |
| --- |
| 公众号 **认知觉醒能量站** —— 写工具、AI 用法和投资复盘 |
| 邮箱 **jzszlxx@163.com** |
| 仓库 [github.com/jzszlxx](https://github.com/jzszlxx) |

<br />

<div align="center">
<sub>把复杂的事做简单，把简单的事做扎实。</sub>
</div>