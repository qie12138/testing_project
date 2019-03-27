# Header 1
## Header 2
### Header 3
#### Header 4
##### Header 5
###### Header 6

> This is a blockquote with two paragraphs. This is first paragraph.
>
> This is second pragraph.Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.

> This is another blockquote with one paragraph. There is three empty line to seperate two blockquote.

## un-ordered list
*   Red
*   Green
*   Blue

## ordered list
1.  Red
2.  Green
3.  Blue

### Task List
Task lists are lists with items marked as either [ ] or [x] (incomplete or complete). For example:

- [ ] a task list item
- [ ] list syntax required
- [ ] normal **formatting**, @mentions, #1234 refs
- [ ] incomplete
- [x] completed



```
function test() {
  console.log("notice the blank line before this function?");
}
```

syntax highlighting:
```ruby
require 'redcarpet'
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html
```

### Math Blocks

You can render LaTeX mathematical expressions using MathJax.

$$
\mathbf{V}_1 \times \mathbf{V}_2 =  \begin{vmatrix} 
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
\frac{\partial X}{\partial u} &  \frac{\partial Y}{\partial u} & 0 \\
\frac{\partial X}{\partial v} &  \frac{\partial Y}{\partial v} & 0 \\
\end{vmatrix}
$$

### Tables

| First Header  | Second Header |
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |

| Left-Aligned  | Center Aligned  | Right Aligned |
| :------------ |:---------------:| -----:|
| col 3 is      | some wordy text | $1600 |
| col 2 is      | centered        |   $12 |
| zebra stripes | are neat        |    $1 |

### Footnotes

[^footnote]: Here is the *text* of the **footnote**.

---

This is [an example](http://example.com/ "Title") inline link.

[This link](http://example.net/) has no title attribute.


### Strikethrough

**double asterisks**

### Emoji :happy:
哈哈哈哈 :smile:

### Subscript

H~2~O


### Superscript

X^2^

### Highlight

==highlight==

![task](https://img.shields.io/badge/type-task-yellow.svg) ![v1.0](https://img.shields.io/badge/version-1.0-green.svg) ![v1.0](https://img.shields.io/badge/state-done-blue.svg) ![task](https://img.shields.io/badge/type-task-yellow.svg)


- [ ] 学习DOM虚拟方法 <img src="https://img.shields.io/badge/done-green.svg"/> <img src="https://img.shields.io/badge/must-red.svg"/> <img src="https://img.shields.io/badge/201901011111-201902013322-yellow.svg"/>

