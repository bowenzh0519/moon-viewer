# 观月｜真实月相

此刻、此地的真实月相、月面与观测信息。

## 在线访问

https://bowenzh0519.github.io/moon-viewer/

## 技术栈

- 纯前端 HTML/CSS/JS，无框架依赖
- [Astronomy Engine](https://github.com/cosinekitty/astronomy) — 天文计算
- [@photostructure/tz-lookup](https://github.com/photostructure/tz-lookup) — IANA 时区
- NASA SVS CGI Moon Kit 4K — 月面纹理
- 高德地图 JS API 2.0 — 地点选点
- WebGL — 月面渲染

## 更新方式

本地开发文件位于上层目录 `moon_observer_v3.html`，修改并完成本地验证后执行：

```bash
cp ../moon_observer_v3.html index.html
cp -R ../moon_tiles_v3 ./moon_tiles_v3
git add -- index.html moon_tiles_v3
git commit -m "更新月相页面"
git push
```

推送后 GitHub Pages 自动部署，1-2 分钟生效。
