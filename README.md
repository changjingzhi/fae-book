# 《怎么做 FAE》（暂名）

一本关于"怎么做 FAE"的书稿项目：Why（为什么需要 FAE）/ Who（FAE 是一群什么样的人）/ What（FAE 怎么做事）。

## 在线阅读

用 [mdBook](https://rust-lang.github.io/mdBook/) 构建，推送 `main` 分支后由 GitHub Actions 自动发布：

**https://changjingzhi.github.io/fae-book/**

- 目录配置：`书稿/SUMMARY.md`（新增章节需在此登记）
- 站点配置：`book.toml`
- 自动部署：`.github/workflows/deploy.yml`

本地预览（需先安装 mdBook：`cargo install mdbook`）：

```bash
mdbook serve --open
```

## 目录结构

- `书稿/` —— 各章正文（按章节编号）
  - `SUMMARY.md` —— 全书目录（mdBook 构建入口，新增章节必须在此登记）
  - `00_前言_缘起/` —— 前言
  - `01_鸿沟_为什么这个世界需要FAE/` —— 第 1 章
  - `02_面孔_FAE是一群什么样的人/` —— 第 2 章
  - `03_长路_这门手艺怎么长出复利/` —— 第 3 章
  - `04_做事上_把能做变成客户要的/` —— 第 4 章
  - `05_做事下_让承诺立得住留得下/` —— 第 5 章
  - `06_尾声_留给下一个FAE的话/` —— 尾声
- `book.toml` —— mdBook 站点配置
- `.github/workflows/deploy.yml` —— 推送 `main` 后自动构建并发布

## 写作约定

- 写法：提出问题 → 回答问题
- 语言：中文
