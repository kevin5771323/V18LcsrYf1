## 前言

欢迎来到宿舍管理系统小程序项目，该项目是基于SSM框架开发的，旨在为高校宿舍管理提供便捷、高效的服务。通过本系统，可以实现宿舍分配、维修、考勤等功能的在线操作，提高宿舍管理的效率。以下将为您详细介绍本项目的相关内容。

## 内容介绍

宿舍管理系统小程序主要包括以下功能模块：宿舍分配、宿舍维修、宿舍考勤、公告通知等。系统采用前后端分离的开发模式，前端负责展示页面及交互，后端负责数据处理与业务逻辑。通过微信小程序，学生和管理员可以随时随地查看宿舍相关信息，实现便捷的宿舍管理。

## 技术介绍

- **语言**：Java
- **使用框架**：Spring、Springmvc、MyBatis、微信小程序
- **前端技术**：JS、Vue、CSS3、Uniapp
- **开发工具**：IDEA/Eclipse、Uniapp
- **数据库**：MySQL 5.7/8.0
- **数据库管理工具**：phpstudy/Navicat
- **JDK版本**：jdk1.8
- **Maven**：apache-maven 3.8.1-bin
- **前端环境**：Node.Js 12\14\16

## 核心代码

以下为宿舍管理系统中的一小段核心代码，展示了如何通过MyBatis实现宿舍分配功能：

```java
// 宿舍分配接口
public interface DormitoryMapper {
    // 查询空闲宿舍
    List<Dormitory> selectFreeDormitory();
    
    // 分配宿舍
    int allocateDormitory(@Param("dormitoryId") int dormitoryId, @Param("studentId") int studentId);
}

// 宿舍分配Mapper.xml
<mapper namespace="com.example.mapper.DormitoryMapper">
    <!-- 查询空闲宿舍 -->
    <select id="selectFreeDormitory" resultType="com.example.entity.Dormitory">
        SELECT * FROM dormitory WHERE status = 0
    </select>
    
    <!-- 分配宿舍 -->
    <update id="allocateDormitory">
        UPDATE dormitory SET status = 1, student_id = #{studentId} WHERE id = #{dormitoryId}
    </update>
</mapper>
```

## 免费源码获取

```
5000套系统成品在线演示视频，复制到流浪器： 
```
```
https://www.yuque.com/yuqueyonghux32e1j/kxdc9g/ad8oz3bamkxmay0e#Cxun
```
![下载](https://img12.360buyimg.com/ddimg/jfs/t1/339687/11/1349/28408/68ad865fF412d7877/adaa650483a100f2.jpg)

## 项目截图
![封面图片](https://img10.360buyimg.com/ddimg/jfs/t1/342609/23/3063/188175/68c57086F2bc1df56/3cb579b1611f9514.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/338596/29/10369/45712/68c5705eFda3e380a/ed2765d18c205a6f.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/326206/27/19687/37218/68c5705eF7647c85a/8665aafef0b87697.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/350317/15/2980/43566/68c5705eF1af824f1/81993ae42e868310.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/346880/38/3000/52297/68c5705fFdd0913be/97ac2d341c59e0b9.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/336240/10/10330/22778/68c5705fF283282c1/f6610a4e86a5ff37.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/332044/37/12921/51840/68c57060Fa2fd0a71/88f43ad4719df855.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/328588/19/19639/147283/68c57060F78c743bc/e9ad1d2c4483868b.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/328741/29/19603/51763/68c57060Fa593ed7c/101c4b81854382ae.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/341578/35/2527/22186/68c57061F0f8e35b4/cf31cd760c3a36ed.jpg)


## 万字文档
![文档介绍](https://img14.360buyimg.com/ddimg/jfs/t1/338393/1/3576/156947/68b1ad0cF74dc525c/ff9cd6c574295685.jpg)
