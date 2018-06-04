﻿## TEACHER 表 (学生)

字段| 类型| 主外键 | 可以为空|默认值|说明|
---|---|---|---|---|---|
ID | INT(11)| 主键|否||自增|
TCH_NO | VARCHAR(255)| |否||教师编号|
TCH_NAME | VARCHAR(255)| |是||教师姓名|
GITHUB_NAME | VARCHAR(255)| |是||教师GitHub的名称|
TCH-PWD | VARCHAR(255)| |否||教师密码|
STATUS | VARCHAR(255)| |否||教师是否禁用|

## STUDENT 表 (老师)

字段| 类型| 主外键 | 可以为空|默认值|说明|
---|---|---|---|---|---|
ID | INT(11)| 主键|否||自增|
COURSE_NO|VARCHAR(255)|外键|否||课程编号|
STU_NO | VARCHAR(255)| |否||学生编号|
STU_NAME | VARCHAR(255)| |是||学生姓名|
GITHUB_NAME | VARCHAR(255)| |是||学生GitHub的名称|
STU_PWD | VARCHAR(255)| |否||学生密码|
STU_CLASS | VARCHAR(255)| |否||学生班级|
 

## COURSES 表 (课程)

字段| 类型| 主外键 | 可以为空|默认值|说明|
---|---|---|---|---|---|
ID | INT(11)| 主键|否||自增|
TERM_ID|VARCHAR(255)|外键|否||学期编号|
STU_NO|VARCHAR(255)|外键|否||学生编号|
TCH_NO|VARCHAR(255)|外键|否||教师编号|
COURSE_NO|VARCHAR(255)||否||课程编号|
COURSE_NAME | VARCHAR(255)| |否||学生编号|
ADDTIME | DATETIME| |否||学生创建时间|
 

## GRADES 表 (分数)

字段| 类型| 主外键 | 可以为空|默认值|说明|
---|---|---|---|---|---|
GRADE_ID | INT(11)| 主键|否||自增|
TEST_ID|VARCHAR(255)|外键|否||实验编号|
COURSE_NO|VARCHAR(255)|外键|否||课程编号|
STU_NO|VARCHAR(255)|外键|否||学生编号|
GRADE_1|FLOAT||否|0|分数1|
GRADE_2 | FLOAT| |是|0|分数2|
ADDTIME | DATETIME| |否||创建时间|

## TESTS 表 (实验)

字段| 类型| 主外键 | 可以为空|默认值|说明|
---|---|---|---|---|---|
TEST_ID | INT(11)| 主键|否||自增|
COURSE_NO|VARCHAR(255)|外键|否||课程编号|
TITLE|VARCHAR(255)||否||实验名称|
ADDTIME | DATETIME| |否||创建时间|

## TERMS 表 (学期)

字段| 类型| 主外键 | 可以为空|默认值|说明|
---|---|---|---|---|---|
TERM_ID | INT(11)| 主键|否||学期编号|
TITLE|VARCHAR(255)||否||学期名称|
ADDTIME | DATETIME| |否||创建时间|

## STU_COURSE 表 (学生课程表)

字段| 类型| 主外键 | 可以为空|默认值|说明|
---|---|---|---|---|---|
ID | INT(11)| 主键|否||自增|
COURSE_NO|VARCHAR(255)|外键|否||课程编号|
STU_NO|VARCHAR(255)|外键|否||学生编号|
ADDTIME | DATETIME| |否||创建时间|
