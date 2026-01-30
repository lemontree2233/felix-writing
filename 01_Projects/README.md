# Projects 文件夹结构说明

本文件夹包含所有内容创作项目的素材、配方和输出。

---

## 📁 文件夹结构

```
01_Projects/
├── blog_sample/              # 📝 已发布的博客文章存档
├── blog_skill/               # 📚 Blog 写作技能素材库
│   ├── 00_原始素材库/          # Felix 的个人背景、经历、观点
│   ├── 01_爆款公式/            # 爆款公式分析（博客爆款公式分析.md）
│   ├── 02_核心配方生成/        # 写作结构模板、论证框架
│   └── 03_素材库/              # 案例库、数据库、引用库
├── x_skill/                  # 🐦 X (Twitter) 写作技能素材库
│   ├── 00_原始素材库/
│   ├── 01_爆款公式/
│   ├── 02_核心配方生成/
│   └── 03_素材库/
└── xhs_skill/                # 📱 小红书写作技能素材库
    ├── 00_原始素材库/
    ├── 01_爆款公式/
    ├── 02_核心配方生成/
    └── 03_素材库/
```

---

## 📋 各文件夹用途

### `blog_sample/` - 博客存档
**用途**: 保存所有已发布的英文博客文章

**当前文章** (6 篇):
- How to Manage a Company When the CEO Disappears - Culture Does
- How to beat AI at its own game (the rise of the "Human Glitch" and the end of the perfect brand）
- Mini Games: AI's Testing Ground for Mass Game Production
- Selling AI in 2025 - What I've Gotten Wrong
- The Enterprise AI Sweet Spot - Unlocking 80% of Untapped Efficiency
- Work, Leisure, and the Paradox of Innovation

**命名规范**: 使用完整英文标题作为文件名

---

### `blog_skill/` - Blog 写作技能库

#### `00_原始素材库/`
- 个人背景.md - Felix 的个人经历、价值观、观点库
- 其他个人素材

#### `01_爆款公式/`
- **博客爆款公式分析.md** - 基于 6 篇样本文章分析的 5 种爆款公式
  - 三阶段框架型 (Framework-Driven)
  - 范式颠覆型 (Paradigm Shift)
  - 实战复盘型 (Lessons Learned)
  - 赛道洞察型 (Market Insight)
  - 哲学思辨型 (Philosophical)

#### `02_核心配方生成/`
- Blog写作结构.md - 详细的写作结构模板
- 论证框架
- 节奏控制指南

#### `03_素材库/`
- 案例库 - 具体公司/产品案例
- 数据库 - 行业数据、统计数字
- 引用库 - 权威人士观点、经典理论

---

### `x_skill/` - X (Twitter) 写作技能库

**结构与 blog_skill 一致**，专门用于 X 平台的短文写作。

#### `00_原始素材库/`
- 个人定位、Twitter 风格素材

#### `01_爆款公式/`
- X 爆款推文公式分析

#### `02_核心配方生成/`
- X_writer.md - X 写作配方
- 推文结构模板

#### `03_素材库/`
- X 平台相关案例、数据、话题

---

### `xhs_skill/` - 小红书写作技能库

**结构与 blog_skill 一致**，专门用于小红书平台的内容创作。

#### `00_原始素材库/`
- 个人定位、小红书风格素材

#### `01_爆款公式/`
- 小红书爆款笔记公式分析

#### `02_核心配方生成/`
- XHS_writer.md - 小红书写作配方
- 笔记结构模板

#### `03_素材库/`
- 小红书平台相关案例、数据、话题

---

## 🔗 与 Skills 的关系

实际的 Skill 工具存放在 `.claude/skills/` 目录：
- `.claude/skills/blog-writer/` - Blog 写作 Skill
- `.claude/skills/x-writer/` - X 写作 Skill
- `.claude/skills/xhs-writer/` - 小红书写作 Skill

这些 Skill 会**引用** `01_Projects/` 下对应的素材库：
- blog-writer → `01_Projects/blog_skill/` + `01_Projects/blog_sample/`
- x-writer → `01_Projects/x_skill/`
- xhs-writer → `01_Projects/xhs_skill/`

---

## 📝 使用方式

### 写博客
1. 启动: `/blog-writer` 或告诉 Claude "我想写博客"
2. 采访: 完成 5 轮深度采访
3. 生成: AI 基于爆款公式生成文章
4. 保存: 文章自动保存到 `01_Projects/blog_sample/`

### 写 X 推文
1. 启动: `/x-writer` 或告诉 Claude "我想写 X"
2. 生成: 基于 X 爆款公式生成推文
3. 参考: 使用 `x_skill/` 中的素材

### 写小红书
1. 启动: `/xhs-writer` 或告诉 Claude "我想写小红书"
2. 生成: 基于小红书爆款公式生成笔记
3. 参考: 使用 `xhs_skill/` 中的素材

---

## 🎯 维护原则

1. **分离存储**:
   - 已发布内容 → `*_sample/` 文件夹
   - 创作素材 → `*_skill/` 文件夹

2. **统一结构**:
   - 所有 skill 文件夹保持相同的 4 个子文件夹结构
   - 便于管理和跨平台复用

3. **按需读取**:
   - Skill 不会一次性加载所有素材
   - 根据需要动态读取相关文件

4. **定期更新**:
   - 新文章发布后，添加到对应的 `*_sample/` 文件夹
   - 定期更新爆款公式分析

---

**最后更新**: 2026-01-27
**当前状态**:
- ✅ blog_skill 完整 (爆款公式已分析)
- 🔄 x_skill 待完善
- 🔄 xhs_skill 待完善
