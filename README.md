# judyzjy.com — Judy Z · Brand Strategist

品牌策略师个人作品集站。中英双语，单页响应式设计。

## 部署

### 方案一：GitHub Pages（推荐，免费）

```bash
# 1. 先在 github.com 创建仓库 judyzjy.com（不要初始化 README）
# 2. 本地推送
git remote add origin git@github.com:<你的用户名>/judyzjy.com.git
git branch -M main
git push -u origin main

# 3. 在 GitHub 仓库 Settings → Pages 中：
#    - Source: Deploy from a branch
#    - Branch: main, / (root)
#    - Save
```

等待 1-2 分钟，访问 `https://<你的用户名>.github.io/judyzjy.com/`

### 方案二：自定义域名

在 GitHub Pages 设置中填写自定义域名（如 judyzjy.com），同时在域名 DNS 添加 CNAME 记录指向 `<你的用户名>.github.io`。

### 方案三：本地预览

```bash
npx serve .
# 或
python3 -m http.server 8000
```

## 结构

```
judyzjy.com/
├── index.html    # 完整单页站点（含 CSS + JS）
├── photo.jpg     # 个人照片
└── README.md     # 本文件
```

## 特性

- 中英双语切换（localStorage 持久化）
- 浅色/深色主题切换
- 响应式设计（桌面/平板/手机）
- 案例可展开/收起
- 平滑滚动导航

## 旧版 PDF 作品集

iCloud Drive 中有《作品集.pdf》（39页，15.8MB），内容为新媒体运营/PR 定位的旧版作品集。新版网站已重新定位为品牌策略师方向。

## 维护

修改 `index.html` 后重新 commit 并 push 即可自动更新 GitHub Pages。

```bash
git add -A
git commit -m "更新说明"
git push
```
