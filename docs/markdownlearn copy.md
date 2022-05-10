title: markdown
# <b>Markdown 学习笔记<b><!-- omit in toc -->
- [Basic Syntax](#basic-syntax)
- [Extended Syntax](#extended-syntax)

## Basic Syntax

**1.标题**: heading

`# H1 `  一级标题  
`## H2`  二级标题  
`### H3` 三级标题  

**2.加粗**: `**bold text**`  
效果:  
**bold text**

**3.斜体**: `*italicized*`  
效果:  
*italicized*

**4.引用**: `> 这是一段引用。`  
效果:  
>这是一段引用。

**5.有序列表**:  直接在文本前面加上序号  
1.first item  
2.seconde item  
3.third item  

**6.无序列表**: 在文本签加上hyphen`-`  
- First item  
- Second item  
- Third item  

**7.代码块**: \` code \`  
效果: `code`

**8.水平分割线**: 注意分隔线上下空一行，否则会显示为heading
```
Try to put a blank line before...

---

...and after a horizontal rule.
```  
效果:
Try to put a blank line before...

---

...and after a horizontal rule.

**9.链接**:
```
[peixuan-wu's website](https://peixuan-wu.github.io/)
```  
效果:  
[peixuan-wu's website](https://peixuan-wu.github.io/)

**10.图像**:
```
![alt text](https://myoctocat.com/assets/images/base-octocat.svg)
```
效果:  
![alt text](https://myoctocat.com/assets/images/base-octocat.svg)

## Extended Syntax

**1.表格**: 
```
| Syntax | Description |
| ----------- | ----------- |
| Header | Title |
| Paragraph | Text |
```  
效果:  
>注意表格前需要空一行

| Syntax | Description |
| ----------- | ----------- |
| Header | Title |
| Paragraph | Text |

**2.大代码块**:  使用三个` ``` `号包裹代码块
```
/```
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
/```
```  
效果:  
```
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

**3.脚注**:

Here's a simple footnote,[^1] and here's a longer one.[^bignote]

[^1]: This is the first footnote.











