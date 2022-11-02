# 											front
## 整体使用效果：

### 登录页面MyLogin.vue

![image-20221101201740049](C:/Users/86189/AppData/Roaming/Typora/typora-user-images/image-20221101201740049.png)

简单登录页面（用的明码，没有设计具体安全性）

对应的MyLogin.vue

账号admin

密码123456

### 整体布局

![整体布局](../../../整体布局.png)

### 所有节点展示页面MyNodes.vue

![image-20221101202025208](C:/Users/86189/AppData/Roaming/Typora/typora-user-images/image-20221101202025208.png)

后续删除，这个功能有点鸡肋



### 流程选择页面MyProcessChoice.vue

![image-20221101201908651](C:/Users/86189/AppData/Roaming/Typora/typora-user-images/image-20221101201908651.png)

**tips.上下翻页功能方法没有实现**



#### 执行查询

![image-20221101202215301](C:/Users/86189/AppData/Roaming/Typora/typora-user-images/image-20221101202215301.png)

Mock中设置了选中Done，会响应测试样例

![image-20221101202311375](C:/Users/86189/AppData/Roaming/Typora/typora-user-images/image-20221101202311375.png)

#### 点击查看详情MyProcessDetail.vue

进入具体流程展示

![image-20221101202629130](C:/Users/86189/AppData/Roaming/Typora/typora-user-images/image-20221101202629130.png)

**0.通过给定的ExcetionId然后寻找对应的ProExcetions以及多份tasks，利用antvx6图像化，形成流程图**

![image-20221101203248408](C:/Users/86189/AppData/Roaming/Typora/typora-user-images/image-20221101203248408.png)

**1.查看所有节点信息功能不需要的话，后期可以改成查看某个部门节点信息**

**具体功能待实现**

![image-20221101203044249](C:/Users/86189/AppData/Roaming/Typora/typora-user-images/image-20221101203044249.png)

**2.运行流程Done进度条，可以删掉了如果和设计冲突的话**

**具体功能待实现**

![image-20221101203129420](C:/Users/86189/AppData/Roaming/Typora/typora-user-images/image-20221101203129420.png)

**3.在左侧显示当前Done的节点并且可以选择下一节点执行**

![image-20221101203155517](C:/Users/86189/AppData/Roaming/Typora/typora-user-images/image-20221101203155517.png)

## 前后端对接需要修改的地方

在src\js\path.js文件中

保存了会用到的axios访问的地址

![image-20221101203345114](C:/Users/86189/AppData/Roaming/Typora/typora-user-images/image-20221101203345114.png)

在我的mock中的baseUrl是     baseUrl:"http://127.0.0.1:4523/m1/1706927-0-default",

如果换成用后端调用数据，可以修改这里的baseUrl即可
