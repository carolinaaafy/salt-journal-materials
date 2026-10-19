# 盐系手帐素材 · Salt Journal Materials

一个用于生成**盐系手帐素材页**与**拼贴灵感参考**的 Codex Skill。

给它一段日常、一种心情或一个配色，它会先整理成可裁切的素材纸、便签、纸条与小装饰；需要时，再继续用同一套素材制作拼贴示范。

## 效果示例

### 雾霾蓝 · after work

<table>
  <tr>
    <td width="50%" align="center"><strong>素材页</strong></td>
    <td width="50%" align="center"><strong>拼贴灵感</strong></td>
  </tr>
  <tr>
    <td><img src="examples/fog-blue-materials.png" alt="雾霾蓝 after work 盐系手帐素材页"></td>
    <td><img src="examples/fog-blue-collage.png" alt="雾霾蓝 after work 拼贴灵感"></td>
  </tr>
</table>

### 秋日桂花 · cool air

<table>
  <tr>
    <td width="50%" align="center"><strong>素材页</strong></td>
    <td width="50%" align="center"><strong>拼贴灵感</strong></td>
  </tr>
  <tr>
    <td><img src="examples/autumn-osmanthus-materials.png" alt="秋日桂花盐系手帐素材页"></td>
    <td><img src="examples/autumn-osmanthus-collage.png" alt="秋日桂花拼贴灵感"></td>
  </tr>
</table>

## 它会做什么

- 从日记片段中提炼主题和情绪，不逐句图解。
- 生成协调的素材纸、书写便签、胶带、标签与小装饰。
- 根据情绪主动选择约三种主色，并控制主色、支持色与跳色的比例。
- 使用淡淡的纸张纹理、笨拙自然的平涂手绘和少量晕染。
- 优先采用花枝、星点、波浪、蝴蝶结等装饰性意象，避免把事件机械翻译成鞋子、背包等具体物品。
- 在用户需要时，继续生成一组、两组或三组拼贴灵感，并处理遮挡、留白和书写区层级。

## 视觉特点

- **浅而不灰**：颜色柔和，但仍保留足够辨识度。
- **少量主色**：通常由一个主导色、一至两个支持色组成，小装饰可以跳色。
- **自然手绘**：线条和色块允许轻微不规整，避免漫画式粗描边。
- **留白参与构图**：留白会进入拼贴内部，而不只是剩在页面四周。
- **平贴关系**：拼贴通过遮挡表达层次，默认不使用投影、悬浮、翘边和厚重立体感。
- **书写优先**：书写区保持中等尺度，可用一主一辅两个区域，不让大便签吞掉全部素材。

## 安装

将仓库克隆到 Codex 的 skills 目录：

```bash
git clone https://github.com/carolinaaafy/salt-journal-materials.git ~/.codex/skills/salt-journal-materials
```

也可以下载仓库压缩包，再把整个文件夹放入：

```text
~/.codex/skills/salt-journal-materials
```

重新打开 Codex 对话后即可使用 `$salt-journal-materials`。

## 使用示例

只给主题也可以：

```text
使用 $salt-journal-materials 帮我做一组手帐素材：
秋天到了，天气变冷了，空气里都是桂花香。
```

指定情绪和配色：

```text
使用 $salt-journal-materials 生成手帐素材：
周一心情有点低落，晚上准备去健身。
想用雾霾蓝、淡紫和奶油白。
```

继续制作拼贴：

```text
用刚才那套素材做一张拼贴灵感。
关系简单一些，但整体需要撑住画面，纸张要有自然遮挡。
```

## 工作方式

1. 先根据主题生成一张可裁切的素材页。
2. 保留原素材、配色与尺寸关系。
3. 用户需要时，再生成拼贴灵感参考。
4. 拼贴会根据素材决定一组、两组或三组构图，不固定套用同一种模板。

## 仓库结构

```text
salt-journal-materials/
├── SKILL.md
├── agents/
│   └── openai.yaml
├── references/
│   ├── material-design.md
│   ├── collage.md
│   └── ...
└── examples/
    ├── fog-blue-materials.png
    ├── fog-blue-collage.png
    ├── autumn-osmanthus-materials.png
    └── autumn-osmanthus-collage.png
```

## 说明

- 拼贴图是构图概念参考，不是经过毫米级校准的打印模板。
- 素材页默认保留直边；撕边通常在拼贴阶段表现。
- 参考图片用于学习颜色、画法和构图关系，不复制其中的文字、水印或品牌元素。

