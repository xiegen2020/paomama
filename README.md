# 跑马吗 · 隐私政策托管页

「跑马吗」（HarmonyOS 应用）上架用的隐私政策。单文件静态站，零外部依赖：
不引 CDN 字体、不引统计脚本、不引外部图片，因此这个页面本身不会产生任何第三方请求。

## 部署到 Cloudflare Pages

1. Cloudflare 控制台 → Workers & Pages → Create → Pages → Connect to Git，选择本仓库。
2. Framework preset = None；Build command 留空；Build output directory = `/`
   （index.html 就在仓库根目录）。
3. 部署后得到 https://<project>.pages.dev/ 。

> 用于国内应用市场上架时，建议改用已备案域名的二级域名（如 privacy.example.com）：
> *.pages.dev 在部分网络环境下可达性不稳，审核人员打不开就等于「隐私政策无法访问」。
> 设置位置：该 Pages 项目 → Custom domains。

## 维护约定

政策正文里的「零权限 / 运行时零网络请求 / 无第三方 SDK / 收藏仅存本机」是按应用当前实现写的。
一旦新版本引入任何联网行为、权限申请或第三方 SDK，必须先修改本政策并重新取得用户同意，
再上线该功能（政策第八节已就此向用户作出承诺）。

应用内「关于」中声明的政策版本号与生效日期，须与本页面保持一致。
