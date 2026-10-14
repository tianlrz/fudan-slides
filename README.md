# Fudan Slides · 复旦学术汇报

复旦风格的学术演示稿 Skill，适用于开题、组会、文献汇报和答辩。保留用户 Claude Design 模板的主要版式，以一个 HTML 和必要 logo 为核心。

[在线查看 12 种版式](https://tianlrz.github.io/fudan-slides/)

## 用法

将本目录复制到个人 skills 目录，文件夹名保持 `fudan-slides`。

例如，安装到 Codex 的默认个人技能目录：

```sh
git clone https://github.com/tianlrz/fudan-slides.git "$HOME/.codex/skills/fudan-slides"
```

已存在同名目录时先确认其中内容，再选择更新或换位置安装。

> 用 $fudan-slides，根据这份研究方案制作 5—8 分钟的开题汇报。

> 用 $fudan-slides，根据这份材料生成 HTML 演示稿，带独立演讲稿窗口，并保存为 PDF。

打开 `assets/reference.html` 查看版式。此文件只包含可替换的标题和内容位置，不含虚构实验结果。方向键翻页，S 或 Presenter 按钮打开独立讲稿窗口，主窗口与讲稿窗口可双向同步翻页，讲稿窗口同时显示页码和计时。浏览器拦截时需允许本地页面弹窗。

## 文件

- `SKILL.md`：生成 prompt、版式与素材说明。
- `assets/reference.html`：12 种代表性版式，样式与交互内嵌。包括封面、目录、章节过渡、研究问题、技术路线、图文分析、方法对照、结果表格、工作计划、总结局限、参考资料和致谢。
- `assets/logo-blue.png`：用户原设计包提供的蓝色校徽校名组合。
- `assets/logo-white.png`：从复旦大学官网获取的反白原件。

标识规范：[复旦大学标识系统](https://www.fudan.edu.cn/bsxt/)。反白原件：[官网资源](https://www.fudan.edu.cn/_upload/site/00/02/2/logo.png)。两份 logo 保持原比例与色彩，用于浅色/深色背景，具体使用遵循学校规范。校徽与校名等标识权益属于相应权利人，公开此项目不意味着为这些标识授予额外许可。

紫色来自用户提供的 Claude Design 参考，是本模板的设计选择；不代表学校官方标准色。本项目是个人模板整理，不是复旦大学官方发布。

## 格式

HTML 模板在本地浏览器运行，不依赖外部字体或脚本，默认不制作 PPTX。浏览器打印选择“另存为 PDF”，一张幻灯片对应一页；开启背景图形以保留色带。演示运行时复用用户原 ZIP 的 `deck-stage.js` 并内嵌在 HTML 中，不增加独立脚本文件。

讲稿同步已补充消息去重，避免在线演示时多个通信通道导致一次操作重复跳页。

导航已移除模糊过渡，画布在支持的浏览器中使用布局缩放并保留兼容回退。页面和元素带有稳定标识及内容角色，方便 AI 定位局部修改、识别相似页；当前仍为演示模板，未加入拖拽编辑或自动跨页改写界面。
