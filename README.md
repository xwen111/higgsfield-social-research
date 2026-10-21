# Higgsfield 社媒视觉研究

36 条 Instagram 样本与封面、16 个可追溯的观察，以及前三秒 Hook、节奏、MG 动画和多 showcase 组织方式的拆解。

阅读入口：`index.html`，完整报告为 `research/report.html`。配图附样本编号、截帧时间和原帖链接；交互播放器支持阶段定位与慢放。

## 本地阅读

在本文件夹执行：

```sh
python3 research/serve_report.py
```

打开 http://127.0.0.1:8765/ 。该服务器支持视频 Range 请求。

## 部署包

```sh
python3 scripts/build_site.py
```

将 `dist/` 作为静态网站根目录部署。报告中的图片、音轨、开头片段和交互播放器均使用相对路径，不依赖本地服务器地址。

仓库保持 private；在线网页可公开阅读。仅改变仓库可见性不会自动改变网站访问权限。

## 更新

```sh
python3 research/report.py
python3 scripts/build_site.py
```

`research/report.py` 与相关数据文件生成报告；`scripts/build_site.py` 校验静态资源并整理上线文件。原始长视频、临时试验文件和抓取清单保留在本机，不加入 Git；网页实际使用的研究片段、截图和音轨随网站保存。

## 研究边界与素材

研究日期：2026-10-21。报告基于视觉分镜抽样，音乐听审未完成，未证实使用 Remotion。完整方法和限制见报告阅读说明。Higgsfield 封面、视频及音轨归相应权利人所有；本仓库用于研究和学习，不授予素材的再利用许可。
