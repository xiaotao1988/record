## 第三节 关于cookie的问题
cookie 主要用于登录验证，提高用户体验。
在多个域名下只需要登录一次，想想就觉得很方便。
但是实现起来需要一些技巧，首先是跨域的问题， 
设置cookie 时候 加上 header(P3P;....) 便可以跨与写cookie ，
然后是隐藏提交iframe信息，在多个域名下redirect ，并将cookie种在对应的域名下。
以此来变相实现单点登录

#还有一种是 开源项目 CAS 想了解可以google下 这个项目
