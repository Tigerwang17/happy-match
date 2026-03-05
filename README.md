# Happy Match for Claudia

三消小游戏 — Cute Animal Kingdom。  
使用 GitHub Pages 部署后，访问：**https://tigerwang17.github.io/happy-match/**

## 本地运行

用浏览器直接打开 `index.html` 或 `match.html` 即可。

## 部署到 GitHub Pages

1. 在 GitHub 仓库 [Tigerwang17/happy-match](https://github.com/Tigerwang17/happy-match) 中开启 Pages：
   - 打开仓库 → **Settings** → **Pages**
   - **Source** 选择 **Deploy from a branch**
   - **Branch** 选 `main`，目录选 **/ (root)**，保存

2. 将本目录推送到该仓库：

```bash
cd happy-match-deploy
git init
git add index.html match.html pig-bomb.png README.md
git commit -m "Deploy Happy Match for Claudia"
git branch -M main
git remote add origin https://github.com/Tigerwang17/happy-match.git
git push -u origin main
```

3. 等待 1–2 分钟后访问：**https://tigerwang17.github.io/happy-match/**

## 技术说明

- 纯前端：HTML + CSS + JavaScript，无构建步骤
- 样式：Tailwind CSS（CDN）
- 数据：排行榜等存于浏览器 LocalStorage
