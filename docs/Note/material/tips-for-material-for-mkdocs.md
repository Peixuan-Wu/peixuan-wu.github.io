title: tips for material
# tips for material 
## [点击 installation](https://squidfunk.github.io/mkdocs-material/getting-started/)  
使用pip 可以将所有需要的插件 以及mkdocs依赖组件下载安装好

## [点击 creating your site](https://squidfunk.github.io/mkdocs-material/creating-your-site/)  
理清文件结构及作用，对于 `schema.json` 解释请参考[what is schema?](what-is-Json-Schema.md)  

## [点击 publishing your site](https://squidfunk.github.io/mkdocs-material/publishing-your-site/)  
### 什么是Github Actions？
可以帮助你自动化部署你的网站，需要在你仓库的根目录下创建`.github/workflows/ci.yml`

## 进阶
### customization 自定义
#### adding CSS
如果你想对于material这个主题进行微调，比如调整颜色或者一些组建的位置  
你可以在docs目录下添加一个`.CSS`格式的文件来记录你的微调
```
.
├─ docs/
│  └─ stylesheets/
│     └─ extra.css
└─ mkdocs.yml
```

#### adding JavaScript
如果你想要使得其他语言获得高亮，或者添加其他逻辑在你的主题中
可以添加JavaScript 文件在docs中  
```
.
├─ docs/
│  └─ javascripts/
│     └─ extra.js
└─ mkdocs.yml
```


