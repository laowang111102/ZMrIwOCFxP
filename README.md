## 前言

本项目是基于Spring Boot和MySQL开发的古典舞在线交流平台，适用于计算机专业毕业设计和实战项目。平台提供了用户注册、登录、发布动态、评论、点赞、搜索、私信、舞蹈教程分享等功能，为古典舞爱好者提供一个便捷的在线交流和学习空间。项目采用Java语言，结合Spring Boot框架，实现高效、稳定的系统运行。前端部分使用Vue.js、CSS3等技术，提供了良好的用户体验。以下为项目详细介绍。

## 内容介绍

古典舞在线交流平台是一个专为古典舞爱好者设计的在线平台，用户可以在这里发布舞蹈动态，与其他用户互动，交流舞蹈心得。平台包括用户管理、动态管理、评论管理、私信等功能，用户可以方便地上传舞蹈视频、教程等资源，分享给其他用户。此外，平台还提供了搜索功能，用户可以通过关键词搜索相关动态和用户，便于发现更多有趣的舞蹈内容。项目采用Java语言开发，前端部分使用Vue.js、CSS3等技术，提供了良好的用户体验。项目代码清晰规范，易于理解与二次开发。

## 技术介绍

- **语言**：Java
- **使用框架**：Spring Boot
- **前端技术**：JS、Vue、CSS3
- **开发工具**：IDEA/Eclipse
- **数据库**：MySQL 5.7/8.0
- **数据库管理工具**：phpstudy/Navicat
- **JDK版本**：jdk1.8
- **Maven**：apache-maven 3.8.1-bin
- **前端环境**：Node.js 12\14\16

## 核心代码

```java
@RestController
@RequestMapping("/user")
public class UserController {

    @Autowired
    private UserService userService;

    @Autowired
    private UserMapper userMapper;

    @PostMapping("/register")
    public String register(@RequestBody User user) {
        boolean result = userService.register(user);
        if (result) {
            return "注册成功";
        } else {
            return "注册失败";
        }
    }

    @PostMapping("/login")
    public String login(@RequestBody User user) {
        User u = userMapper.login(user.getUsername(), user.getPassword());
        if (u != null) {
            return "登录成功";
        } else {
            return "登录失败";
        }
    }
}
```

## 免费源码获取

```
8000套系统成品在线演示视频，复制到流浪器： 
```
```
https://www.yuque.com/yuqueyonghux32e1j/kxdc9g/ad8oz3bamkxmay0e#Cxun
```
![下载](https://img12.360buyimg.com/ddimg/jfs/t1/339687/11/1349/28408/68ad865fF412d7877/adaa650483a100f2.jpg)

# 项目截图

![封面图片](https://img14.360buyimg.com/ddimg/jfs/t1/326427/35/4196/109601/689c8dddFd14bcfd8/81e3e866a6f61d1f.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/289989/4/5684/51171/689c8db8Fafed2046/d074b0bf8d373766.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/291102/3/26537/37947/689c8db8F520f6af7/1c83cbde46326494.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/325286/40/4056/35809/689c8db9Fdcfc6a19/8983ef8ba0b80fd2.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/305597/15/26957/42194/689c8dbaF12545ba4/1562150e2869a87d.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/303620/25/27037/15464/689c8dbaFac4feec5/f100cb01a8ec8d30.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/324528/7/4159/61881/689c8dbbFa1176d80/d4a2f6a2e4da08bc.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/298482/19/7112/34567/689c8dbbFf4fdc17b/26062dc0f3b9cd5a.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/327571/24/4008/20193/689c8dbdFfcd5f947/6c5b1f8f67b67343.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/314415/39/26109/32865/689c8dbdF9ce64d01/cde5b08d0876d353.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/320039/7/24894/11647/689c8dbdF3c63c9a8/99437965d142f3d2.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/309569/24/26054/20398/689c8dbeF580e9492/015198c3aeb07039.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/303596/23/26843/62262/689c8dbfFf4e724e6/99f1bdd73fba2e7d.jpg)


## 万字文档
![文档介绍](https://img14.360buyimg.com/ddimg/jfs/t1/338393/1/3576/156947/68b1ad0cF74dc525c/ff9cd6c574295685.jpg)
