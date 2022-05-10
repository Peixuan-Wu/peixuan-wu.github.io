# **what is Schema?**
 在学习**Material for Mk Docs**的时候，官方手册中提示我们可以设置
 **schema.json**进行**configuration validation and auto-complete**
 在VScode的settings中可以进行这样设定

 ```json
 { 
  "yaml.schemas": {
    "https://squidfunk.github.io/mkdocs-material/schema.json": "mkdocs.yml"
    }
 }
 ```

要知道什么是**schema**我们首先要知道什么是**json**，如上段代码所示就是一个标准的json结构；
简单的来说在**中括号包裹起来**的结构代表了Json中的**对象**的概念，其实可以看成是Python中的字典结构。

以下是json和pyhton的类比概念


json | python
:--- | ---:
string | string
number | int/float
object | dict
array  | list
boolean| bool
null   | None


比如我们想要描述一个人
```json
{
    "name": "George Washington",
    "birthday": "February 22, 1732",
    "address": "Mount Vernon, Virginia, United States"
}
```

json简单明了的表达对象的属性，但是当计算程序执行并向你请求一个对象的记录时，你交给计算机的json文件需要有一个正确的表达结构，比如我们不能将 `name 赋值为 123` 也不能将`birthday 赋值为一串字符串`计算机在接受复杂格式文件时会去验证你所赋值的结构的正确性。

这时候Schema Json可以来帮助计算机进行验证

例如以下的schema：
```json
{
    "type": "object",
    "properties": {
    "first_name": { "type": "string" },
    "last_name": { "type": "string" },
    "birthday": { "type": "string", "format": "date" }
    }
}
```
可以看出Schema json本质也是json格式编写的，没错，它之时一种声明性的格式来告诉计算机
**“其他文件的结构是怎么组织的的”** 一旦我们把非"string"类型的值赋给"name"时，计算机对于
你所给出的json文件就会验证失败。

**最后**
Material for Mk Docs作者给出了这一设定相当与给**mkdocs.yml**这一文件设置一种schema（中文译作：图解，结构解）,这样当我们在设置yml文件中的feature时，计算机会判断我们的输入是否正确，比如
出现`name 赋值为 123`的情况会报错等（这一步即为Schema的validation功能）。当然最方便的功能时通过设置Schema实现auto-complete功能，即当写下**birthday：** 时程序会自动弹出年月日供我们选择，
更加实例的来讲当写下**color:**时程序会自动弹出红黄绿供我们选择

这一切都归功于作者设置的**yaml.Schema for mkdocs.yml**

更加详细的解释参考：
[what is a schema?](https://json-schema.org/understanding-json-schema/about.html)

**本文如有错误请指出，谢谢（^_^）！**
