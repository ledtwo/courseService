# **学生课程信息管理系统 服务端操作说明**

题目提供了一个简单的后端系统，可独立运行（分为Windows版本和Linux版本），地址为<http://localhost:8004>，请选择一套运行环境（Windows或Linux）按要求为系统开发前端页面部分（前后端互相独立，只有数据交互）。

后端运行说明：WINDOWS版直接运行“前端面试.exe”；LINUX版直接运行”前端面试“。

**题目要求：**

1.学生列表页、课程列表页，实现增删改查等基本功能

2.（进阶选做）在上述功能基础上，在学生列表页增加“选课”、“删课”的功能

**提交要求：**

1.提交最终作品代码

2.提交作品部署说明文档

 

# **系统后端接口说明**

| URL                                | 方法 | 接口功能         | 备注                             |
| ---------------------------------- | ---- | ---------------- | -------------------------------- |
| /Students/Index                    | Get  | 获取所有学生数据 |                                  |
| /Students/Create                   | Get  | 增加学生示例页面 | 示例页面仅供参考                 |
| /Students/Create                   | Post | 增加学生数据     | Post数据参照示例                 |
| /Students/Edit?id={id}             | Get  | 修改学生示例页面 | 示例页面仅供参考                 |
| /Students/Edit?id={id}             | Post | 修改学生数据     | Post数据参照示例                 |
| /Students/Delete?id={id}           | Get  | 删除学生数据     |                                  |
|                                    |      |                  |                                  |
| /Courses/Index                     | Get  | 获取所有课程数据 |                                  |
| /Courses/Create                    | Get  | 增加课程示例页面 | 示例页面仅供参考                 |
| /Courses/Create                    | Post | 增加课程数据     | Post数据参照示例                 |
| /Courses/Edit?id={id}              | Get  | 修改课程示例页面 | 示例页面仅供参考                 |
| /Courses/Edit?id={id}              | Post | 修改课程数据     | Post数据参照示例                 |
| /Courses/Delete?id={id}            | Get  | 删除课程数据     |                                  |
|                                    |      |                  |                                  |
| /Enrollments/Index                 | Get  | 获取所有选课数据 |                                  |
| /Enrollments/Create                | Get  | 增加选课示例页面 | 示例页面仅供参考                 |
| /Enrollments/Create                | Post | 增加选课数据     | Post数据参照示例                 |
| /Enrollments/Delete?id={id}        | Get  | 删除选课数据     |                                  |
|                                    |      |                  |                                  |
| /api/EnumInfoApi/GetEnum?id={enum} | Get  | 获取枚举对应表   | 例如{enum}填写StudentType或Grade |

 

# **系统后端运行方法**

Windows版：双击运行目录下 “前端面试.exe”

Linux版：上传至Linux系统后，运行“前端面试”（可能需要为该文件添加执行权限）