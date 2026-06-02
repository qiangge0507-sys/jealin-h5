# Jealin H5 运营说明

这是一个可推广的移动端饰品售卖 H5，适合先用静态站方式上线，再用 WhatsApp 承接预约和购买咨询。

## 当前文件

- `index.html`：客户访问的 H5 售卖页
- `admin.html`：本地商品管理台
- `data.js`：正式上线使用的商品和站点配置
- `assets/`：图片素材目录

## 日常改商品

1. 打开 `admin.html`。
2. 修改 WhatsApp 号码、首页主视觉、商品名称、价格、分类、描述、图片路径。
3. 点击“保存到本机预览”，再回到 `index.html` 看效果。
4. 确认无误后点击“生成 data.js 配置”。
5. 把生成内容替换到 `data.js`，再部署上线。

## 更换产品图片

建议把真实商品图片放到：

```text
assets/products/
```

例如：

```text
assets/products/gold-studs-01.jpg
assets/products/necklace-01.jpg
assets/products/ring-01.jpg
```

然后在管理台的“商品图片路径”里填写对应路径。图片建议使用竖图或 4:5 商品图，背景干净，首饰清晰，文件尽量压缩到 300KB 到 800KB。

## 上线需要什么

最小上线链路：

1. 域名：例如 `jealinjewelry.com`、`shopjealin.com`、`jealin.ng`。
2. 托管平台：Vercel、Netlify、Cloudflare Pages 都适合这个静态 H5。
3. WhatsApp Business：把正式号码填进 `admin.html` 或 `data.js`。
4. 产品图片：真实商品图越清晰，推广转化越稳。
5. 分享图：当前使用 `assets/jealin-hero-jewelry.png` 作为社交分享图。

## 推荐上线流程

1. 先用免费预览域名测试，比如平台自动生成的 `.vercel.app`、`.netlify.app` 或 `.pages.dev`。
2. 确认手机访问、WhatsApp 跳转、商品图片、价格都正确。
3. 购买并绑定正式域名。
4. 配置 HTTPS，主流平台通常会自动处理。
5. 用正式链接投放 Instagram、TikTok、WhatsApp Status、Google Business Profile。

## 什么时候需要真正后台

当前版本适合早期运营：商品数量不多，修改后重新部署即可。

当你需要这些能力时，就应该升级成真正后台：

- 多人登录管理
- 在线上传图片
- 库存管理
- 在线支付
- 订单状态
- 客户资料沉淀
- 广告转化统计

下一阶段可以接 Supabase、Firebase、Airtable、Google Sheets 或一个轻量 Node 后台。

## 推广前检查

- WhatsApp 号码已经填好
- 每个商品都有真实图片
- 价格是最新的 NGN
- 首页首屏能看出是饰品品牌
- Instagram Bio 链接可打开
- WhatsApp 分享预览标题和图片正常
- 至少准备 5 到 10 张商品图用于广告和社媒内容
