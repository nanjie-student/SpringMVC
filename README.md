# SpringMVC
# Handling Requests and Responses in Spring MVC
Use of Spring MVC in a Spring Boot Application
1.Scenario: “This Site Can’t Be Reached” Error When Accessing https://localhost
报错原因：出现这个现象，要么服务没启动，要么端口号不正确
在本次项目中，我们在application.properties中将系统默认的8080 修改成80 所以可以简写为localhost:/xxx

2.在pojo对象中，get对象不需要传参，如果传参数，会显示500错误
报错信息显示：No coverter found for return value of type: class com.cy.pj.module.pojo.ResponseResult

3.springmvc参数请求中，客户端向服务端提交请求的参数，服务器端没有取到这个参数
//(http://localhost/doParam01?name=mvcname)
public String doMethodParam02(RequestParameter param) 我们需要检查param有没有获取到参数，很可能url中的url与
RequestParameter中的SetName名字不一样，不匹配



