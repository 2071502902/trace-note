# Trace Note PWA 部署安装说明

这是基于 `trace_note_mobile_v39_fixed.html` 制作的 PWA 版本。

## 文件说明

- `index.html`：App 主页面
- `manifest.json`：PWA 安装配置
- `service-worker.js`：离线缓存配置
- `icons/`：桌面图标

## 部署到 GitHub Pages

1. 新建 GitHub 仓库，例如 `trace-note`。
2. 上传本文件夹里的全部内容，注意 `index.html` 必须在仓库根目录。
3. 进入 `Settings → Pages`。
4. Source 选择 `Deploy from a branch`。
5. Branch 选择 `main`，Folder 选择 `/root`。
6. 保存后等待部署完成。

## 手机安装

打开 GitHub Pages 网址后：

- Android Chrome：右上角菜单 → 添加到主屏幕 / 安装应用
- iPhone Safari：分享按钮 → 添加到主屏幕

## 注意

AI 报告生成需要联网。API Key 仅保存在本机浏览器，正式上线时建议改成后端代理。
