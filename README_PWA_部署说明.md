# 未竟本 Trace Note PWA 版本

这是一个可以部署成网页、并在手机上“添加到主屏幕”的 PWA App。

## 文件结构

```text
trace_note_pwa_app/
├─ index.html
├─ manifest.json
├─ service-worker.js
└─ icons/
   ├─ icon-192.png
   └─ icon-512.png
```

## 本地预览

直接双击 `index.html` 可以看界面，但 PWA 安装能力通常需要通过本地服务器或线上 HTTPS 访问。

推荐在该文件夹打开终端运行：

```bash
python -m http.server 8000
```

然后浏览器打开：

```text
http://127.0.0.1:8000
```

## 部署方式

把整个文件夹上传到任意静态网站托管平台，例如：

- Vercel
- Netlify
- GitHub Pages
- Cloudflare Pages

部署后用手机浏览器打开网址。

## 手机上安装

### Android / Chrome

打开网址后，点击浏览器菜单，选择：

```text
添加到主屏幕 / 安装应用
```

### iPhone / Safari

打开网址后，点击分享按钮，选择：

```text
添加到主屏幕
```

## 注意

PWA 的离线缓存已经配置。AI API 调用仍需要联网。
正式上线时，不建议把自己的 DeepSeek / 豆包 API Key 放在前端；更安全的方式是使用后端代理。
