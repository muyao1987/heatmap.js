# heatmap.js
Dynamic Heatmaps for the Web. 

[<img src="http://www.patrick-wied.at/static/heatmapjs/assets/img/heatmapjs-examples-docs-banner.jpg" width="100%">](http://www.patrick-wied.at/static/heatmapjs/?utm_source=gh "View the heatmap.js website with usage examples, showcases, best practises, plugins ( googlemaps heatmap, leaflet) and more.")

## 本仓库说明（Fork）

本仓库是 [pa7/heatmap.js](https://github.com/pa7/heatmap.js) 的 fork，由 [火星科技 木遥](http://www.marsgis.cn) 维护，用于 web 环境的发布与示例演示，对应的 npm 包为 [`@mars3d/heatmap.js`](https://www.npmjs.com/package/@mars3d/heatmap.js)。除 README 外，本仓库不修改库源码，以便与上游保持同步。在 fork 基础上的改动见下方 [mars3d update](#mars3d-update) 小节。

### 目录结构

| 目录 | 说明 |
| --- | --- |
| `src/` | 库源码（`core.js`、`data.js`、`config.js`、`util.js` 及 `renderer/` 下的 canvas2d / webgl / vml 渲染器） |
| `build/` | 构建产物（`heatmap.js` 与压缩版 `heatmap.min.js`） |
| `plugins/` | 各平台插件：`angular-heatmap`、`gmaps-heatmap`（Google Maps）、`leaflet-heatmap`（Leaflet）及 `svg-area-heatmap.js`、`segment-heatmap.js` 等 |
| `examples/` | 本地可运行的示例页面 |
| `docs/` | 文档站点（快速开始、FAQ、迁移指南等） |
| `tests/` | 测试 |

### 常用命令

以下命令来自 `package.json` 的 `scripts`：

```bash
npm run build   # 通过 grunt 构建源码（grunt build）
npm run push    # 发布 npm 包（npm publish --access public）
```

本地预览示例见下文 "How to run the local examples"。

---

以下为上游原始 README 内容（保留原文、署名与链接）：

---

## mars3d update
- fix: An error "Cannot assign to read only property 'data' of object '#<ImageData>'"
- add: Added support for typescript in index.d.ts
- The NPM package was released  `@mars3d/heatmap.js`


## How to get started

The fastest way to get started is to install heatmap.js with bower. Just run the following command:

`bower install @mars3d/heatmap.js-amd`

This will download the latest working version of heatmap.js and put it in your bower_components folder.

Alternatively you could just download [the latest release](https://github.com/pa7/heatmap.js/releases) from github and unzip it.


The file you're ultimately looking for is **heatmap.js** or **heatmap.min.js**



heatmap.js is also hosted on npm:

`npm install @mars3d/heatmap.js`



### How to run the local examples

Start a webserver (e.g. python SimpleHTTPServer from the project directory root):

`python -m SimpleHTTPServer 1337 &`

Then browse to 

`http://localhost:1337/examples/`


## Get involved

Please have a look at the [contribution guidelines](CONTRIBUTE.md) before submitting contributions. 

**Disclaimer**: PRs can take time to receive feedback or be merged ( I'm only one person with very little time ) but I'm trying to get back to everyone eventually

## Questions?

In order to keep technical questions in a central place where other people can learn from it, the best thing you can do is [post your question to stackoverflow with the tag **heatmap.js**.](http://stackoverflow.com/questions/ask?tags=heatmap.js) 

If you do have a very specific question (or need commercial support) don't hesitate to contact me directly [via email](mailto:heatmap-q@patrick-wied.at).


## Mailing list

Want to receive the latest updates and news about heatmap.js? 

There is a [mailing list](http://eepurl.com/0mmV5). No spam, just news and important updates.
