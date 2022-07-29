## 租房辅助对比excel模板

### 使用

[下载](https://github.com/ednow/rent-house-templete/raw/main/%E7%A7%9F%E6%88%BF.xlsx)此模板，将收集到的信息填入

### 特性

+ 输入房租、水电费等信息自动计算总成本。省去手动计算的麻烦。
+ 对于离散的属性，如朝向、通风行等提供复选框。方便快速记录。

### Q & A

#### Q: 为什么会做这个表格

从客观环境来看，租房的时候会出现各种外部因素的暴雷，如蛋壳公寓、二手房东、隔断房等问题。使得必须要有相应的手段，去降低自己租房时候出现的外部条件风险的概率。

从个人偏好看，自己租房的时候有很多维度的需求，但很多时候不会出现完美契合自己标准的房子，这时候需要一种直观对比手段，方便自己快速做出判断应该需要选取哪间。

考虑再三，表格无疑是一种物美价廉的手段。

#### Q: 总成本的计算模型是什么
`每月成本=房租+单次通勤成本*上班天数*2+水费*用水量+电费*用电量+一次性成本/一次成本的折算次数`

关于一次性成本的折算：假如你预估这次房子会租`6`个月。一次性的一些成本/`6`的值将会被合入每月成本中。
#### Q: 表格中租房参数怎么来的

主要是收集了B站一些博主的经验，具体笔记总结在「[租房的学问](https://ednow.github.io/2022/07/24/%E7%A7%9F%E6%88%BF%E7%9A%84%E5%AD%A6%E9%97%AE/)」。

<!-- #### Q：这个excel怎么做的 -->

<!-- 百度，具体一些技巧记录在「[excel](https://ednow.github.io/2022/07/24/excel/)」。 -->

#### Q: 该仓库下old文件夹的作用

未接入git版本控制管理之前的历史版本备份

### 版本变更

#### v5
+ sheet「cost」的名字变更为「总成本超参数」
+ sheet「测试」的名字变更为「其他候选租房参数」
+ sheet「正式」的第二列填充更多示例内容
+ 总成本的计算式，考虑每个月上班时间不是30天并考虑往返费用要`*2`。

### v4
+ 减少列数，方便导入腾讯文档

### v3
+ 增加总成本的自动计算

### 附录

#### sheet「正式」的属性解释
|属性|解释|
|----|----|
|房屋地址|推荐填入一个可以辨认这个房子的描述。|
|房租（元）|数值。推荐数值。每月房租。  |
|地铁距离（min）|推荐计算从出门到最近地铁站的距离。  |
|上班时间(min)|推荐计算从出门到公司楼下的时间。  |
|单次通勤成本(元)|数值。 例如从家到公司地铁+其他交通工具的一次性成本是多少元。 |
|面积大小|推荐租的房子总面积，或者可利用面积。  |
|楼层|租的房子在第几层。  |
|朝向|推荐记录大窗户的朝向。  |
|通风好不好（窗户大不大）|考量窗户大不大、窗户数量、空气流通情况。  |
|水费|数值。一吨水的单价。单位：吨/元。  |
|电费|数值。一吨水的单价。单位：度/元。  |
|租付模式|从下面类型中选择「押1付1、押1付2、押1付3」 。 |
|房屋来源|从下面类型中选择 「链家、贝壳、豆瓣小组、自如、直租、小中介、阿姨 」。|
|三甲医院距离(min)|推荐计算从出门到医院楼下的时间。  |
|网络情况（运营商是什么）|从下面类型中选择 「电信、移动、联通、其他 」。  |
|洗衣机是否和房间分开|从下面类型中选择 「是、否」。  |
|厨房是否和房间分开|从下面类型中选择 「是、否」。  |
|噪音情况|从下面类型中选择 「好、中、差」。  |
|看房时间| 从下面类型中选择 「早、中、晚、早中、早晚、中晚、早中晚」。  |
|一梯多少户（上下班可能会排队）|  |
|是否能换锁芯| 从下面类型中选择 「是、否」。  |
|是否复式|从下面类型中选择 「是、否」。   |
|是否漏水|从下面类型中选择 「是、否」。   |
|电视机试用|从下面类型中选择 「好、中、差」。  |
|空调试用（是否喷水）|从下面类型中选择 「好、中、差」。  |
|洗衣机试用|从下面类型中选择 「好、中、差」。  |
|水电交割，物业费是否正常缴纳|从下面类型中选择 「是、否」。  |
|确认合同条款1：房东违约和租户违约的赔偿规则|从下面类型中选择 「是、否」。  |
|确认合同条款2：房东收租金的卡号|从下面类型中选择 「是、否」。  |
|确认房产证信息|从下面类型中选择 「是、否」。  |
|物业信息（电话、地址）|填写小区的物业的电话、接待地址等。  |
|其他补充信息|其他对于这间房子的描述  |
|其他一次性成本（中介费）| 数值。填写其他未被上面提及一次性如中介费等，押金等的总成本。 |
|其他每月固定成本（物业费，管理费，燃气费）| 数值。如其他未被上面提及的物业费，管理费，燃气费等的总成本。 |
|总成本（元/月）|见[总成本是如何计算的](#Q:总成本的计算模型是什么)|

<!--  -->
<!-- |$1|  |\n -->

#### sheet「总成本超参数」的属性解释
填写关于总成本计算相关的一些超参数。



|属性|解释|
|----|----|
|用水量（吨/月）|数值。每个月大概用多少水。|
|用电量（度/月）|数值。每个月大概用多少电。|
|一次性成本折算(次)|数值。比如预估会租6个月就折算6次，填6。|
|上班天数|数值。预估上班的天数。|

