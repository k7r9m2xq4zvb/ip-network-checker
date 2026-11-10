# IP / 网络检测工具

一键检测你的公网 IP、位置、运营商、时区、延迟与连通性。纯前端单文件工具，数据只在浏览器里查询，不会上传到任何服务器。

## 功能

- 公网 IP、国家 / 城市、省份、运营商 / ISP、ASN、时区
- 延迟检测：Google、Cloudflare、GitHub、百度
- 本地信息：浏览器时区、本地时间、User-Agent、本地 IP（WebRTC）
- 复制结果 / 下载 JSON

## 使用

直接打开 `index.html` 就能用，也可以部署到 GitHub Pages：

仓库 Settings → Pages → Build and deployment → Source 选择 `Deploy from a branch`，Branch 选择 `main` / `(root)`，保存后访问 `https://<用户名>.github.io/ip-network-checker/`

## 说明

IP 信息会依次尝试 ipapi.co、ipinfo.io、ip-api.com，某个接口失败会自动换下一个。延迟是用 fetch 计时测的，不是 ICMP ping，仅供参考。
