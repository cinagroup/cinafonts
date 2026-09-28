# CinaFonts 字历 · 开源中文字体展示

CinaFonts（字历）是**海内集团 CinaGroup** 推出的开源中文字体展示与试用作品。项目以网页字体排版出当日日期、干支、农历、二十四节气与十二生肖，让设计师与开发者在一张张字历中直接比较中文字体的排版效果。

本仓库是展示站的本地化版本：站点形象已按 [cinabrand](https://github.com/cinagroup/cinabrand) 品牌规范（v2.1.1 传承字标 + Geist）完成本地化，移除 Google 品牌元素，品牌 Logo 与字体资源均自仓库内置，不依赖运行时 CDN。

## 品牌本地化内容

- **品牌标识**：右上角固定「CinaFonts」字标（Geist 字体），右下角为海内集团传承字标，链接至 https://cinagroup.com/。
- **品牌颜色**：全站墨色由 `#222` 统一替换为品牌深蓝 `deepSea #123B56`；字标与装饰延续品牌青色渐变（`#5DBFE3 / #02A4DC / #44BBE3`）。
- **品牌资产**：Logo、favicon、apple-touch-icon 取自 `cinabrand` 的 `assets/`，随仓库固定版本使用。
- **依赖本地化**：jQuery 3.2.1 与 WebFont 1.6.26 已下载至 `third_party/`，页面不再请求 `ajax.googleapis.com`；代码块字体改用系统等宽字体，移除 Roboto Mono 外部依赖。
- **文案**：「关于」页说明、页面标题、作者署名均改为 CinaGroup 与项目描述。

> 说明：思源黑体（Noto Sans SC / TC）仍通过 `fonts.googleapis.com/earlyaccess` 按需加载——字体文件体积较大、仓库未内置，属于字库内容依赖而非品牌依赖；如需完全离线，可另行将 Noto Sans 字体文件放入 `/fonts` 并更新 `styles.css` 的 `@font-face`。

## 字历用法

- 默认繁体（TC），右上角可切换 简 / 繁。
- 页面右侧导航在 网站介绍 / 思源黑体 / 思源宋体 / 瀨戶字體 / 思源柔黑體 之间切换。
- 「使用字体」可查看每款字体的引用代码与说明。
- URL hash 支持 `#sc-NotoSerif-20260928` 这类深链。

## 收录字体与许可

| 字体 | 说明 | 许可 |
| --- | --- | --- |
| Noto Sans CJK（思源黑体） | Google 开源无衬线字体 | OFL 1.1 |
| Noto Serif CJK（思源宋体） | Google & Adobe 开源衬线字体 | OFL 1.1 |
| Seto Font（瀨戶字體） | 瀬戸のぞみ 手写字体 | 见 `/fonts/seto` |
| Gen Jyuu Gothic（思源柔黑體） | 自家製フォント工房 圆角字体 | SIL OFL 1.1 |
| HanaMin（花园明朝） | GlyphWiki 开源汉字字体 | 见 `/fonts/HanaMin` |

各字体以各自许可条款分发，详见 `/fonts` 下对应目录。

## 品牌与代码许可

- 本站代码与原项目一样以 Apache 2.0 许可分发（见 `LICENSE.txt`）。
- 品牌 Logo、图标与「CinaGroup / 海内集团」标识来自 [cinabrand](https://github.com/cinagroup/cinabrand)，使用须遵守 [BRAND_POLICY.md](BRAND_POLICY.md)。
- Geist 字体（`/fonts/geist`）为官方 v1.7.2 Regular，SIL OFL 1.1 许可，来源与校验值见 cinabrand `sources/fonts/geist/README.md`。

## 本地运行

直接双击打开 `index.html` 即可，无需构建步骤；建议在桌面端浏览器全屏查看。
