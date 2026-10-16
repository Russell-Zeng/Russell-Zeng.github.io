# Yuan Zeng (曾元) — Academic Homepage

Personal academic homepage based on [w-r-s/academic-homepage-template](https://github.com/w-r-s/academic-homepage-template), upstream commit `3e688b9cdb8928aa90ce2469b932cd4661723f97`.

Website: https://russell-zeng.github.io/

## 当前状态

已根据曾元提供的简历填入简介、照片、邮箱、13 篇论文、4 段教育经历、2 段工作/实习经历、6 个项目、3 项授权专利和 ICMIP 2020 报告奖。

主页使用英文主体，保留中文姓名、机构及项目名称。论文在审状态按简历明确标注；未提供的社交账号及 Google Scholar 链接不展示。完整内容来源及维护说明见 `CONTENT_NOTES.md`。

## 本地预览

```bash
python3 -m http.server 8080 --bind 127.0.0.1
```

打开 http://127.0.0.1:8080 。纯静态页面，无需安装依赖或构建。

## 内容维护

- `index.html`：公开学术主页。
- `cv.html`：可阅读、打印或通过浏览器另存 PDF 的公开 CV 视图；不含手机号、出生日期和籍贯，原始简历未上传。
- `images/profile.jpg`：简历照片。
- `images/paper/`：来自对应研究项目页面的论文配图。
- `stylesheet.css`：原模板样式；`custom.css`：内容和响应式布局补充。
- 更新论文时同步修改分类按钮、状态和公开 CV。分类计数自动生成。

## GitHub Pages

仓库 `Russell-Zeng/Russell-Zeng.github.io` 从 `master` 分支根目录 `/` 发布。`.nojekyll` 使页面按静态文件发布。旧模板遗留的 `CNAME`（原作者域名）已移除，当前使用 `russell-zeng.github.io`。

## 旧版备份

迁移基点：`bb58ea6ba10b82431256f4cc31cfbaa5d355cf1b`。

Git 标签：`backup/pre-template-2026-10-16`。本地另存完整历史备份 `.migration/previous-homepage.bundle`，已通过 `git bundle verify`。`.migration/` 不会提交或部署。

恢复查看旧版可使用 `git show backup/pre-template-2026-10-16:index.html`。恢复上线可以回退本次迁移提交，无需重写仓库历史。

原模板作者及来源归属保持不变；上游仓库未提供单独 LICENSE 文件，本项目不为其新增授权声明。
