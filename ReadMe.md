# 需求分析
![img](/就业信息管理系统需求.png)
---
# 进度管理

时间 | 强哥 | 俊杰 | 科杰 | 志哥 | 备注
---|---|---|---|---|--- 
周一 | 软件需求说明书 | ... | ... | ... |共同完成管理员需求说明书，强哥俊杰负责企业，科杰志哥负责学生
完成度|完成
周二 | 上午数据流图，下午ER图



# 软件需求说明
---
## 管理员功能说明
- 企业模块管理
    - 对企业资质认证及信息修改请求的审核
    - 对企业列表信息进行查改
    - 对企业进行删除
    - 对企业发布招聘信息进行的查看及审核
- 学生模块管理
    - 对学生的信息批量导入
    - 对学生的注册登记信息审核
    - 对学生相关信息进行查看（按照学校专业班级查询）
    - 对学生的就业信息的登记处理
- 管理员自身管理
    - 对自身信息的修改

### 管理员用例图
![img](/管理员用例图.png)



## 学生功能说明
- 注册功能
- 申请修改自身个人信息，包括提交个人认证
- 填写求职意向并发放自身求职简历
- 查询企业招聘信息
- 向对应企业发送求职简历
- 登记就业信息

### 学生用例图
![学生用例图](/学生用例图.png)

## 企业功能说明
- 可以用手机号进行注册
- 企业基本信息的填写，包括企业名称、企业地址、企业简介、联系方式、企业的资质证明，并等待管理员审核。
- 企业招聘信息的填写，包括具体的岗位以及相关的要求
- 对企业的基本信息、招聘信息的修改，并等待管理员审核。
- 企业可以查看申请岗位人员简历信息

### 企业用例图
![img](/企业用例图.PNG)

### 企业用例描述


- 输入企业基本信息用例

用例名称 | 输入企业基本信息
--- | ---
用例描述 | 企业在就业管理系统完成输入企业基本信息整个过程
参与者 | 企业
状态 | 通过审查
前置条件 | 企业成功以企业身份登录系统
后置条件 | 企业输入企业基本信息后可进行后续修改信息操作
基本操作流程 | 企业进入基本信息输入页面<br>企业输入企业基本信息<br>企业输入完毕等待审核<br>审核通过将信息保存到数据库<br>企业可进行后续输入修改企业基本信息
可选操作流程 | 审核不通过，企业重新输入
假设 | 企业成功以企业身份登录系统


- 发布招聘信息用例

用例名称 | 发布招聘信息
--- | ---
用例描述 | 企业在就业管理系统完成发布招聘信息整个过程
参与者 | 企业
状态 | 通过审查
前置条件 | 用户成功以企业角色登录系统
后置条件 | 企业发布招聘信息后可进行后续修改招聘信息操作
基本操作流程 | 企业进入招聘信息发布页面<br>企业输入招聘信息并上传相关文件<br>企业输入信息并上传文件完毕，等待审核<br>审核通过后，系统发布招聘信息<br>企业可进行后续修改操作并重新发布
可选操作流程 | 审核不通过，企业重新输入
假设 | 企业成功以企业身份登录系统

- 查看求职者信息用例

用例名称 | 查看求职者信息
--- | ---
用例描述 | 企业完成查看求职者信息整个过程
参与者 | 企业
状态 | 通过审查
前置条件 | 用户成功以企业角色登录系统
后置条件 | 企业查看求职者信息后决定是否向求职者发送面试通知
基本操作流程 | 企业进入求职者信息查看页面企业查看求职者信息
可选操作流程 | 企业向求职者发送面试通知
假设 | 企业成功以企业身份登录系统



## 游客功能说明
- 浏览企业的招聘信息

### 游客用例图
![游客用例图](/游客浏览网页用例.png)


