# 明日序官网

明日序 V1.0.0 静态官网，包含真实界面截图、桌面小部件介绍和 APK 直链下载。

## 本地预览

```powershell
python -m http.server 8080 --directory website
```

然后打开 http://localhost:8080/

## 免费部署

### GitHub Pages

1. 新建 GitHub 仓库 `mingrixu`。
2. 把 `website` 目录里的文件上传到仓库根目录。
3. 打开仓库 Settings -> Pages，Source 选择 `main` 分支，目录选择 `/root`。
4. 网站地址为 `https://你的用户名.github.io/mingrixu/`。

APK 已经在 `downloads/mingrixu-v1.0.0.apk`，部署后首页“下载”按钮就是直链。

### Cloudflare Pages 或 Netlify

直接把 `website` 目录拖进 Cloudflare Pages 或 Netlify Drop 即可，不需要服务器。

## 更新版本

1. 替换 `downloads/mingrixu-v1.0.0.apk`。
2. 修改 `index.html` 里的版本号、文件大小和更新日期。
3. 重新部署。
