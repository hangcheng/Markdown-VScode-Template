### 水平线|分隔线

```markdown
--- 水平线|分隔线
```

_效果：_

---

### 标题

```markdown
# 一级标题

## 二级标题

### 三级标题

#### 四级标题

##### 五级标题

###### 六级标题
```

### 文本

#### 普通文本

> 不做任何修饰

_效果：_

这是一段普通的文本

### 单行代码

> 使用一对反引号，同样对单词或代码有高亮作用

```
`Hi，大家好，我叫杭杭！`
 `Hi`，大家好，我叫杭杭！我会`Java`、`Go`、`Rust`、`JS`等语言！
```

_效果：_
`Hi，大家好，我叫杭杭！`
`Hi`，大家好，我叫杭杭！我会`Java`、`Go`、`Rust`、`JS`等语言！

### 代码块

#### 语法 1

> 在连续几行的文本开头加入 1 个 Tab 或者 4 个空格

```
    Hi，大家好，我叫杭杭！
```

_效果：_

    Hi，大家好，我叫杭杭！

#### 语法 2

> 使用一对三反引号，常见场景为代码块展示，直接显示源码，在第一个三反引号后面加上语言名称即可展示对应代码风格，如常见的`java`、`go`、`rust`、`javascript`、`css`、`sh`、`bash`、`json`等

````
    ```
    Hi，大家好，我叫杭杭！
    ```
    ```json
    {
        "editor.quickSuggestions": {
            "strings": true
        },
        "editor.tabSize": 2,
        "editor.fontLigatures": true
    }
    ```
````

_效果：_

```
   Hi，大家好，我叫杭杭！
```

```json
{
  "editor.quickSuggestions": {
    "strings": true
  },
  "editor.tabSize": 2,
  "editor.fontLigatures": true
}
```

### 换行

- 直接回车不能换行，回车两次可以
- 可以在上一行文本后面补两个空格
- 在两行文本直接加一个空行,不过这个行间距有点大。
- `<br>` 使用 HTML 标签进行换行

### 斜体、粗体、删除线

> 斜体、粗体、删除线可混合使用

| 语法                      | 效果                     |
| ------------------------- | ------------------------ |
| `*斜体1*`                 | _斜体 1_                 |
| `_斜体2_`                 | _斜体 2_                 |
| `**粗体1**`               | **粗体 1**               |
| `__粗体2__`               | **粗体 2**               |
| `这是一个 ~~删除线~~`     | 这是一个 ~~删除线~~      |
| `***斜粗体1***`           | **_斜粗体 1_**           |
| `___斜粗体2___`           | **_斜粗体 2_**           |
| `***~~斜粗体删除线1~~***` | **_~~斜粗体删除线 1~~_** |
| `~~***斜粗体删除线2***~~` | ~~**_斜粗体删除线 2_**~~ |

### 图片

> 基本语法：

```
![alt](URL title)
```

- alt 和 title 即对应 HTML 中的 alt 和 title 属性（都可省略）：
  - alt 表示图片显示失败时的替换文本
  - title 表示鼠标悬停在图片时的显示文本（注意这里要加引号）
  - URL 即图片的 url 地址，如果引用本仓库中的图片，直接使用**相对路径**就可了，如果引用其他 github 仓库中的图片要注意格式，即：`仓库地址/raw/分支名/图片路径`，如：`https://avatars.githubusercontent.com/u/1124304?s=96&v=4`

```
![baidu](https://www.baidu.com/img/bdlogo.gif '百度logo')
```

_效果：_

![baidu](https://www.baidu.com/img/bdlogo.gif '百度logo')

```
![baidu](https://www.baidu.com/img/bdlogo.gif)
```

_效果：_

![baidu](https://www.baidu.com/img/bdlogo.gif)

### 链接

#### 链接外部 URL

```
[我的Github](https://github.com/hangcheng "悬停显示")
```

_效果：_
[我的 Github](https://github.com/hangcheng '悬停显示')

```
[我的 Github][github]
```

> 此种语法适合重复引用，与定义变量有异曲同工之妙,建议定义在文件末尾！语法: eg：`[github]: https://github.com/hangcheng '我的Github'`

_效果：_
[我的 Github][github]

#### 链接本仓库里的 URL

```
[模板](/template/index.md)
```

_效果：_

[模板](/template/index.md)

#### 图片链接

> 给图片加链接的本质是混合图片显示语法和普通的链接语法。普通的链接中[ ]内部是链接要显示的文本，而图片链接[ ]里面则是要显示的图片。直接混合两种语法当然可以，但是显得很乱，为此我们可以使用 URL 标识符的形式。

```
[![baidu](https://www.baidu.com/img/bdlogo.gif)](https://www.baidu.com)
```

_效果：_
[![baidu](https://www.baidu.com/img/bdlogo.gif)](https://www.baidu.com)

> 代码过长杂乱 我们优化一下

```
[![baidu_logo]][baidu_url]
```

_效果：_
[![baidu_logo]][baidu_url]

### 锚点

> 每一个标题都是一个锚点，和 HTML 的锚点（`#`）类似！注意，标题中的英文字母都被转化为*小写字母*了。

```
[回到顶部](#关于)
```

_效果：_
[回到顶部](#关于)

### 列表

#### 无序列表

> 可以使用 `-`和`*` 建议使用`-`

```
- 姓名
- 性别
- 年龄

OR

* 姓名
* 性别
* 年龄
```

_效果：_

- 姓名
- 性别
- 年龄

#### 无序列表多级嵌套

```
- 编程语言
  - 前端
    - JavaScript
    - CSS
  - 后端
    - Java
    - Go
```

_效果：_

- 编程语言
  - 前端
    - JavaScript
    - CSS
  - 后端
    - Java
    - Go

#### 有序列表

> 在数字后面加一个点（半角英文），再加一个空格。。

```
编程语言：
1. Java
2. Go
3. JavaScript
4. CSS
```

_效果：_

编程语言：

1. Java
2. Go
3. JavaScript
4. CSS

#### 有序列表多级嵌套

> 和无序列表一样，有序列表也可以多级嵌套。建议使用`Tab`进行分级,使用空格不一致就会错乱

```
1. 编程语言
   1. 前端
      1. JavaScript
      2. CSS
   2. 后端
      1. Java
      2. Go
```

_效果：_

1. 编程语言
   1. 前端
      1. JavaScript
      2. CSS
   2. 后端
      1. Java
      2. Go

#### 定义列表

> 类似 HTML 中 `<dl><dt><dd>`结构

```
定义列表
: 列表 1
: 列表 2
```

_效果：_

定义列表
: 列表 1
: 列表 2

### 任务列表｜复选框

```
- [x] 已完成任务
- [ ] 未完成任务
```

_效果：_

- [x] 已完成任务
- [ ] 未完成任务

### 引用块

```
> 引用块
```

_效果：_

> 引用块

#### 引用块多级嵌套

```
> 引用块
>
> > 二级引用块
> >
> > > 三级引用块
> > >
> > > > 四级引用块
> > > >
> > > > > 五级引用块
```

_效果：_

> 引用块
>
> > 二级引用块
> >
> > > 三级引用块
> > >
> > > > 四级引用块
> > > >
> > > > > 五级引用块

### 表格

> 表格单元中的内容可以和其他大多数 GFM 语法配合使用

```
| 表头 1   | 表头 2   |
| -------- | -------- |
| 表格单元 | 表格单元 |
| 表格单元 | 表格单元 |
```

_效果：_
| 表头 1 | 表头 2 |
| -------- | -------- |
| 表格单元 | 表格单元 |
| 表格单元 | 表格单元 |

#### 对齐

> 表格可以指定对齐方式 `:`在哪边就是哪边对齐 两头都有`:`是居中

```
| 左对齐            |     居中     |       右对齐 |
| :---------------- | :----------: | -----------: |
| Content Cell  | Content Cell | Content Cell |
| Content Cell  | Content Cell | Content Cell |
| Content Cell  | Content Cell | Content Cell |
```

_效果：_

| 左对齐       |     居中     |       右对齐 |
| :----------- | :----------: | -----------: |
| Content Cell | Content Cell | Content Cell |
| Content Cell | Content Cell | Content Cell |
| Content Cell | Content Cell | Content Cell |

### 表情

> Github 的 Markdown 语法支持添加 emoji 表情，输入不同的符号码（两个冒号包围的字符）可以显示出不同的表情。

比如`:blush:`，可以显示:blush:。

具体每一个表情的符号码，可以查询 GitHub 的官方网页[http://www.emoji-cheat-sheet.com](http://www.emoji-cheat-sheet.com)。

但是这个网页每次都打开**奇慢**。。所以我整理到了本 repo 中，大家可以直接在此查看[emoji](./emoji.md)。

### diff 语法

> 版本控制的系统中都少不了 diff 的功能，即展示一个文件内容的增加与删除
> GFM 中可以显示的展示 diff 效果。使用绿色表示新增，红色表示删除。

> 其语法与代码高亮类似，只是在三个反引号后面写 diff，
> 并且其内容中，可以用 `+ `开头表示新增，`- `开头表示删除。
> 另外还有有 `!`和`#`的语法。

````
    ```diff
    + 增加一行代码
    - 删除一行代码
    ! 代码警告
    # 注释代码
    ```
````

_效果：_

```diff
+ 增加一行代码
- 删除一行代码
! 代码警告
# 注释代码
```

### 常用 HTML 语法

> markdown 是支持 HTML 语法的，虽然不鼓励大量使用 HTML 语法，毕竟那样就丧失了 markdown 的意义，但是有一些 HTML 语法在写 README 的时候是很少的补充。

#### 折叠

```
<details>
<summary>折叠</summary>
    <p>Content 1 Content 1 Content 1 Content 1 Content 1</p>
</details>
```

_效果：_

<details>
<summary>折叠</summary>
    <p>Content 1 Content 1 Content 1 Content 1 Content 1</p>
</details>

#### 居中

> 很多地方都会用到居中的效果，比如标题居中

```
#### <center>标题居中</center>
```

_效果：_

#### <center>标题居中</center>

### 脚注

> 与 上述引用相似 但必须使用`^`开头后面跟上数字或字母不能有空格，数字是因为好记或者英文字母 注：如果使用英文字母默认转为数字

```
这是一个脚注使用例子 [^1]
```

_效果：_
这是一个脚注使用例子 [^1]

### 徽章

> 绘制徽章，首选就是[shields.io](https://shields.io/) 具体语法去官网探索。

```
![LICENSE](https://img.shields.io/badge/license-MIT-green)
```

_效果：_
![LICENSE](https://img.shields.io/badge/license-MIT-green)

### 热键

```
<kbd>⌘F</kbd>
```

_效果：_
<kbd>⌘F</kbd>

#### 热键列表

| Key       | Symbol |
| --------- | ------ |
| Option    | ⌥      |
| Control   | ⌃      |
| Command   | ⌘      |
| Shift     | ⇧      |
| Caps Lock | ⇪      |
| Tab       | ⇥      |
| Esc       | ⎋      |
| Power     | ⌽      |
| Return    | ↩      |
| Delete    | ⌫      |
| Up        | ↑      |
| Down      | ↓      |
| Left      | ←      |
| Right     | →      |

### star 历史

> star 历史可以使用这个网站[star-history.com](https://star-history.com/)

```
[![Star History Chart](https://api.star-history.com/svg?repos=hangcheng/Markdown-VScode-Template.git&type=Date)](https://star-history.com/#hangcheng/Markdown-VScode-Template.git&Date)
```

_效果：_

[![Star History Chart](https://api.star-history.com/svg?repos=hangcheng/Markdown-VScode-Template.git&type=Date)](https://star-history.com/#hangcheng/Markdown-VScode-Template.git&Date)


[github]: https://github.com/hangcheng '我的Github'
[baidu_logo]: https://www.baidu.com/img/bdlogo.gif
[baidu_url]: https://www.baidu.com

[^1]: 这是脚注