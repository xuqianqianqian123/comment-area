# comment-area
## 环境依赖
vue<br>
element ui
## 网页简介
本页是一个评论区，提供一个交流的平台，在里面进行自由的讨论
## 功能说明
输入正确的名称（非空）、学号（不知道学校的学号要求是什么，所以暂时设定为13位数）和年龄（大于等于18），然后在评论区打出想要发表的言论即可发出。点击对应的评论可以进行回复。双击上方按钮可以切换主题颜色
## 代码实现
1、使用vue和element ui实现双击切换的功能<br>
2、JS函数：<br>
onload函数在网页加载完成后立即执行初始化评论initTreeComment，分为两种情况：无评论时调用nocomment函数，在页面中显示nocommnet；有评论时调用havecomment函数，会显示所有评论，同时会调用showbutton函数，当鼠标移到（onmouseover）评论人名字时会显示回复按钮<br>
renderReplyBar函数是渲染回复时的提示例如“还可以输入XX字符”“取消回复按钮”等<br>
submitTree函数内部嵌套sumitButton函数实现了用户评论的提交<br>
alarmIfEmpSpace函数对于不符合提交要求的评论将进行警告<br>
cancelReply函数实现当点击取消回复时相关的显示<br>
ifHaveReply函数在已经有回复时对评论的显示<br>
## 目录结构
├── Readme.md // help<br>
├── index.html<br>
├── vue.js
