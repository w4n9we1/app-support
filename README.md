# app-support — Lababacy 产品站（lababacy.com）

所有 App 的官方站。域名：**lababacy.com**（Cloudflare DNS + GitHub Pages，`CNAME` 文件在仓库根）。
旧路径 `w4n9we1.github.io/app-support/<app>/` 永久 301 到 `lababacy.com/<app>/`，路径保持。

## 域名政策（2026-10-08 定）

1. **以后所有新项目一律使用 lababacy.com**，不再新增 github.io 路径。
2. **已上架 App 的 ASC 三个 URL 保持原 github.io 值不动**（经 301 永久可达，所有者拍板）；**新 App 上架时直接填**：
   - Marketing URL → `https://lababacy.com/<app>/`
   - Support URL → `https://lababacy.com/<app>/support/`
   - Privacy Policy URL → `https://lababacy.com/<app>/privacy/`
3. **新 App 提审 checklist**：三页建齐 → push → 线上逐页 200 → 再在 ASC 填 URL。

## 每个 App 的三页结构

| 页面 | 承担 | 要点 |
|---|---|---|
| `/<app>/`（产品页 = Marketing URL） | **SEO 主战场** | 规范见下节 |
| `/<app>/support/` | 支持页 | FAQ + 恢复购买 + 联系方式（mailto 带 App 名 subject） |
| `/<app>/privacy/` | 隐私政策 | 数据收集口径如实披露；模板参考 voxmail/ringlight 现有页 |

## 产品页（Marketing URL）的极致 SEO 规范

依据：2026-10 实测证据链（商店页被 Google 完整索引；品牌 SERP 第 2 位曾被爬虫站 mwm.ai 占据；ASC 来源数据 ChatGPT 161 展示→14 下载→$66；google.com 314 展示→12 下载）。名字精确匹配 = 站内词位 + Google 答案位 + ChatGPT 推荐位三重杠杆，产品页是这个杠杆在自有域上的延伸。规则：

1. **Front matter 必填**（`<title>` 与 meta description 的生成来源）：
   - `title` = 用户搜索的问题原句 + App 名，如「Open MDB & ACCDB Files on iPhone — Access Database Viewer」。title 是全页权重最高的 SEO 字段，必须精确匹配目标查询词。
   - `description` = ≤150 字符的直答句（Google 摘要直接采用）。
2. **正文第一句 = 问题的直答**（Google snippet 与 ChatGPT 摘要都取开头），禁止营销开场白。
3. **正文铺词**：格式全称（.wpd/.pub/.odt 每种至少出现一次）、动作词（open/view/convert/export）、场景原句（sent by Outlook / created in Publisher）。目标 = 覆盖该 App 全部长尾问法。
4. **内链**：页尾「All apps」链回根主页（footer 已内置）——域内链接全血传递权重，N 个产品互喂 = 工厂复利引擎。
5. **与商店 description 同源不逐字**：同素材不同排版，避免与 apps.apple.com 互为重复内容。
6. **站级基建（已配好，勿删）**：`_config.yml`（jekyll-sitemap + jekyll-seo-tag）、`_layouts/default.html`（含 `<head>`/og 标签）、`robots.txt`、`/sitemap.xml` 自动生成。
7. **上线后验证清单**：`view-source:` 确认 `<title>`/`<meta name="description">`/og 标签存在 → `/sitemap.xml` 含该页 → Google `site:lababacy.com/<app>` 可达。

## 站点结构

```
index.md                # 产品矩阵主页（互链枢纽）
support/index.md        # 全站支持中心（FAQ/联系方式）
<app>/index.md          # 产品页（Marketing URL 落点，front matter 必填）
<app>/support/index.md  # App 支持页
<app>/privacy/index.md  # 隐私政策
<app>/terms/index.md    # 服务条款（部分 App）
_layouts/default.html   # 全站布局：<head> 含 seo 标签 + footer 互链
_config.yml             # Jekyll 配置（域名/插件）
robots.txt              # 全允许 + sitemap 声明
CNAME                   # lababacy.com
```

## 遗留可选项

- [ ] GitHub Pages Enforce HTTPS 勾选（Settings → Pages；http://lababacy.com 暂不强制跳 https）
- [ ] GitHub 账号级域名校验（Settings → Pages → Add domain，防接管）
- [ ] Google Search Console 添加 lababacy.com + 提交 sitemap
