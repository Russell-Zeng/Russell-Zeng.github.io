# Russell Zeng — Academic Homepage

Personal academic homepage based on [w-r-s/academic-homepage-template](https://github.com/w-r-s/academic-homepage-template), upstream commit `3e688b9cdb8928aa90ce2469b932cd4661723f97`.

Website: https://russell-zeng.github.io/

## 当前状态

新模板已替换旧版网站，保留橙色链接、论文卡片与分类筛选、项目标签云、返回顶部及景观页脚。当前只有 GitHub 公开姓名 Russell Zeng 和 GitHub 链接属于已确认个人信息；头像、机构、论文、经历、项目、服务、教学及获奖信息均为明确标注的占位内容。论文配图仅为原模板版式预览，后续需替换。

## 本地预览

在本目录运行：

```bash
python3 -m http.server 8080 --bind 127.0.0.1
```

打开 http://127.0.0.1:8080 。纯静态页面，无需安装 Node.js、Jekyll 或执行构建。

## 后续按简历更新

- `index.html`：姓名、简介、联系方式、News、论文、经历、项目、服务教学、荣誉和页脚。
- `images/template/avatar.svg`：当前占位头像；拿到照片后替换图片并更新 HTML 路径。
- `images/paper/`：论文示意图。
- `images/experience/`：景观页脚背景。
- `stylesheet.css`：原模板样式。
- `custom.css`：占位内容及手机排版的少量补充样式。

邮箱、CV 和 Scholar 未提供前显示灰色占位文字。提供 PDF 简历后可放到 `files/cv.pdf` 并启用 CV 链接。项目云暂用占位标签，没有虚构星标数。更新内容时同时更新页脚日期及论文分类按钮；分类计数自动生成。

## GitHub Pages

仓库 `Russell-Zeng/Russell-Zeng.github.io` 从 `master` 分支根目录 `/` 发布。`.nojekyll` 使页面按静态文件发布。旧模板遗留的 `CNAME`（原作者域名）已移除，当前使用 `russell-zeng.github.io`。

## 旧版备份

迁移基点：`bb58ea6ba10b82431256f4cc31cfbaa5d355cf1b`。

Git 标签：`backup/pre-template-2026-10-16`。本地另存完整历史备份 `.migration/previous-homepage.bundle`，已通过 `git bundle verify`。`.migration/` 不会提交或部署。

恢复查看旧版可使用 `git show backup/pre-template-2026-10-16:index.html`。恢复上线可以回退本次迁移提交，无需重写仓库历史。

原模板作者及来源归属保持不变；上游仓库未提供单独 LICENSE 文件，本项目不为其新增授权声明。
