# Oil Frontgame Demo

石油 Front Game 的长期可玩原型仓库。

## V0.1 基线

V0.1 直接基于原始 `index (1).html` 迁移，保留现有 Three.js 吸油玩法：角色移动、自动拿取吸头、软管张力/绕障碍/回缩、连续黏稠油面、预吸与正式吸取、油团流动、镜头震动、残油自动收尾、触屏拖动与键盘操作。

## 本地运行

需要 Node.js 22.12 或更新版本，推荐 Node.js 24。

```bash
npm ci
npm run dev
```

## 构建

```bash
npm run build
```

## GitHub Pages

仓库内已包含 `.github/workflows/deploy.yml`。每次 push 到 `main` 后会自动构建并部署 `dist/`。

本仓库已将 GitHub Pages 的 Source 设置为 **GitHub Actions**。

试玩地址：https://s1044173749-design.github.io/oil-frontgame-demo/

Vite 的 `base` 为 `/oil-frontgame-demo/`，与仓库的 Pages 路径对应。构建采用锁定依赖的 `npm ci`，部署工作流使用 Node.js 24。

## 操作

键盘与触屏操作保持原 Demo 的实现，以页面内说明为准。`H` 切换调试信息，空格或页面按钮放下吸头，重置按钮重新开始。
