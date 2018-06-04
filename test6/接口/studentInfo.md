#### 用例： 学生信息
- 权限： 学生/老师都能看到列表，访客不能看到列表。
- 功能： 返回对应学生的信息。
- API请求地址： 接口基本地址/v1/api/getStudentInfo/<stu_no>
- 请求方式 ： GET
- 请求参数说明: 

请求参数| 说明
---|---
stu_no | 学生编号

- 返回实例说明：
```
 {
      "status": true,
      "info": "获取结果成功",
      "data": 
          {
          "GITHUB_ NAME": "luotf",
          "ID":15,
          "STU_NO": "201510414213",
          "STU_CLASS": "软件(本)15-2",
          "STU_NAME": "罗廷方",
          "STATUS":"1",
          "ADDTIME": "2018-05-22 17:48:01",
          "TERM_ID":2,
          "GRADE_ID":2,
          "TEST_ID":2,
          "COURSE_NO":25,
          "GRADE_1":95,
          "GRADE_2":85,
          "GRADE_3":90,
          "MOME":"这个同学完成的还不错",
          ...
          }
  }

```
- 返回参数说明：

参数名称	| 说明
---|---
status | bool类型，true表示正确的返回，false表示有错误
info | 返回结果说明信息
data | 所有学生集合
GITHUB_ NAME | 	GITHUB 用户名
STU_NO | 学号
STU_NAME | 真实姓名
ADDTIME | 增加日期
ID | 数据库中编号
STATUS | 是否正常
TERM_ID | 学期编号
GRADE_ID | 成绩编号
TEST_ID | 实验编号
COURSE_NO | 课程编号
GRADE_1 | 分数
GRADE_2 | 分数
GRADE_3 | 分数
MOME | 评价
