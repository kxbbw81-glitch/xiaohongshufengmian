---
name: image-style-copywriter
description: Generate Xiaohongshu-ready Chinese copy from portrait, outfit, lifestyle, or AI-generated images. Use when the user uploads or references an image and asks for captions, 小红书文案, 配文, 爆款标题, tags, outfit notes, portrait mood copy, or multiple style options; analyze the visible person, outfit, scene, color, light, and atmosphere, then produce differentiated title, body, hashtag, and short-caption combinations.
---

# Image Style Copywriter

根据图片中的人物肖像、穿搭、场景和视觉氛围，生成适合小红书发布的多风格短文案。优先输出自然、有画面感、可直接发布的中文内容，避免空泛夸张和明显 AI 味。

## Core Workflow

1. **Analyze the image**
   - 人物：年龄视觉感、气质、表情、姿态、妆发、穿搭重点。
   - 场景：室内/街拍/咖啡馆/自然环境/旅行/通勤/居家等。
   - 视觉：色调、光线、构图、镜头距离、画面质感。
   - 氛围：清冷、温柔、松弛、复古、甜美、酷飒、高级、治愈等。

2. **Match 3 differentiated styles**
   - 从 `references/styles.md` 的 8 种风格中选出最贴合图片的 3 种。
   - 三种风格必须有明显差异，避免只是同义改写。
   - 如果图片信息不足，基于可见元素生成，并明确说明“未见到的细节不做虚构”。

3. **Generate Xiaohongshu copy**
   - 每种风格输出：标题、正文、标签。
   - 正文控制在 60-140 中文字，适合手机端阅读。
   - 标签组合遵循 `references/hashtag-rules.md`。
   - 标题策略参考 `references/title-patterns.md`。

4. **Add viral-ready extras**
   - 额外输出 5 个可替换标题。
   - 额外输出 3 条短文案，适合直接配图发布。

## Output Format

```markdown
## 图片分析

人物/穿搭：
...

场景/光线：
...

整体氛围：
...

推荐风格：
1. ...
2. ...
3. ...

---

## 方案一：<风格名>

**标题：**
...

**正文：**
...

**标签：**
#... #... #...

---

## 方案二：<风格名>

**标题：**
...

**正文：**
...

**标签：**
#... #... #...

---

## 方案三：<风格名>

**标题：**
...

**正文：**
...

**标签：**
#... #... #...

---

## 爆款标题备选

1. ...
2. ...
3. ...
4. ...
5. ...

## 短文案备选

1. ...
2. ...
3. ...
```

## Style Reference

Read `references/styles.md` when choosing style directions or matching vocabulary.

Read `references/title-patterns.md` when the user asks for more titles, stronger click appeal, or "爆款标题".

Read `references/hashtag-rules.md` when refining tags or when the image spans multiple scenes.

Read `references/examples.md` when a complete output example is useful.

## Writing Rules

- 使用简体中文。
- 文案要像真实小红书用户写的内容，不要像广告稿、新闻稿或商品详情页。
- 优先写氛围、摄影语言、生活方式、穿搭感受和情绪价值。
- 不虚构身份、地点、品牌、价格、职业、关系、经历。
- 不对真人做敏感属性判断。
- 不使用低俗擦边、外貌羞辱、年龄焦虑、身材羞辱或过度性化表达。
- 少用“绝绝子”“天花板”“封神”“人间尤物”“顶级美女”等低质夸张词。
- 标签保持相关，不堆无关热词。

## Quality Checklist

Before finalizing, confirm:

- 3 种风格确实不同。
- 标题和正文能独立发布。
- 标签覆盖流量、场景、风格和内容定位。
- 没有编造图片中看不到的信息。
- 语气自然，读起来不像模板替换。
