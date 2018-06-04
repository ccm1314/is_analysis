## “修改用户信息”用例

### 1. 用例规约

用例名称 | 修改用户信息
---|---
功能 | 修改用户的GitHub用户名称
参与者 | 学生、老师
前置条件 | 必须先登录，并且查看用户现有的GitHub用户名
后置条件 | 
主事件流 | 1.用户填写GitHub用户名称 <br> 2.用户提交修改信息 <br> 3.系统存储修改后的GitHub用户名称
备选事件流 | 1a. 如果用户输入的GitHub用户名称为空 <br> 1.系统清空用户的GitHub用户名称

### 2. 业务流程（顺序图）
无

### 3. 接口调用
 
- API接口调用
    - 接口1：[getStudentsInfo](../接口/studentInfo.md)
    - 接口2：[getTeachersInfo](../接口/getTeacherInfo.md)
    - 接口4：[setTeachersInfo](../接口/setTeacherInfo.md)

### 4. 算法描述
无


### 5. 参照表
- [STUDENTS](../数据库设计.md)
- [TEACHERS](../数据库设计.md)
