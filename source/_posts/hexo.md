---
title: hexo config
categories: 666
abbrlink: 5e1b6d3c
---

你可以直接在文章的front-matter区域里添加sticky: 1属性来把这篇文章置顶。数值越大，置顶的优先级越大。

如果不要显示顶部图，可直接配置 disable_top_img: true。

配置解释
index_img 主页的 top_img
default_top_img 默认的 top_img，当页面的 top_img 没有配置时，会显示 default_top_img
archive_img 归档页面的 top_img
tag_img tag子页面 的 默认 top_img
tag_per_img tag子页面的 top_img，可配置每个 tag 的 top_img
category_img category 子页面 的 默认 top_img
category_per_img category 子页面的 top_img，可配置每个 category 的 top_img
其它页面 （tags/categories/自建页面）和文章页的top_img，请到对应的 md 页面设置front-matter中的top_img。

你可以直接在文章的front-matter区域里添加sticky: 1属性来把这篇文章置顶。数值越大，置顶的优先级越大。
文章的markdown文档上，在Front-matter添加cover，并填上要显示的图片地址。如果不配置cover，可以设置显示默认的cover；如果不想在首页显示cover，可以设置为false。

## pdf

```
# 1.本地文件:在md文件路径下创建一个同名文件夹，其内放pdf文件名为xxx.pdf的文件
{% pdf xxx.pdf %}
# 2.在线链接
{% pdf https://cdn.jsdelivr.net/gh/Justlovesmile/CDN/pdf/小作文讲义.pdf %}
```

1. 带 {% u 下划线 %} 的文本
2. 带 {% emp 着重号 %} 的文本
3. 带 {% wavy 波浪线 %} 的文本
4. 带 {% del 删除线 %} 的文本
5. 键盘样式的文本 {% kbd command %} + {% kbd D %}
6. 密码样式的文本：{% psw 这里没有验证码 %}

{% tip warning faa-horizontal animated %}warning{% endtip %}
{% tip ban faa-flash animated %}ban{% endtip %}
