<h1 align="center">Markdown Nice 旧版</h1>

## 简介

本项目基于 [markdown-nice](https://github.com/mdnice/markdown-nice) 进行二次开发，再次对原项目所有贡献者表示感谢🙏

- 保留原项目所有功能
- 去除登录及主题商店功能
- 去除版本更新提示
- 修复部分主题图片无法正常加载
- 调整主题菜单项顺序
- 调整默认代码主题为 ***atom-one-dark***，并默认开启 ***Mac 风格*** 配置
- 新增主题 「极简黑」，「凝夜紫」

> 有疑问请参考 [如何有效的解决 mdnice 相关问题？](https://github.com/mdnice/markdown-nice/issues/163)

## 部署

可以选择下载整个项目，自行编译，也可以只下载  mdnice.zip 然后直接上传到网站根目录下直接使用。

## 主题


阿喵我自定义的主题css如下

### 预览图
![image](https://github.com/user-attachments/assets/c04eaf46-0ee0-42e1-ac94-ddaa2e439a4c)


### CSS代码
```css

/* 全局属性
 * 页边距 padding: 30px;
 * 全文字体 font-family: ptima-Regular;
 * 英文换行 word-break: break-all;
 */


#nice {
  line-height: 1.75;
  color: #595959;
  letter-spacing:2px;
  font-family: LXGW WenKai;
  
  background-image: linear-gradient(90deg, rgba(50, 0, 0, 0.05) 3%, rgba(0, 0, 0, 0) 3%), linear-gradient(360deg, rgba(50, 0, 0, 0.05) 3%, rgba(0, 0, 0, 0) 3%);
  background-size: 20px 20px;
  background-position:center center;
}




/* 段落，下方未标注标签参数均同此处
 * 上边距 margin-top: 5px;
 * 下边距 margin-bottom: 5px;
 * 行高 line-height: 26px;
 * 对齐 text-align: left;
 * 颜色 color: #3e3e3e;
 * 字体大小 font-size: 14px;
 * 首行缩进 text-indent: 2em;
 */



#nice p {
  font-size: 15px;
  word-spacing: 3px;
  letter-spacing: 2px
}
/* 一级标题 */
#nice h1 {  
  color: RGB(242,121,121);
}

/* 一级标题内容 */
#nice h1 .content {
  font-size: 25px;
  border-bottom: 2px solid RGB(242,121,121);
}

/* 二级标题 */
#nice h2 {
}
/* 二级标题内容 */
#nice h2 .content {
  background-color: RGB(242,121,128);
  color: #FFF;
  padding: 1px 11px;
  border-radius: 3px;
}
/* 二级标题修饰 请参考有实例的主题 */
#nice h2:after {
}

/* 三级标题 */
#nice h3 {
  font-size: 16px;
  font-weight: bold;
  text-align: center;
}

/* 三级标题内容 */
#nice h3 .content {
  
  font-size: 18px;
  color: #595959;
  border-bottom: 1px solid RGB(242,121,121);
}

/* 三级标题修饰 请参考有实例的主题 */
#nice h3:after {}

/* 无序列表整体样式
 * list-style-type: square|circle|disc;
 */
#nice ul {
}
/* 有序列表整体样式
 * list-style-type: upper-roman|lower-greek|lower-alpha;
 */
#nice ol {
}
/* 列表内容，不要设置li
 */
#nice li section {
}
/* 引用
   * 左边缘颜色 border-left-color:black;
   * 背景色 background:gray;
   */
#nice .multiquote-1 {
    font-style: normal;
    border-left: none;
    padding: 1px 1px;
    line-height: 1.75;
    border-radius: 4px;
    color: #353535;
    background: #f5f5f5;
}

#nice .multiquote-1:before {
    content: "”";
    display: block;
    font-size: 2em;
    color: rgb(248, 57, 41);
    font-family: Arial, serif;
    line-height: 1em;
    font-weight: 700;
}

/* 引用文字 */
#nice .multiquote-1 p {
    color: #353535;
    font-size: 16px;
    margin: 0 10px;
    display: block;
}

#nice .multiquote-1:after {
    content: "”";
    float: right;
    display: block;
    font-size: 2em;
    color: rgb(248, 57, 41);
    font-family: Arial, serif;
    line-height: 1em;
    font-weight: 700;
}



/* 链接 
 * border-bottom: 1px solid #009688;
 */
#nice a {
}
/* 加粗 */
#nice strong {
  color: #3594F7;
  font-weight: bold;
}

#nice strong::after {
  content: '';
}

/* 斜体 */
#nice em {
  font-style: normal;
  color: #3594F7;
  font-weight:bold;
}

/* 加粗斜体 */
#nice em strong {
  color: #3594F7;
}

/* 删除线 */
#nice del {
  color: #3594F7;
}


/* 分隔线
* 粗细、样式和颜色
* border-top: 1px solid #3e3e3e;
*/
#nice hr {
  border-top: 1px dashed #dddddd;
}
/* 图片
* 宽度 width: 80%;
* 居中 margin: 0 auto;
* 居左 margin: 0 0;
*/
#nice img {
  border-radius: 10px;
  border: 1px solid #F27979;
}
/* 图片描述文字 */
#nice figcaption {
}
/* 行内代码 */
#nice p code, #nice li code {
}
/* 非微信代码块
 * 代码块不换行 display: -webkit-box !important;
 * 代码块换行 display: block;
 */
#nice pre code {
}
/*
   * 表格内的单元格
   * 字体大小 font-size: 16px;
   * 边框 border: 1px solid #ccc;
   * 内边距 padding: 5px 10px;
   */
#nice table tr th,
#nice table tr td {
    font-size: 16px;
    color: #645647;
}

#nice table tr th {
    color: #353535;
    background-color: #dbd9d8;
}

#nice .footnotes {
    font-size: 16px;
}
/* 脚注文字 */
#nice .footnote-word {
}
/* 脚注上标 */
#nice .footnote-ref {
}
/* "参考资料"四个字 
 * 内容 content: "参考资料";
 */
#nice .footnotes-sep:before {
}
/* 参考资料编号 */
#nice .footnote-num {
}
/* 参考资料文字 */
#nice .footnote-item p { 
}
/* 参考资料解释 */
#nice .footnote-item p em {
}
/* 行间公式
 * 最大宽度 max-width: 300% !important;
 */
#nice .block-equation svg {
}
/* 行内公式
 */


```
### 内置主题
目前内置原版所有主题，可在编辑器页面顶部主题菜单中查看，如下所示：

- 默认主题 `@zhning12`
- 山吹 `@ElyhG`
- [蔷薇紫](https://mp.weixin.qq.com/s/x0xqSpQixW2xj5qXCgWSyA) `@HeyRain`
- [全栈蓝](https://mp.weixin.qq.com/s/_lO3cd0FcF0Dg3TRnHPdwg) `@Nealyang`
- [凝夜紫](https://mp.weixin.qq.com/s/0IDhUGxZtMDFGD-Z9Ij_Cg) `@童欧巴` : 适配微信以及Safari的深色模式。“凝夜紫”，寓意在深色模式中也可以发光。
- [萌绿](https://mp.weixin.qq.com/s/iK3r9I28NMWApEydH046-w) `@koala`
- [极简黑](https://mp.weixin.qq.com/s/6UQmAhyXQY6AaYcyd1npIg) `@小鱼` : 公众号自律神仙ScarSu同款~
- [橙心](https://mp.weixin.qq.com/s?__biz=MzIwNTA4NzI1Mw==&mid=2247485062&amp;idx=1&amp;sn=0eaa314bb165c71a8f57c8baf4226f57&source=41#wechat_redirect) `@zhning12`
- 墨黑 `@May和ev`
- 姹紫 `@djmaxwow`
- [绿意](https://mp.weixin.qq.com/s/gpancJ62Dkd4ccXzFg2g5Q) `@夜尽天明`
- 嫩青 `@画手`
- [WeChat-Format](https://mp.weixin.qq.com/s?__biz=MzIwNTA4NzI1Mw==&mid=2247485061&amp;idx=1&amp;sn=36047ec080d1daaf63d733d18e546ba7&source=41#wechat_redirect) `@画手`
- [兰青](https://mp.weixin.qq.com/s/iL8xlH0I3yOEOrhcBqc0kg) `@Krahets`
- [前端之巅同款](https://mp.weixin.qq.com/s/sSJwPflpzan1R_7kmBRwmQ) `@HeyRain`
- 极客黑 `@hyper-xx`
- 红绯 `@HeyRain`
- [蓝莹](https://mp.weixin.qq.com/s/OfRQaBe3XVXXjE7f84nSwA) `@谭淞宸`
- [科技蓝](https://mp.weixin.qq.com/s/hEQA4GEFycBjvScko4DeqQ) `@夜尽天明`
- [简](https://mp.weixin.qq.com/s/JawcVvG_y8igDK5reRDktg) `@aco`
