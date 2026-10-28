# 韩国 SOOP / PandaTV 舞蹈主播中英韩 ID 对照百科

Korean dance streamer ID roster (Chinese, Hangul, and broadcast ID) for SOOP, PandaTV, and Twitch.

This repository is a text reference roster. It does not host or play video. Each streamer row links to that person’s dance archive on [看看爱看的](https://www.kkakd.com).

## 打开页面

GitHub Pages：<https://shu-0110.github.io/korean-bj-dance-roster/>

发布设置是 `main` 分支的仓库根目录（`/`）。如果页面还没有生效，打开仓库 Settings → Pages，Build and deployment 选 Deploy from a branch，分支 `main`，文件夹 `/ (root)`，保存后再等一分钟。

本地查看时，在仓库根目录启动静态服务器后再打开 `index.html`（页面会读取 `data/roster.json`）：

```bash
python3 -m http.server 8080
```

然后访问 <http://127.0.0.1:8080/>。

## 数据

`data/roster.json` 只保留来源为 `streamers`、分类为舞蹈（韩舞）的条目。短视频 / 写真（`shorts`）没有收录。

快照日期：2026-10-28。字段包括中文名、韩文名、英文 ID / 别名、平台、kkakd.com 合集链接和来源页上的最近日期。链接使用数据里的 `site_url`，形式为 `https://www.kkakd.com/?streamer=<title>#dance`。

## 页面

单页静态站点：可按中文名、韩文名、ID 或平台搜索，可按列排序，也可用平台筛选。表头为：中文名、韩文名、ID / 别名、平台、最近日期、官网合集。
