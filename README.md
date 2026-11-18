# doc.shengpan.net 的旧链接入口

此目录仅保存两个已公开的旧隐私政策地址的跳转页。政策正文统一在个人网站 `site/src/content/policies/` 维护，原文恢复自旧服务器备份。

| 旧地址 | 正文地址 |
| --- | --- |
| https://doc.shengpan.net/privacy/eldenring/ | https://www.shengpan.net/privacy/eldenring/ |
| https://doc.shengpan.net/zelda-ptivacy-policy/ | https://www.shengpan.net/privacy/zelda-recipes/ |

GitHub Pages 的静态跳转使用 HTML meta refresh，并提供规范地址与可点击链接，不依赖 JavaScript。它不是服务器端的 HTTP 301。

## 托管

GitHub Pages 每个站点单独配置自定义域名，因此本目录发布至独立仓库 `MrPans/shengpan-doc-redirects`。该仓库的 Pages 从 `main` 根目录发布，自定义域名为 `doc.shengpan.net`。无需服务器、Node.js 运行环境或新增访问凭证。

阿里云 DNS 记录：

| 主机记录 | 类型 | 记录值 | TTL |
| --- | --- | --- | --- |
| doc | CNAME | MrPans.github.io | 600 |

先在 GitHub 配置文档站的自定义域名，再添加 DNS 记录。DNS 生效且 GitHub 证书签发完成后，为该 Pages 站点启用 Enforce HTTPS。

两份政策只在主站修改。只有旧地址或正文地址改变时，才需要修改此目录并将内容同步到跳转仓库。

旧 `doc` 目录包含其他历史文件，未复制到公开网站。完整备份保存在本机 `.backups/2026-11-18-doc-recovery/doc-original.tar.gz`。
