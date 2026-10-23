# 把照片请上皮影戏台

将照片中的人物、动物、建筑、植物、器物或风景，转译为中国传统彩色皮影海报的 Codex Skill。

默认版式为 **3:4 竖版，上半原照、下半皮影，各占 50%**。皮影保留原主体的轮廓、姿态与叙事关系，采用半透明彩染、镂空雕刻、操纵竹签、米黄或浅琥珀暖光幕布及大量留白。

## 使用

将本仓库克隆到本机 Codex 的 Skills 目录：

```bash
git clone https://github.com/GUOCHENN/photo-shadow-puppet.git ~/.codex/skills/photo-shadow-puppet
```

Windows PowerShell：

```powershell
git clone https://github.com/GUOCHENN/photo-shadow-puppet.git "$env:USERPROFILE\.codex\skills\photo-shadow-puppet"
```

也可以点击 **Code → Download ZIP**，解压后把包含 `SKILL.md` 的文件夹命名为 `photo-shadow-puppet`，放入 `~/.codex/skills/`。若同名目录已经存在，先保留自己的修改。

上传需要处理的照片后输入：

```text
使用 $photo-shadow-puppet，把这张照片做成皮影海报。
```

也可以指定只输出皮影部分、无字、横版或只提供提示词。

## 内容

- `SKILL.md`：执行流程、视觉规则、工具使用和成品检查。
- `agents/openai.yaml`：Skill 的显示名称和默认调用提示。
- `references/original-prompt-zh.md`：两页原始提示词的人工转录。
- `references/visual-guide.md`：参考图索引、读图要点和附件说明。
- `references/images/`：用户提供的 7 张完整参考截图。

参考截图是教学与风格资料；使用时仍需提供自己的待处理照片。内置图像工具可用时生成图像，仅需要提示词时可直接输出提示词。

## 许可

本仓库新编写的 `SKILL.md`、`agents/openai.yaml` 与本使用说明采用 [MIT 许可](LICENSE)，允许使用、修改和分享。用户提供的参考截图和截图提示词转录不在此许可范围内，其权利归原权利人所有。
