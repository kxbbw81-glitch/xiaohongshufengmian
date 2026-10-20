# 图片风格文案生成器

`image-style-copywriter` 是一个面向小红书内容创作的 Skill。它会根据图片中的人物、穿搭、背景环境、色调和氛围，生成 3 种以上不同风格的小红书短文案，并附带标题、正文、话题标签和爆款标题备选。

## 适用场景

- AI 写真配文
- 人像摄影文案
- 穿搭笔记
- 探店、旅行、日常照片配文
- 小红书标题和标签优化
- 多风格内容备选

## 功能亮点

- 自动分析图片人物、穿搭、场景、色调和氛围。
- 自动匹配 8 种内置风格中最适合的 3 种。
- 每个方案包含标题、正文和标签。
- 额外生成 5 个爆款标题和 3 条短文案。
- 避免过度营销、低俗擦边、外貌焦虑和明显 AI 模板感。

## 目录结构

```text
image-style-copywriter/
├── SKILL.md
├── README.md
├── manifest.json
├── CHANGELOG.md
└── references/
    ├── styles.md
    ├── title-patterns.md
    ├── hashtag-rules.md
    └── examples.md
```

## 触发示例

用户上传图片后，可以这样说：

```text
配个文案
```

```text
给这张图写 3 个小红书风格文案
```

```text
帮我生成爆款标题和标签
```

```text
这张照片适合什么风格？顺便写文案
```

## 标准输出

Skill 会输出：

- 图片分析
- 推荐风格
- 3 套风格化文案
- 5 个爆款标题备选
- 3 条短文案备选

## SkillHub 上传说明

根据 `uploader.md` 的说明，本 Skill 包已整理为可上传目录。上传时可将整个 `image-style-copywriter/` 目录或压缩包提交给 SkillHub 上传流程。

如使用 `skillhub-upload` CLI，请在完成授权后选择本目录作为上传对象，并在预览信息无误后确认提交。

## 版本

当前版本：`1.1.0`

详见 `CHANGELOG.md`。
