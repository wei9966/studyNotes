request对象常用方法、应用
----------------
- 1. 什么是HttpServletRequest?
 `HttpServletRequest对象代表客户端的请求，当客户端通过HTTP协议访问服务器时`
`HTTP请求头中的所有信息都封装在这个对象中，开发人员通过这个对象的方法，可以获得客户这些信息	`

HttpServletRequest常用方法
------------------------
获得客户机【浏览器】信息
----------------------------------------
- 1.getRequestURL方法返回客户端发出请求时的完整URL。
- 2.getRequestURI方法返回请求行中的资源名部分。
- 3.getQueryString 方法返回请求行中的参数部分。
- 4.getPathInfo方法返回请求URL中的额外路径信息。额外路径信息是请求URL中的位于Servlet的路径之后和查询参数之前的内容，它以“/”开头。
- 5.getRemoteAddr方法返回发出请求的客户机的IP地址
- 6.getRemoteHost方法返回发出请求的客户机的完整主机名
- 7.getRemotePort方法返回客户机所使用的网络端口号
- 8.getLocalAddr方法返回WEB服务器的IP地址。
- 9.getLocalName方法返回WEB服务器的主机名

获得客户机请求头
--------
- getHeader方法
- getHeaders方法
- getHeaderNames方法
