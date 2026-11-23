# 桃子果冻

一个可以拖拽果肉、弹出果核、切换品种的 3D 桃子果冻小游戏。

[在线体验](https://sunmengmm.github.io/peach-jelly/) · [GitHub 仓库](https://github.com/sunmengmm/peach-jelly)

## 操作

拖动果冻或果核，拖动空白处旋转视角；使用面板切换品种、调整参数、暂停或重置。支持触控，尚未做手机真机验证。

## 本地运行

需要 Python 3 和支持 WebGPU 的浏览器，无需安装依赖。在项目目录运行：

```sh
python3 -m http.server 5173 --bind 127.0.0.1
```

访问 <http://127.0.0.1:5173>，按 `Ctrl+C` 停止服务。

## 文件

`index.html` 包含完整游戏。`references/` 为本地参考资料，已被 Git 忽略。

## 发布

GitHub Pages 使用 `main` 分支的 `/(root)` 目录。修改后提交并推送到 GitHub，网站会自动更新；仅保存本地文件不会更新网站。
