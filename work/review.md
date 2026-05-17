# Review — 简历审核与待确认清单

> 由 cv-skill 的 resume-review-and-delivery 步骤生成

## ✅ 已确认项

| # | 项 | 状态 |
|:--|:---|:----:|
| 1 | 基本信息完整（姓名/手机/邮箱/学校/专业/城市） | ✅ |
| 2 | 教育背景准确（含核心课程） | ✅ |
| 3 | 技术技能基于用户提供的技术栈 | ✅ |
| 4 | 所有4个项目经历基于用户提供事实 | ✅ |
| 5 | 黑客松明确标注"进行中/原型开发中" | ✅ |
| 6 | 无编造GPA、奖项、论文、实习经历、排名 | ✅ |
| 7 | 无"精通"等夸大词 | ✅ |
| 8 | GitHub链接已确认不包含 | ✅ |
| 9 | 联系方式仅含用户提供的手机+邮箱 | ✅ |
| 10 | claim-source-map.md 完整，每项可溯源 | ✅ |

## 📋 建议用户确认

| # | 建议确认项 | 说明 |
|:--|:----------|:-----|
| 1 | **入学年份 2023 → 2027** | 按大二推算。如果实际不同，请纠正 |
| 2 | **核心课程列表** | 目前基于 resume_master.md。如果你有其他想突出的课，告诉我 |
| 3 | **MIMIC 项目时间标"2024"** | 你未提供具体时间，我暂且写2024。如有确切月份，请补充 |
| 4 | **F1 项目时间标"2024"** | 同上，暂写2024。有确切时间告诉我 |
| 5 | **AUC 0.950 的写法** | OOF AUC ≈ 0.950，没有写比赛排名。可以接受？ |
| 6 | **AI工具链模块** | 放在"技术技能"的最后一段，是否希望独立成块？ |

## 📄 输出文件

| 文件 | 路径 | 状态 |
|:-----|:-----|:----:|
| 简历 LaTeX 源码 | `resume.tex` | ✅ |
| 简历类文件 | `common/resume.cls` | ✅ |
| Claim-Source Map | `work/claim-source-map.md` | ✅ |
| Review 本文 | `work/review.md` | ✅ |
| PDF | 待编译 — 见下方 | ⏳ |

## 🔧 如何编译 PDF

### 方案 A：Overleaf（推荐，零安装）
1. 访问 https://www.overleaf.com
2. 新建项目 → 上传文件
3. 上传 `resume.tex` 和 `common/resume.cls`（保持目录结构）
4. 编译器选 **XeLaTeX**
5. 点击编译 → 下载 PDF

### 方案 B：本地编译
```bash
# 安装 TeX Live（如已装则跳过）
# macOS: brew install --cask mactex-no-gui
# Ubuntu: sudo apt install texlive-xetex

cd 包含resume.tex和common/的目录
xelatex resume.tex
```

## 📌 GitHub 仓库

所有文件已推送至：https://github.com/buzhidaoa8848-hash/resume-cv

- `resume.tex` — LaTeX 源码
- `common/resume.cls` — 简历类文件
- `work/claim-source-map.md` — 溯源表
- `work/review.md` — 本文

---

**下一步：** 请确认上述6项确认项，我即刻更新。Overleaf 编译约需2分钟。
