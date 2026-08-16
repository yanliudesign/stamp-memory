<div align="center">

**中文** · [English](./README.md)

# Stamp Memory

---

**把主题、记忆、物件与照片，变成安静的民艺小印。**

[![Version](https://img.shields.io/badge/VERSION-1.0.0-2ea44f?style=flat-square&labelColor=333)](./SKILL.md)
[![Skills](https://img.shields.io/badge/SKILLS-1-2ea44f?style=flat-square&labelColor=333)](./SKILL.md)
[![Stars](https://img.shields.io/github/stars/yanliudesign/stamp-memory?style=flat-square&label=STARS&color=e37f2c&labelColor=333)](https://github.com/yanliudesign/stamp-memory/stargazers)

[![Claude Code](https://img.shields.io/badge/Claude_Code-Skill-d97757?style=flat-square&labelColor=1a1a1a&logo=anthropic&logoColor=white)](https://claude.ai/code)
[![SKILL.md](https://img.shields.io/badge/Agent-SKILL.md-214f9b?style=flat-square&labelColor=1a1a1a)](./SKILL.md)

</div>

输入一句话、一个物件、一段记忆，或者上传一张照片，生成一枚原创的小型印刷图章。Skill 会保留一个清楚可识别的主体，把它压缩成适合雕刻的线、块面与负形，再放进大面积暖纸留白中。

它延续的是一套视觉系统，而不是复制某张参考图：克制的炭黑、钴蓝、朱红与苔绿；略显朴拙的手刻边缘；紧凑而有人味的字体；以及私人纪念物般的沟通气质。

## 案例

<table>
  <tr>
    <td align="center" width="33%"><a href="./summer-night-walk.png"><img src="./summer-night-walk.png" width="100%" alt="夏夜散步印章"></a><br><sub>夏夜散步</sub></td>
    <td align="center" width="33%"><a href="./read-slowly-bookplate.png"><img src="./read-slowly-bookplate.png" width="100%" alt="慢慢读藏书票印章"></a><br><sub>慢慢读</sub></td>
    <td align="center" width="33%"><a href="./starting-again-sprout.png"><img src="./starting-again-sprout.png" width="100%" alt="重新开始嫩芽印章"></a><br><sub>重新开始</sub></td>
  </tr>
  <tr>
    <td align="center" width="33%"><a href="./grandmothers-garden.png"><img src="./grandmothers-garden.png" width="100%" alt="外婆花园浇水壶印章"></a><br><sub>外婆的花园</sub></td>
    <td align="center" width="33%"><img src="./examples-index.png" width="100%" alt="Stamp Memory 八个案例索引"></td>
    <td align="center" width="33%"><a href="./grazing-deer-memory.png"><img src="./grazing-deer-memory.png" width="100%" alt="照片转低头鹿印章"></a><br><sub>照片转印章</sub></td>
  </tr>
  <tr>
    <td align="center" width="33%"><a href="./rainy-window.png"><img src="./rainy-window.png" width="100%" alt="雨窗印章"></a><br><sub>雨窗</sub></td>
    <td align="center" width="33%"><a href="./pocket-orange.png"><img src="./pocket-orange.png" width="100%" alt="口袋橙子印章"></a><br><sub>口袋橙子</sub></td>
    <td align="center" width="33%"><a href="./seaside-found-objects-sheet.png"><img src="./seaside-found-objects-sheet.png" width="100%" alt="十二枚海边拾物印章页"></a><br><sub>海边拾物</sub></td>
  </tr>
</table>

## 它能做什么

| 系统 | 规则 |
|---|---|
| **输入** | 主题、短句、物件、记忆或用户上传的照片 |
| **主体** | 一个可识别的核心象征，最多两个辅助标记 |
| **配色** | 暖纸底 + 一种主墨色 + 不超过印刷面积 8% 的可选强调色 |
| **留白** | 画布的 65%–85% 保持为未印刷纸面 |
| **画法** | 朴拙刀刻轮廓、实心墨块、开放负形与克制的漏墨 |
| **字体** | 可选的紧凑手刻字；只使用用户提供的准确文字 |
| **输出** | 位图成品、实际使用的完整 Prompt 与简短视觉配方 |

## 工作方式

```text
1  读取主体与含义  →  找到一个意义和一个识别特征
2  选择印章外形    →  无边框、椭圆、软矩形或不规则石片形
3  压缩为可雕刻图  →  合并阴影、打开缝隙、删除脆弱细节
4  应用固定视觉 DNA →  暖纸、克制墨色、大面积留白
5  生成并检查      →  核对身份、缩略图识别度与原创性
```

### 语言生成印章

直接用自然语言描述主题。抽象概念会被转化成一个具体象征，而不是堆成拥挤的完整场景。

```text
做一枚关于“重新开始”的朱红色民艺印章，不要文字。
```

### 照片转印章

上传人物、宠物、植物、地点或物件照片。Skill 会保留关键识别特征、姿态与结构，再把图像重建为适合印刷的线、块面和负形。它不会只套一个阈值滤镜，也不会照搬照片构图。

```text
把这张我和猫的照片变成一枚安静的钴蓝色藏书票印章。
```

## 视觉规则

1. **纸张是主角。** 暖象牙、粉笔白或浅燕麦色占据主要画面。
2. **一种主墨色。** 炭黑、钴蓝、朱红或苔绿承担主体；第二种颜色不超过印刷标记的 8%。
3. **留白参与构图。** 默认单枚印章只占画布面积的 18%–34%。
4. **雕刻逻辑优先。** 图形缩小到约 25–45 mm 的实体印章尺寸后仍应清楚。
5. **身份特征不丢失。** 人物、宠物和物件照片保留其决定性特征。
6. **文字保持从属。** 不虚构品牌、日期、机构、签名或装饰性伪文字。
7. **参考图只提供语法。** 每次输出都必须与任一风格参考至少有五项结构差异。

## 它不是什么

- 不是企业 Logo、App 图标、徽章或贴纸合集
- 不是光亮蜡封、浮雕样机或产品摄影
- 不是光滑矢量图，也不是一键自动描摹
- 不是伪造的古代书法、纹章或机构身份
- 不是对任何参考作品的重绘或复刻

## 安装

将仓库克隆到 Claude Code 的 skills 目录：

```bash
git clone https://github.com/yanliudesign/stamp-memory.git \
  ~/.claude/skills/stamp-memory
```

安装后重启 Claude Code。其他 Agent 环境也可以把 [`SKILL.md`](./SKILL.md) 作为 skill 入口文件加载。

## 试试看

```text
做一枚关于夏夜散步的印章。
```

```text
做一枚纪念外婆花园的苔绿色小印。
```

```text
做一枚写着“慢慢读”的藏书票印章，里面有一本打开的小书。
```

```text
把这张花朵照片简化成朱红色手刻章，不要文字。
```

```text
做一页 12 枚关于海边散步拾到的小物件印章，大小不要完全一致。
```

## 输出格式

每次运行返回：

1. 一张生成的位图成品；
2. 实际用于生成的完整可复用 Prompt；
3. 一份简短配方，说明墨色、外形、刀刻处理、文字处理与原创性变化。

如果当前环境不具备图片生成能力，Skill 会返回可直接用于图片模型的完整 Prompt，并明确说明限制，而不会假装已经生成图片。

## 仓库结构

```text
stamp-memory/
├── SKILL.md                 # 触发规则、工作流、视觉 DNA 与质量检查
├── README.md                # English documentation
├── README.zh.md             # 中文说明
├── examples-index.png       # 3×3 案例九宫格的中心索引卡
└── *.png / *.svg            # 八个位图案例与对应的可编辑母版
```

## 原创性

这个 Skill 只提取配色、材质、密度、线条行为和情绪温度等系统级特征。它不会复制参考印章的主体处理、边框、内部刀痕、文字、字形或物件排列。

当用户上传自己的照片时，身份特征会作为内容得到保留；裁切、抽象方式、边框、刀刻节奏和文字位置仍会重新设计。

---

Created by [Dreameryanyan](https://www.linkedin.com/in/yanliudesign/) · [LinkedIn](https://www.linkedin.com/in/yanliudesign/) · [X](https://x.com/yanliudreamer)