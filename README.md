# `Markdown` 结合 `VSCode` 插件编辑文档模板

> 基于 VScode 编写 Markdown 文档的模板，默认设置对应插件，可直接参考复制模板编辑，提高编写效率！

## 关于

> `Markdown-VScode-Template` 以下简称 `MVSC`,`MVSC`该工程用来展示写 `README`或技术文档的各种 `Markdown` 语法与`VSCode`插件推荐。下载或 `clone`该工程即可编写文档，提高编写效率，已内置工作区推荐的插件及设置，无需额外安装对应插件！

> `GitHub` 的 `Markdown` 语法在标准的 `Markdown` 语法基础上做了扩充，称之为`GitHub Flavored Markdown`。简称`GFM`，`GFM` 在 `GitHub` 上有广泛应用，除了 `README` 文件外，`issues` 和 `wiki` 均支持 `Markdown` 语法。

## 默认配置的 `VScode` 插件

- `Markdown` 预览增强 `hd101wyy.markdown-preview-enhanced`
- `Markdown` 多合一 `yzhang.markdown-all-in-one`
- `Markdown` 格式化`esbenp.prettier-vscode`
- `Draw.io`插件 `hediet.vscode-drawio`
- `Draw.io`插入`mermaid`的插件 `nopeslide.vscode-drawio-plugin-mermaid`
- `Excalidraw` 插件 `pomdtr.excalidraw-editor`
- `PlantUML`插件 `jebbs.plantuml`
- `Mermaid` 插件 `bierner.markdown-mermaid`
- `Mermaid` 高亮插件 `bpruitt-goddard.mermaid-markdown-syntax-highlighting`

## `Markdown` 语法

> 完整 的 `Markdown` 语法 详见 `/template/index.md`

## 数学公式

> 完整 的 `Markdown` 数学公式语法 详见 `/template/index.md`

## 画图

### `Draw.io` 绘图

> 基于 `Draw.io VS Code Integration` 插件，可以把 `drawio` 绘图插入到 `Markdown`中，详见工程中示例

- 具体实现
  - 安装`Draw.io VS Code Integration`插件,基于此工程更顺利，已内置好配置
  - 在目录中建立 `*.drawio.svg` 或 `*.drawio.png` 文件，如：`test.drawio.svg` 双击打开便可以自由绘图, 与 `drawio`在线绘图或本地客户端绘图效果一样，无法这样是直接保存为图片模式
  - 在`Markdown`中 使用引用图片语法即可，如：`![测试](test.drawio.svg)`

### `Excalidraw` 白板

> `Excalidraw` 可以自由绘图，相比较 `Draw.io` 更自由一点，`Draw.io`更专业，都有自己的独特之处，选择适合自己的更重要
>
> 基于 `Excalidraw` 插件，可以自由绘图并插入到 `Markdown`中，详见工程中示例

- 具体实现
  - 安装`Excalidraw`插件,基于此工程更顺利，已内置好配置
  - 在目录中建立 `*.excalidraw.svg` 或 `*.excalidraw.png` 文件，如：`test.excalidraw.svg` 双击打开便可以自由绘图
  - 在`Markdown`中 使用引用图片语法即可，如：`![测试](test.excalidraw.svg)`

### `PlantUML` `UML`绘图

> 语法详见 [PlantUML](https://plantuml.com/zh/)
>
> 基于 `PlantUML`插件进行编辑 `UML`,如果离线操作需要安装`Java` 相关驱动,基于此工程更顺利，已内置好相关配置，在线服务
>
> `puml` 或者 `plantuml` 代码块中的内容将会被 `PlantUML` 渲染。
>
> 完整 的 `Markdown PlantUML` 示例 详见 `/template/index.md`

### `Mermaid` 绘图

> 官网[Mermaid](https://mermaid.js.org/) > `Mermaid` 是一个基于 JavaScript 的图表和图表工具，相比较`PlantUML`更友好，选择适合自己的即可，不满足需求可两者结合使用
>
> 安装`Markdown Preview Mermaid Support`和 `Mermaid Markdown Syntax Highlighting` 插件
>
> `mermaid` 代码块中的内容将会渲染 `mermaid` 图像。
>
> 完整 的 `Markdown Mermaid` 示例 详见 `/template/index.md`

### `WaveDrom` 绘图

> 官网 [WaveDrom](https://wavedrom.com/)
>
> `wavedrom` 代码块中的内容将会被 `WaveDrom` 渲染。
>
> 完整 的 `Markdown WaveDrom` 示例 详见 `/template/index.md`

### `GraphViz` 绘图

> 官网[GraphViz](https://viz-js.com/)
>
> `viz` 或者 `dot` 代码块中的内容将会被 `Viz.js` 渲染。  
> 你可以通过 `{engine="..."}` 来选择不同的渲染引擎。 引擎 `circo，dot，neato，osage`，或者 `twopi` 是被支持的。默认下，使用 `dot` 引擎。
>
> 完整 的 `Markdown GraphViz` 示例 详见 `/template/index.md`

### `Vega` 和 `Vega-lite` 图表

> 官网[Vega & Vega-Lite](https://vega.github.io/)
>
> `vega` 代码块中的内容将会被 `vega` 渲染。
> `vega-lite` 代码块中的内容将会被 `vega-lite` 渲染。
> `JSON` 以及 `YAML` 的输入是支持的。
>
> 完整 的 `Markdown Vega` 示例 详见 `/template/index.md`

## `Markdown` 拆分合并

> 基于 `Markdown Preview Enhanced` 插件可以进行 `Markdown` 拆分合并，解决`md` 文件过长过大但又必须在一起展示并导出的问题！

### 使用语法

```markdown
## 导入模板文件

@import "/template/index.md"
```

## `Markdown` 导出

> - 基于 `Markdown Preview Enhanced`插件预览后进行选择导出对应格式文件
> - princexml 模式导出
>   - 导出时先安装 [princexml](https://www.princexml.com/download/)
> - 如果不想安装`princexml`可直接选择 `chrome(Puppeteer)`模式导出
>   - 推荐`chrome(Puppeteer)`模式导出

## TOC 目录

> `Markdown` 顶部加入以下代码即可

```markdown
---
toc:
  depth_from: 1
  depth_to: 6
  ordered: false
---

[TOC]

标题不加入目录示例：

# 一级目录不展示在 TOC 中 {ignore=true}
```

- `orderedList` 是否使用有序列表。
- `depthFrom`, `depthTo [1~6]` 包含的。
- `ignoreLink` 如果设置为 `true`，那么 `TOC` 将不会被超链接。 即 标题后面加入 `{ignore=true}`

## 效果如下

![](template.png)

## 如有建议或想法请大家 issues
