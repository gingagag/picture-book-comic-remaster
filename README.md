# 绘本分镜重绘与竖版漫画排版技能

这个 Codex 技能可将一张拍摄或扫描的多格儿童绘本页，处理为逐格无文字重绘图、黑字优化拼页，以及竖版漫画长图。它保留原故事的角色、色彩和情节，并按规则检查手指、头发、文字和气泡排版。

## 安装

在 Codex 中提供本仓库地址，并说：

> 请从 https://github.com/gingagag/picture-book-comic-remaster 安装 `picture-book-comic-remaster` 技能。

也可以手动安装。先确认电脑已安装 Git，然后运行适合当前系统的命令：

Windows PowerShell：

```powershell
git clone https://github.com/gingagag/picture-book-comic-remaster.git "$env:USERPROFILE\.codex\skills\picture-book-comic-remaster"
```

macOS / Linux：

```bash
git clone https://github.com/gingagag/picture-book-comic-remaster.git "$HOME/.codex/skills/picture-book-comic-remaster"
```

安装后重新打开 Codex，或开始一个新任务，让它重新载入技能列表。如果目标目录已经存在，请先检查现有版本，不要直接覆盖其中的修改。

## 使用

上传一张绘本页面图片，然后说：

> 使用 `$picture-book-comic-remaster` 处理这张图片，生成黑字优化拼页和竖版漫画长图。

技能会逐格分析与重绘，优先使用修正后的无文字分镜，再分别制作两种排版。最终图片会保存在当前任务的工作目录中。图像生成质量、可用字体和输出路径取决于使用者的 Codex 环境。

## 文件

- [`SKILL.md`](SKILL.md)：完整执行流程。
- [`references/redraw-prompts.md`](references/redraw-prompts.md)：逐格重绘及局部修正规范。
- [`references/composition-spec.md`](references/composition-spec.md)：拼页、竖版长图、字体与气泡规范。
- [`agents/openai.yaml`](agents/openai.yaml)：技能在 Codex 中的显示和调用配置。
