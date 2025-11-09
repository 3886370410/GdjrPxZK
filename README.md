# 前言

欢迎来到基于SSM（Spring+SpringMVC+MyBatis）的宿舍管理系统设计与实现项目。本项目致力于为高校宿舍管理人员提供一套便捷、高效的管理工具，同时也为在校大学生提供一个舒适、和谐的居住环境。

# 内容介绍

本项目主要实现了以下功能：

1. 学生信息管理：包括学生基本信息录入、修改、查询和删除。
2. 宿舍楼信息管理：包括宿舍楼基本信息维护、宿舍房间分配与查询。
3. 缴费管理：实现宿舍水电费等费用的录入、查询和缴纳。
4. 报修管理：学生可以在线提交报修申请，管理员进行维修派单和处理。
5. 公告管理：管理员可以发布宿舍相关公告，方便学生及时了解宿舍动态。

# 技术介绍

- **语言：** Java
- **使用框架：** Spring、SpringMVC、MyBatis
- **前端技术：** JS、Vue、CSS3
- **开发工具：** IDEA/Eclipse
- **数据库：** MySQL 5.7/8.0
- **数据库管理工具：** phpstudy/Navicat
- **JDK版本：** jdk1.8
- **Maven：** apache-maven 3.8.1-bin
- **前端环境：** Node.Js 12\14\16

# 核心代码

以下是本项目中的一段核心代码，展示了如何通过MyBatis实现查询学生信息的功能：

```java
// StudentMapper.xml
<mapper namespace="com.example.dao.StudentMapper">
    <select id="selectStudentById" resultType="com.example.entity.Student">
        SELECT * FROM student WHERE id = #{id}
    </select>
</mapper>

// StudentMapper.java
public interface StudentMapper {
    Student selectStudentById(int id);
}

// StudentService.java
@Service
public class StudentService {
    @Autowired
    private StudentMapper studentMapper;

    public Student getStudentById(int id) {
        return studentMapper.selectStudentById(id);
    }
}
```

# 免费源码获取

```
5000套系统成品在线演示视频，复制到流浪器： 
```
```
https://www.yuque.com/yuqueyonghux32e1j/kxdc9g/ad8oz3bamkxmay0e#Cxun
```
![下载](https://img12.360buyimg.com/ddimg/jfs/t1/339687/11/1349/28408/68ad865fF412d7877/adaa650483a100f2.jpg)

# 项目截图

![封面图片](https://img14.360buyimg.com/ddimg/jfs/t1/349508/36/1953/168829/68c1bd4eFf00ef749/6063d75841fd076a.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/345643/21/1949/117203/68c1bd26F284ad9b3/b537febafc71fbb5.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/331882/13/11769/126531/68c1bd26F731fffba/c32f23aa1e4e4ae0.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/341756/16/1929/39033/68c1bd27F46bdde62/8001a65e66c948f1.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/343939/31/1738/78156/68c1bd27Fd0f451b8/4018500a3eb39b06.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/327775/6/18247/32296/68c1bd27F057bfd34/62b085bb6e3ea74e.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/323656/1/18384/42561/68c1bd28F299b629a/3a7e670e2324ab4c.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/342071/31/1923/25424/68c1bd28Fe1bb9c2f/3d3d04124dbe8acf.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/325670/26/18620/36377/68c1bd28F50dd0cad/08cc5ee1bfbd6728.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/344880/15/1992/34222/68c1bd29F6d572948/566b9635f967c2e1.jpg)

