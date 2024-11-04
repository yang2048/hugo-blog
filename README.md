# Hugo FixIt 博客模板（Go）

👉 中文 | [English](README.en.md)

这是 Hugo 主题 [FixIt](https://github.com/hugo-fixit/FixIt) 的快速启动模板。它使用 [Hugo 模块](https://gohugo.io/hugo-modules/) 功能加载主题。

它提供了基本的主题结构和配置。已经设置了 GitHub Actions，可以自动部署博客到 GitHub Pages。此外，还有一个定时任务，每天自动更新主题。

## 目录结构

```bash
▸ .github/       # GitHub configuration
▸ archetypes/    # page archetypes (like scaffolds of archetypes)
▸ assets/        # css, js, third-party libraries etc.
▸ config/        # configuration files
▸ content/       # markdown files for hugo project
▸ data/          # blog data (allow: yaml, json, toml), e.g. friends.yml
▸ public/        # build directory
▸ static/        # static files, e.g. favicon.ico
▸ themes/        # theme submodules
▸ go.mod
▸ go.sum
```

## 快速入门

完整的快速入门，请参阅此 [页面](https://fixit.lruihao.cn/documentation/getting-started/)。

### 准备

- [Go](https://go.dev/dl/)
- [Hugo](https://gohugo.io/installation/): >= 0.112.0 (extended version)

### 启动站点

```bash
# 开发环境
hugo server
# 生产环境
hugo server -e production
```

### 构建站点

当你的站点准备部署时，运行以下命令：

```bash
hugo
```

### 更新主题

之后，你可以使用以下命令升级主题：

```bash
# 手动更新主题
hugo mod get -u github.com/hugo-fixit/FixIt@latest
hugo mod tidy
```

<details>
  <summary>通过 NPM 脚本启动</summary>

  ```bash
  # 构建博客
  npm run build
  # 运行带有监视的本地调试服务器
  npm run server
  # 在生产环境中运行本地调试服务器
  npm run server:production
  # 更新主题子模块
  npm run update:theme
  ```

</details>


## 故障排除

