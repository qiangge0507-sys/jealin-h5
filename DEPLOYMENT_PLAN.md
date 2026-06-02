# Jealin H5 部署与域名执行方案

## 当前推荐路线

优先推荐：Vercel。

原因：

- 当前项目是纯静态 H5，不需要服务器。
- Vercel 可以直接部署 `index.html`、`data.js`、`assets/`。
- 绑定自定义域名和 HTTPS 流程简单。
- 以后如果要升级后台，也可以继续扩展。

备选：

- Netlify：也很适合静态站，操作同样简单。
- Cloudflare Pages：适合已经用 Cloudflare 管理域名的情况。

## 你现在还不能直接正式推广的原因

当前链接是：

```text
http://127.0.0.1:4173/index.html
```

这是本地预览地址，只能在你这台电脑上访问。客户手机无法访问。

正式推广需要得到一个公网链接，例如：

```text
https://shopjealin.com
https://jealinjewelry.com
https://jealin.vercel.app
```

## 我已经完成的部署准备

- 已添加 `vercel.json`
- 已添加 `netlify.toml`
- 已添加 `_redirects`
- 已添加 `robots.txt`
- 已添加 `sitemap.xml`
- 已添加 `assets/favicon.svg`
- 已整理本地管理台 `admin.html`
- 已拆分商品数据 `data.js`

## 部署前需要你决定

### 1. 选择平台

建议选 Vercel。

你需要一个 Vercel 账号，可以用 GitHub、Google 或邮箱注册。

### 2. 选择域名

如果还没买域名，建议先部署到平台免费域名测试。

域名建议：

- `shopjealin.com`
- `jealinjewelry.com`
- `jealinlagos.com`
- `jealin.ng`

### 3. 准备 WhatsApp Business 号码

格式建议只保留数字和国家区号，例如：

```text
2348012345678
```

## Vercel 部署步骤

1. 打开 https://vercel.com/
2. 登录或注册账号。
3. 创建 New Project。
4. 上传或导入当前项目文件。
5. Framework Preset 选择 Other。
6. Build Command 留空。
7. Output Directory 留空或使用根目录。
8. 点击 Deploy。
9. 得到一个 `.vercel.app` 预览链接。
10. 手机打开测试 H5、商品详情、预约清单、WhatsApp 跳转。

## 绑定域名步骤

1. 在 Vercel 项目里进入 Domains。
2. 添加你的域名，例如 `shopjealin.com`。
3. 按 Vercel 提示去域名服务商修改 DNS。
4. 等待 DNS 生效。
5. Vercel 会自动配置 HTTPS。
6. 用手机访问正式域名确认。

## 域名确定后需要改的文件

把下面两个文件里的 `YOUR_DOMAIN_HERE` 替换成真实域名：

- `robots.txt`
- `sitemap.xml`

如果域名是 `shopjealin.com`，就替换成：

```text
shopjealin.com
```

## 正式推广前最后检查

- 正式域名能打开
- HTTPS 正常
- WhatsApp 跳转正常
- 商品图片显示正常
- 价格正确
- 手机端无横向滚动
- Instagram/WhatsApp 分享卡片显示正常
- 管理台不放在公开宣传入口

## 我能继续帮你做什么

下一步你只需要给我其中一种信息：

1. 你已经有域名，把域名发我。
2. 你还没有域名，我帮你确定最合适的候选域名。
3. 你已经有 Vercel / Netlify / Cloudflare 账号，我陪你部署。
4. 你想先用免费 `.vercel.app` 链接上线测试。
