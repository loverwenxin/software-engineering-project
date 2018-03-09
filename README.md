# 软件工程课程设计

> 本文是课程设计的相关资料

## 目录
* [实验题目：博物馆应用平台系统](#实验题目：博物馆应用平台系统)
    * [博物馆网站数据采集子系统](#博物馆网站数据采集子系统)
    * [博物馆新闻采集分析子系统](#博物馆新闻采集分析子系统)
    * [博物馆信息浏览子系统](#博物馆信息浏览子系统)
    * [博物馆导览子系统](#博物馆导览子系统)
    * [后台管理子系统](#后台管理子系统)
 
* [实验内容](#实验内容)  
* [实验要求](#实验要求)
* [评分标准](#评分标准)
* [交付物](#交付物)
* [时间表](#时间表) 
* [相关文件](#相关文件)
    
## 实验题目：博物馆应用平台系统

### 博物馆网站数据采集子系统

编写一个本地应用程序，通过程序自动从博物馆网站上爬取信息，进行加工处理。主要包括以下功能：

1）数据爬取：爬取全国一级博物馆（130家左右）的网站信息，包括博物馆基本的介绍、参观信息（开放时间等）、展览信息、教育活动、经典藏品信息、学术研究信息等，对于展览信息可以定时更新。

2）数据加工：对于爬取的信息进行过滤和加工，抽取需要的内容。例如：对于展览页面，要得到展览主题、展览时间、展览地点、展览介绍等信息。

3）数据导入：采用合适的方式保存抽取的数据，能够导入到数据库中。

4）数据更新：支持数据的持续更新。例如：根据情况，每天或每周爬取一次新的数据，更新原有数据。

注意：数据的加工最好采用可配置的方式，能够用于多家博物馆网站的页面和内容。

 
### 博物馆新闻采集分析子系统

编写一个本地应用系统，通过程序能从主要的新闻网站上爬取博物馆相关的新闻信息，进行加工处理。主要包括以下功能：

1）数据获取：爬取主要的新闻网站中的博物馆相关新闻（如百度新闻）。可以支持爬取指定时间范围内的新闻，如1年内的新闻，半年内的新闻等。

2）数据加工：对于爬取的信息进行过滤和加工，抽取需要的内容。例如，抽取新闻的发布时间、新闻的标题、新闻的内容、新闻涉及的博物馆等。

3）数据分析：对于加工好的新闻，分析是正面新闻还是负面信息。可采用已有的可直接调用的服务和代码实现。

4）数据定制服务：可以根据指定的某一家博物馆，获取该博物馆的指定时间的新闻，并进行加工分析，得到该博物馆指定时间内的主要新闻，正面新闻和负面新闻。

### 博物馆信息浏览子系统

编写一个Android手机应用程序，支持用户浏览1和2中采集的数据，并对数据进行分析显示。

1）数据浏览：在手机端可以浏览各博物馆的介绍、参观信息、展览、教育活动、藏品、新闻等。可以采用列表方式，或地图方式，或其他便于用户定位的方式显示各博物馆。

2）数据查询：支持数据的查询功能。例如，按照博物馆查询、按照展览查询、按照藏品名称查询。

3）用户反馈：支持用户评论、打分等功能。可以按照展览、服务、环境三个方面让用户对一个博物馆进行打分。

4）数据分析：分析博物馆信息以及用户反馈信息，用排名列表和可视化方式显示分析结果。如，各博物馆一年举办的展览次数的排名列表。



### 博物馆导览子系统

编写一个Android手机应用程序，支持博物馆的讲解导览。可利用1中采集的部分基本信息。主要支持以下功能：

1）地图浏览：在地图上标注每个城市的博物馆，可以根据定位显示距离最近的博物馆。针对博物馆，在地图上标注该博物馆的近期展览和博物馆相关讲解。从地图可进入博物馆信息浏览、讲解等。

2）博物馆信息浏览：显示博物馆的基本信息、展览信息、藏品信息等。

3）播放讲解：播放一个博物馆、展览、藏品的相关讲解。

4）自制讲解：用户可以录制并上传关于博物馆、展览和藏品的讲解，并上传到平台，平台审核通过后，可以在手机应用中播放该讲解。

5）用户个人信息管理：用户可以注册登录该系统，设置用户名密码等个人信息。

注意：利用1中采集的130家博物馆的信息，支持一级博物馆的讲解导览。


### 后台管理子系统

主要包括：

1）用户管理：管理后台用户信息、后台管理员日志、手机端用户信息。如增加管理员，修改管理员密码，禁止一个发布过非法评论的手机端用户再次发布评论等。

2）讲解审核：审核用户上传的讲解。

3）数据管理：管理1-4系统中涉及所有数据，如一个博物馆的基本信息、展览信息、藏品信息、新闻信息、讲解信息、评论等。例如，删除一个用户发布的非法评论信息。

4）数据备份和恢复：支持本系统的数据库和服务器端重要文件的备份和恢复。

## 实验内容

开发一个博物馆应用平台系统。系统一共分为五个子系统：博物馆网数据采集子系统、博物馆新闻采集分析子系统、博物馆信息服务子系统、博物馆导览子系统、后台管理子系统。
   
进行分组开发，所有学生按照班级分成5个团队，每团分5组，每组5-6人。每组完成一个子系统，每个团队最后提交一个完整的系统。
   
分组时首先确定小组长，小组长间协商组成团队，指定团长，然后小组长招募组员。每个小组完成的子系统题目采用团队内部自愿协商的方式确定，若协商不成，则采用抽签的方式。每个团队内部采用的开发语言、开发工具、数据库应该协商一致。如果一个团长被一半以上组长投诉，则该团可重新选择团长。
   
第二周确定并提交团长和组长名单，提交分组名单。分组名单格式见文件《分组名单标准格式》。 
   
助教：王微微博士          

分团和分组时注意技术力量均衡，女生要分散到各组。  
组长注意任务分配和人员分工，尽量让每个组员能发挥所长。  

## 实验要求

（1）提交文档：项目管理计划、需求规格说明，设计报告，测试报告、用户使用手册和项目个人总结。其中项目个人总结为每人一份，其余文档每组提交一份。每个团队将各小组的文档综合到一起提交。所有文档需要提交电子版。

（2）程序检查：一共两次。第一次检查每个小组的子系统运行情况。第二次检查每个团队内五个小组集成后完整的系统运行情况，检查完成后需要提交程序源文件和可执行的系统。程序检查安排在上机时间进行。

（3）演讲：一共一次，在项目完成时进行总结汇报。

## 评分标准

各部分分值  

（1）文档（30分）：项目管理计划（5）、需求规格说明（10）、设计报告（10）、测试报告（5）、用户使用手册（5）  
（2）演讲（10分）  
（3）系统检查（50分）：子系统运行检查（30）、集成运行检查（20分）  
（5）个人总结（10分）  

分数计算规则  

（1）团队分数=系统集成运行检查分数  
（2）小组分数=小组文档分数+子系统运行检查分数+演讲分数+团队分数  
（3）个人分数

 - 团长分数=小组平均分+个人总结分数+额外分。教师确定，+-10分。  
 - 组长分数=小组分数+个人总结分数+额外分。团长确定。
     - 各团除团长外各组长额外分之和不超过20分。
 - 组员分数=小组分数+个人总结分数+额外分。组长确定。 
     - 各组除组长外小组分总和不超过10分    


## 交付物

| 交付物 | 阶段 |
| --- | --- |
| 项目管理计划 | 在项目初始阶段形成，在后续每一个阶段更新 |
| 需求规格说明 | 在需求分析阶段结束形成，在后续的设计和开发阶段更新 |
| 设计报告 | 在设计阶段形成，在后续开发阶段补充和更新 |
| 测试报告 | 在软件开发阶段形成，在后续的测试阶段更新 |
| 用户手册 | 在需求分析阶段结束形成，在后续阶段更新，在系统交付阶段交付 |
| 个人总结 | 在系统交付阶段完成 |
| 源代码 | 在开发阶段形成，在测试阶段更新 |
| 可执行系统 | 在开发阶段形成，在测试阶段更新 |

## 时间表

接收文档邮箱：software_buct@qq.com

<style>
table th:first-of-type {
    width: 90px;
}
table th:nth-of-type(2) {
    width: 160px;
}
</style>
| 关键时间 | 任务 | 要求 |
| --- | --- | --- |
| 第二周 | 确定团长、组长和分组 | 电子版分组名单提交到邮箱，团长汇总提交 |
| 第三周 | 制定项目管理计划 | 管理计划提交到邮箱，团长汇总提交 |
| 第四周 | 完成需求规格说明初稿 | 电子版提交到邮箱，团长汇总提交 |
| 第五周 | 完成设计报告初稿 | 电子版提交到邮箱，团长汇总提交 |
| 第七周 | 子系统运行检查 | 以小组为单位进行，每个小组10分钟左右。|
| 第十一周 |  |
| 第十二周 | 总结汇报演讲 | 以团队为单位，按照顺序进行。|
| 第十二周 | 系统集成后的运行检查 | 以团队为单位进行，组长和主要程序开发人员参加。此时提交各种文档的电子版；提交电子版源代码和可执行系统。团长提前预约时间。 |


## 相关文件

《课程设计题目-博物馆应用平台系统》

《分组名单标准格式》   
 
《计算机软件文档编制规范》

韩万江软件文档范例

孙家广学生文档范例
