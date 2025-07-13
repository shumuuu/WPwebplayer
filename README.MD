# WPWebPlayer（html网站播放组件）  
一款简单，简洁，轻量的网站音乐播放器  
![示例](https://imgbed.yunsen2025.top/file/1752422083916.png)  
[项目主页文章（博客）](https://www.yunsen2025.top/023-wpmusicplayer) | [示例界面](https://wpwebplayer.112601.xyz/) | [NPM包（前端资源）](https://www.jsdelivr.com/package/npm/wpwebplayer?tab=files)
> [!NOTE]
>
> **README仅展示基础玩法，推荐前往上方项目文章查看更多**
---
# 项目特性：
- 简洁：仅需引入css与js文件，统一使用`<wp-music-player>`标签
- 简单：无更多冗杂功能，回归最基础的【网站音乐播放】
- 可控性强：支持多个自定义参数，播放功能 ui颜色均可自定义
- 通用性强：可用于任何html项目中
---  
# 使用方式：  
1. 在`<head>`标签中引入css与js文件  
```
<link rel="stylesheet" href="https://npm.webcache.cn/wpwebplayer@1.0.1/min-css.css">     
<script src="https://npm.webcache.cn/wpwebplayer@1.0.1/min-js.js"></script>
```
2. 在`<body>`中使用`<wp-music-player>`标签  
```
    <wp-music-player 
    src="" 
    title="" 
    artist=""
    cover=""
    autoplay="true"
    loop="true"
    volume="0.3"
    fixed="true"
    mini="true"
    theme="#ff6b6b">
  </wp-music-player>
```
（代码示例请前往[example.html](https://github.com/yunsen2025/WPwebplayer/blob/main/example.html))
---
# 参数说明
| 属性         | 类型                   | 说明                |
| ---------- | -------------------- | ----------------- |
| `src`      | string               | 音频地址              |
| `title`    | string               | 歌曲标题              |
| `artist`   | string               | 作者           |
| `cover`    | string               | 封面图片地址            |
| `autoplay` | `true` / `false` | 是否自动播放（默认 false）  |
| `loop`     | `true` / `false` | 是否循环播放（默认 true）   |
| `volume`   | 0\~1                 | 初始音量              |
| `fixed`    | `true` / `false` | 是否固定样式            |
| `mini`     | `true` / `false` | 是否迷你样式            |
| `theme`    | 色值                   | 主题颜色，例如 `#00c3ff` |
## 说明
- src&cover：均需将图片上传至图床并引用
- autoplay：参数失效 浏览器安全策略禁止未经允许的音频自动播放[Chrome 中的自动播放政策](https://developer.chrome.com/blog/autoplay?hl=zh-cn)（需要用户手动操作后才能播放）
- volume：0~1对应0%~100%
- fixed：使播放器始终固定在页脚，不会因页面滚动产生的相对位置变化影响播放器实际位置（默认为 true）
- mini：“迷你模式”和“完整模式”切换 完整模式支持更多功能（有bug 还没修）
- theme：主题颜色 默认为#00c3ff
