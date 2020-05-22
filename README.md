# hexo-theme-lnzu
这是一个简约的hexo主题，慢慢完善吧，能力有限哈哈，目前还需要有更多修复完善的地方。

#### [主题项目地址](https://github.com/lnzu/hexo-theme-lnzu)

#### [预览地址](https://lnzu.github.io)

### 配置安装主题

#### 1.安装
```yaml
git clone https://github.com/lnzu/hexo-theme-lnzu themes/lnzu
```

#### 2.hexo站点配置文件下修改**_config.yml**
```yaml
theme: lnzu
```

#### 3.主题使用了**hexo-prism-plugin**插件高亮代码
安装插件
```bash
npm i -S hexo-prism-plugin
```
在hexo根目录下的**_config.yml**下修改
```yaml
highlight:
  enable: false
  line_number: false
  auto_detect: 
  tab_replace: ''
  wrap: true
  hljs: false

prism_plugin:
  mode: 'preprocess'    # realtime/preprocess
  theme: 'default'
  line_number: ture    # default false
  custom_css: 'path/to/your/custom.css' #此项不要修改
```

#### 4.标签云页
新建一个页面
```bash
hexo new page tags
```
打开hexo目录下**source/tags/index.md**修改如下
```yaml
---
title: tags
date: 2020-05-21 11:44:15
type: tags
---
```

#### 5.分类页
新建一个页面
```bash
hexo new page categories
```
打开hexo目录下**source/categories/index.md**修改如下
```yaml
---
title: categories
date: 2020-05-21 12:18:13
type: categories
---
```

#### 6.搜索页
新建一个页面
```bash
hexo new page search
```
打开hexo目录下**source/search/index.md**修改如下
```yaml
---
title: search
date: 2020-05-21 10:52:16
type: search
---
```

#### 7.主题下的_config.yml配置选项
```yaml
#主题风格样式 light dark
colorscheme: light

menu:
  home: /
  about: /about/
  search: /search
  tags: /tags
  categories: /categories
```







