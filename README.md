# 桃子果冻 · Work 版

当前唯一网页入口是 `index.html`，由原文件 `peach-jelly桌面端work版.html` 改名而来，页面内容未修改。

## 文件

- `index.html`：完整的单文件小游戏，包含页面、物理模拟和 WebGPU 渲染；不依赖外部资源或后端。
- `references/`：仅保存在本地的参考资料，已被 Git 忽略，不随项目推送。

## 本地运行

在本目录打开终端，运行：

```sh
python3 -m http.server 5173 --bind 127.0.0.1
```

浏览器访问 <http://127.0.0.1:5173>。停止服务时在终端按 `Ctrl+C`。

无需安装 npm 依赖。运行环境需要 Python 3，以及支持 WebGPU 的浏览器和设备。请通过本地服务器或 HTTPS 网站打开。

## 操作

- 拖动果冻或果核，拖动空白处旋转视角。
- 使用面板切换桃子品种、弹出或放回果核、重置、暂停及调整参数。
- 已包含窄屏布局和触控拖拽，尚未做手机真机验证。
- 当前没有 WebGL 备用渲染；设备不支持 WebGPU 时会显示提示。

## 发布

在线体验：<https://sunmengmm.github.io/peach-jelly/>。

GitHub 仓库：<https://github.com/sunmengmm/peach-jelly>。

已通过 GitHub Pages 发布 `main` 分支根目录中的 `index.html`，使用 HTTPS。网站和仓库均公开；访问游戏不需要登录。

本地 `main` 分支已关联远程仓库的 `origin/main`。修改网页后，在本目录执行：

```sh
git add index.html
git commit -m "Update peach jelly"
git push
```

`commit` 保存本地版本，`push` 上传到 GitHub；推送完成后，Pages 会自动重新部署。仅保存文件不会更新线上网页。

运行 `git status` 可以查看尚未提交的修改，以及本地是否有未推送的提交。如果在 GitHub 网页或其他电脑上修改过文件，先运行 `git pull --ff-only` 拉取更新。

发布网站只需要 `index.html`，参考提示词不参与运行。
