**文档编号： [ ]{.underline}**

**版 本 号： [ ]{.underline}**

**密 级： [ 保 密 ]{.underline}**

> **金蝶EAS和BOS**
>
> **开发培训教程**

金蝶软件（中国）有限公司 成都分公司开发部

作者：杨剑

  -------- ----------- -------- -------- --------------------
  版本号   更新日期    编制人   审核人   修改的章节号及内容
  1        2012-3-5    杨剑     杨剑     
  2        2017-3-10   杨剑     杨剑     
  3        2017-7-16   杨剑     杨剑     
  -------- ----------- -------- -------- --------------------

前言

为企业定制开发ERP业务是一项复杂的工程，需要把开发相关的产品、技术、平台进行综合贯彻到企业的需求和应用中。

金蝶EAS和BOS是一整套面向企业ERP开发的优秀解决方案，它集ERP产品、ERP业务平台、ERP开发工具、运行环境于一体。这套方案在提供了高效率开发ERP业务的同时，也对开发者提出了更高的要求：

-   熟练掌握BOS开发工具及其开发理念、开发方法

-   熟练掌握EAS所提供的ERP业务平台，例如：工作流、单据转换、报表、套打、编码平台、后台事务等

-   熟悉EAS所提供的的ERP基础框架，例如：组织职位、用户及权限、职员、客商物料等等

-   其他：具有良好的业务理解能力、沟通能力等

所以，在很多分公司的EAS开发中，如果缺少一个经验丰富的EAS核心开发骨干带领，新人员的成长将会非常困难，其入门门槛远远大于传统软件开发，很多顾问刚接触BOS开发时会淹没在各种平台和技术文档的海洋中而无所适从。

本教程为准备学习EAS和BOS开发的零EAS开发基础的顾问提供一个从零开始学习路径，学习本教程的人员应当具有基本的Java开发。

不教程不是开发知识库，不是大而全的开发书籍和代码库，而是从分公司项目开发实战出发，总结大量项目开发案例，介绍核心开发要领和关键方法，其目的就是抛开海量的开发教程，删繁就简，快速引导顾问具有基本开发技能并具有自我学习和进步的方法。

目 录

[1.]{.underline} [EAS和BOS开发概述]{.underline} 12

[1.1.]{.underline} [ERP软件开发的特点]{.underline} 12

[1.1.1.]{.underline} [注重管理和业务]{.underline} 12

[1.1.2.]{.underline} [注重用户感受]{.underline} 12

[1.1.3.]{.underline} [需求和结果容易出现偏差]{.underline} 12

[1.1.4.]{.underline} [持续建设]{.underline} 12

[1.2.]{.underline} [EAS和BOS平台开发的优势]{.underline} 12

[2.]{.underline} [EAS和BOS平台]{.underline} 14

[2.1.]{.underline} [EAS的架构]{.underline} 14

[2.2.]{.underline} [EAS和BOS的构成]{.underline} 14

[2.3.]{.underline} [EAS和BOS安装]{.underline} 14

[2.3.1.]{.underline} [安装包说明]{.underline} 14

[2.3.2.]{.underline} [EAS开发平台安装]{.underline} 15

[2.4.]{.underline} [EAS演示帐套]{.underline} 15

[2.5.]{.underline} [EAS服务器]{.underline} 16

[2.5.1.]{.underline} [重要特性]{.underline} 16

[2.5.2.]{.underline} [EAS服务器的重要目录]{.underline} 16

[2.6.]{.underline} [EAS管理控制台]{.underline} 16

[2.6.1.]{.underline} [开发需要关注的内容]{.underline} 17

[2.7.]{.underline} [EAS客户端]{.underline} 17

[2.7.1.]{.underline} [重要特性]{.underline} 17

[2.7.2.]{.underline} [EAS客户端的重要目录]{.underline} 17

[2.7.3.]{.underline} [EAS客户端框架]{.underline} 18

[2.7.4.]{.underline} [客户端移植]{.underline} 18

[2.8.]{.underline} [BOS开发工具]{.underline} 18

[2.8.1.]{.underline} [BOS开发透视图]{.underline} 19

[2.8.2.]{.underline} [反编译设置]{.underline} 20

[2.9.]{.underline} [BOS解决方案]{.underline} 20

[2.9.1.]{.underline} [导入解决方案]{.underline} 20

[2.9.2.]{.underline} [解决方案目录]{.underline} 21

[2.9.3.]{.underline} [设置解决方案]{.underline} 22

[2.9.4.]{.underline} [测试账套设置]{.underline} 22

[2.9.5.]{.underline} [解决方案移植]{.underline} 23

[2.9.6.]{.underline} [备份解决方案]{.underline} 23

[2.10.]{.underline} [BOS和解决方案更新]{.underline} 23

[2.10.1.]{.underline} [更新BOS工具]{.underline} 24

[2.10.2.]{.underline} [更新解决方案]{.underline} 24

[3.]{.underline} [BOS开发总体介绍]{.underline} 25

[3.1.]{.underline} [模型驱动开发（MDA）]{.underline} 25

[3.2.]{.underline} [模型要素及构成]{.underline} 25

[3.2.1.]{.underline} [模型的关键要素]{.underline} 25

[3.2.2.]{.underline} [元数据]{.underline} 25

[3.3.]{.underline} [BIM和BOS Studio介绍]{.underline} 26

[3.4.]{.underline} [BOS开发成果的发布、部署和运行]{.underline} 26

[3.4.1.]{.underline} [发布和部署]{.underline} 26

[3.4.2.]{.underline} [手工打包部署]{.underline} 27

[3.4.3.]{.underline} [开发代码在发布和部署中的传递]{.underline} 27

[3.4.4.]{.underline} [JVM运行期加载开发成果]{.underline} 28

[3.5.]{.underline} [客户化开发冲突]{.underline} 28

[3.5.1.]{.underline} [场景]{.underline} 28

[3.5.2.]{.underline} [元数据二开冲突解决]{.underline} 28

[3.5.3.]{.underline} [代码的版本冲突处理]{.underline} 28

[3.6.]{.underline} [子系统树及生成]{.underline} 29

[3.7.]{.underline} [EAS和BOS二次开发规范]{.underline} 30

[4.]{.underline} [元数据介绍及开发关注点]{.underline} 31

[4.1.]{.underline} [什么是元数据]{.underline} 31

[4.2.]{.underline} [实体（Entity）]{.underline} 32

[4.2.1.]{.underline} [基础信息]{.underline} 33

[4.2.2.]{.underline} [实体属性]{.underline} 33

[4.2.3.]{.underline} [实体方法]{.underline} 35

[4.2.4.]{.underline} [BOSTYPEID]{.underline} 35

[4.3.]{.underline} [查询（query）]{.underline} 36

[4.3.1.]{.underline} ["定义"页签]{.underline} 36

[4.3.2.]{.underline} ["字段"页签]{.underline} 37

[4.3.3.]{.underline} ["其他"页签]{.underline} 38

[4.3.4.]{.underline} ["SQL"页签]{.underline} 38

[4.4.]{.underline} [表（table）]{.underline} 39

[4.5.]{.underline} [界面（UI）]{.underline} 39

[4.5.1.]{.underline} [常见的UI类型有：]{.underline} 39

[4.5.2.]{.underline} [重要视图及作用]{.underline} 40

[4.5.3.]{.underline} [常见UI开发调整]{.underline} 40

[4.6.]{.underline} [业务功能（facade）]{.underline} 41

[4.7.]{.underline} [功能（FUNCTION）]{.underline} 41

[4.8.]{.underline} [枚举（Enum）]{.underline} 42

[4.9.]{.underline} [业务异常（exception）]{.underline} 43

[4.10.]{.underline} [权限（permission）]{.underline} 43

[4.11.]{.underline} [日志（log）]{.underline} 43

[4.12.]{.underline} [两个重要的配置文件]{.underline} 44

[4.13.]{.underline} [常见BOS Studio开发]{.underline} 44

[5.]{.underline} [BIM建模和模型调整]{.underline} 45

[5.1.]{.underline} [建模前的准备]{.underline} 45

[5.2.]{.underline} [EAS模型的业务类别和业务属性]{.underline} 45

[5.2.1.]{.underline} [业务类别]{.underline} 45

[5.2.2.]{.underline} [业务属性]{.underline} 45

[5.3.]{.underline} [建立包]{.underline} 45

[5.4.]{.underline} [建立模型（业务单元）]{.underline} 46

[5.5.]{.underline} [模型属性设置]{.underline} 48

[5.6.]{.underline} [为模型增加属性（字段）]{.underline} 49

[5.6.1.]{.underline} [数据来源]{.underline} 49

[5.6.2.]{.underline} [字段的属性]{.underline} 50

[5.7.]{.underline} [界面布局和调整]{.underline} 51

[5.7.1.]{.underline} [控件位置排布工具]{.underline} 51

[5.7.2.]{.underline} [字段运行时的录入和显示顺序]{.underline} 52

[5.7.3.]{.underline} [KD\_Layout布局]{.underline} 52

[5.7.4.]{.underline} [字段锚定]{.underline} 52

[5.8.]{.underline} [为模型增加功能和菜单按钮]{.underline} 53

[5.8.1.]{.underline} [增加功能]{.underline} 53

[5.8.2.]{.underline} [增加菜单和工具栏]{.underline} 54

[5.8.3.]{.underline} [功能的事务属性设置]{.underline} 55

[5.8.4.]{.underline} [功能的参数设置]{.underline} 55

[5.8.5.]{.underline} [功能的异常设置]{.underline} 57

[5.9.]{.underline} [为模型添加权限项]{.underline} 57

[5.9.1.]{.underline} [在BIM中添加权限项]{.underline} 57

[5.9.2.]{.underline} [增加无功能权限项]{.underline} 58

[5.9.3.]{.underline} [权限项在EAS客户端使用和授权]{.underline} 60

[5.9.4.]{.underline} [权限项编码规范化]{.underline} 61

[5.9.5.]{.underline} [权限文件规范化]{.underline} 62

[5.9.6.]{.underline} [建立权限文件的时机建议]{.underline} 62

[5.10.]{.underline} [为模型添加日志项]{.underline} 62

[5.10.1.]{.underline} [在BIM中添加日志项]{.underline} 62

[5.10.2.]{.underline} [日志项使用方法]{.underline} 63

[5.10.3.]{.underline} [日志项编码规范化]{.underline} 63

[5.10.4.]{.underline} [日志文件规范化]{.underline} 63

[5.10.5.]{.underline} [建立日志文件的时机建议]{.underline} 63

[5.11.]{.underline} [BOS Studio对模型的常见调整]{.underline} 63

[5.11.1.]{.underline} [BOS Studio发布元数据]{.underline} 64

[5.12.]{.underline} [模型挂接到系统主菜单]{.underline} 64

[5.13.]{.underline} [模型发布和测试]{.underline} 65

[5.13.1.]{.underline} [同步数据库]{.underline} 65

[5.13.2.]{.underline} [发布错误分析处理]{.underline} 66

[5.14.]{.underline} [自动生成代码]{.underline} 66

[5.15.]{.underline} [测试运行]{.underline} 66

[5.16.]{.underline} [部署开发成果]{.underline} 67

[5.17.]{.underline} [单据模型中通常需要增加的字段]{.underline} 68

[5.17.1.]{.underline} [【单据体】单据状态]{.underline} 68

[5.17.2.]{.underline} [【分录】分录状态]{.underline} 68

[5.17.3.]{.underline} [【单据体】审核时间]{.underline} 68

[5.17.4.]{.underline} [【单据体】来源单据编号]{.underline} 68

[5.17.5.]{.underline} [【分录】来源分录ID，来源分录序号]{.underline} 68

[5.17.6.]{.underline} [【分录】来源单据ID，来源单据编号]{.underline} 69

[5.18.]{.underline} [单据模型通常需要增加的功能]{.underline} 69

[5.18.1.]{.underline} [审核和反审核]{.underline} 69

[5.19.]{.underline} [BOS开发的过程总结]{.underline} 69

[5.20.]{.underline} [BOS建模开发技巧]{.underline} 70

[5.20.1.]{.underline} [模型共享]{.underline} 70

[5.20.2.]{.underline} [产品早期基础数据引用]{.underline} 72

[5.21.]{.underline} [元数据校验]{.underline} 73

[6.]{.underline} [BOS代码体系]{.underline} 74

[6.1.]{.underline} [抽象类和实现类]{.underline} 74

[6.2.]{.underline} [客户端和服务端代码分工]{.underline} 75

[6.3.]{.underline} [值对象和值集合]{.underline} 75

[6.3.1.]{.underline} [值对象（Info）]{.underline} 75

[6.3.2.]{.underline} [值对象的两类get/set方法及应用]{.underline} 75

[6.3.3.]{.underline} [关于getLogInfo方法]{.underline} 76

[6.3.4.]{.underline} [值集合（Collection）]{.underline} 76

[6.3.5.]{.underline} [值对象和值集合示例]{.underline} 76

[6.4.]{.underline} [接口和工厂]{.underline} 77

[6.5.]{.underline} [EditUI，ListUI，ControllerBean]{.underline} 77

[7.]{.underline} [BOS核心代码开发]{.underline} 78

[7.1.]{.underline} [开发必备基础]{.underline} 78

[7.1.1.]{.underline} [ID和BosObjectType]{.underline} 78

[7.1.2.]{.underline} [上下文]{.underline} 80

[7.1.3.]{.underline} [客户端和服务端代码分工]{.underline} 81

[7.1.4.]{.underline} [消息提示]{.underline} 82

[7.2.]{.underline} [controllerbean.java]{.underline} 83

[7.2.1.]{.underline} [两种方法]{.underline} 83

[7.2.2.]{.underline} [要开发的框架方法]{.underline} 84

[7.2.3.]{.underline} [常见开发内容]{.underline} 84

[7.2.4.]{.underline} [数据更新]{.underline} 85

[7.2.5.]{.underline} [代码示例：\_save和\_submit]{.underline} 86

[7.2.6.]{.underline} [代码示例：\_delete]{.underline} 88

[7.2.7.]{.underline} [代码示例：\_audit]{.underline} 88

[7.2.8.]{.underline} [代码示例：\_unAudit]{.underline} 90

[7.3.]{.underline} [EditUI.java]{.underline} 92

[7.3.1.]{.underline} [层次结构]{.underline} 92

[7.3.2.]{.underline} [关于editData]{.underline} 92

[7.3.3.]{.underline} [重要方法说明]{.underline} 94

[7.3.4.]{.underline} [获取界面控件]{.underline} 94

[7.3.5.]{.underline} [控件定制]{.underline} 96

[}else{]{.underline} 97

[//
计算总人天=汇总表格所有行的人天数据，判断当前编辑的列＝人天列]{.underline}
99

[7.3.6.]{.underline} [控件监听/自动处理]{.underline} 100

[7.3.7.]{.underline} [新增默认值]{.underline} 101

[7.3.8.]{.underline} [Action开发]{.underline} 102

[7.4.]{.underline} [LISTUI.java]{.underline} 104

[7.4.1.]{.underline} [ListUI的层次结构]{.underline} 104

[7.4.2.]{.underline} [关于mainQueryPK和mainQuery]{.underline} 104

[7.4.3.]{.underline} [重要方法]{.underline} 105

[7.4.4.]{.underline} [获取单据ID]{.underline} 105

[7.4.5.]{.underline} [Action开发]{.underline} 108

[8.]{.underline} [EAS平台开发]{.underline} 110

[8.1.]{.underline} [数据库操作]{.underline} 110

[8.1.1.]{.underline} [数据库查询结果集]{.underline} 110

[8.1.2.]{.underline} [关于KSQL]{.underline} 110

[8.1.3.]{.underline} [客户端数据库操作]{.underline} 110

[8.1.4.]{.underline} [服务端数据库操作]{.underline} 111

[8.1.5.]{.underline} [客户端查询分析器]{.underline} 111

[8.2.]{.underline} [异常处理]{.underline} 113

[8.2.1.]{.underline} [BOSException]{.underline} 113

[8.2.2.]{.underline} [EASBIZEXCEPTION]{.underline} 113

[8.2.3.]{.underline} [重要！异常捕获处理]{.underline} 114

[8.3.]{.underline} [视图和OQL]{.underline} 115

[8.3.1.]{.underline} [OQL]{.underline} 115

[8.3.2.]{.underline} [视图]{.underline} 116

[]{.underline} [选择项集合SelectorItemCollection]{.underline} 116

[8.4.]{.underline} [F7定制]{.underline} 117

[8.4.1.]{.underline} [基本属性]{.underline} 117

[8.4.2.]{.underline} [SelectUI]{.underline} 117

[8.4.3.]{.underline} [视图]{.underline} 118

[8.4.4.]{.underline} [监听]{.underline} 119

[8.4.5.]{.underline} [常见F7定制方法]{.underline} 119

[8.5.]{.underline} [弹窗开发]{.underline} 121

[8.5.1.]{.underline} [子窗体接收参数]{.underline} 121

[8.6.]{.underline} [自定义BOTP函数]{.underline} 122

[8.6.1.]{.underline} [开发FormulaFunction类]{.underline} 122

[8.6.2.]{.underline} [在Entity上注册FormulaFunction类]{.underline} 123

[8.7.]{.underline} [多级基础资料]{.underline} 124

[8.7.1.]{.underline} [多级基础资料模板]{.underline} 124

[8.7.2.]{.underline} [关键属性]{.underline} 124

[8.8.]{.underline} [套打数据源开发]{.underline} 125

[8.8.1.]{.underline} [默认单据套打方法]{.underline} 125

[8.8.2.]{.underline} [员工花名册套打方法]{.underline} 125

[8.8.3.]{.underline} [费用申请单套打方法]{.underline} 125

[8.9.]{.underline} [元数据开发]{.underline} 125

[8.9.1.]{.underline} [元数据引擎]{.underline} 126

[8.9.2.]{.underline} [获取Entity及其Bean]{.underline} 126

[Method method = clsFactory.getMethod(\"getLocalInstance\",
Context.**class**);]{.underline} 126

[8.9.3.]{.underline} [构造Entity对应的值对象]{.underline} 127

[8.9.4.]{.underline} [检索Entity中的属性]{.underline} 127

[8.10.]{.underline} [权限检查]{.underline} 128

[8.11.]{.underline} [自动编码]{.underline} 129

[8.12.]{.underline} [产品报表分析]{.underline} 129

[9.]{.underline} [EAS产品改造开发]{.underline} 132

[9.1.]{.underline} [元数据改造]{.underline} 132

[9.2.]{.underline} [EditUI/ListUI.java扩展]{.underline} 132

[9.3.]{.underline} [ControllerBean.java扩展]{.underline} 133

[9.4.]{.underline} [DEP脚本扩展]{.underline} 133

[9.4.1.]{.underline} [pluginCtx.getUI()]{.underline} 134

[9.4.2.]{.underline} [UI脚本示例]{.underline} 134

[9.4.3.]{.underline} [entity脚本示例]{.underline} 134

[9.5.]{.underline} [DEP+BOS的功能扩展]{.underline} 134

[9.5.1.]{.underline} [UI界面/实体方法扩展]{.underline} 134

[9.5.2.]{.underline} [UI界面增加控件]{.underline} 135

[9.5.3.]{.underline} [UI界面Java引用控件]{.underline} 137

[// 定义EAS80升级后增加的DEP控件对象]{.underline} 138

[10.]{.underline} [产品和错误分析]{.underline} 139

[10.1.]{.underline} [产品分析]{.underline} 139

[10.1.1.]{.underline} [客户端日志]{.underline} 139

[10.1.2.]{.underline} [主菜单]{.underline} 139

[10.1.3.]{.underline} [线程挂起]{.underline} 140

[10.1.4.]{.underline} [方法断点]{.underline} 141

[10.1.5.]{.underline} [人为制造阻塞或异常]{.underline} 142

[10.1.6.]{.underline} [类加载断点]{.underline} 143

[10.2.]{.underline} [错误分析]{.underline} 143

[10.2.1.]{.underline} [错误堆栈]{.underline} 143

[10.2.2.]{.underline} [异常断点使用]{.underline} 144

[10.3.]{.underline} [跟踪调试]{.underline} 146

[10.3.1.]{.underline} [调试视图]{.underline} 146

[10.3.2.]{.underline} [表达式视图]{.underline} 147

[10.3.3.]{.underline} [显示视图]{.underline} 147

[10.3.4.]{.underline} [变量视图]{.underline} 148

[11.]{.underline} [EAS接口开发]{.underline} 150

[11.1.]{.underline} [数据流向]{.underline} 150

[11.2.]{.underline} [物理连接]{.underline} 150

[11.2.1.]{.underline} [连接配置]{.underline} 151

[11.2.2.]{.underline} [连接实现]{.underline} 151

[11.3.]{.underline} [运行平台]{.underline} 158

[11.4.]{.underline} [接口内容]{.underline} 159

[11.4.1.]{.underline} [XML格式]{.underline} 159

[11.4.2.]{.underline} [XML开发示例]{.underline} 159

[Iterator\<Element\> iterator =
element\_datas.elementIterator();]{.underline} 162

[11.4.3.]{.underline} [Json格式]{.underline} 163

[11.4.4.]{.underline} [Json开发示例]{.underline} 163

[11.4.5.]{.underline} [数据格式转换]{.underline} 164

[11.5.]{.underline} [基础数据体系]{.underline} 164

[11.5.1.]{.underline} [基础数据映射]{.underline} 164

[11.5.2.]{.underline} [基础数据转换]{.underline} 164

[11.6.]{.underline} [业务数据处理]{.underline} 165

[11.6.1.]{.underline} [业务数据检查]{.underline} 165

[11.6.2.]{.underline} [业务数据确认]{.underline} 165

[11.7.]{.underline} [Excel导入导出]{.underline} 165

[11.7.1.]{.underline} [业务及设计]{.underline} 165

[11.7.2.]{.underline} [Excel工具类]{.underline} 166

[11.7.3.]{.underline} [Excel导入完整案例]{.underline} 166

[11.7.4.]{.underline} [Excel导入代码示例]{.underline} 167

[// 计算行数和列数]{.underline} 168

[// 获取所选文件名称]{.underline} 169

[11.8.]{.underline} [关于EIP平台]{.underline} 169

[12.]{.underline} [EAS工作流]{.underline} 171

[12.1.]{.underline} [总体介绍]{.underline} 171

[12.2.]{.underline} [工作流模型设计开发]{.underline} 171

[12.2.1.]{.underline} [自动审核节点参与人]{.underline} 171

[12.2.2.]{.underline} [提交单据进入工作流]{.underline} 172

[12.3.]{.underline} [工作流状态图]{.underline} 172

[12.3.1.]{.underline} [查看流程属性]{.underline} 172

[12.3.2.]{.underline} [错误日志]{.underline} 172

[12.4.]{.underline} [单据审批界面]{.underline} 174

[12.4.1.]{.underline} [业务单据操作集成]{.underline} 175

[12.5.]{.underline} [单据流程检查]{.underline} 175

[13.]{.underline} [EAS单据转换]{.underline} 177

[13.1.]{.underline} [BOTP业务案例]{.underline} 177

[13.1.1.]{.underline} [案例及设计]{.underline} 177

[13.1.2.]{.underline} [反写和检查点]{.underline} 178

[13.1.3.]{.underline} [上下游关系获取]{.underline} 178

[13.1.4.]{.underline} [按分录控制]{.underline} 179

[13.1.5.]{.underline} [分组合并的限制]{.underline} 179

[13.1.6.]{.underline} [反写和检查的顺序]{.underline} 179

[13.2.]{.underline} [转换规则]{.underline} 179

[13.2.1.]{.underline} [单头转换规则]{.underline} 179

[13.2.2.]{.underline} [分录转换规则]{.underline} 180

[13.2.3.]{.underline} [分组规则和数值合计]{.underline} 181

[13.2.4.]{.underline} [规则过滤和单据过滤]{.underline} 181

[13.2.5.]{.underline} [BOTP公式平台]{.underline} 182

[13.2.6.]{.underline} [组织隔离]{.underline} 183

[13.3.]{.underline} [转换关系记录]{.underline} 183

[13.4.]{.underline} [界面操作]{.underline} 183

[13.5.]{.underline} [反写和检查控制]{.underline} 185

[13.5.1.]{.underline} [方法事务属性]{.underline} 185

[13.5.2.]{.underline} [源单数据更新]{.underline} 185

[13.6.]{.underline} [代码调用BOTP平台]{.underline} 186

[} catch (RemoteException e) {]{.underline} 187

[// 获取BOTP引擎服务实例]{.underline} 187

[// 执行BOTP转换]{.underline} 187

[// 保存生成的目标单据及BOTP关联关系]{.underline} 187

[14.]{.underline} [EAS扩展报表]{.underline} 188

[14.1.]{.underline} [开发方法概述]{.underline} 188

[14.1.1.]{.underline} [报表开发步骤]{.underline} 188

[14.1.2.]{.underline} [数据源设计方法]{.underline} 188

[14.2.]{.underline} [SQL数据集开发]{.underline} 189

[14.2.1.]{.underline} [参数设计]{.underline} 189

[14.2.2.]{.underline} [SQL设计]{.underline} 190

[14.2.3.]{.underline} [预览]{.underline} 190

[14.2.4.]{.underline} [组织范围控制]{.underline} 191

[SELECT FID, FName\_l2, FNumber, FLongNumber]{.underline} 191

[14.2.5.]{.underline} [参数的关联控制]{.underline} 192

[14.2.6.]{.underline} [自定义参数插件]{.underline} 192

[14.3.]{.underline} [Java数据源]{.underline} 192

[14.3.1.]{.underline} [新增数据源定义]{.underline} 192

[14.3.2.]{.underline} [开发Java数据源]{.underline} 193

[14.4.]{.underline} [报表界面]{.underline} 194

[15.]{.underline} [EAS基础数据]{.underline} 196

[15.1.]{.underline} [组织]{.underline} 196

[15.1.1.]{.underline} [管理单元（CU）]{.underline} 196

[15.1.2.]{.underline} [业务组织]{.underline} 197

[15.1.3.]{.underline} [实体组织和虚体组织]{.underline} 199

[15.1.4.]{.underline} [组织委托关系]{.underline} 200

[15.2.]{.underline} [用户]{.underline} 202

[15.2.1.]{.underline} [用户类型]{.underline} 202

[15.2.2.]{.underline} [缺省组织]{.underline} 203

[15.2.3.]{.underline} [用户组织范围]{.underline} 203

[15.2.4.]{.underline} [用户功能权限]{.underline} 204

[15.3.]{.underline} [EAS职员和职位]{.underline} 204

[15.4.]{.underline} [物料和客商]{.underline} 206

[15.4.1.]{.underline} [基本信息]{.underline} 206

[15.4.2.]{.underline} [多标准分类]{.underline} 206

[15.4.3.]{.underline} [多业务属性]{.underline} 207

[15.4.4.]{.underline} [组织隔离和共享]{.underline} 208

[15.4.5.]{.underline} [物料计量单位]{.underline} 209

[15.4.6.]{.underline} [物料辅助属性]{.underline} 210

[15.5.]{.underline} [仓库和库存]{.underline} 211

[15.6.]{.underline} [核算项目]{.underline} 211

[15.6.1.]{.underline} [自定义辅助核算项目]{.underline} 211

[15.6.2.]{.underline} [添加非标核算项目]{.underline} 212

[15.7.]{.underline} [其他业务知识]{.underline} 212

[15.7.1.]{.underline} [税率税额]{.underline} 212

[15.7.2.]{.underline} [价格和折扣]{.underline} 212

[15.7.3.]{.underline} [数量计量]{.underline} 213

[15.7.4.]{.underline} [币别和金额]{.underline} 213

[16.]{.underline} [WAFII开发]{.underline} 214

EAS和BOS开发概述
================

ERP软件开发的特点
-----------------

### 注重管理和业务

软件为企业管理服务，IT作为一种工具和平台用于解决企业的管理和业务问题，改善流程提高效率。软件开发公司和团体必须对服务的对象、内容、范围、目标有清晰准确的认识。软件最终应用效果的好坏，和管理、业务的流程是否科学合理有着直接的关系，优秀的ERP软件公司和开发顾问不仅仅是技术上优秀，在对业务的理解、分析、洞察上同样优秀。

### 注重用户感受

ERP软件最终是交付给人使用的，软件的界面友好性、美观性非常重要。关键/非关键信息的排布浏览，界面信息录入次序、界面的齐整、操作的快捷方便、响应速度和信息提示等等，这些要素是和软件代码质量和功能同等重要的要素，从设计、开发到测试环节都要应该用心设计。

### 需求和结果容易出现偏差

软件开发存在这样一个信息传递的过程：最初用户需求---＞用户内部梳理---＞需求调研---＞需求分析---＞方案设计---＞编码---＞测试---＞交付，在这样一个链条中，各环节会由不同专业不同部门来承担，特别是大型企业和ERP项目，信息面广、涉及的部门多、业务复杂、人员能力和配合程度各不相同，容易造成信息在传递过程中遗漏、丢失、改变。

### 持续建设

企业经营发展过程中，其管理流程和业务模式处于不断变化的状态中，会有改变、调整、延伸、深化细化等等，这些变化有的可以用现有IT服务满足，有的则超出范围，需要对IT系统和服务做持续的改进或扩展。

EAS和BOS平台开发的优势
----------------------

-   快速搭建业务模型，建立业务实现框架

-   专注于业务开发，屏蔽大量底层开发

传统开发中的网络通讯，数据库及连接/读写、数据和界面的交互等由平台处理；Java开发中令人头疼的UI设计、控件设计在图形化设计工具中即可完成。

-   常见ERP软件功能平台提供了大量功能强大的实现

例如：权限和日志，用户和安全认证，消息中心，工作流的配置/管理/维护，套打设计和实现，单据转换配置和实现，报表设计和发布，自动编码平台，后台事配置和调度等等

-   大量成熟的基础模块、业务模块可以直接使用

ERP开发中常见的组织架构、职员、物料、客户供应商、计量单位、区域等等在平台中已经强大的功能实现，无需从头构建。

![](media/media/image2.png){width="6.4118055555555555in"
height="4.285416666666666in"}

 EAS和BOS平台
=============

EAS的架构
---------

-   EAS是典型的三层架构，基于J2EE技术搭建

-   EAS的标准客户端不是传统意义上的浏览器，是基于Java GUI技术的客户端

-   EAS提供基于浏览器的Portal门户，可以基于BOS开发WEB应用。

EAS和BOS的构成
--------------

-   EAS系统由EAS应用服务器、EAS客户端、数据帐套构成；

-   EAS应用服务器由Apusic服务器、部署在其上的EAS产品和应用、EAS服务管理器三个主要部分构成。Apusic服务器是标准的J2EE服务器，用户也可以使用WebSphere、WebLogic作为J2EE服务器。

-   BOS开发体系由BOS开发工具、开发解决方案（即开发项目）构成。

EAS和BOS安装
------------

### 安装包说明

本次培训提供的EAS版本为8.2，安装包目录及说明如下：

![](media/media/image3.png){width="6.415972222222222in"
height="2.3069444444444445in"}

-   Server\_CDROM：EAS服务器安装程序

-   Client\_CDROM：EAS客户端安装程序

-   BOSModular\_CDROM： BOS安装程序

-   DemoDC：EAS演示帐套，MS SQL
    Server2008R2数据库的备份文件，用于EAS测试运行。

### EAS开发平台安装

本步骤说明是按照培训目的给出，在实际项目开发中视情况可忽略部分步骤。每一步骤的详细操作可参考后面章节的内容。

-   安装MS SQL Server2008R2，恢复演示帐套到数据库；

-   安装EAS
    Server，安装过程中按照提示注册演示帐套、建立服务器实例和部署；如果在安装过程中数据库注册和实例部署未完成，可以启动EAS管理控制台完成；

-   在EAS管理控制台中导入Apusic许可证和EAS产品许可证，用于测试服务器的服务器，在安装完成后会自动生成一个有期限、部分模块的EAS产品许可证；

-   安装EAS客户端，并按提示完成连接配置；

-   安装BOS开发工具，完成后切换到BOS建模开发透视图，完成在线注册（需要自行注册一个金蝶开发社区账号）；

-   在BOS建模开发透视图下，从EAS服务器导入解决方案。

-   建议安装一个支持UTF8格式的文本编辑器，例如：Sublime、EditPlus、UltraEdit等。

EAS演示帐套
-----------

EAS标准版提供了基于MSSQL
Server2008R2的演示帐套的备份文件，开发测试人员可以还原到MSSQL
Server2008R2中未来作为EAS数据帐套。一个EAS服务器可以注册多个数据帐套。

不可以在数据库服务器中新建一个空数据库作为EAS的数据帐套，因为EAS运行、管理需要大量的基础数据库表。

可以在EAS服务器管理控制台的数据中心管理中通过【新建】新建数据帐套。作为开发和测试目的的数据帐套，不推荐通过这种方式建立数据帐套，因为ERP系统运行所需的大量基础资料和规则配置需要你自己花大量时间进行搭建。

新建和演示帐套会有两个登录账号，用户名和密码：administrator/kdadmin，user/kduser，前者是系统管理账号，后者是业务管理账号。

一般EAS的用户会和职员、客商关联，但是administrator和user没有，在EAS的某些模块测试（HR、协同等）、工作流测试中不可用。

EAS服务器
---------

### 重要特性

-   一个EAS服务器可以建立多个服务实例，这些实例可以通过集群控制器建立集群应用；

-   一个EAS服务器可以管理多个数据帐套；

### EAS服务器的重要目录

假设EAS服务器安装目录是D:\\Kingdee

-   D:\\Kingdee\\apusic：存放Apusic服务器的代码和配置文件；

-   D:\\
    Kingdee\\eas\\admin：存放EAS服务器管理控制台的代码、配置、下载的补丁；

-   D:\\
    Kingdee\\eas\\server：存放EAS产品和应用的代码、元数据、配置、本地数据；

-   D:\\ Kingdee\\eas\\server\\properties：存放EAS服务器的配置；

-   D:\\
    Kingdee\\eas\\server\\profiles\\server1（1\~n）：EAS服务实例的日志输出、配置、本地数据；子目录**Logs存放日志输出，开发人员应当重点关注并经常通过日志分析错误**。

-   目录：lib存放代码Jar包；metas存放元数据Jar包；bin存放执行文件；

EAS管理控制台
-------------

![](media/media/image4.png){width="7.024305555555555in"
height="3.46875in"}

### 开发需要关注的内容

-   BIM服务器：BOS远程导入解决方案、更新解决方案、部署解决方案时需要启动此服务；如果服务器有多网卡，需要指定服务绑定的IP地址。

-   数据中心：新建或者注册已有的数据库帐套，对于开发人员，推荐注册已有的演示帐套或者客户的测试数据帐套，避免在系统中从零开始进行初始化实施工作（常见的有：组织架构搭建，新增用户并授权，建立职位、人员、物料、客商等基础资料，配置自动编码、BOTP等规则，添加必要的工作流，等等）。

-   服务器日志：当任务执行发生错误时，可以通过此处查看服务端的日志输出进行分析处理；服务器日志中的内容和日志文件是同步的。服务器日志不会自动刷新，需要执行【刷新】才能查看最新内容。

-   服务器虚拟内存分配：由于JVM的限制，服务器内存不能大于1.5G，否则服务器不能启动；对于大内存服务器，可以通过建多服务实例（通过集群控制器联接）来扩展可用内存容量。

-   应用服务器移植：需要修改部分配置文件；视移植环境可能需要修改数据中心配置。

EAS客户端
---------

### 重要特性

-   客户端启动时连接服务器时，如果服务器的代码和元数据有更新时，客户端会自动更新

-   客户端提供小助手功能，可以在后台运行监控和提示消息；

-   一个客户端可以选择登录不同的数据帐套；

### EAS客户端的重要目录

假设EAS客户端安装目录是D:\\Kingdee：

-   D:\\ Kingdee\\eas\\client：存放EAS客户端所有文件；

-   D:\\
    Kingdee\\eas\\client\\logs：**存放日志输出，开发人员应当重点关注并通过日志分析错误**。

-   D:\\ Kingdee\\eas\\client\\lib：存放代码Jar包；

-   D:\\ Kingdee\\eas\\client\\metas存放元数据Jar包；

-   D:\\ Kingdee\\eas\\client\\bin存放执行文件；

### EAS客户端框架

![](media/media/image5.png){width="5.7868055555555555in"
height="4.043055555555555in"}

### 客户端移植

可以把安装目录整个拷贝到其他目录或计算机直接使用，需要修改文件：【安装目录】\\eas\\client\\bin\\set-client-env.bat，修改其中的变量"EAS\_HOME、JAVA\_HOME"为实际的路径。

BOS开发工具
-----------

BOS开发工具实质是在IBM的Eclipse开发框架上，金蝶做了大量的插件和功能模块，形成面向金蝶EAS的ERP开发平台。

这些插件的最核心功能就是实现了金蝶独有的"面向模型开发"思想。面向模型开发包括：

-   可视化建模工具

-   模型编译：依据模型生成Java框架代码

-   模型运行时引擎：Java运行时对模型的访问和操作支持

![](media/media/image6.png){width="6.416666666666667in"
height="3.8201388888888888in"}

### BOS开发透视图

[[]{#OLE_LINK1 .anchor}]{#OLE_LINK2
.anchor}切换透视图：菜单【窗口】【打开透视图】【其他】，或者工具栏右侧的【透视图切换】

![](media/media/image7.png){width="5.7444444444444445in"
height="4.048611111111111in"}

-   金蝶BOS业务建模工具（BIM）：面向模型的高级建模工具，提供整体建模功能

-   金蝶BOS设计开发工具（BOS
    Studio）：对模型"零件"进行编辑修改的工具，通常用于模型的细节调整

-   工作流连接：建立到EAS服务器和数据帐套的连接配置，用于工作流编辑

-   工作流编辑：获取数据帐套中的工作流配置，可以建立、修改、删除流程配置

-   K-SQL
    Tool：基于K-SQL语言的查询分析器，因为有其它替代查询分析器，所以基本不用

### 反编译设置

对于开发人员学习EAS产品的开发方法、分析产品问题、改造产品功能逻辑来说，在BOS上安装反编译工具查看部分源码对于实现目的和提高效率是非常关键的。BOS8.0及以后版本已经集成反编译工具，作者强烈建议开启反编译功能的两个选项设置：输出原始行号，行号对齐代码。该选项位于菜单"窗口------首选项------Java------反编译器"

![](media/media/image8.png){width="5.191666666666666in"
height="1.7090277777777778in"}

BOS解决方案
-----------

### 导入解决方案

BOS刚安装好时没有解决方案（开发方案），需要从EAS服务器上导入。切换到BIM透视图，在业务单元管理空白区域点右键选择【导入解决方案】，或者从菜单执行。支持两种导入方式：

-   本地导入：需要本机安装EAS服务器，指定EAS服务器路径（**到server目录**）；

-   远程导入：需要EAS服务器启动BIM服务，输入服务器的IP地址、端口、口令（管理控制台BIM服务的用户和口令，默认是admin/admin）。

![](media/media/image9.png){width="3.2916666666666665in"
height="2.0104166666666665in"}![](media/media/image10.png){width="3.78125in"
height="2.9166666666666665in"}

![](media/media/image11.png){width="3.279861111111111in"
height="1.8430555555555554in"}

注意：作者在EAS8.2的一些实例环境上执行远程导入时，遇到过已经显示"导入完成"但是并没有生成解决方案，原因是从服务器上下载某些语言包时发生异常。遇到该问题最简单的办法就是把服务器的server目录拷贝到本地，采用"本地导入"的方式完成导入。

### 解决方案目录

> 选择解决方案根节点，右键点击【打开资源目录】。重要目录和文件如下：

-   ![](media/media/image12.png){width="3.18125in"
    height="2.357638888888889in"}basemetas：从服务器导入的元数据Jar包；

-   newMetas：更新解决方案后保存新的元数据Jar

-   lib：从服务器导入的元数据Jar包；

-   metadata：二次开发新增或者产品中被改动过的元数据文件；

-   depoyed\_metas：发布模型会在此路径下生成当时的元数据文件拷贝；

-   src：二次开发形成的Java源代码文件；

-   classes：src中的源代码编译成执行时的class字节码文件；

-   runtime：BOS快速测试运行所需的服务端、客户端的配置文件；

-   **datacenters.xml**：解决方案的数据中心配置文件，当数据库连接配置变化时，可修改此文件。

### 设置解决方案

建议取消勾选"元数据显示为单树"，把产品元数据和二次开发元数据单独列示，更清晰。

![](media/media/image13.png){width="1.8333333333333333in"
height="1.2784722222222222in"}![](media/media/image14.png){width="4.793055555555555in"
height="2.4819444444444443in"}

注意："文件过滤"和"目录过滤"设置会影响在BIM透视图中看到的目录和模型文件。

### 测试账套设置

![](media/media/image15.png){width="6.221527777777778in"
height="3.2631944444444443in"}

关键功能：

-   数据库帐套更新和测试：当EAS服务器注册的数据中心有变化时，可以通过这里的更新帐套功能进行同步更新。这里的数据中心配置将保存到datacenters.xml文件中。

-   手工修改或添加数据中心：找到文件"\[解决方案目录\]\\datacenters.xml"，用支持UTF-8格式的文本编辑器打开，例如BOS、sublime、EditPlus、UltraEdit等，仿照原文本格式，复制datacenter节点并修改其中的"dbname、dbuser、dbpassword、datasource、id、name"等属性，id属性必须唯一

![](media/media/image16.png){width="5.564583333333333in"
height="2.915277777777778in"}

### 解决方案移植

有时需要通过拷贝已有解决方案建立另外的开发方案，当源路径和目标路径不同是，修改以下配置文件中的路径：

-   \[解决方案目录\]\\\[方案名称\]\_lib.xml：EAS产品Jar包路径配置

-   \[解决方案目录\]\\runtime\\apusic\\config\\server.xml：apusic路径配置

### 备份解决方案

解决方案的磁盘空间占用很大，整体备份耗费时间和磁盘空间相当长，作为开发和测试人员，可以仅选择备份metadata和src即可。备份方法是把这两个目录统一打成压缩包，以约定的命名习惯拷贝到指定的目录中。

BOS和解决方案更新
-----------------

### 更新BOS工具

EAS服务中安装的补丁中可能含有BOS工具的代码和组件更新，可以执行菜单【工具】【更新BOS工具】，按照系统提示完成更新。

更新完成后，需要清理BOS过时的配置，否则在使用BOS、进行BOS快测时会遇到各种不可预料的错误。清理方法：执行批命令：\<BOS安装目录\>\\
BOSModular\\ clear\_bosmodular\_env.bat

### 更新解决方案

解决方案中保留了服务器上的元数据和代码Jar包副本，当服务器安装补丁或者升级以后，两边的元数据和代码就不再一致，可以通过更新解决方案的功能从服务器同步元数据和代码Jar包到解决方案中。

执行更新解决方案功能方法：菜单【方案】【更新解决方案】。更新解决方案操作同"导入解决方案"，更新前需要选中解决方案根节点。

 BOS开发总体介绍
================

模型驱动开发（MDA）
-------------------

"模型驱动"包含两个方面：

-   模型：把企业经营管理活动中的各种基础数据、业务及数据抽象成模型，利用BOS工具建立对应的模型去描述这些数据和业务。

-   驱动：BOS能够对模型进行发布和编译，把模型转换成在J2EE平台上可运行的JAVA代码。

BOS的MDA开发优点：

-   提供可视化建模工具，快速建立、维护业务模型；

-   通过模型快速生成可运行的整体代码，大大降低开发代码工作量；

-   没有数据库设计、建模、管理的过程，数据库由BOS工具依据模型自动维护；

-   开发人员无需关注底层实现细节，专注于业务逻辑的开发实现。

模型要素及构成
--------------

### 模型的关键要素

-   界面：模型的外观，包括信息列表界面和信息展示界面；

-   数据：模型需要记录、处理的数据；

-   功能及菜单：模型能够提供的功能和操作方法；

-   权限；模型功能的执行许可分配

### 元数据

是描述数据（模型）的数据，用于记录保存模型的所有数据。BOS建立的模型数据并不是放在单一文件中，而是按照模型的内容进行分割存储在多个文件，所有模型（元数据）文件的格式为UTF-8编码的XML文件。

一个简单的模型包含的元数据文件有：编辑界面EditUI，列表界面ListUI，实体Entity，关系Relation，表Table，查询Query，功能Function，单元集成描述BizUnit，。此外还有为支撑模型及代码开发的元数据：枚举Enum，异常Exception，权限permission，日志Log，业务功能Façade，包Pakage。

BIM和BOS Studio介绍
-------------------

BOS按透视图分为2大部分：业务建模工具BIM，BOS设计开发工具BOS Studio

BIM提供从整体上快速建模的功能，建模时会自动生成模型所需的各种元数据；提供整体发布模型、编译代码的功能；BIM中无法看到模型的各个构成部分和部分细节。

BOS
Studio能够看到模型的所有细节，可以单独构建和调整所有的元数据及其细节，但是开发效率比BIM低很多。BOS
Studio提供对单个元数据文件进行发布的功能，**但是发布后生成的Java代码不会自动编译，开发人员需要手工在Java透视图中刷新代码**，让Eclipse去编译Java产生class。

一般的，我们在BIM里快速建立模型主体和绝大部分功能，然后在BOS
Studio里进行局部调整。

BOS开发成果的发布、部署和运行
-----------------------------

二次开发增加模块或者修改产品，并不会改动标准产品Jar包和补丁包中的代码和元数据，而是形成新的代码和元数据文件，部署时形成专门的Jar包放在服务器上。JVM在运行时会按照EAS约定的加载顺序加载代码和元数据，加载顺序：二次开发Jar＞补丁Jar＞标准产品Jar

### 发布和部署

在BOS中完成建模后，需要对模型进行发布，产生代码框架，然后进行代码开发；开发完成后需要部署到EAS服务器上运行。

EAS7.5及更早版本中，所有的开发成果（元数据和代码）统一打成2个Jar包，一个是元数据Jar包，一个是代码Jar包，部署在EAS服务器和客户端指定的目录如下：

+-----------------+-----------------+-----------------+-----------------+
| **位置**        | **类别**        | **路径（以\<安装路径\\e | **作 用** |
|                 |                 | as\\\>为相对路径）** |            |
+-----------------+-----------------+-----------------+-----------------+
| EAS服务器       | 元数据          | server\\metas\\ | 服务器运行期使用 |
|                 |                 | sp-bim-metas.ja |                 |
|                 |                 | r               |                 |
+-----------------+-----------------+-----------------+-----------------+
|                 |                 | server\\deploy\ | 客户端更新下载使用 |
|                 |                 | \fileserver.ear |                 |
|                 |                 | \\easWebClient\ |                 |
|                 |                 | \               |                 |
|                 |                 |                 |                 |
|                 |                 | metas\\[[]{#OLE |                 |
|                 |                 | _LINK4          |                 |
|                 |                 | .anchor}]{#OLE_ |                 |
|                 |                 | LINK3           |                 |
|                 |                 | .anchor}sp-bim- |                 |
|                 |                 | metas.jar       |                 |
+-----------------+-----------------+-----------------+-----------------+
|                 | 代码            | server\\lib\\sp | 服务器运行期使用 |
|                 |                 | \\eas\_sp.jar   |                 |
+-----------------+-----------------+-----------------+-----------------+
|                 |                 | server\\deploy\ | 客户端更新下载使用 |
|                 |                 | \fileserver.ear |                 |
|                 |                 | \\easWebClient\ |                 |
|                 |                 | \               |                 |
|                 |                 |                 |                 |
|                 |                 | lib\\sp\\eas\_s |                 |
|                 |                 | p.jar           |                 |
+-----------------+-----------------+-----------------+-----------------+
| EAS客户端       | 元数据          | client\\metas\\ | 客户端运行期使用 |
|                 |                 | sp-bim-metas.ja |                 |
|                 |                 | r               |                 |
+-----------------+-----------------+-----------------+-----------------+
|                 | 代码            | client\\lib\\sp | 客户端运行期使用 |
|                 |                 | \\eas\_sp.jar   |                 |
+-----------------+-----------------+-----------------+-----------------+

EAS8.0及后续版本提供了分包部署功能，用户可以对二开元数据和代码按照包路径进行分割，打成若干Jar文件，服务器的部署目录相应的调整为：lib\\bim\\、metas\\bim\\

###  手工打包部署

对于无法使用BOS部署功能进行部署的服务器，开发人员需要自行打包，以及拷贝文件到EAS服务器相应目录。

打包命令示例（可以保存到bat文件）：

D:\\kingdee75\\bos\\BOSModular\\jdk\\bin\\jar -cvf
D:\\待部署\\sp\_contface\_src.jar -C E:\\workspace\\HFGas75\\classes .

D:\\kingdee75\\bos\\BOSModular\\jdk\\bin\\jar -cvf
D:\\待部署\\sp\_contface\_metas.jar -C
E:\\workspace\\HFGas75\\deployed\_metas .

### 开发代码在发布和部署中的传递

### JVM运行期加载开发成果

服务器和客户端加载元数据和代码Jar的优先顺序：**二次开发 ＞ 补丁 ＞
产品**

这意味着若产品中的元数据和代码在BOS中被改动，将来部署到服务器以后，产品中的同路径名的元数据和代码在运行期将不再被加载，JVM会从二次开发包中优先加载改动后的元数据和代码。

也意味着，我们开发改造产品以后，未来如果想要恢复产品原有的功能，只需要从解决方案中删除相应内容，或者从服务器二次开发Jar包中删除相应内容即可。

客户化开发冲突
--------------

### 场景

如上节描述，二次开发的元数据优先于产品和补丁生效，那么当遇到下面情形：开发人员在1月1日修改并部署了产品中"职员"模型相关的元数据，金蝶总部在2月1日发布了新的补丁对"职员"元数据进行了调整并增加了新的属性和功能，在EAS服务器上安装该补丁后，补丁提供的新属性和功能在运行期不会生效，因为其代码和元数据不会被加载。如果补丁中的其他模块引用该属性，运行时就会产生异常错误（找不到属性）。

### 元数据二开冲突解决

在EAS7.0之前总部提供了合并元数据工具，能够识别出补丁和客户化开发增加的内容，但是该工具很难使用并且不能100%解决问题。项目加入二开内容后，在后续的补丁按照和版本升级过程中，仍然需要开发人员介入，帮助合并元数据以及处理合并过程中的错误。

在EAS7.0以及后续版本，总部推出了DEP平台（动态扩展平台），该平台提供在运行期对加载到内存中的元数据进行动态调整的强大功能，而不需要在BOS中静态修改和部署元数据，在DEP平台上改动元数据几乎对补丁和升级不产生冲突。此后只要DEP可以做到的标准产品元数据扩展开发，全部转移到DEP平台上完成。

关于DEP的开发方法，后面有专门章节进行介绍。

### 代码的版本冲突处理

类似的多版本冲突在代码开发中可能也会遇到，一般来说，EAS已经提供了对前端UI和后端服务的代码进行扩展的方法（扩展类），开发人员应当进行利用代码的扩展类来做产品的扩展改造。但是不排除某些需要的实现必须反编译产品代码并做修改，这样就会产生代码冲突。BOS没有提供代码冲突的解决办法，只能由开发人员进行判断和人工合并。

子系统树及生成
--------------

![](media/media/image17.png){width="4.39375in"
height="2.111111111111111in"}EAS的很多系统配置管理中，需要按模块及业务单元进行规则的设定和管理，例如工作流配置、编码规则配置、单据转换规则配置、数据权限配置等等，所有模块及业务单元以树形列示，称为子系统树。

![](media/media/image18.png){width="4.739583333333333in"
height="3.53125in"}

![](media/media/image19.png){width="2.161111111111111in"
height="3.2354166666666666in"}

![](media/media/image20.png){width="4.635416666666667in"
height="2.9895833333333335in"}

开发人员在BOS中新增包、单据以后，应当通过生成子系统树功能把它加入到子系统树中，生成子系统树的方法有：

-   选择解决方案，点击菜单【工具】【生成子系统树】。对于EAS8.0及后续版本，该方法仅用于BOS测试运行

-   从包更新子系统树：生成子系统树的过程比较长，开发人员可以在开发成果所在包的右键菜单中执行【从包更新子系统树】，仅更新指定包的子系统树，可以大大减少子系统树更新的耗时。对于EAS8.0及后续版本，该方法仅用于BOS测试运行

-   [[]{#OLE_LINK11 .anchor}]{#OLE_LINK10
    .anchor}管理控制台更新子系统树：BOS8.0及后续版本，由于采用分包部署机制，BOS中产生的子系统树不会部署到服务器，因此需要在服务器上的管理控制台上执行"生成子系统树"。EAS8.0及以上的某些版本中，如果二次开发增加了新的包路径，还需要在生成子系统树前修改eas\\server\\properties\\SubSystem\_bos.xml文件，把二开增加的包路径注册到该文件中，否则不会为新路径下的单据生成子系统树。生成的子系统树文件位于server\\metas\\bos\\
    mdbview-metas.jar

![](media/media/image21.png){width="6.658333333333333in"
height="3.678472222222222in"}

EAS和BOS二次开发规范
--------------------

> 请参考金蝶公司颁布的相关文档。重点强调：

-   应当对所有模块和业务单元分目录（包）建立，可参考产品中各模块的包路径；

-   所有元素的命名采用英文或英文简写组合，做到简练、含义清晰；

 元数据介绍及开发关注点
=======================

**为了避免初学者陷入细节的陷阱，本章仅对开发需要关注的元数据进行局部介绍。或者初学者直接跳到第5章节先行学习。**

查看元数据的方法：先在BIM透视图下相对独立的路径下，建立一个简单的模型，然后切换的BOSStudio透视图中观察。

什么是元数据
------------

请设想：你在BOS中建立一个单据，在界面上增加字段、修改样式、拖拉控件位置和大小......做了一系列操作后，保存单据并关闭BOS。然后，下次当你再次打开这张单据时，看到的还是上次修改保存后的样子。BOS是如何做到的呢？

首先它一定要有一整套标记语言用来描述你修改后的单据里有哪些字段和控件、控件的样式（位置、大小、前景色、背景色......等等），那么这些用来描述开发成果（单据、基础资料、界面等等）的数据，就称为元数据。

百度给出的解释是：元数据（Metadata），为描述数据的数据（data about
data）。BOS采用了XML格式来描述元数据，并且称之为"模型"，下图是BOS中一种名为entity的元数据的内容

![](media/media/image22.png){width="6.416666666666667in"
height="3.3027777777777776in"}

> 其次，你应该可以想到这些数据可能是存储在某个特定的数据库或者文件里，以便后来打开这些单据时，还能完整的读取出来。是的，BOS采用了文件存储的方式，所有的元数据都是XML文件。

![](media/media/image23.png){width="6.415277777777778in"
height="3.00625in"}

最后，你在BOS里开发了一张单据，BOS是否使用了唯一的文件来存储这个单据的所有元数据呢？理论上当然可以，但是BOS没这么做。BOS把单据的元数据划分了类型，按照类型分别生成相应的文件来保存这些元数据，你可以认为这些"拆开"的元数据，是完整单据（模型）的各种"零件"。

-   实体（Entity）：保存单据的基本信息、字段定义、功能定义、事件定义等

-   界面（UI）：保存单据的界面和控件的基本信息、样式数据、数据绑定规则等

-   查询（Query）：描述一个SQL语句，当然提供了很多属性定义，这些属性未来在EAS各种应用场合中控制SQL查询所具有的行为和样式

-   权限（Permission）：描述开发者为单据添加的需要做权限控制的"点"，即权限项

-   其它：Table、Relation、Façade、Function、Enum、Exception等等

实体（Entity）
--------------

实体是模型中最核心的元数据，记录了模型的部分基本属性、对应的Table元数据、模型属性及对应的数据库字段、方法和事件，记录模型的BOSTYPEID，定义模型发布后生成的核心框架类。实体可以继承。对于一个具有分录的单据模型来说，BOS会生成单据体的Entity，各分录的Entity。

![](media/media/image24.png){width="3.6006944444444446in"
height="0.9486111111111111in"}

### 基础信息

![](media/media/image25.png){width="6.460416666666666in"
height="3.654861111111111in"}

#### 重要扩展属性

-   billFormulaClass：用于为单据增加BOTP自定义函数定义；

-   ControllerBeanEx：用于生成服务端ControllerBean的扩展类。

#### 对应表对象

可快速查找实体对应的数据库表名。

### 实体属性

![](media/media/image26.png){width="6.098611111111111in"
height="3.688888888888889in"}

![](media/media/image27.png){width="4.582638888888889in"
height="2.8784722222222223in"}

#### 两种属性

-   钥匙图标：自有属性，与其他表和对象没有关系；

-   圆点图标：关联属性，引用对象实例（其他表的数据记录），保存对象的ID（数据记录的FID字段），其含义类似于数据库中的外键。

#### 多语言属性

限字符类型的自有属性，如果勾选，则数据库表会用3个字段保存该属性的英文值、简体中文值、繁体中文值，其后缀分别是：\_L1、\_L2、\_L3。

DataBase.entity实体中的name和description属性是多语言属性，因此从该实体继承下来的所有基础资料的name和description属性，其数据库对应的字段是：FName\_L1、FName\_L2、FName\_L3和FDescription\_L1、FDescription\_L2、FDescription\_L3。

#### 字段命名

可以方便的查找各属性对应的数据库表字段，字段命名规则如下：

-   产品或基类实体的自有属性：F\<属性名\>

-   产品或基类实体的多语言自有属性：F\<属性名\>\_L1，F\<属性名\>\_L2，F\<属性名\>\_L3

-   产品或基类实体的关联属性：F\<属性名\>ID

-   二次开发增加的自有属性：CF\<属性名\>

-   二次开发增加的多语言自有属性：CF\<属性名\>\_L1，CF\<属性名\>\_L2，CF\<属性名\>\_L3

-   二次开发增加的关联属性：CF\<属性名\>ID

#### 属性的重要扩展属性

-   isInCode：是否参与编码规则的属性取值

-   isForMapping：是否参与BOTP映射

-   isForGrouping：是否要参与BOTP分组合并

### 实体方法

发布后在业务单据对应的接口、ControllerBean中会生成框架方法，通过Factory进行远程或本地调用，方法的关键属性：

-   事务属性：定义方法执行时的事务管理类型，一般需要修改成Required

-   参数：方法执行时所需的参数，一般根据需要增加

-   异常：定义方法执行时可能会抛出的异常，一般会增加EASBizException

![](media/media/image28.png){width="6.409027777777778in"
height="3.877083333333333in"}

### BOSTYPEID

所有实体都有一个唯一的类型ID：BOSTYPEID，8位字符串，可切换到"源代码"页签，查找bostype标签里的值。这个ID的用途主要有：

-   向数据库相应的表中插入记录，需要生成记录的FID，EAS数据库中有一个NewBOSID函数，需要传递BosTypeID作为参数；

-   在代码中用BosTypeID判断和匹配单据的类型。

查询（query）
-------------

用于描述一个数据库查询语句，常用于：在ListUI的数据绑定和获取；BizPromptBox控件弹出窗体中显示数据的查询。相对于一个SQL语句，以元数据形式描述的Query能够封装更多的属性设置，并在运行时根据这些属性设置，定制界面和查询操作。

可以在代码中为Query定制过滤条件、字段选择和排序项，由QueryExecutorFactory及引擎转换成数据库SQL。

### "定义"页签

![](media/media/image29.png){width="6.413194444444445in"
height="2.8645833333333335in"}

"子对象"定义主实体对象和子对象、子对象的子对象，如何关联，可理解为SQL语句中的多表联合查询时，各表之间的关联定义，例如：

T\_SD\_SaleOrder SaleOrder

> **INNER JOIN** T\_SD\_SaleOrderEntry SOE **ON**
> SaleOrder.FID=SOE.FParentID
>
> **INNER JOIN** T\_PM\_User User **ON** SaleOrder.FAuditID=User.FID
>
> ......

开发人员可以根据需要自己添加子对象，有两种添加方式

-   导入方式：通过实体间的关联属性自动引入其他子对象；

-   增加方式：主、从对象无关联属性，两者的关系需要人为建立。

无论是那种添加方式，开发者都需要关注**连接类型**选项：

-   "默认类型"最终转换成 内连接（Inner Join）；

-   "父对象所有行"最终转换成 左连接（Left Join）；

-   "子对象所有行"最终转换成 右连接（Right Join）；

不同的方式对于查询出的结果集会产生不同的影响。一般来说，连接应当设置成"父对象所有行"，以避免在运行时某些数据由于某个字段为空而不能正确的查询显示。

表达式：当父子实体连接的判断条件不止一个时，表达式用于描述多个条件的组合关系。例如SQL语句：A
Inner Join B ON A.a1=B.b1 AND (A.a2\<B.b2 or
A.a2\>=B.B3)，表达式写成"\#0 AND (\#1 OR \#2)"。

###  "字段"页签

> 定义从实体（表）需要查询的字段，通过"导入"按钮可增加字段。

![](media/media/image30.png){width="6.409722222222222in"
height="3.189583333333333in"}

字段的关键扩展属性

-   isCommonQueryFilter：是否在通用过滤中显示作为过滤字段；

-   isCommonQuerySorter：是否在通用过滤中参与排序；

-   isUsingF7：在通用过滤中，用户选择对象时是否需要使用F7；

-   isVisibleForKDTable：控制查询对象中某列是否在KDTable中显示；

-   colWidthInKDTable：控制查询对象中某列在KDTable的显示宽度；

通用过滤说明：所有单据列表界面都提供了【查询】操作，点击后弹出的查询对话框中会包含一个通用过滤定义页签和一个排序定义页签。

F7查询说明：所有BizPromptBox（F7控件），点击放大镜按钮后，弹出数据选择窗体，此窗体的数据一般是根据设置的Query元数据查询获得。后2个属性控制其显示样式。

其他扩展属性一般很少修改，开发人员自行根据BOS给出的解释进行理解和尝试。

### "其他"页签

定义查询的参数、过滤条件、排序、主键定义，因为Query在代码中可随时定义视图（EntityViewInfo，包含过滤、选择、排序设置），所以一般不推荐在这里设置。

**关于主键**：如果建模时业务单元没有分录（例如基础资料），开发人员在其上额外增加了分录体，那么一定要修改这里的主键定义，必须把主分录的Id添加进去。否则运行时列表查询的结果集不完整。

### "SQL"页签

开发人员修改或者新增一个查询后，可以切换到"SQL"页签，观察生成的SQL语句。如果元数据有错误，系统会给予提示。

![](media/media/image31.png){width="6.413194444444445in"
height="2.966666666666667in"}

表（table）
-----------

![](media/media/image32.png){width="6.415972222222222in"
height="3.2743055555555554in"}

用于描述实体属性对应的数据库字段定义，开发人员一般不需要关注。

**关于主键：**主键名称由BOS自动生成，极少数情况下，主键名称会和其他模块重名，导致发布模型时会失败，提示"系统主键约束XXXX已经存在"，开发人员可在此修改主键名称，保持唯一。

界面（UI）
----------

### 常见的UI类型有：

-   从EditUI继承的编辑界面，从ListUI继承的列表界面；

-   从com.kingdee.eas.base.commonquery.client.CommonQueryPanel继承的自定义查询界面；

-   从CoreUI继承的各种自定义窗体界面；

![](media/media/image33.png){width="6.409722222222222in"
height="4.377083333333333in"}

### 重要视图及作用

如果在BOS
Stuido中没有出现所需视图，请从菜单【窗口】【显示视图】中选择打开。

-   包分类：以树形展示metadata和basemetas下的所有元数据和文件；

-   大纲：分类显示UI上所有的元素，例如：界面控件、按钮、菜单、Action等

-   属性：显示和设置指定UI元素的属性

-   数据绑定：显示和设置EditUI和ListUI上的数据绑定规则

-   校验信息：元数据校验信息输出

### 常见UI开发调整

-   表格样式调整：双击表格，弹出表格编辑对话框；

-   增加Action：在大纲中右键点击"Actions"节点，选择"新建Action"；

-   增加按钮或者菜单：从"控件选用板"中拖拽按钮或菜单控件到大纲的工具栏、菜单栏或者界面上，一般要绑定Action；

-   修改数据绑定：打开数据绑定视图，切换到"已绑定的控件"页签，可以增加或删除绑定规则

业务功能（facade）
------------------

类似于在Entity上定义的方法，系统中经常遇到一些方法，是很多单据都要使用，或者与单据无关，例如：获取服务器时间、获取服务器文件资源、某个模块下所有单据的共有操作等等，（如果定义在某个Entity上，就不清晰合理，维护也不方便），这些方法可以用Facade元数据定义。

Facade发布后会生成独立的接口、Factory、ControllerBean，可以通过Factory进行远程或本地的调用执行其中的方法。Façade里定义的方法，也需要注意事务属性、参数、异常、返回值等设置，和Entity方法的开发和注意事项相同。

![](media/media/image34.png){width="6.411111111111111in"
height="3.107638888888889in"}

功能（FUNCTION）
----------------

Function是对Entity和Facade中定义的功能进行包装描述（记住：只是描述，没有增加新的内容），经过Function包装描述的方法才能在工作流、后台事务中调用。

在BIM中为模型增加功能定义时，有个选项"功能绑定至工作流"，如果勾选，BIM就会自动把这个方法放到Function中包装描述。

![](media/media/image35.png){width="6.4118055555555555in"
height="4.247222222222222in"}

枚举（Enum）
------------

注意：BOS中用到的所有枚举，都应当在BOS Studio中事先建好。

新增枚举时数据类型默认是"STRING"，**强烈建议把数据类型设置成"INTEGER"**，这样未来在代码中进行比较、报表中进行数据分析时，会很方便。

枚举发布后，会产生独立的枚举类。

![](media/media/image36.png){width="6.413194444444445in"
height="1.957638888888889in"}

业务异常（exception）
---------------------

> 业务异常表示在系统运行过程中，可预见的业务逻辑错误。

![](media/media/image37.png){width="6.415972222222222in"
height="3.3465277777777778in"}

所有的业务异常都必须从EASBizException或其子类继承。异常消息中可以定义形如{0}、{1}
的参数。代码中构造异常时的常见写法：

**throw** **new** HeFeiBizException(HeFeiBizException.*NULL\_FIELD*,
**new** Object\[\]{\"项目\"});

Object\[ \]数组即用于替换参数，形成明确的异常信息。

权限（permission）
------------------

开发人员根据系统中需要控制的功能，定义相应的权限项，实现方式：

-   通过BIM的权限管理快速批量为业务单据的功能定义权限项（推荐）；

-   在BOS Studio中手工增加权限文件和权限项，并和功能绑定；

BOS中定义的权限项，以权限元数据文件进行保存；在运行时登录EAS客户端打开用户管理通过【文件】【同步权限数据】功能，把权限项定义从元数据文件读入数据库保存，然后在用授权中即可进行授权使用。请参考第5章节关于权限开发的描述。

日志（log）
-----------

开发人员根据系统中需要记录的功能，定义相应的日志项，实现方式：

-   通过BIM的日志管理快速批量为业务单据的功能定义日志项（推荐）；

-   在BOS Studio中手工增加日志文件和日志项，并和功能绑定；

BOS中定义的日志项，以日志元数据文件进行保存；在运行时登录EAS客户端打开日志管理通过【文件】【同步日志数据】功能，把日志项定义从元数据文件读入数据库保存。请参考第5章节关于日志开发的描述。

两个重要的配置文件
------------------

发布Entity和Façade后，系统自动建立或者修改以下两个文件：

-   entity\_pkmapping.properties

-   facade\_pkmapping.properties

保存BOSTypeID和元数据包路径和名称的对应关系。如果丢失这种关系，系统运行时会提示找不到XXXXXXXX对应的元数据。

常见BOS Studio开发
------------------

-   调整Entity和Query属性，一般Entity需要调整的有：事务属性、参数、异常；Query属性的字段扩展属性，关联属性的显示名称。

<!-- -->

-   调整EditUI和ListUI属性和控件设置

-   增加系统所需的Façade、异常、枚举

-   拷贝定制Query，为套打、F7控件另外制作Query，可通过拷贝后修改的方法简化工作。

<!-- -->

-   定制UI，常见的有：FilterUI，UI对话框和消息框，UI报表开发。

 BIM建模和模型调整
==================

建模前的准备
------------

您需要按照第2章的内容建立BOS开发工具、解决方案，并对BOS开发工具和各透视图有所了解。

在实际开发的建模前，您需要花费时间和精力去整理和分析你要做的事情，也就是用户需求，并规划和设计好需要在BOS里建立哪些模型，模型应当具备的属性、功能等，各模型之间的业务关系。

本章节不对业务需求及其分析做过多阐述，仅描述建模的操作过程和关键点。

EAS模型的业务类别和业务属性
---------------------------

### 业务类别

EAS中的模型分为两大类：

-   业务单据：用于记录、处理企业经营管理活动中各种业务的模型，例如销售订单、销售出库单、领料单等等。企业每发生一次业务，就需要一张或多种单据来记录和处理业务。

-   基础资料：记录企业的基础信息，例如组织、职员、物料、客商等等，为ERP业务系统提供数据支撑，基础资料不反映企业的经营管理活动。

### 业务属性

ERP中常见的管理业务有：行政、财务、人力资源、采购、库存、销售、生产、成本、配送等，作为记录企业经营活动的业务单据及相应模型，也就具有这些业务类别的属性。

当为一个模型设定业务属性后，EAS提供这些模型单据在使用过程中，按照相应的业务组织进行自然隔离的功能，并且建立的权限项也是按业务组织进行授权和验权。

建立包
------

在一个大型项目开发过程中会建立很多单据模型，把这些模型分类存放对维护和管理模型是非常重要的。在BOS中按照包来分类存放模型，你可以简单的把包理解为文件路径。一般按照各单据的业务分类来建立包及其路径，你可以参考解决方案中基础元数据（EAS标准产品元数据）的分类方法。

![](media/media/image38.png){width="3.8541666666666665in"
height="2.8854166666666665in"}![](media/media/image39.png){width="4.416666666666667in"
height="3.301388888888889in"}

子系统简码：对模型的数据库表命名有影响，模型对应的表命名规则：

-   模型的数据表命名：T/CT\_\<子系统简码\>\_\<模型/实体名称\>

举例说明，客户化开发某个单据的名称如果是HouseRequest，所在包的子系统简码是HOU，那么数据库对应的表名称是：CT\_HOU\_HouseRequest。

建议：同一个业务系统下的不同包，取同一个子系统简码；不同业务系统之间子系统简码尽量不要相同。好处是以后在数据操作和维护时，可以清晰的在数据库中找到对应的表。

建立模型（业务单元）
--------------------

> 在相应的包目录上右键选择【新建】【业务单元】，按照向导操作如下：

![](media/media/image40.png){width="3.8020833333333335in"
height="2.8541666666666665in"}![](media/media/image41.png){width="3.8020833333333335in"
height="2.8541666666666665in"}![](media/media/image42.png){width="4.259027777777778in"
height="3.33125in"}

![](media/media/image43.png){width="3.8069444444444445in"
height="2.8513888888888888in"}

![](media/media/image44.png){width="4.270833333333333in"
height="2.375in"}

-   关于创建方式：选择"复制基础模板"，不要选择"新建"，因为基础模板已经提供了模型基础字段和功能，以及这些功能的代码实现，例如单据的新增、保存、修改、删除等等，如果选择"新建"，那么这些功能你需要全部自己来新增和实现。另外可以选择"复制已定义单元"，从以前设计的模型复制（以后详述）。

-   关于模板选择：一般选择"多分录单据基础模板"；如果不需要分录，则在下一步字段选择中可以把分录勾选框取消勾选；如果单据需要多分录，可以在向导完成后，手工添加分录；

-   单据头和分录：单据头是某次业务活动整体信息的记录，分录是活动中可能存在的相同结构多条数据的记录，例如销售订单，单据头用于记录销售活动的信息，如时间、销售员、销售部门、收款和送货方式等，分录用于记录销售的物料明细，例如物料名称及规格型号、数量、价格、金额、送货时间等等。单据是否需要分录、属性应该放在单据头还是分录，需要结合具体业务和用户操作方便性决定。

模型属性设置
------------

打开模型，菜单【业务单据】【单据信息】：

![](media/media/image45.png){width="5.903472222222222in"
height="3.5548611111111112in"}

-   这里可以调整模型的业务属性、业务组织字段；可以为单据增加更多的分录，或者删除分录

-   如需通过自动编码平台对单据进行自动编号，并使用"不允许断号"，则必须勾选"当编码规则不允许断号下自动填补断号"，否则自动编号将不能正常工作。推荐所有单据都勾选此项

为模型增加属性（字段）
----------------------

在模型空白处右键点击，从弹出菜单里选择【新增字段】，或者选择【字段管理】，在字段管理对话框中新增字段；如果要在分录中增加字段，需要右键点击分录表体，选择【新增字段】。

![](media/media/image46.png){width="2.2916666666666665in"
height="2.5833333333333335in"}![](media/media/image47.png){width="4.042361111111111in"
height="2.870833333333333in"}

### 数据来源

-   ![](media/media/image48.png){width="3.0548611111111112in"
    height="1.8590277777777777in"}手工录入：数据完全由用户"自由"录入，类型有：文本、日期、时间、布尔、数量。不同类型的字段，BOS会使用相应的界面控件进行处理和显示。

![](media/media/image49.png){width="2.0493055555555557in"
height="0.18125in"}![](media/media/image50.png){width="2.425in"
height="1.8041666666666667in"}

![](media/media/image51.png){width="1.363888888888889in"
height="0.18125in"}

-   基础资料类别：数据已经事先定义，用户只能从已定义的数据集合中选择录入。例如物料、人员等，用户不能随意录入，只能从物料表、人员表中选择。BOS自动为这种类型的字段绑定BizPromptBox控件，又称为F7控件。

![](media/media/image52.png){width="2.7916666666666665in"
height="1.2395833333333333in"}![](media/media/image53.png){width="4.21875in"
height="1.5833333333333333in"}

"显示字段"：基础资料对象有很多属性，例如物料的编码/名称/规格型号/类别/计量单位/体积/重量......等等，当用户选择了一个物料后，控件应当显示对象的哪一个属性，既是"显示字段"确定的。一般使用对象的名称或者编码字段作为"显示字段"。

-   已有基础资料相关属性：数据是其它基础资料对象字段的关联属性。例如：单据上已有"物料"字段，显示物料名称，但是用户还想看到规格型号，此时可另建一个字段叫"规格型号"，数据来源就是"已有基础资料相关属性"，基础资料字段是"物料"，相关属性选择"规格型号"。

![](media/media/image54.png){width="2.8in"
height="1.4333333333333333in"}

-   ![](media/media/image55.png){width="3.15625in"
    height="0.90625in"}固定下拉列表：数据来源是枚举数据。在BOS中枚举数据是用Enum类型的元数据描述的，需要先建立相应的枚举，才能在这里引用。

![](media/media/image56.png){width="2.8125in" height="0.84375in"}

-   其他业务单据：和"基础资料类别"类似，区别是：基础资料的数据来源只能选择"基础资料"类型的单元，本数据来源只能选择"业务单据"类型的单元，其他功能和操作是相同的。

### 字段的属性

选择字段，在"属性"视图中查看和修改（如果界面上没有显示属性视图，可以从【窗口】【显示视图】中找到并打开它）。

![](media/media/image57.png){width="6.240277777777778in"
height="3.7375in"}

需要关注的属性有：描述、标签文字、查询可见、录入可见、是否可用、是否必录项、是否在通用过滤中排序、是否在通用排序中显示。

界面布局和调整
--------------

### 控件位置排布工具

![](media/media/image58.png){width="6.441666666666666in"
height="2.466666666666667in"}

选择多个控件，对其位置进行齐整化，常用的例如：左对齐、顶对齐、宽度相等、高度相等、水平等间距、垂直等间距。BOS提供"规范布局"，按预定的规范对所有控件的位置、大小进行重设。

**注意：控件的尺寸、位置和排布对于用户体验非常重要，开发人员一定要注意避免混乱、不合理的界面字段排放。**

### 字段运行时的录入和显示顺序

在"字段管理"中，可以设置：

-   编辑界面中，各控件的Tab焦点转移顺序，表格的列焦点转移顺序；

-   列表界面中，各数据列的前后排放顺序

**注意：对于用户使用体验非常重要，开发人员一定要注意避免不合理的字段录入和显示顺序。**

### KD\_Layout布局

当界面窗体的大小改变时，整个界面的控件应当能够进行合理的缩放和位置调整。Java的标准Layout不支持这种应用，金蝶提供了能够解决此问题的布局KD\_Layout。

可以在业务单元的"属性"视图中找到并修改布局。

![](media/media/image59.png){width="5.147222222222222in"
height="1.4444444444444444in"}

### 字段锚定

设置当窗体大小发生变化时，各控件的位置如何调整。仅当界面布局是KD\_Layout，在字段的属性视图中找到"约束""anchor"，

![](media/media/image60.png){width="5.111805555555556in"
height="1.6944444444444444in"}

可以参考产品中已经实现KD\_Layout及字段缩放功能的单据上的字段锚定设置，例如销售订单、销售出库单等。

为模型增加功能和菜单按钮
------------------------

### 增加功能

为单据增加可以执行或者调用的业务功能。单据模板已经提供了大量功能，开发人员只需要增加其中没有的需要用到的功能。打开单据，如下图点击菜单：

![](media/media/image61.png){width="4.0in"
height="3.0104166666666665in"}

![](media/media/image62.png){width="5.7125in"
height="3.1527777777777777in"}

-   "功能绑定至工作流"：在EAS工作流设计时，需要把[]{#OLE_LINK8
    .anchor}工作流和单据绑定，或者在流程中调用单据功能自动执行，另外在后台事务平台中也需要调用单据的功能。此处勾选后，此功能才能在流程设计和后台事务定义中可见，其实质是在模型的Function元数据中增加了对此功能的描述。推荐业务处理类型的功能都勾选此项。

-   关于"功能位置"：定义此功能在列表界面和编辑界面中的存在。其实质是UI界面自动为功能添加相应的Action。

-   在ERP业务中，单据一般都会有审核确认和取消审核确认的需要，EAS基础单据模板没有提供这两个功能，开发人员应当为单据增加这两个操作："审核"、"反审核"。

-   增加功能的实质是：在Entity实体上增加相应的方法和事件。

### 增加菜单和工具栏

> 注意：此处说的菜单不是系统主菜单，是单据列表界面和编辑界面的菜单栏。

单据模板已经提供了其原有功能相应的菜单和工具栏，开发人员只需要为自己新增的功能添加菜单和工具栏按钮。打开单据，如下图点击菜单：

**注意：开发人员应当合理设置菜单和按钮的名称、位置**

![](media/media/image63.png){width="4.917361111111111in"
height="3.402083333333333in"}

![](media/media/image64.png){width="5.572916666666667in"
height="3.3541666666666665in"}

-   设置菜单项或按钮绑定的功能。

-   **规范修改菜单项和按钮的名称**，未来会作为Java类中相应控件的变量名。

-   增加菜单和按钮的实质，是在EditUI和ListUI上增加KDMenuItem和KDButtion，并和指定的Action做绑定。

### 功能的事务属性设置

在BIM中无法设置功能的（数据库）事务属性，需要切换到BOS
Studio透视图，找到并打开实体，切换到"方法"页签，如下图：

![](media/media/image65.png){width="6.417361111111111in"
height="2.942361111111111in"}

开发会涉及的事务属性有3种：

-   Supports：方法被调用时不会启动事务，但是支持上层调用方法启动事务；

-   Required：方法被调用时，如果上层调用方法未启动事务则本方法启动新事务；如果上层方法已经启动事务，则本方法不启动新事务；

-   RequiredNew：方法被调用时，必定启动一个新事务；

BIM新增功能的默认事务属性是"Supports"，若功能涉及数据库操作，**则必须修改为"Required"**

### 功能的参数设置

BIM新增功能默认只有一个参数，名称和类型为
model（ObjectValue），一般会使用模型的值对象作为实际传递的值。通常情况下，还需要增加一个ObjectPK类型的参数，以便于以后调用方法时按照单据对象的ID传递参数。

![](media/media/image66.png){width="6.420138888888889in"
height="1.6347222222222222in"}

如果在EditUI/ListUI中为功能添加了菜单或按钮，BOS会自动在相应的Action中添加代码，EditUI的代码一般如下：

> **public void** actionPerformed(ActionEvent e){
>
> com.kingdee.eas.devdemo.SaleBonusFactory.getRemoteInstance().audit(editData);
>
> }

ListUI的代码一般如下：

> **public void** actionPerformed(ActionEvent e){
>
> if (getSelectedKeyValue() == null) return;
>
> com.kingdee.eas.devdemo.SaleBonusInfo editData =
>
> (com.kingdee.eas.devdemo.SaleBonusInfo)getBizInterface().getValue(
>
> **new** ObjectUuidPK(BOSUuid.read(getSelectedKeyValue())));
>
> com.kingdee.eas.devdemo.SaleBonusFactory.getRemoteInstance().audit(editData);
>
> }

如果修改了功能的参数，BOS不会自动调整这些代码（实际上系统也无法猜到开发顾问添加参数的意图以及参数如何取值）。**当模型发布时系统就会提示编译错误**，生成的抽象类中会包含上述代码，其中方法参数不正确。解决方法是在BOS
Studio中找到EditUI/ListUI中相应的Action，删掉方法体，开发人员未来在实现类中自己做功能调用和参数赋值的工作。

在实体的"事件"页签中，一般也会有和方法对应的事件定义，其中的参数设置建议作同步修改，和方法相对应。

### 功能的异常设置

BIM新增功能默认不设置异常，但是一般功能方法实现中需要抛出业务类异常，开发人员应当为功能添加业务异常基类：com.kingdee.eas.common.[]{#OLE_LINK32
.anchor}EASBizException

![](media/media/image67.png){width="5.830555555555556in"
height="1.3222222222222222in"}

上述针对功能的3项设置完成后，都需要在BOS
Studio中执行【清除元数据缓存】操作，重新回到BIM中发布模型，或者在BOS
Studio中发布相应实体。

为模型添加权限项
----------------

### 在BIM中添加权限项

-   选择解决方案根节点，点击菜单【方案】【权限管理】；

-   在权限管理对话框中点按钮【新建】【根据功能创建权限项】（不要选【新建权限项】）；

-   在功能列表对话框中点【浏览...】，在选择业务单元；

![](media/media/image68.png){width="4.881944444444445in"
height="2.9166666666666665in"}

![](media/media/image69.png){width="4.771527777777778in"
height="2.661111111111111in"}

-   在功能列表中，勾选需要进行权限控制的功能，最后确定；一般基础资料和业务单据需要做权限控制的功能如右图示：

![](media/media/image70.png){width="4.881944444444445in"
height="3.2416666666666667in"}![](media/media/image71.png){width="1.5590277777777777in"
height="1.4930555555555556in"}

![](media/media/image72.png){width="1.5590277777777777in"
height="1.3590277777777777in"}

-   权限项默认保存在bim.permission。如果开发者已经建立了自己的权限文件用于分模块存放权限项的话，可以通过"选择权限文件..."功能，改变权限项的保存文件。

### 增加无功能权限项

某些情况下，我们需要增加权限项，仅在代码中调用权限接口检查控制权限，这些权限项没有功能对应，解决方法：

-   切换到BOS Studio中，找到权限文件并打开，切换到"权限项"页签；

![](media/media/image73.png){width="6.409722222222222in"
height="2.2180555555555554in"}

-   按照规范输入权限项名称；

-   组别和组名：权限项自动按照组别进行分类，在EAS客户端权限管理中看到的权限树，也是按照组别自动进行分类的。也就是说开发者不需要单独维护组别。

-   设置权限项的扩展属性，**特别是orgRelation和permItemType**，参考已有权限项设置。permItem含义解释：

> 10系统功能------权限项绑定的功能被认为是系统管理功能，普通用户不可用；

20业务功能------权限项绑定的功能被认为是业务功能，系统管理员不可用；

15业务管理功能------对应功能是普通用户和系统管理员都可被授权使用

-   如果权限需要启用数据权限，需要设置[]{#OLE_LINK33
    .anchor}enableDataPermission为True；同时需要为权限项绑定相应的Query。

![](media/media/image74.png){width="6.414583333333334in"
height="1.9631944444444445in"}

![](media/media/image75.png){width="5.778472222222222in"
height="2.551388888888889in"}

### 权限项在EAS客户端使用和授权

在BOS
Studio中发布权限元数据文件，部署解决方案到服务器以后，用Administrator账户登录，在用户权限管理模块中，执行"同步权限项"功能，系统把保存在元数据中的权限项同步到数据库中，然后就可以在用户授权时看到新增的权限项。![](media/media/image76.png){width="6.4118055555555555in"
height="2.9659722222222222in"}

![](media/media/image77.png){width="5.897916666666666in"
height="3.990972222222222in"}

### 权限项编码规范化

在BIM中添加权限项后，应当在BOS
Studio中对权限项重编码，使其规范化，原因是：BIM权限管理中自动添加的权限项，编码是不规范的，多人在不同的BOS环境中为自己的模块做权限项时，编码很容易相同，后期同步权限项时会报错，并且权限项不能正常生效。操作方法：

-   切换到BOS Studio中，找到权限文件并打开，切换到"权限项"页签；

![](media/media/image78.png){width="6.413888888888889in"
height="2.8125in"}

-   对每个权限项按照预订编码规则，重新编码；编码规则不宜太长，以能够看出模块和确保唯一性为原则。

![](media/media/image79.png){width="6.413194444444445in"
height="3.063888888888889in"}

### 权限文件规范化

在BIM中添加权限项后，应当在BOS
Studio中对权限文件进行规范调整，原因是：BIM权限管理中添加的权限项默认都保存在bim.permission文件中，多人在不同的BOS环境中为自己的模块添加权限时，最后难以进行合并。操作方法：

-   开发者可以先在BOS
    Studio中，在自己的模块下建立专用的权限文件；在BIM中创建权限项之前，通过"选择权限文件..."，切换权限项的保存目标文件。

-   ![](media/media/image80.png){width="3.1493055555555554in"
    height="3.2993055555555557in"}如果已经在bim.permission中建立了权限，可以在BOS
    Studio中找到文件，右键选【复制】，输入目标的包路径和名称。复制完成后，删除bim.permission。

![](media/media/image81.png){width="4.409722222222222in"
height="1.9840277777777777in"}

### 建立权限文件的时机建议

在开发建模初期，为了模型和代码测试方便，开发者可先不做权限项，等到模型和代码设计工作完成、功能性测试大部分完成后，再建立权限，以及进行权限项和权限文件的规范化。

为模型添加日志项
----------------

### 在BIM中添加日志项

-   选择解决方案根节点，点击菜单【方案】【日志管理】；

-   日志项的新增过程和权限项相似，不再描述；权限项保存在bim.log中，需要注意的是：**开发人员在日志管理中无法切换日志文件**。

### 日志项使用方法

在BOS
Studio中发布日志元数据文件，部署解决方案到服务器以后，用Administrator账户登录，在日志管理模块中，执行"同步日志项"功能，系统把保存在元数据中的日志项同步到数据库中。

### 日志项编码规范化

和权限项类似，日志项也需要做编码规范化，操作方法相同。

### 日志文件规范化

和权限文件类似，日志文件也需要规范化，操作方法相同。需要注意的是。

### 建立日志文件的时机建议

由于日志管理中无法切换日志文件，建议在建模工作结束以后，再建立各模型的日志，以及进行日志项和日志文件的规范化。如果后期需要添加日志项，开发者需要恢复bim.log文件（或者把现有日志文件复制成bim.log），日志添加完成以后，对新增部分和日志文件重新做规范化。

BOS Studio对模型的常见调整
--------------------------

-   调整Entity属性，一般Entity需要调整的有：事务属性、参数、异常；

-   调整Query属性的字段扩展属性，关联属性的显示名称。

<!-- -->

-   在ListUI及其绑定的Query元数据上增加关联对象和字段

-   定制套打Query：BIM建模及生成的代码中，套打使用的Query和ListUI绑定的Query是同一个，不排除套打对取数有特殊要求，导致需要另外做套打Query，并修改代码实现部分。

-   EditUI调整：对页签标题、控件状态/样式、分录表格的列标题/列宽/显示格式/列隐藏/列锁定等进行细节调整。

-   ListUI调整：对页签标题、表格的列标题/列宽/显示格式/列隐藏等进行细节调整。有时会加入树控件、界面分隔控件等。

### BOS Studio发布元数据

在BOS
Studio中修改保存元数据后，养成一个良好的习惯，**执行【清除元数据缓存】**，特别是发布前，否则实际发布可能是对内存中过时的元数据进行发布，导致出现各种不可预料的错误。发布完以后，需要手工**在Java透视图中刷新自动生成的代码**，才会自动编译成class。

模型挂接到系统主菜单
--------------------

-   选择解决方案根节点，点击菜单【方案】【主菜单管理】；

-   按照模块分类和路径建立菜单组，请参考产品已有模块菜单的分类方法；

-   输入菜单名称、描述；选择菜单对应的业务单元；状态：指菜单打开后进入录入界面还是列表界面，一般选择"[]{#OLE_LINK30
    .anchor}序时簿"。

注：有时会在BOS
Studio中增加UI界面并需要挂到系统主菜单，这种UI无法通过主菜单管理实现，只能在客户端用administrator登录后，在【系统】【客户化菜单编辑】中增加菜单。

![](media/media/image82.png){width="4.507638888888889in"
height="4.157638888888889in"}

![](media/media/image83.png){width="3.4722222222222223in"
height="2.65625in"}

模型发布和测试
--------------

建好模型以后，执行【发布业务单据】，BOS执行以下工作：检查和校验模型各元数据，自动编译（按照模型生成Java代码），同步数据库表及字段，自动生成默认套打模板。发布元数据时，BOS需要连接数据库。

![](media/media/image84.png){width="4.989583333333333in"
height="2.3125in"}![](media/media/image85.png){width="2.5208333333333335in"
height="2.8333333333333335in"}

发布前需要关注解决方案的帐套设置，如下图，BOS只对选中的数据库帐套进行数据库同步和生成套打模板：

![](media/media/image86.png){width="6.413194444444445in"
height="2.8541666666666665in"}

### 同步数据库

在EAS7.5及以前版本，在BIM中发布模型时会依据模型属性字段，自动同步数据库的表。EAS8.0及以后版本取消了自动同步功能，开发人员需要手工在模型的右键菜单中找到【更新数据库】并执行，然后才会在所连接的数据库账套中同步更新表结构。

### 发布错误分析处理

如果发布过程中遇到编译错误（compile
error），可查看ant日志，定位和分析错误；如果遇到校验错误，可以查看BIM日志，定位和分析错误。发布过程中还可能会遇到数据库连接错误，这是需要确定数据库服务是否启动，开发计算机能否正常连接，数据库账户和口令是否正确等。

自动生成代码
------------

EAS和BOS会为模型生成一整套运行时代码体系，一般来说，开发人员开发工作主要是以下几方面：

-   编辑和查看界面：控件的行为/样式/约束，控件监听和自动处理功能，新增数据的默认值，用户交互（弹窗），操作的客户端逻辑

-   列表界面：数据范围控制，[[]{#OLE_LINK6 .anchor}]{#OLE_LINK5
    .anchor}自定义过滤条件，操作的客户端逻辑；

-   控制器Bean：保存/提交时的状态检查、数据检查、补充计算，删除前的状态和业务检查，审核和反审核的逻辑及关联业务反写处理，数据库操作

测试运行
--------

开发工作完成后，可以启动BOS内置的服务器和客户端，直接测试运行。

![](media/media/image87.png){width="6.414583333333334in"
height="2.2243055555555555in"}

部分版本的EAS解决方案，启动服务器后大约需要2\~3分钟后，控制台出现服务器启动就绪的信息，然后再启动客户端登录，过早登录系统会提示错误，可能是由于服务器尚未就绪造成。

快测运行期修改代码，如果是：新增方法、删除方法、方法名、方法参数和异常变化，则需要重启相应的服务端或者客户端。如果仅修改方法体内的代码修改则不需要重启服务，保存后自动生效。修改元数据发布，视其生成的代码变化情况判断是否需要重启服务器，但是需要手工刷新其生成的Java类，使其编译产生class文件。

部署开发成果
------------

建模及调整、模型发布、代码、测试工作完成后，需要开发成果部署到服务器，使其对用户生效。部署解决方案时指定路径的方法和导入解决方案相同，请参考相关章节。

![](media/media/image88.png){width="3.5708333333333333in"
height="3.145138888888889in"}

![](media/media/image89.png){width="4.157638888888889in"
height="2.7715277777777776in"}

部署前应当停止EAS服务，防止由于EAS服务进程锁定需要更新的Jar文件导致部署失败。

如果部署过程中出现以下提示，说明服务器的元数据、代码环境和解决方案不一致，需要使用【方案】【更新解决方案】，按照提示完成方案更新。

![](media/media/image90.png){width="4.383333333333334in"
height="1.0819444444444444in"}

单据模型中通常需要增加的字段
----------------------------

### 【单据体】单据状态

一般有：新增、保存、提交、审核中、已审核、已关闭，特殊单据可能需要更多的状态。单据状态是枚举型字段，引用的枚举元数据需要事先定义好；查询编辑可见，不可修改。

**重要注意事项：**开发者为具有类似状态的所有单据设计公共的单据状态枚举，枚举值的类型为Integer；单据状态字段命名建议统一，一般命名为"baseStatus"。这样在未来的单据状态控制功能的实现上可以做到最大程度的简化和代码重用，做多单据联合查询报表的SQL取数也会最大程度简化和重用代码。

### 【分录】分录状态

视实际业务需要。一般有：保存、审核、关闭，特殊单据可能需要更多的状态。其设计时的注意事项和"单据状态"一样。

字段名：entryStatus，类型是分录状态枚举，查询编辑可见，不可修改。

### 【单据体】审核时间

用于记录单据审核时间，字段名：auditTime，日期型，查询编辑可见，不可修改。

### 【单据体】来源单据编号

从企业业务流程看，不同环节的单据间存在上下游关系，这种关系在下游单据上应当予以记录（EAS中也有专门的表记录这种关系）。

单据体的基类有一个属性sourceBillId，可用于记录上游单据的ID。这个字段界面上是不可见的，为了方便用户，需要增加一个来源单据编号，用于记录和显示上游单据的单据编号。

字段名：sourceBillNumber，类型是文本，用户查询编辑可见，不可修改。字段的值一般是在BOTP规则中配置，由BOTP平台完成赋值。

### 【分录】来源分录ID，来源分录序号

增加字段原因如上条所述。很多单据会设计分录以记录业务的明细数据，上下游分录也存在关联关系需要记录。

来源分录ID：sourceEntryID，文本型，用户查询编辑不可见，不可修改。

来源分录序号：sourceEntrySeq，整型，用户查询编辑可见，不可修改。

字段的值一般是在BOTP规则中配置，由BOTP平台完成赋值。

### 【分录】来源单据ID，来源单据编号

往往下游单据的分录集合中的分录是来源于上游的多张单据分录，因此分录中还应当记录来源分录的单据ID和编号。

来源单据ID：sourceBillId，文本型，用户查询编辑不可见，不可修改。

来源单据编号：sourceBillNumber，文本型，用户查询编辑可见，不可修改。

字段的值一般是在BOTP规则中配置，由BOTP平台完成赋值。

单据模型通常需要增加的功能
--------------------------

### 审核和反审核

一般单据都会有确认和取消的过程，需要添加相应的功能。建议所有单据的这两个功能都统一命名和设置参数、异常，这样在未来的单据状态控制功能的实现上可以做到最大程度的简化和代码重用。

审核功能名称：audit；反审核功能名称：unAudit；

功能设置：位置"全部"，绑定到工作流；参数/类型：model/ObjectValue，pk/ObjectPK；异常：com.kingdee.eas.common.EASBizException；事务类型：Required；事件对应的参数调整和方法一致。

BOS开发的过程总结
-----------------

> []{#OLE_LINK31 .anchor}一般的BIM建模和BOS
> Studio开发工作总结如下（建议打印出来作为开发参考）：

-   进行需求分析，合理设计开发方案和建模方案，尽可能利用产品和EAS平台功能，避免过于复杂的模型设计和代码开发，避免性能和安全陷阱；

-   在BOS
    Studio中建立模型所需的枚举和异常，设置枚举值类型，设置异常子项；在BOS
    Studio中建立公用的Façade元数据和方法，设置方法的事务属性/参数/异常；

-   在BOS Studio中新增的元数据，需要在BOS
    Studio中单独发布，发布前执行【清除元数据缓存操作】，并需要切换到"Java透视图"手工刷新Java代码；

-   建立公共的单据模板，认真调整模板模型的各项属性和设置，参考以下两项调整工作：

-   **在BIM中建模：**为模型增加字段和功能，**注意字段名称类型的统一规范**，设置模型布局，调整界面元素的排放和锚定，设置字段的属性、录入和查询顺序；设置功能所需的菜单和按钮；

    -   通常需要添加的字段：单据状态，审核时间，来源单据编号，分录.来源分录ID

    -   通常需要添加的功能：审核，反审核

-   **在BOS
    Studio中调整模型细节**：编辑和列表界面table的优化调整，UI新增
    Action自动代码清除，调整实体方法的事务属性/参数/异常，检查和修改Query中关联字段的显示属性；

-   生成子系统树：新增目录或单据时需要执行本操作

-   **把模型挂接到系统主菜单；**

-   为模型设置权限项和日志项（可放在开发后期对所有模型一起做），**对权限项和日志项的编码进行规范化，对权限文件和日志文件进行规范化；**

-   **在BIM发布模型，**如果在BOS
    Studio中增加了元数据，请参考第3项单独发布它；

-   进行代码设计开发，主要是：EditUI、ListUI、ControllerBean

-   **启动BOS内置服务器和客户端进行测试，**灵活运用调试工具分析错误和跟踪执行过程；

-   部署模型，可能需要更新解决方案，部署时尽量不要选择正式帐套；

-   后期实施开发工作：同步权限项和用户授权、同步日志项、工作流配置、单据转换规则配置、自动编码规则配置、套打模板调整和新增等等。

-   报表开发和报表授权、发布：建议通过EAS扩展报表平台快速开发报表。

-   **重要事项：**建模过程中，请开发人员养成备份模型的良好习惯，备份方法：把metadata目录打包放到专门的备份目录中。

BOS建模开发技巧
---------------

### 模型共享

如果开发人员有很多单据需要建模，建议先建立一个基础的业务单据作为模板使用，在该模板中建立共有的字段、功能、按钮和菜单、界面控件，设置好单据属性、界面布局、表格样式、字段排序、功能的事务属性/参数/异常、action自动代码等等。然后其他建立其他业务单据时，选择从模板业务单据复制后再修改调整，可以极大的降低建模开发工作量。

![](media/media/image91.png){width="4.688888888888889in"
height="3.4451388888888888in"}

![](media/media/image92.png){width="4.688888888888889in"
height="3.4451388888888888in"}

结合分公司项目开发经验，本文推荐一套模板业务单据，模型界面如下：

![](media/media/image93.png){width="6.409722222222222in"
height="3.2729166666666667in"}

模型元数据及关联公共元数据：内含3个单据模板，其中"无组织单据"即是上图所示。模型的功能及按钮、参数、异常设置，UI调整已按调整可用，可直接复制新模型使用。

![](media/media/image94.png){width="2.782638888888889in"
height="1.0326388888888889in"}

### 产品早期基础数据引用

业务建模时会引用EAS已有的基础资料，部分早期EAS开发的基础资料，例如：会计科目类型、HR里的薪酬方案和薪酬项目等等，只有entity、query、editUI、listUI等这些"零件"，没有组装形成BIM可用的业务单元（没有提供bizUnit元数据），这样在BIM透视图中找不到无法引用。这种情形下，需要开发人员自己为这些基础资料通过引用已有元数据建立对应的业务单元（bizUnit）。

首先建立和已有元数据同样的包路径，新建业务单据，业务单元名称和entity名称保持相同，选择"通过引入创建"，在单元配置对话框中选择对应的元数据，其中entity、query、listUI、editUI是必须要选配的。

![](media/media/image96.png){width="4.397916666666666in"
height="3.2319444444444443in"}![](media/media/image97.png){width="4.397916666666666in"
height="3.2319444444444443in"}

元数据校验
----------

在建模过程中，往往会由于一些意外原因造成模型不能正常打开或者发布报错，可以通过元数据校验发现一些有价值的线索。最常见的情形是：业务单据引用了另外一个业务单据、或基础资料、或元数据，被引用的单元、元数据被删除或者不存在。

右键点击业务单元选择"校验业务单元"，结果输出在"校验信息"视图里。

![](media/media/image98.png){width="2.995138888888889in"
height="2.6666666666666665in"}

![](media/media/image99.png){width="4.145833333333333in"
height="2.2083333333333335in"}

 BOS代码体系
============

抽象类和实现类
--------------

业务模型在BOS中发布后，系统会自动生成一些类代码，其中一部分是以Abstract开头的Java抽象类，另一部分是从抽象类继承的实现类。抽象类中提供了模型代码的实现，由BOS自动生成，每次发布模型都会重新生成；实现类提供给开发人员编写代码。通过这种方式，实现了模型代码和人工代码的位置分离和功能结合。

一般项目开发中，开发者只需要对EditUI、ListUI、ControllerBean三种Java类做代码设计。

注意：开发者应当在实现类里完成代码编写，对抽象类做任何改动，在下次发布模型后都会丢失。

![](media/media/image100.png){width="3.5833333333333335in"
height="3.5208333333333335in"}

![](media/media/image101.png){width="4.865972222222222in"
height="2.373611111111111in"}

下面是EditUI和ControllerBean的抽象类和实现类的示例：

客户端和服务端代码分工
----------------------

-   服务端：单据的业务功能实现，核心计算逻辑实现，状态检查控制、字段检查控制逻辑、上下游业务检查控制、工作流检查控制等，数据库操作，上下游关联业务处理；

-   客户端：**界面控件的设置**，**数据过滤**和展现，信息输出和初步加工处理，为了改善用户体验的检查校验，**控件的自动计算和范围控制**，权限控制，**新增默认值**。

值对象和值集合
--------------

### 值对象（Info）

类似POJO对象，Java运行时封装业务模型对象各属性字段的值，并提供整套Get/Set方法。值对象的基类[]{#OLE_LINK34
.anchor}PropertyContainer定义了一个类变量：protected Map
values，以键值对的形式保存Info的各属性值，key取属性名称。

### 值对象的两类get/set方法及应用

-   属性强相关方法，例如：getNumber()/setNumber(value)、getOrgUnit()/setOrgUnit(value)等，这些是BOS根据模型中定义的属性自动生成；

-   属性无关方法，例如：get(key)/ put(key, value)、getString(key)/
    setString(key, value)、getDate(key)/ setDate(key, value)、getInt
    (key)/ setInt(key,
    value)......等等；这些方法是PropertyContainer提供的，和模型的属性定义无关，但是可以通过key获取相应的值。

在通常的代码中，我们获取单据的各个字段值，用属性强相关方法更方便，并且方法有类型检查，出现错误在开发阶段就可以及时发现。

**属性无关方法通常的应用案例场景一**：在动态单据平台（DEP）为实体增加字段，BOS代码中是不会为实体生成相应的get/set方法，要获取或设置这些字段的值，就必须使用get/set/put方法。

**属性无关方法通常的应用案例场景二**：建立了若干单据，这些单据有一些共同的检查控制逻辑，可以设计一个公用方法统一处理，只能为公共方法传递这些单据的基类，这样要获取或设置单据的共同字段，就只能使用get/set/put方法，示例代码：

> **public static void** checkJobAttachInfo(Context ctx, IObjectValue
> model)
>
> throws BOSException, EASBizException
>
> {
>
> if(**model.get(\"seq\")**==null)
>
> **throw new** HeFeiBizException(HeFeiBizException.NULL\_FIELD);
>
> if(**model.get(\"sourceType\")**==null)
>
> **throw new** HeFeiBizException(HeFeiBizException.NULL\_FIELD);
>
> }

### 关于getLogInfo方法

日志系统记录用户操作时，会记录当前操作对象（一般是某个单据值对象）的概要信息，此方法告诉日志系统关于当前单据记录的信息。对于基础资料，其基类把number字段作为返回值；但是对于单据，其基类ObjectBaseInfo把lastUpdateUser.name属性（最后修改人姓名）作为返回值，不能满足要求，开发者需要视情形覆盖此方法，通常把number单据编号作为返回值。示例代码：

**public String** getLogInfo(){

**String** retValue = \"\";

if(getNumber() != null)

retValue = getNumber();

else

retValue = super.getLogInfo();

**return** retValue;

}

可直接反编译修改CoreBillBase的getLogInfo方法，这样所有单据不再需要单独修改。

### 值集合（Collection）

一系列同类型值对象的集合，提供Get/Set/Add/Remove/Contains等方法对集合对象进行操作。值集合的基类AbstractBaseObjectCollection定义类变量protected
List list用于保存值对象。

值集合方法也分为单据相关方法、单据无关方法，后者应用场景同值对象的属性无关方法。

### 值对象和值集合示例

接口和工厂
----------

接口用于描述功能，各功能的调用参数、返回异常等，一般开发者可不关注；

使用工厂的目的是获取各业务单据的远程或者本地Controller实例（实现了接口功能），并进一步调用Controller的各个业务方法，这些方法调用最终会传递到ControllerBean。

服务端通过工厂获取本地Controller实例：

> IProject iproj = ProjectFactory.getLocalInstance(ctx);

客户端通过工厂获取远程Controller实例：

> IProject iproj = ProjectFactory.getRemoteInstance();

-   工厂应用代码示例

<!-- -->

-   保存值对象：ProjectFactory.getLocalInstance(ctx).save(project)

-   获取值对象：ProjectInfo project =
    ProjectFactory.getRemoteInstance().getValue(pk)

-   删除记录：ProjectFactory.getLocalInstance(ctx).delete(pk)

-   提交值集合：ProjectFactory.getRemoteInstance().submit(ProjectCollection)

-   检查单据记录是否存在：ProjectFactory.getRemoteInstance().exists(pk)

开发人员可以自行学习单据Interface有哪些方法，这些方法都可以通过工厂调用。

EditUI，ListUI，ControllerBean
------------------------------

-   编辑界面EditUI和列表界面ListUI：开发人员的UI端代码大部分在这两个类里。

-   ControllerBean[]{#OLE_LINK9
    .anchor}：开发人员的服务端代码主要在这个类中，负责各种业务逻辑的实现。

 BOS核心代码开发
================

BOS开发按照是否涉及标准产品分为两大类：独立开发、产品改造，这两大部分开发方法有很大不同：

-   独立开发不需要考虑标准产品的补丁和升级，可以完全通过BOS自由发挥

-   产品改造则需要考虑补丁和升级的问题，首先需要小心翼翼的分析了解标准产品及其功能的设计实现方法，然后结合开发目标确定合理的开发方案，既能满足客户需求，又要尽可能避免产品二开冲突

开发必备基础
------------

### ID和BosObjectType

ID是单据和基础资料数据的唯一标识，EAS系统里的所有数据都具有ID，都是通过ID进行识别。ID在把数据保存到数据库的时候生成，开发者也可以调用生成id的方法提取为单据生成ID。

BosObjectType是单据类型的唯一标识，是在BIM或BOS
Studio建立模型时，BOS自动计算固化下来。一般的单据ID里会包含BosObjectType信息，可以根据单据ID获取相应的BosObjectType。

#### ID对象

系统提供了BOSUuid、IObjectPK用于描述单据的ID，IObjectPK是一个Interface，对应的常用实现类是ObjectUuidPK。

BOSUuid、ObjectUuidPK及String间的相互转化方法如下：

  ------------------------ ------------------------ -----------------------------
  **源类型**               **目标类型**             **方 法**
  String                   ObjectUuidPK/IObjectPK   new ObjectUuidPK(String)
  BOSUuid                  ObjectUuidPK/IObjectPK   new ObjectUuidPK(BOSUuid)
  String                   BOSUuid                  BOSUuid.read(String)
  ObjectUuidPK/IObjectPK   BOSUuid                  ObjectUuidPK .getKeyValue()
  BOSUuid                  String                   BOSUuid.toString()
  ObjectUuidPK/IObjectPK   String                   ObjectUuidPK.toString()
  ------------------------ ------------------------ -----------------------------

#### BosObjectType

BOSObjectType是单据类型标识，8位字符串，每个entity和facade都有唯一的BOSObjectType，BOS根据元数据的包路径和名称生成，发布时会分别在entity\_pkmapping.properties和facade\_pkmapping.properties这两个文件中注册，部署时也需要同步部署到EAS服务器，保存BOSObjectType和元数据包路径和名称的对应关系，如果丢失这种关系，系统运行时会提示找不到XXXXXXXX对应的元数据。。

系统提供BOSObjectType对象描述单据类型标识，代码获取BOSObjectType，以及从BOSObjectTypeID创建单据ID的方法如下：

  --------------- --------------- ----------------------------------
  **源类型**      **目标类型**    **方 法**
  ObjectUuidPK    BOSObjectType   ObjectUuidPK .getObjectType()
  BOSUuid         BOSObjectType   BOSUuid.getType()
  BOSObjectType   ObjectUuidPK    BOSUuid.create(BOSObjectType)
  BOSObjectType   BOSUuid         new ObjectUuidPK (BOSObjectType)
  --------------- --------------- ----------------------------------

查找BOSObjectType的方法：在BOS
Studio中找到并打开相应的entity或facade，切换到"源代码"，找到bosType标签，里面的值就是BOSObjectType。

![](media/media/image111.png){width="6.243055555555555in"
height="2.0972222222222223in"}

#### Java代码生成ID

-   id字符串转换为IObjectPK/ObjectUuidPK：ObjectUuid pk = new
    ObjectUuidPK(String);

-   []{#OLE_LINK35
    .anchor}已有BOSObjectType，创建BOSUuid：info.setId(BOSUuid.create(BOSObjectType));

-   已有BOSUuid转为IObjectPK：ObjectUuid pk = new
    ObjectUuidPK(BOSUuid.toString());

-   已有IObjectPK转为BOSUuid：BOSUuid.read(IObjectPK.toString)

#### 数据库生成ID

开发中经常遇到从数据库直接Insert数据，这时候需要在数据库层创建EAS单据的ID，EAS在账套数据库中会自动创建一个专用于创建单据的函数：newbosid(BOSObjectType)
，注意在SQL
Server的查询分析器中需要限定owner，需要写成：dbo.newbosid(BOSObjectType)

使用示例：insert into table (FID,FNumber,FName\_l2,......) values
(newbosid(\'D8002BA9\'), \'001\', \'大型项目\', ......)

### 上下文

上下文是代码执行时关于环境的信息，在EAS中上下文本质是一个Map。

#### 获取客户端系统上下文

**系统上下文在客户端登录后，任何地方都可以获取**，和单据生命期无关。

![](media/media/image112.png){width="3.3743055555555554in"
height="1.8527777777777779in"}SysContext.getSysContext()，可以获取当前组织、用户、登录账套、语言等环境信息

![](media/media/image113.png){width="3.3743055555555554in"
height="1.8576388888888888in"}

#### 获取客户端UI上下文

单据UI基类CoreUIObject提供方法[]{#OLE_LINK83
.anchor}getUIContext()，用于获取单据的上下文。单据上下文在UI构造方法调用时尚未传递进去，此方法在onLoad()及生命期之后，才能获取上下文数据。

从单据上下文可以获取：当前窗体的父窗体，父窗体向当前窗体传递的各种参数、数据，菜单执行时向窗体传递的参数，工作流调用窗体时当前流程实例和活动信息，单据转换平台调用窗体时的相关BOTP信息等等。

可以在BOS快测运行时，为某个单据的onLoad()或其他方法上设置断点，捕获断点后，在"显示"视图中输入"getUIContext()"，选中按"ctrl+shift+i"，观察getUIContext()返回的上下文内容。

![](media/media/image114.png){width="2.7402777777777776in"
height="2.6590277777777778in"}![](media/media/image115.png){width="6.5152777777777775in"
height="4.063888888888889in"}

#### 获取服务端方法上下文

服务端方法通常有一个类型com.kingdee.bos.Context的变量ctx，代表当前方法执行时的上下文，类似客户端系统上下文，可以获取当前组织、用户、登录账套、语言、客户端IP等会话信息

可以使用工具类com.kingdee.eas.util.app.ContextUtil快速从ctx中获取信息。

某些特殊场合，服务端执行的方法未通过参数提供上下文，开发者可以通过com.kingdee.bos.ContextUtils.getContextFromSession()
获取当前会话对应的上下文

### 客户端和服务端代码分工

有些开发逻辑，既可以放在服务端也可以放在客户端执行，例如检查字段必填、金额自动计算（＝数量×价格）等等。

作者建议：**核心检查和业务处理逻辑，必须放在服务端执行**。这是因为：

如果代码放在UI界面，则意味着单据对象必须是在通过UI传到服务端时才能被执行。而有些场景下单据对象并非通过UI产生，例如：某些BOTP规则下推保存的单据、在Java代码中构造或加工处理的单据对象、通过接口从第三方系统获取的单据对象等等。

客户端保留的代码主要是：必须留着前端的操作处理，控件定制、需要即时计算并显示的计算逻辑、用户交互、为了改善用户体验的检查处理等

### 消息提示

EAS提供了消息提示的工具类：[]{#OLE_LINK36
.anchor}com.kingdee.eas.util.client.MsgBox，可以提示简单的信息、警告、错误，也提供具有2个或3个按钮的"确认取消

忽略"的对话框。

示例：

**if**(MsgBox.*YES*!=MsgBox.*showConfirm2*(\"对所选单据进行审核，是否继续\"))

> **return**;

 controllerbean.java
--------------------

### 两种方法

举例，用户为单据增加了审核方法：audit(Contex, IObjectValue,
IObjectPK)，那么在ControllerBean的抽象类里会自动生成两个相关的方法

-   audit(Context, ProjectPlanInfo)

-   \_audit(Context, IObjectValue)

观察两个方法体：

**public** **void** audit(Context ctx, ProjectPlanInfo model) **throws**
BOSException, EASBizException

{

**try** {

> 服务上下文

ServiceContext svcCtx = createServiceContext([**new**
~~MetaDataPK~~(\"1a9da5be-be45-48ab-a125-718cd48f638e\")]{.underline},
**new** Object\[\]{ctx, model});

invokeServiceBefore(svcCtx);

**if**(!svcCtx.invokeBreak()) {

\_audit(ctx, model);

}

invokeServiceAfter(svcCtx);

} **catch** (BOSException ex) {

**this**.setRollbackOnly();

**throw** ex;

} **catch** (EASBizException ex0) {

**this**.setRollbackOnly();

**throw** ex0;

} **finally** {

**super**.cleanUpServiceState();

}

}

***protected** **void** \_audit(Context ctx, IObjectValue model,
IObjectPK pk) **throws** BOSException, EASBizException*

*{*

***return**;*

*}*

在audit方法里系统要做调用前后的准备、前/后置处理、异常和事物处理，\_audit方法是一个空方法。如果直接继承扩展audit，那么其中的前后置业务处理将无法得到正确执行，因此开发人员实现audit功能，应当在实现类中改写\_audit方法，而不能直接改写audit方法。

**开发者改写ControllerBean的所有方法，都必须改写以下划线开头的方法。**

### 要开发的框架方法

-   \_save(Context ctx, IObjectValue
    model)，对应单据的保存或者基础资料的暂存方法

-   \_submit(Context ctx, IObjectValue
    model)，对应单据的提交或者基础资料的保存方法

-   \_submit(Context ctx, IObjectPK pk, IObjectValue
    model)，工作流审批环节的提交操作，会调用对应单据的此方法

-   \_delete(Context ctx, IObjectPK pk)，对应单据和基础资料的删除操作

-   \_cancel(Context ctx, IObjectPK pk, IObjectValue model)
    ，对应基础资料的禁用操作

-   \_cancel Cancel (Context ctx, IObjectPK pk, IObjectValue model)
    ，对应基础资料的启用操作

一般我们会为单据增加审核audit和反审核unAudit方法，参数为ObjectValue和ObjectPK，异常为EASBizException，这样我们还需要开发：

-   \_audit(Context ctx, IObjectValue model)

-   \_unAudit(Context ctx, IObjectValue model)

### 常见开发内容

-   \_save和\_submit在保存前检查单据状态，检查单据字段，补充计算

-   \_delete在删除前检查单据状态，检查单据是否在工作流中，检查是否已生成下游单据

-   \_audit在执行前检查单据状态（不允许重复审核），检查单据字段；修改单据状态，记录操作人和操作时间；执行来源单据或其他关联数据的反写，执行上游业务检查控制逻辑

-   \_unAudit在执行前检查单据状态（不允许重复反审核），检查单据无下游单据；修改单据状态，清除操作人和操作时间；执行来源单据或其他关联数据的反写，执行上游业务检查控制逻辑

注意：检查单据状态应当**以数据库中实时读取的单据状态为准**，而不是以通过参数传递过来的IobjectValue对象中保存的状态字段值为准

### 数据更新

把对象数据持久化到数据库，开发人员必备技能。对于\_save、\_submit、\_delete、\_update方法，框架已经为我们写好了底层实现，开发人员只需要调用即可。

在一些应用中，例如：审核反审核时修改单据的"状态、审核人/时间"，下游单据反写上游单据的执行数据等场合，开发者需要掌握了解多种更新方法及其利弊。

修改数据库中的单据数据，通常有以下方法：

#### 值对象更新

方法说明：取得单据的Info对象，修改Info对象属性值，然后用\_update方法写到数据库。

-   优点：容易理解和使用

-   缺点：无论开发者希望更新多少字段，哪怕只有一个字段，值对象更新都会把内存里保存的对象属性值全部写回数据库。对于只做少量字段的更新操作，例如审核时修改状态、反写时更新已执行数据，当所更新的单据存在较大业务并发时，容易造成内存的过时数据覆盖数据库中的最新数据，**产生并发数据丢失**

因此，对于少量数据更新，**本文要求避免使用这种方式**。示例：

[]{#OLE_LINK37 .anchor} ProjectPlanInfo billInfo =
(ProjectPlanInfo)model;

billInfo.setBaseStatus(BillBaseStatusEnum.*AUDITED*);

billInfo.setAuditTime(**new** Date());

billInfo.setAuditor(ContextUtil.*getCurrentUserInfo*(ctx));

\_update(ctx, **new** ObjectUuidPK(billInfo.getId()), model);

#### 值对象属性更新

方法说明：取得单据的Info对象，修改Info对象属性值，然后用\_updatePartial方法写到数据库。

\_updatePartial方法要求开发者传递一个属性集合，用于说明需要更新的字段。

-   优点：容易理解和使用，并且能极大减少并发冲突产生的数据丢失。

> 该方式是本文认为可以使用的数据更新方式。示例：

ProjectPlanInfo billInfo = (ProjectPlanInfo)model;

billInfo.setBaseStatus(BillBaseStatusEnum.AUDITED);

billInfo.setAuditTime(new Date());

billInfo.setAuditor(ContextUtil.getCurrentUserInfo(ctx));

SelectorItemCollection selector = new SelectorItemCollection();

selector.add(\"baseStatus\");

selector.add(\"auditTime\");

selector.add(\"auditor\");

\_updatePartial(ctx, billInfo, selector);

#### SQL更新

> 方法说明：开发者写带参SQL，用SQL执行工具执行数据更新

-   优点：能够完全避免并发冲突产生的数据丢失

-   缺点：无法使用Java提供的代码检查功能检查可能存在数据操作错误

> 该方式是本文强烈推荐使用的数据更新方式。示例：

String upSQL = \"update T\_PRJ\_ProjectPlan set FBaseStatus=?,
FAuditTime=?, FAuditorID=? where FID=?\";

com.kingdee.eas.util.app.DbUtil.execute(ctx, upSQL, new Object\[\]{

BillBaseStatusEnum.AUDITED\_VALUE, new java.sql.Date(new
Date().getTime()),

ContextUtil.getCurrentUserInfo(ctx).getId().toString(),

billInfo.getId().toString()});

### 代码示例：\_save和\_submit 

**protected** IObjectPK \_save(Context ctx, IObjectValue model)

**throws** BOSException, EASBizException

{

ProjectPlanInfo info = (ProjectPlanInfo)model;

// 单据的字段检查

checkFields(ctx, info);

// 单据的状态检查

checkBillUnAudit(ctx, info);

info.setBaseStatus(BillBaseStatusEnum.*ADD*);

**return** **super**.\_save(ctx, model);

}

**protected** **void** checkFields(Context ctx, ProjectPlanInfo info)

**throws** BOSException, EASBizException

{

**if**(info.getProject()==**null**)

**throw** **new** EASBizException(EASBizException.*CHECKBLANK*, **new**
Object\[\]{\"项目\"});

**if**(info.getAdminOrgUnit()==**null**)

info.setAdminOrgUnit(ContextUtil.*getCurrentAdminUnit*(ctx));

**if**(info.getBizDate()==**null**)

info.setBizDate(**new** Date());

ProjectPlanEntryInfo entryInfo = **null**;

**for**(**int** i=0; i\<info.getEntrys().size(); i++)

{

entryInfo = info.getEntrys().get(i);

**if**(entryInfo.getJob()==**null**)

**throw** **new** EASBizException(EASBizException.*CHECKBLANK*,

**new** Object\[\]{\"第\"+(i+1)+\"行分录的任务\"});

**if**(entryInfo.getManday()==**null**)

entryInfo.setManday(BigDecimal.*ZERO*);

}

}

// 检查单据未审核

**protected** **void** checkBillUnAudit(Context ctx, ProjectPlanInfo
info)

**throws** BOSException, EASBizException

{

**if**(info.getId()!=**null**)

{

> //获取属性集合

SelectorItemCollection selector = **new** SelectorItemCollection();

> //增加基础

selector.add(\"baseStatus\");

> //获得单据id

ObjectUuidPK pk = **new** ObjectUuidPK(info.getId());

> //搜索表

**if**(\_exists(ctx, pk))

{

> //从数据库获取实体属性

ProjectPlanInfo dbInfo = (ProjectPlanInfo) \_getValue(ctx, pk,
selector);

> //查看是否审核

**if**(dbInfo.getBaseStatus()!=**null** &&
dbInfo.getBaseStatus().getValue()\>=BillBaseStatusEnum.*AUDITED\_VALUE*)

**throw** **new** SCMBillException(SCMBillException.*CHECKAUDITEDOK*);

}

**else**

{

**if**(info.getBaseStatus()!=**null** &&
info.getBaseStatus().getValue()\>=BillBaseStatusEnum.*AUDITED\_VALUE*)

**throw** **new** SCMBillException(SCMBillException.*CHECKAUDITEDOK*);

}

}

}

### 代码示例：\_delete

**protected** **void** \_delete(Context ctx, IObjectPK pk) **throws**
BOSException, EASBizException

{

// 已审核单据不允许删除

SelectorItemCollection selector = **new** SelectorItemCollection();

selector.add(\"baseStatus\");

ProjectPlanInfo dbInfo = (ProjectPlanInfo) \_getValue(ctx, pk,
selector);

//如果已经审核会抛出异常

checkBillUnAudit(ctx, dbInfo);

// 是否有下游单据的检查

[ArrayList]{.underline} destObjId =
BotRelationUtil.*getDestObjectIdByDestType*(ctx, pk.toString(),
**null**);

**if** (destObjId != **null** && destObjId.size() \> 0)

**throw** **new**
SCMBillException(SCMBillException.*HASDESTBILL\_CANNOTUNAUDIT*,

**new** Object\[\]{\"此单据已经关联生成其他单据\"});

**super**.\_delete(ctx, pk);

}

### 代码示例：\_audit

**protected** **void** \_audit(Context ctx, []{#OLE_LINK38
.anchor}IObjectValue model)**throws** BOSException, EASBizException

{

//对象

ProjectReportInfo billInfo = (ProjectReportInfo)model;

// billInfo = (ProjectReportInfo) \_getValue([ctx]{.underline}, new
ObjectUuidPK(billInfo.getId()));

// 字段和状态检查

checkFields(ctx, billInfo);

checkBillUnAudit(ctx, billInfo);

// 设置单据状态、审核人、审核时间

billInfo.setBaseStatus(BillBaseStatusEnum.*AUDITED*);

billInfo.setAuditTime(**new** Date());

billInfo.setAuditor(ContextUtil.*getCurrentUserInfo*(ctx));

// 单据更新方法1：整单更新（不推荐）

// \_update([ctx]{.underline}, new ObjectUuidPK(billInfo.getId()),
model);

// 单据更新方法2：对象属性更新（推荐）

// SelectorItemCollection selector2 = new SelectorItemCollection();

// selector2.add(\"baseStatus\");

// selector2.add(\"auditTime\");

// selector2.add(\"auditor\");

// updatePartial([ctx]{.underline}, billInfo, selector2);

// 单据更新方法3：单据状态的SQL更新（推荐）

String upSQL = \"update T\_PRJ\_ProjectReport set FBaseStatus=?,
FAuditTime=?, FAuditorID=? where FID=?\";

com.kingdee.eas.util.app.DbUtil.*execute*(ctx, upSQL,

**new** Object\[\]{BillBaseStatusEnum.*AUDITED\_VALUE*,

**new** java.sql.Date(**new** Date().getTime()),

ContextUtil.*getCurrentUserInfo*(ctx).getId().toString(),

billInfo.getId().toString()});

// 按分录反写来源项目计划分录及业务控制检查

ProjectReportEntryInfo entryInfo = **null**;

获取

IProjectPlanEntry [iPlanEntry]{.underline} =
ProjectPlanEntryFactory.*getLocalInstance*(ctx);

String sql = \"update T\_PRJ\_ProjectPlanEntry set FIsReported=1,
FReportedManday=IsNull(FReportedManday,0)+? where FID=?\";

**for**(**int** i=0; i\<billInfo.getEntrys().size(); i++)

{

entryInfo = billInfo.getEntrys().get(i);

**if**(entryInfo.getSrcEntryID()==**null**)

**continue**;

// throw new EASBizException(EASBizException.CHECKBLANK, new
Object\[\]{\"第\"+(i+1)+\"行分录不是BOTP生成的\"});

// 反写更新方法1：用值对象反写 （不推荐）

// ProjectPlanEntryInfo srcEntryInfo =
iPlanEntry.getProjectPlanEntryInfo(

// new ObjectUuidPK(entryInfo.getSrcEntryID()));

// srcEntryInfo.setIsReported(true);

// if(srcEntryInfo.getReportedManday()==null)

// srcEntryInfo.setReportedManday(BigDecimal.ZERO);

// srcEntryInfo.setReportedManday(srcEntryInfo.getReportedManday().add(

// entryInfo.getManday()));

// // 反写更新方法2：对象属性更新（推荐）

// SelectorItemCollection selector = new SelectorItemCollection();

// selector.add(\"isReported\");

// selector.add(\"reportedManday\");

// iPlanEntry.updatePartial(srcEntryInfo, selector);

// 反写更新方法3：用SQL反写（推荐）

com.kingdee.eas.util.app.DbUtil.*execute*(ctx, sql,

**new** Object\[\]{entryInfo.getManday(), entryInfo.getSrcEntryID()});

// 上游业务检查：累计汇报人天数不能超过计划人天数

String selSql = \"select FReportedManday, FManday from
T\_PRJ\_ProjectPlanEntry where FID=? and FReportedManday\>FManday\";

IRowSet rowSet = com.kingdee.eas.util.app.DbUtil.*executeQuery*(ctx,

selSql, **new** Object\[\]{entryInfo.getSrcEntryID()});

**try**

{

**if**(rowSet.next())

{

**throw** **new** EASBizException(EASBizException.*CHECKBLANK*,

**new**
Object\[\]{\"来源计划的累计汇报人天（\"+rowSet.getString(1)+\"）超出计划人天（\"+rowSet.getString(2)+\"）\"});

}

}

**catch** (SQLException e)

{

// 必须注意！！！异常必须抛出！！！

e.printStackTrace();

**throw** **new** BOSException(e);

}

}

}

### 代码示例：\_unAudit

**protected** **void** \_unAudit(Context ctx, IObjectValue model)
**throws** BOSException, EASBizException

{

//获取目标对象

ProjectReportInfo billInfo = (ProjectReportInfo)model;

// 状态检查

checkBillAudit(ctx, billInfo);

// 单据状态的SQL更新

String upSQL = \"update T\_PRJ\_ProjectReport set FBaseStatus=?,
FAuditTime=null, FAuditorID=null where FID=?\";

com.kingdee.eas.util.app.DbUtil.*execute*(ctx, upSQL, **new**
Object\[\]{

BillBaseStatusEnum.[]{#OLE_LINK78 .anchor}*TEMPORARILYSAVED\_VALUE*,

billInfo.getId().toString()});

// 按分录反写来源项目计划分录及业务控制检查

ProjectReportEntryInfo entryInfo = **null**;

String sql = \"update T\_PRJ\_ProjectPlanEntry set
FReportedManday=IsNull(FReportedManday,0)-? where FID=?\";

String sql2 = \"update T\_PRJ\_ProjectPlanEntry set FIsReported=0 where
FID=? and FReportedManday=0\";

**for**(**int** i=0; i\<billInfo.getEntrys().size(); i++)

{

entryInfo = billInfo.getEntrys().get(i);

**if**(entryInfo.getSrcEntryID()==**null**)

**continue**;

// 反写更新方法3：用SQL反写（推荐）

com.kingdee.eas.util.app.DbUtil.*execute*(ctx, sql, **new** Object\[\]{

entryInfo.getManday(), entryInfo.getSrcEntryID()});

com.kingdee.eas.util.app.DbUtil.*execute*(ctx, sql2, **new** Object\[\]{

entryInfo.getSrcEntryID()});

// 上游业务检查：累计汇报人天不能不能小于0

String selSql = \"select FReportedManday from T\_PRO\_ProjPlanEntry
where FID=? and FReportedManday\<0\";

IRowSet rowSet = com.kingdee.eas.util.app.DbUtil.*executeQuery*(ctx,

selSql, **new** Object\[\]{entryInfo.getSrcEntryID()});

**try**

{

**if**(rowSet.next())

{

**throw** **new** EASBizException(EASBizException.*CHECKBLANK*,

**new** Object\[\]{\"来源计划的累计汇报人天小于0\"});

}

}

**catch** (SQLException e)

{

// 必须注意！！！异常必须抛出！！！

e.printStackTrace();

**throw** **new** BOSException(e);

}

}

}

 EditUI.java
------------

实现编辑和查看界面的Java类，由EditUI元数据发布生成，在EAS客户端运行。

### 层次结构

整个EditUI实质是一个Panel，如下面的层次结构图，EAS构造和初始化完EditUI后，会把它加入Window或者Frame，使其在窗口中显示。

![](media/media/image116.png){width="5.4527777777777775in"
height="2.973611111111111in"}

EditUI窗体的可见元素，除了设计时看到的Panel及其上排放的控件，还有在CoreUIObject中定义的（ListUI也是如此）：

-   工具栏：protected KDToolBar toolBar

-   菜单栏：protected KDMenuBar menuBar;

-   状态栏：protected KDStatusBar statusBar;

### 关于editData

EditUI界面控件的数据绑定到一个Info对象，变量名是editData。UI加载数据时，从editData获取各字段值赋给界面控件，保存数据时从UI控件取值赋给editData相应字段。EditUI各控件值和editData属性的绑定规则可以在BOS
Studio的数据绑定视图中调整，BIM建模时会自动设置绑定规则。

在BOS
Studio中打开单据编辑界面，在数据绑定视图中可以找到界面所绑定的entity，以及控件和Entity属性的绑定规则。

![](media/media/image117.png){width="6.417361111111111in"
height="3.7527777777777778in"}

![](media/media/image118.png){width="3.6354166666666665in"
height="2.0340277777777778in"}

在EditUI生成的抽象类里可以看到，BOS为绑定对象生成了局部变量editData

![](media/media/image119.png){width="6.4118055555555555in"
height="1.7958333333333334in"}

### 重要方法说明

+-----------------+-----------------+-----------------+-----------------+
| **方法名**      | **执行次数**    | **调用时间点**  | **主要代码方法** |
+-----------------+-----------------+-----------------+-----------------+
| \<构造方法\>    | 1               | new对象         | 上下文和值对象无关的控件初始化 |
+-----------------+-----------------+-----------------+-----------------+
| onLoad          | 1               | 类加载后        | 与上下文相关的控件初始化 |
+-----------------+-----------------+-----------------+-----------------+
| loadFields      | 多次            | onLoad、保存后、 | 与值对象相关的控件初始化 |
|                 |                 |                 |                 |
|                 |                 |                 |                 |
|                 |                 | 提交后、上下查操作 |              |
+-----------------+-----------------+-----------------+-----------------+
| storeFields     |                 | 保存前、提交前、 | editData赋值调整 |
|                 |                 |                 |                 |
|                 |                 |                 |                 |
|                 |                 | 窗体关闭        |                 |
+-----------------+-----------------+-----------------+-----------------+
| getOprtState    |                 | 获取单据状态    |                 |
+-----------------+-----------------+-----------------+-----------------+
| setOprtState    |                 | 设置单据状态    | 根据指定的状态设置单据控件状态 |
+-----------------+-----------------+-----------------+-----------------+
| createNewData   |                 | 新增记录        | 为新值对象设默认值 |
+-----------------+-----------------+-----------------+-----------------+
| actionPerformed |                 | 点击按钮或菜单项 | 功能调用，检查控制 |
+-----------------+-----------------+-----------------+-----------------+
| getSelectors    |                 | 从服务端获取editData | 添加额外的SelectorIt |
|                 |                 |                 | emInfo          |
+-----------------+-----------------+-----------------+-----------------+
| applyDefaultVal |                 | 设置控件默认值  | 修改默认值设置  |
| ue              |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| getBizInterface |                 | 获取对应的接口实例 |              |
+-----------------+-----------------+-----------------+-----------------+

### 获取界面控件

BIM建模过程中添加的属性，默认都会在UI上生成对应的控件，例如文本、日期、F7、下拉框等，需要注意这样一个字段的控件![](media/media/image120.png){width="3.2805555555555554in"
height="0.3333333333333333in"}实际上有两部分，在BOS
Studio中打开UI观察该控件，可以看出由"标签容器KDLabelContainer＋编辑控件"构成。

![](media/media/image121.png){width="6.4118055555555555in"
height="2.384027777777778in"}

在发布生成的抽象类中，所有控件都以类成员变量形式存在，开发人员可以直接通过控件名命名的变量操作该控件

![](media/media/image122.png){width="6.409027777777778in"
height="2.91875in"}

#### 获取表格编辑控件

表格本身具有类变量，名称例如：kdtEntrys，但是BIM中在分录中增加的各种字段，例如物料、人员、枚举状态等，其所需的编辑控件却并没有作为类变量存在，如果需要定制这些控件，则需要开发人员自己获取。

示例：获取表格的客户F7控件，通常是开发人员在实现类里自己定义一个类成员变量用来保存表格编辑控件

[]{#OLE_LINK39 .anchor}**protected** KDBizPromptBox prmtCustomer;

**public** FeeAcctAdjustBillEditUI() **throws** Exception

{

**[super]{.underline}**();

> prmtCustomer =
> (KDBizPromptBox)kdtEntrys.getColumn(\"customer\").getEditor().getComponent();

prmtCustomer.setEnabledMultiSelection(**true**);

}

### 控件定制

控件的初始化、样式定制、行为定制、事件监听处理。

-   和上下文、单据无关的控件定制可放在构造方法中

示例：某单据禁止用户执行修改操作，可在构造方法中执行actionEdit.setEnabled(false);

说明：控件方法放在onLoad方法中也能达到相同效果。

提醒：在做标准产品二开定制控件时，必须分析清楚标准产品的控件定制代码和二开定制代码的执行先后顺序，避免二开代码不生效。

-   上下文相关、单据无关的控件定制可放在onLoad方法中

示例：某客户要求单据的某个字段正常编辑可见，在工作流审批时隐藏。单据是否在工作流可以通过单据上下文获取相应变量进行识别，这时必须在onLoad方法取得单据上下文及识别标志，然后设置控件样式。

-   单据相关的控件开发可放在loadFields方法

示例：销售订单上有销售组织F7和物料F7字段，物料F7中可选物料受销售组织限制，考虑到已有单据打开编辑时、前翻后翻修改单据时也必须满足这一限制，因此设置物料F7过滤条件的代码应当放在loadFields方法，此发时根据具体的单据对象的销售组织设置物料F7的过滤条件。

在EAS中常用控件的开发中，比较复杂的控件是KDBizPromptBox（F7控件）和KDTable控件

控件样式定制示例：

**this**.chkautoCreateTo.setEnabled(**false**);

**this**.txtDescription.setEnabled(**false**);

**this**.prmtcustomFundType.setEnabled(**false**);

**this**.pkBizDate.setTimeEnabled(**false**);

**this**.contDescription.setEnabled(**false**);

**this**.pkAuditTime.setTimeEnabled(**true**);

**this**.pkLastupdateTime.setTimeEnabled(**true**);

**this**.pkCreateTime.setTimeEnabled(**true**);

**this**.prmtSaleOrgUnit.setEnabled(**false**);

#### F7控件定制示例

// 设置人员F7控件

**protected** **void** setPersonF7()

{

// 设置F7的基本样式

**this**.prmtmanager.setVisible(**true**);

**this**.prmtmanager.setEditable(**true**);

**this**.prmtmanager.setRequired(**false**);

// 设置F7中对象的显示/查询属性

**this**.prmtmanager.setDisplayFormat(\"\$name\$\");

**this**.prmtmanager.setEditFormat(\"\$number\$\");

**this**.prmtmanager.setCommitFormat(\"\$number\$\");

// 设置F7弹出窗体所列示数据的来源

**this**.prmtmanager.setQueryInfo(\"com.kingdee.eas.hr.affair.app.PersonAllQuery\");

//
以下是构建F7控件的对象查询视图，视图包括：对象属性(select)，过滤条件(where)，排序(order
by)

//
设置F7弹出窗体列示数据的对象视图，注意view里的SorterItemCollection不支持通配符\*

EntityViewInfo view = **new** EntityViewInfo();

// 设置视图过滤条件

view.setFilter(getPersonFilterInfo());

// 设置视图排序

SorterItemCollection sorter = **new** SorterItemCollection();

> //设置排序规则

sorter.add(**new** SorterItemInfo(\"number\"));

> //视图调用排序规则

view.setSorter(sorter);

> //当前控件调用

prmtmanager.setEntityViewInfo(view);

//
定义对象的查询属性，如果需要把通配符\*加入SorterItemCollection，则应当在getQueryAgent上设置

SelectorItemCollection selector = **new** SelectorItemCollection();

selector.add(\"\*\");

selector.add(\"position.\*\");

selector.add(\"position.adminOrgUnit.\*\");

prmtmanager.getQueryAgent().setSelectorCollection(selector);

}

// 获取当前行政部门及下属部门的人员过滤条件

**protected** FilterInfo getPersonFilterInfo()

{

> //管理部门的值

AdminOrgUnitInfo adminOrg = (AdminOrgUnitInfo)
prmtadminOrgUnit.getValue();

FilterInfo filter = **new** FilterInfo();

**if**(adminOrg==**null**){

filter.appendFilterItem(\"number\", \"====none===\");

[]{#_Toc487979252 .anchor}}else{

filter.getFilterItems().add(**new**
FilterItemInfo(\"AdminOrgUnit.longNumber\",

adminOrg.getLongNumber(), CompareType.*EQUALS*));

filter.getFilterItems().add(**new**
FilterItemInfo(\"AdminOrgUnit.longNumber\",

adminOrg.getLongNumber()+\"!%\", CompareType.*LIKE*));

filter.setMaskString(\"\#0 or \#1\");

}

**return** filter;

}

#### KDTable控件定制示例

**int** rowIndex = 0, colIndex = 0;

// 获取表格行

IRow row = kdtEntrys.getRow(rowIndex);

// 获取表格列

IColumn [column]{.underline} = kdtEntrys.getColumn(colIndex);

// 获取表格单元格

ICell cell = kdtEntrys.getCell(rowIndex, colIndex);

// 获取行单元格

ICell [cell2]{.underline} = row.getCell(colIndex);

// 获取单元格值

Object [value]{.underline} = cell.getValue();

// 获取表格标题行

IRow headRow = kdtEntrys.getHeadRow(0);

// 获取标题行单元格

ICell [cell3]{.underline} = headRow.getCell(colIndex);

// 设置表格样式---可编辑

kdtEntrys.getStyleAttributes().setLocked(**false**);

// 设置行样式---不可编辑

row.getStyleAttributes().setLocked(**true**);

// 设置表格列样式---隐藏

column.getStyleAttributes().setHided(**true**);

// 设置单元格前景色

cell.getStyleAttributes().setFontColor(Color.*red*);

// 获取表格列的编辑控件

Component [component2]{.underline} = column.getEditor().getComponent();

// 表格的选择管理器，获取表格所选块

KDTSelectManager selectManager = kdtEntrys.getSelectManager();

**for**(**int** i=0; i\<selectManager.size(); i++)

{

KDTSelectBlock block = selectManager.get(i);

**for**(**int** j=block.getTop(); j\<=block.getBottom(); j++) {

IRow [row2]{.underline} = kdtEntrys.getRow(j);

}

}

// 设置表格编辑监听器

kdtEntrys.addKDTEditListener(**new** KDTEditAdapter(){

**public** **void** editStopping(KDTEditEvent e){

kdtEntrys\_Changed(**e.getR**owIndex, **e.getC**olIndex)

}

});

// 常见的表格自动计算示例

**public** **void** []{#OLE_LINK79 .anchor}kdtEntrys\_Changed(**int**
rowIndex,**int** colIndex) **throws** Exception

{

**super**.kdtEntrys\_Changed(rowIndex, colIndex);

// 获取当前编辑行

IRow row = kdtEntrys.getRow(rowIndex);

// 获取当前编辑列的名称（key）

String colName = kdtEntrys.getColumn(colIndex).getKey();

[]{#_Toc487979253 .anchor}//
计算总人天=汇总表格所有行的人天数据，判断当前编辑的列＝人天列

**if** (\"manday\".equalsIgnoreCase(colName))

{

BigDecimal totalManday = BigDecimal.*ZERO*;

**for**(**int** i=0; i\<kdtEntrys.getRowCount(); i++)

{

IRow row2 = kdtEntrys.getRow(i);

BigDecimal value =
TypeConversionUtils.*objToBigDecimal*(row2.getCell(colIndex).getValue());

**if**(value!=**null**)

totalManday = totalManday.add(value);

}

txttotalManday.setValue(totalManday);

}

// 计算：金额＝单价\*数量，判断当前编辑的列＝单价列或数量列

**if** (\"price\".equalsIgnoreCase(colName) \|\|
\"qty\".equals(colName))

{

BigDecimal price =
TypeConversionUtils.*objToBigDecimal*(row.getCell(\"price\").getValue());

BigDecimal qty =
TypeConversionUtils.*objToBigDecimal*(row.getCell(\"qty\").getValue());

**if**(qty!=**null** && price!=**null**)

{

BigDecimal amount = qty.multiply(price).setScale(2,
BigDecimal.*ROUND\_HALF\_UP*);

row.getCell(\"amount\").setValue(amount);

}

}

}

更多KDTable控件开发方法，请参考总部相关控件文档和产品示例。

### 控件监听/自动处理

实现某些事件发生时，自动设置控件样式、自动执行数据计算的功能。通常是在事件发生的控件上添加相应的事件监听器和处理方法。

按照规范的做法，事件监听器和处理方法应当分离，监听器通常是一个匿名内部类，处理方法应当设计出单据方法，由监听器调用，这样事件处理方法可以被继承扩展。示例：

[]{#OLE_LINK40 .anchor} **public** ProjectReportEditUI() **throws**
Exception

{

**super**();

kdtEntrys.addKDTEditListener(**new** KDTEditAdapter() {

**public** **void** editStopped(KDTEditEvent e) {

kdtEntrys\_Changed(e.getRowIndex(),e.getColIndex());

}

});

}

**public** **void**[]{#OLE_LINK49 .anchor} kdtEntrys\_Changed(**int**
rowIndex,**int** colIndex)

{

......

}

#### F7监听注意事项

F7控件添加DataChangeListener监听器，监听数据变化执行自动处理是非常常见的开发内容。需要注意的是：在Java代码中调用F7.setValue方法，例如prmtManager.setValue(person)，会触发DataChangeListener。

案例问题分析：下图中需要开发选择"项目经理"自动获取其对应项目的名称设置到"项目"字段。假设用户选择了"张三"系统自动带出对应的项目名称"XX公司HR实施"，然后用户修改项目为"XX公司OA开发"，然后保存关闭单据。

但是用户下次再打开查看单据时，项目仍然会是"XX公司HR实施"，和数据库里的不一致。这是因为：

a)  系统从数据库获取单据对象，按照EditUI的绑定规则把值对象的数据绑定到控件上

b)  首先为文本字段设置值，此时：项目＝XX公司OA开发

c)  然后为项目经理F7设置值，此时触发了DataChangeListener，项目被重新设置成了"XX公司HR实施"

![](media/media/image123.png){width="5.472916666666666in"
height="2.1166666666666667in"}

-   解决办法

在super.loadFields() 之前卸载F7控件的监听器，super.loadFields()
之后加载F7控件的监听器。为此我们需要把F7监听器定义为类变量，在构造方法中仅做初始化，然后在
super.loadFields() 前后进行卸载和加载。示例：

**protected** DataChangeListener prmtManageListener;

**public** ProjectPlanEditUI() **throws** Exception

{

**super**();

prmtManageListener = **new** DataChangeListener(){

**public** **void** dataChanged(DataChangeEvent ev)

{

prmtManagerChanged((PersonInfo) ev.getNewValue());

}

};

}

**public** **void** loadFields()

{

prmtmanager.removeDataChangeListener(prmtManageListener);

**super**.loadFields();

prmtmanager.addDataChangeListener(prmtManageListener);

}

更多F7控件开发方法，请参考总部相关控件文档和产品示例。

### 新增默认值

在createNewData方法中，设置新增值对象的属性即可，EAS系统会自动把新增的值对象和控制进行绑定。

注意：某些开发人员可能在构造方法、onLoad、loadFields方法中设置控件值，强烈禁止这种做法，这会和已有单据的查看编辑时的控件定制代码混淆在一起，增加代码复杂性，且易产生潜在BUG。

示例代码：

**protected** com.kingdee.bos.dao.IObjectValue []{#OLE_LINK41
.anchor}createNewData(){

BizAcctAdjustBillInfo objectValue = **new** BizAcctAdjustBillInfo();

objectValue.setCreator((UserInfo)[(SysContext.*getSysContext*().~~getCurrentUser~~())]{.underline});

objectValue.setBizDate(**new** Date());

objectValue.[setBaseStatus]{.underline}(BillStatusEnum.*save*);

**try**{

> []{#OLE_LINK50 .anchor}AdjustTypeCollection dtCol =
> AdjustTypeFactory.*getRemoteInstance*()
>
> .getAdjustTypeCollection(\" where number=\'01\'\");
>
> **if**(dtCol.size()\>0)
>
> objectValue.setAdjustType(dtCol.get(0));

} **catch** (BOSException e) {

> e.printStackTrace();

}

objectValue.getEntrys().add(**new** BizAcctAdjustBillEntryInfo());

**return** objectValue;

}

### Action开发

菜单、按钮的实现代码，放在对应Action的[]{#OLE_LINK42
.anchor}actionXXXX\_actionPerformed方法中。

禁止直接为Menu、Button添加鼠标按钮事件监听的做法。

#### 审核和反审核

EditUI调用服务端的审核和反审核方法，并把当前editData作为参数传递过去，完成单据的审核和反审核。

示例代码如下：

[]{#OLE_LINK43 .anchor}**public** **void** []{#OLE_LINK51
.anchor}actionAudit\_actionPerformed(ActionEvent e) **throws** Exception

{

// 未保存的单据不允许审核

**if** (**this**.editData.getId() == **null**)get

**throw** **new** HeFeiBizException(HeFeiBizException.*BILL\_UNSAVE*);

// 调用服务端审核方法

ProjectPlanFactory.*getRemoteInstance*().audit(editData);

com.kingdee.eas.util.client.MsgBox.*showInfo*(\"审核成功\");

// 审核完成后重新加载单据对象

setDataObject(getValue(**new** ObjectUuidPK(editData.getId())));

loadFields();

}

#### 编辑前检查

单据一般会限制已审核的单据不允许修改和删除，该控制逻辑属于核心控制，本文要求开发人员必须把控制代码放在服务端实现，即在服务端的save、submit、delete方法中进行检查控制。

考虑有一种情形，用户打开一张已经审核的单据，点击【编辑】，然后录入了很多内容，最后点击【保存】时，系统才提示单据已经审核不允许修改保存。这种控制的用户体验性非常不好，因此应当在用户点击【编辑】时就给出提示，必须注意：该提示并不能取代服务端的检查控制！

示例代码：

**public** **void** actionEdit\_actionPerformed(ActionEvent e)
**throws** Exception

{

BillStatusEnum status = editData.getBaseStatus();

> **if**(status.getValue()\>=BillStatusEnum.*AUDITED\_VALUE*)
>
> **throw** **new**
> HeFeiBizException(HeFeiBizException.*BILL\_AUDITED*);

**super**.actionEdit\_actionPerformed(e);

}

 LISTUI.java
------------

实现单据数据列示的Java类，由ListUI元数据发布生成，在EAS客户端运行。

### ListUI的层次结构

![](media/media/image124.png){width="5.084027777777778in"
height="2.8965277777777776in"}

### 关于mainQueryPK和mainQuery

ListUI运行时，数据表格绑定到数据查询结果集，结果集是依据指定的Query元数据和过滤条件查询得到。和EditUI不同，ListUI并没有用类变量来保存这个结果集，而是用mainQueryPK变量保存Query元数据的路径名称，用mainQuery变量保存运行时的查询过滤条件。ListUI数据表格各列和Query各字段的绑定规则可以在BOS
Studio的数据绑定视图中调整，BIM建模时会自动设置绑定规则。

![](media/media/image125.png){width="6.188888888888889in"
height="2.8in"}

![](media/media/image126.png){width="5.434722222222222in"
height="1.9951388888888888in"}

### 重要方法

+-----------------+-----------------+-----------------+-----------------+
| **方法名**      | **执行次数**    | **调用时间点**  | **主要代码方法** |
+-----------------+-----------------+-----------------+-----------------+
| \<构造方法\>    | 1               | 类加载          | 上下文无关的控件初始化 |
+-----------------+-----------------+-----------------+-----------------+
| onLoad          | 1               | 类加载后        | 与上下文相关的控件初始化 |
+-----------------+-----------------+-----------------+-----------------+
| actionPerformed | 多次            | 点击按钮或菜单项 | 功能调用，检查控制 |
+-----------------+-----------------+-----------------+-----------------+
| getDefaultFilte |                 | 数据查询        | 修改默认过滤条件 |
| rForQuery       |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| getMainQuery    |                 | 获取运行时过滤条件 |              |
+-----------------+-----------------+-----------------+-----------------+
| getMainQueryPK  |                 | 获取Query元数据路径 |             |
+-----------------+-----------------+-----------------+-----------------+
| checkSelected   |                 | 检查当前是否至少选择一行，没有 |
|                 |                 | 则抛出异常      |
+-----------------+-----------------+-----------------+-----------------+
| getSelectedIdVa |                 | 获取用户所选单据的ID列表，类 |
| lues            |                 | 似方法还有：    |
|                 |                 |                 |
|                 |                 | getSelectedFiel |
|                 |                 | dValues、getSele |
|                 |                 | ctedKeyValues   |
+-----------------+-----------------+-----------------+-----------------+
| getSelectedKeyF |                 | 获取用户所选的第一张单据的ID |
| orAll           |                 | 列表，类似方法还有： |
|                 |                 |                 |
|                 |                 |                 |
|                 |                 | getSelectedKeyV |
|                 |                 | alue            |
+-----------------+-----------------+-----------------+-----------------+
| refreshList     |                 | 刷新列表        |
+-----------------+-----------------+-----------------+-----------------+

### 获取单据ID

ListUI有一个名为"id"的隐藏列，该列专门用于保存单据的ID。在查看/编辑、审核/反审核等针对单据的业务操作中，都是从id列获取单据的ID。

![](media/media/image127.png){width="6.408333333333333in"
height="2.682638888888889in"}

#### 定制列表查询条件

通常修改的框架相关方法：

-   [[]{#OLE_LINK44 .anchor}]{#OLE_LINK52
    .anchor}isIgnoreCUFilter()：只是单据是否按管理单元隔离。通常基础资料会扩展该方法，返回true，表示不需要按管理单元隔离。

-   getDefaultFilterForQuery()：获取列表界面默认的过滤条件，EAS8.0及后续版本中的组织隔离改善很多，此处很少需要开发。

-   getQueryExecutor(IMetaDataPK,
    EntityViewInfo)：最终传送到服务端的过滤条件和查询元数据，此处开发也很少，但是在列表数据取数的调试观察中常用。

-   示例：基础资料取消管理单元隔离

**protected** **boolean** isIgnoreCUFilter()

{

**return** **true**;

}

-   示例：getDefaultFilterForQuery中修改默认过滤条件

/\*

\* 10502下可以看到所有的业务账户

\* 当前组织是记账组织时，查询显示已经许可给当前组织的业务账户；

\* 当前组织不是记账组织时，查询显示已经许可给委托记账组织的业务账户。

\*/

[]{#OLE_LINK47 .anchor}**protected** FilterInfo
getDefaultFilterForQuery()

{

[]{#OLE_LINK46 .anchor} FilterInfo filter = **new** FilterInfo();

OrgUnitInfo curOrg = SysContext.*getSysContext*().getCurrentOrgUnit();

**if**(!\"10502\".equals(curOrg.getNumber()))

{

String curOrgId = curOrg.getId().toString();

String orgFilter = \"SELECT FPARENTID FROM T\_BAC\_BizAccountGrantOrg
WHERE FOrgUnitID=\'\" + curOrgId + \"\' OR FOrgUnitID IN (SELECT
CFBookOrgUnitID FROM CT\_BAC\_BizOrgConfig WHERE CFBizOrgUnitID=\'\" +
curOrgId + \"\')\";

filter.getFilterItems().add(**new** FilterItemInfo(\"id\", orgFilter,
CompareType.*INNER*));

}

**return** filter;

}

#### 定制自定义查询条件面板

很多标准产品列表界面都有在过滤查询时都有如下情形：

![](media/media/image128.png){width="5.065972222222222in"
height="3.7993055555555557in"}

【自定义】【排序】【表格设置】三个页签是框架提供，二开单据不需要额外开发即具有该功能，称为"通用查询过滤"；红框的【条件】面板是个别开发，称为自定义查询面板，是为了方便用户查询单据而设计。

开发自定义面板步骤：

A.  在BOS
    Studio中开发FilterUI元数据（增加UI），添加所需的用户输入控件，父UI选择com.kingdee.eas.base.commonquery.client.CustomerQueryPanel。

B.  发布FilterUI生成代码，进行代码开发，主要开发内容：

-   初始化，在构造方法或OnLoad方法初始化控件

-   getFilterInfo()：整理FilterUI用户输入的数据，形成FilterInfo返回给ListUI

-   getCustomerParams()：当用户点击【保存方案】时，开发人员把当前界面输入的数据整理成Map交给框架，由框架负责保存到数据库。

-   setCustomerParams(CustomerParams)：当用户点击某个查询方案时，框架负责从数据库找到原来保存的方案数据，开发人员负责把Map里的数据还原到控件上、

开发示例文件：

A.  ListUI中为通常查询框加入自定义查询框，主要是扩展initCommonQueryDialog()方法，示例如下：

**protected** CustomerQueryPanel customerQueryPanel = **null**;

**protected** CommonQueryDialog []{#OLE_LINK48
.anchor}initCommonQueryDialog()

{

CommonQueryDialog dialog = **super**.initCommonQueryDialog();

**try**{

dialog.addUserPanel(getUserPanel());

}**catch**(Exception e){

handUIException(e);

}

**return** dialog;

}

**protected** CustomerQueryPanel getUserPanel() **throws** Exception

{

**if** (**this**.customerQueryPanel == **null**)

**this**.customerQueryPanel = **new** ProjectFilterUI();

customerQueryPanel.onLoad();

**return** **this**.customerQueryPanel;

}

### Action开发

菜单、按钮的实现代码，放在对应Action的actionXXXX\_actionPerformed方法中。

禁止直接为Menu、Button添加鼠标按钮事件监听的做法。

#### 审核和反审核

List调用服务端的审核和反审核方法，并把当前所选单据作为参数传递过去，完成单据的审核和反审核，通常需要支持当用户选择多张单据的批量操作。

示例代码如下：

**public** **void** actionAudit\_actionPerformed(ActionEvent e)
**throws** Exception

{

checkSelected();

ArrayList\<String\> selecedIds = [getSelectedIdValues()]{.underline};

// 缓存远程服务示例

IProjectPlan ipp = ProjectPlanFactory.*getRemoteInstance*();

**for**(**int** i=0; i\<selecedIds.size(); i++)

{

ProjectPlanInfo editData = (ProjectPlanInfo)ipp.getValue(**new**
ObjectUuidPK(selecedIds.get(i)));

ipp.audit(editData);

}

com.kingdee.eas.util.client.MsgBox.*showInfo*(\"审核成功\");

refreshList(); // 刷新列表界面

}

#### 编辑前检查

> 和编辑界面的编辑前检查一样，为了提升用户友好性增加的状态检查。

**public** **void** []{#OLE_LINK53
.anchor}actionEdit\_actionPerformed(ActionEvent e) **throws** Exception

{

checkSelected();

BizAcctAdjustBillInfo billInfo =
BizAcctAdjustBillFactory.*getRemoteInstance*().getBizAcctAdjustBillInfo(**new**
[]{#OLE_LINK54 .anchor}ObjectUuidPK(**this**.getSelectedKeyValue()));

BillStatusEnum status = billInfo.getBaseStatus();

**if**(status.getValue()\>=BaseDataStatusEnum.*AUDITED\_VALUE*)

**throw** **new** HeFeiBizException(HeFeiBizException.*BILL\_AUDITED*);

**super**.actionEdit\_actionPerformed(e);

}

 EAS平台开发
============

数据库操作
----------

### 数据库查询结果集

数据库查询返还的结果集一般是IRowSet接口对象，BOS提供的查询工具返还的结果集是一个实现了IRowSet接口的内部结果集对象。

EAS底层完成数据连接和查询操作后，会根据原始数据查询结果集，生成一个与数据库连接无关的IRowSet结果集对象，并关闭原始数据查询结果集，开发人员不需要关注和管理数据库连接。利用查询工具（而不是用数据库连接对象）完成数据查询和操作后，系统会自动关闭原始的数据库查询结果，回收数据库连接。

### 关于KSQL

EAS支持MS
SQLServer、Oracle、DB2、SysBase数据库，这些不同的数据库的SQL语法存在部分差异，开发人员如果面向这些不同的数据库编写SQL语句时，需要人为处理这些差异，增加代码开发工作量和复杂度。金蝶提供了一种中间SQL语言：KSQL，开发人员可使用KSQL编写SQL语句，实际执行过程中，有KSQL引擎根据当前连接的数据库类型，翻译成相应的方言SQL。

建议开发人员养成使用KSQL编写SQL语句的习惯，包括在代码和扩展报表数据源设计中。

关于KSQL的使用可参看金蝶专门的开发文档。

KSQL的日期描述语法：{d 'yyyy-MM-dd HH:mm:ss.SSS'}。

### 客户端数据库操作

客户端不支持事务处理，一般只做数据库的查询操作，对于数据的更新、删除，一般是需要传递到服务端完成，传递途径可以是entity功能，或者定义专用的façade功能。

-   客户端数据查询可使用SQLExecutorFactory，使用方法：

IRowSet result =
SQLExecutorFactory.getRemoteInstance(sql.toString()).executeSQL()

-   BOS80及后续版本中，SQLExecutorFactory也支持insert/update/delete这些数据更新操作。

-   客户端数据查询示例：

*StringBuffer sql = **new** StringBuffer(\"select so.\* from
t\_sd\_saleOrder so \\n\");*

*sql.append(\"inner join t\_sd\_saleOrderEntry soe on
so.fid=soe.fparentid and so.fbasestatus\>=4 \\n\");*

*sql.append(\"where so.fbizdate\>{d '2012-1-1'} \\n\");*

*IRowSet result = SQLExecutorFactory.*

> *getRemoteInstance(sql.toString()).executeSQL();*

***try** { *

***while**(result.next())*

> *System.out.println(rs.getString("fnumber"));*

*} **catch** (Exception e) {*

*MsgBox.showError(e.getMessage());*

*}*

### 服务端数据库操作

-   服务端数据库操作工具类：com.kingdee.eas.util.app.DbUtil，工具类提供了带结果返还的executeQuery方法，不带结果返回的execute方法，并且都可以在SQL语句中用"?"定义参数，执行时向方法传递参数值。

<!-- -->

-   服务端禁止使用SQLExecutorFactory

SQLExecutorFactory也有getLocalInstance方法可在服务端获取实例进行数据查询，但是它会启动新的数据库连接，这意味着可能会发生死锁。在方法体中如果对某个数据集合进行的更新、删除，在方法结束事务提交之前，对于一般默认的数据库锁级别来说，这些数据集合是读锁定的，如果在SQLExecutorFactory中又恰好去取这些数据，那么服务器线程就会处于死锁状态。例如以下代码：

**protected** IObjectPK \_save(Context ctx, IObjectValue model)
**throws** BOSException, EASBizException {

[String]{.underline} sql1 = \"update t\_sd\_saleOrder set
FAmount=FQty\*FPrice where FNumber=\'001\'\";

com.kingdee.eas.util.app.DbUtil.*execute*(ctx, sql1);

String sql2 = \"select FAmount from t\_sd\_saleOrder where
FNumber=\'001\'\";

IRowSet result = SQLExecutorFactory.

> *getLocalInstance*(ctx, sql2).executeSQL();

}

这个示例比较直观，但是在实际的服务端业务执行过程中，复杂业务往往会层层调用多个单据的业务方法，这时候就很难判断SQLExecutorFactory执行的SQL中是否含有被修改的数据了。

### 客户端查询分析器

EAS客户端提供了运行期的SQL查询分析器，但是是一个无显示菜单的隐藏功能，打开【币别】，按【Ctrl＋shift＋q】，输入administrator密码即可打开如下：

![](media/media/image130.png){width="6.413888888888889in"
height="4.155555555555556in"}

常用操作：

【查询UUID】【UUID查表名】：输入一个id字符串，即可获取对应的数据库表查询语句

【实体表搜索】：按中文名称搜索所有的EAS数据库表

【显示表定义】：输入数据库表名称，返回表字段定义数据

 异常处理
---------

### BOSException

![](media/media/image131.png){width="3.65625in"
height="3.3125in"}BOSException用于描述EAS运行过程中各种非业务逻辑性的错误，例如数据库连接错误、网络连接错误、代码和方法调用错误等等。异常

在服务端的所有方法体都会抛出BOSException。客户端捕获到这类异常以下图形式给用户提示：

在这个对话框上，按【Ctrl+E】，对话框显示详细的错误信息。开发者遇到这种错误应当仔细查看错误信息，分析错误发生的位置和原因。

### EASBIZEXCEPTION

EASBizException用于描述各种业务逻辑上的错误，例如字段值为空、字段值不符合预期、逻辑检查错误等。EAS服务端各基类方法一般都会抛出EASBizException，开发人员自己增加的功能应当也习惯增加EASBizException异常。客户端捕获这种异常会以友好的界面进行提示，如下图：

![](media/media/image132.png){width="3.6631944444444446in"
height="1.9777777777777779in"}

这种错误提示对于开发人员来说，往往是不够清晰的，应当配合客户端或者服务端日志进行更细致的错误定位和分析。

一般对于常见需要固化的业务异常、或者需要对不同业务异常需要区别对待时，开发人员需要自己定义继承自EASBizException的业务异常元数据，定义异常子项；在符合异常抛出的地方抛出异常。自定义异常支持定义参数，运行时会以方法中传递的参数值替换异常消息中的参数。

![](media/media/image133.png){width="6.415972222222222in"
height="1.9159722222222222in"}

代码构造和抛出异常的方法：

**if**([billInfo]{.underline}.getStatus()==**null**)

**throw** **new** HeFeiBizException(HeFeiBizException.*NULL\_FIELD*,

> **new** Object\[\]{\"项目状态\"});

其中"**new** Object\[\]{\"项目状态\"}"会替换异常信息中的"{0}"。

### 重要！异常捕获处理

方法体内执行的代码可能会抛出异常需要catch处理，以下是大多数开发新人容易犯的错误：

String selSql = \"select \* from T\_PRJ\_ProjectPlanEntry\";

IRowSet rowSet = DbUtil.*executeQuery*(ctx, selSql);

**try**{

String [number]{.underline} = rowSet.getString(\"FNumber\");

}**catch** (SQLException e){

**e.printStackTrace();**

}

执行SQL发生SQLException，在catch子句中仅仅打印输出结束。这个异常如果是致命的，即异常对方法的整个功能正常执行是不可忽视的，那么这种做法等同于"隐瞒"或者是"吃掉"了这个异常，后续代码会正常执行，整个方法看上去没有异常发生！！

其结果可能会非常严重：一是导致后续方法由于数据异常而错误，或是存储到数据库表里的数据是错误数据，并且这种错误无法被立即发现，可能要等到未来"很久"在"其它"地方发现有问题，很难去跟踪分析错误的来源和原因！

所以，除非开发者认为异常对方法的逻辑没有影响，否则**异常必须"及时汇报"！**即捕获的异常应当立即throw出去。上述示例代码应该改为：

String selSql = \"select \* from T\_PRJ\_ProjectPlanEntry\";

IRowSet rowSet = DbUtil.*executeQuery*(ctx, selSql);

**try**{

String [number]{.underline} = rowSet.getString(\"FNumber\");

}**catch** (SQLException e){

**e.printStackTrace();**

**throw** **new** BOSException(e); // 异常立刻汇报！！！

}

视图和OQL
---------

### OQL

OQL：对象查询语言，区别于SQL的面向数据库查询，OQL是面向对象查询的语言。我们会写OQL片段，例如select部分、where部分、order
by部分。

-   属性：实体和查询元数据中的属性（数据库是字段）；属性可以使用通配符"\*"

-   对象：对应实体或查询元数据（反映到数据库是表和SQL）；属性不能脱离对象单独生效

OQL在最终数据查询和操作时，会由引擎结合对象，翻译成相应的SQL语句。

-   OQL示例，假设当前对象是SaleOrder.entity，以下各属性含义

<!-- -->

-   \*：销售订单**单据体**的所有属性；

-   salePerson.\*：销售订单关联的销售员的所有属性；

-   salePerson.name：销售订单关联的销售员的姓名；

-   entrys.\*：销售订单分录的所有属性；

-   entrys.material.baseUnit.number：销售订单分录的物料的基本计量单位的编码；

> 开发者可参考示例和产品相关代码，编写所需的OQL表达式。

-   常见应用场景

<!-- -->

-   ListUI基于绑定Query元数据查询时，传递过滤条件、字段选择、排序；

-   设置BizPromptBox的视图，包括过滤条件、字段选择、排序；

-   AbstractCoreBaseControllerBean的exists(Context ctx, FilterInfo
    filter)和getValue(Context ctx, String
    oql)方法、AbstractObjectBaseControllerBean的getCollection(Context
    ctx, String oql)和getCollection(Context ctx, EntityViewInfo
    view)方法等，都需要传递基于OQL语言的过滤表达式。示例：

**if**(**this**.\_exists(ctx, \" where
number=\'\"+billInfo.getNumber()+\"\'\"))

**throw** **new** HeFeiBizException(HeFeiBizException.*ERROR*,

> **new** Object\[\]{\"编码已存在\"});

### 视图

这里说的视图是指BOS代码中常用的EntityView对象。EntityViewInfo包含3个部分：

-   []{#_Toc487979277 .anchor}选择项集合SelectorItemCollection

表示属性选择集合，相当于SQL语句中的[]{#OLE_LINK55
.anchor}Select子句。一个SelectorItemCollection中包含一系列的SelectorItemInfo，SelectorItemInfo表示单个属性选择项。

-   过滤条件集合FilterInfo

表示条件过滤，相当于SQL语句中的Where子句；FilterInfo由表示过滤条件集合的FilterItemCollection和表示条件之间如何组合的MaskString组合成；FilterItemCollection包含一系列的FilterItemInfo，FilterItemInfo表示单个的过滤项。

-   排序项集合SorterItemCollection

表示排序项集合，相当于SQL语句中的Order
by子句。一个SorterItemCollection中包含一系列的SorterItemInfo，SorterItemInfo表示单个排序项。

-   EntityViewInfo构造示例

*EntityViewInfo viewInfo = **new** EntityViewInfo();*

*FilterInfo [filter]{.underline} = **new** FilterInfo();*

*filter.getFilterItems().add(**new** FilterItemInfo(\"orgUnit.id\", *

*\"select distinct FOrgID from T\_PM\_OrgRange where FUserID=\'\"*

*+SysContext.getSysContext().getCurrentUserInfo().getId().toString()*

*+\"\'\", CompareType.INNER));*

*filter.appendFilterItem(\"isEnabled\", **new** Integer(1));*

*filter.getFilterItems().add(**new** FilterItemInfo(\"isSysStatus\", *

***new** Integer(0), CompareType.EQUALS));*

*filter.setMaskString(\"\#0 AND (\#1 OR \#2)\");*

*viewInfo.setFilter(filter);*

*SelectorItemCollection selector = **new** SelectorItemCollection();*

*selector.add(\"\*\");*

*selector.add(\"parent.\*\");*

*selector.add(\"status.\*\");*

*selector.add(\"mainClassify.\*\");*

*viewInfo.setSelector(selector);*

*viewInfo.getSorter().add(**new** SorterItemInfo(\"number\"));*

*bizPrompt.setEntityViewInfo(view);*

F7定制
------

开发ERP业务单据会频繁各种基础资料，例如：物料、客商、组织、职员等等，这些字段在界面上用F7控件进行展示和操作。F7控件，即com.kingdee.bos.ctrl.extendcontrols.KDBizPromptBox，![](media/media/image134.png){width="2.4166666666666665in"
height="0.20833333333333334in"}。

### 基本属性

F7控件最基本的需要定制的属性如下：

-   setDisplayFormat：设置对象的显示格式，用\$括起属性，例如：\$name\$-\$number\$

-   setEditFormat：设置F7控件处于编辑状态时的对象显示格式

-   setCommitFormat：用户在F7控件输入文本回车后，F7控件会从QueryInfo模糊查询匹配的对象，如果有多个将提示用户选择。commitFormat决定模糊查询时所查询的对象属性，如果想依据多个属性模糊查询，各属性需要用逗号隔开，例如：\$name\$,\$number\$,\$helpCode\$

-   setQueryInfo：设置F7控件从哪里（哪个查询）获取待选对象集合

上述属性在单据的抽象类中BOS会自动添加定制代码，有些开发场景下，开发者自己初始化或修改这些属性。

### SelectUI

开发者引用标准产品的"物料、客户、供应商、组织、职员......"，用户选择数据时默认弹出的是通用选择框com.kingdee.bos.ctrl.extendcontrols.KDCommonPrompt[]{#OLE_LINK80
.anchor}Dialog

![](media/media/image135.png){width="4.518055555555556in"
height="2.4069444444444446in"}

而所有标准产品的单据中弹出的都是经过定制的更为友好的F7UI，例如销售订单的物料F7使用的是GeneralF7[]{#OLE_LINK56
.anchor}TreeListUI，该UI嵌入了MaterialListUI

![](media/media/image136.png){width="5.101388888888889in"
height="2.941666666666667in"}

一般的SelectUI定制方法是：

-   用户首先要开发一个实现了KDPromptSelector接口的数据显示界面，可以参考标准产品的相关实现类，例如：EntitySelector、FileSelector、DBCenterSelector、CostObjectF7UISelector

-   然后调用KDPromptBox.[]{#OLE_LINK57
    .anchor}setSelector(KDPromptSelector)，把上一步开发的界面设置给F7控件

### 视图

> 设置SelectUI展示数据时使用的视图，包括：过滤、排序、属性集合

-   []{#OLE_LINK58
    .anchor}KDCommonPromptDialog.setEntityViewInfo(EntityViewInfo)

很多F7控件所需的数据过滤和隔离，例如物料/客商的组织和权限范围隔离、基础资料的状态过滤等等，就是为F7控件添加所需的视图过滤条件。

EntityViewInfo构建方法请参考上一节。注意这个方法里的EntityViewInfo的SelectorItemCollection不支持通配符\*。如果要使用通配符，则需要把SelectorItemCollection设置到F7的QueryAgent中，示例如下：

//
定义对象的查询属性，如果需要把通配符\*加入SorterItemCollection，则应当在getQueryAgent上设置

SelectorItemCollection selector = **new** SelectorItemCollection();

selector.add(\"\*\");

selector.add(\"position.\*\");

selector.add(\"position.adminOrgUnit.\*\");

prmtmanager.getQueryAgent().setSelectorCollection(selector);

### 监听

> 获取F7的各种事件，执行自动处理。常见的事件及监听器如下：

-   addDataChangeListener(DataChangeListener)：添加数据改变监听，这是F7最常见的事件和监听。

需要注意：在代码中执行setValue(Object)或setData(Object)
也会触发事件并执行监听程序。该机制可能会导致单据加载时出现一些异常，请参见前面的章节《F7监听注意事项》。

-   addSelectorListener(SelectorListener)：当用户点击![](media/media/image137.bmp){width="0.23958333333333334in"
    height="0.19791666666666666in"}，弹出SelectUI时触发事件，执行监听处理

该监听应用示例：当用户点击![](media/media/image137.bmp){width="0.23958333333333334in"
height="0.19791666666666666in"}时，不想弹出数据选择，而是变更为联查已有对象。开发者为控件添加监听，在willShow方法中弹出对象查看界面，并且取消后续动作。

### 常见F7定制方法

引用标准产品各种基础资料，例如：物料、客商、组织、职员等等，定制这些F7是很繁琐的工作，这里提供供应链产品定制常用F7控件的方法（参考[]{#OLE_LINK84
.anchor}SCMBillEditUI）

#### F7ContextManager

-   F7控件辅助类：com.kingdee.eas.scm.common.util.F7ContextManager
    f7Manager

-   单据super.onLoad之前执行F7ContextManager初始化

> f7Manager = new F7ContextManager(this, getMainBizOrgType());

-   当单据的主业务组织变化时，需要重新设置f7Manager

> f7Manager.setMainOrgContext(getMainOrgContext());
>
> f7Manager.changeF7Context(getUIContext());

-   使用f7Manager设置客户F7

> f7Manager.registerBizCustomerF7(bizCustomerBox, col, queryInfo,
> orgInfo);

设置单据头客户F7示例：f7Manager.registerBizCustomerF7(prmtCustomer,
null, null, null);

-   设置供应商F7的方法

f7Manager.registerBizSupplierF7(KDBizPromptBox, IColumn, String,
OrgUnitInfo)

-   设置物料F7的方法

f7Manager.registerBizMaterialF7(KDBizPromptBox, IColumn, String,
OrgUnitInfo, boolean)

-   设置辅助属性F7的方法，该方法实现了物料变化自动设置辅助属性过滤条件

f7Manager.F7ContextManager.registerAssistPropertyF7(KDTable, String,
String, SCMBillEditUI)

-   设置计量单位F7的方法，该方法实现了物料变化自动设置计量单位过滤条件

f7Manager.registerMeasureUnitF7(KDTable, String, String)

-   设置仓库F7的方法，该方法实现了表头或分录的库存组织变化自动设置仓库过滤条件

f7Manager.registerWarehouseF7(KDBizPromptBox, KDBizPromptBox)

-   设置组织F7的方法

f7Manager.registerBizOrgF7(KDBizPromptBox, IColumn, OrgType, OrgType,
boolean)

#### SCMClientUtils

另一个更轻量的F7控件设置工具类：com.kingdee.eas.scm.common.client.SCMClientUtils，该类还提供了很多供应链业务计算的公共方法

-   setF7MeasureUnit：设置计量单位F7

-   setAsstAttrF7：设置辅助属性F7控件

-   setMainBizOrgF7、setF7OrgUnitBizUnit：设置业务组织F7

弹窗开发
--------

在客户端中经常遇到弹出新窗体以获取用户输入的情形，这种需求包含以下开发步骤：

-   子窗体模型开发：在BOS Studio中设计窗体模型，完成后发布，生成UI类；

-   父窗体弹出窗体功能实现：构建上下文以传递必要的参数，调用窗体工厂创建子窗体，通过上下文或者专门定义的方法获取子窗体返回结果

-   子窗体代码开发：接受父窗体传入的数据，初始化窗体，用户输入检查，输入结果整理返回

// 父窗体弹窗示例代码

**public** **void** actionAbout\_actionPerformed(ActionEvent e)
**throws** Exception

{

AdminOrgUnitInfo value = (AdminOrgUnitInfo) prmtadminOrgUnit.getValue();

**if**(value==**null**)

**return**;

// 可通过上下文向子窗体传递数据

UIContext context = **new** UIContext(**this**);

context.put(\"ID\", editData.getId().toString());

IUIWindow uiWin =
UIFactory.*createUIFactory*(UIFactoryName.*MODEL*).create(

ProjectPlanEditUI.**class**.getName(), context);

ProjectPlanEditUI uiObj = (ProjectPlanEditUI) uiWin.getUIObject();

uiWin.show();

// 可通过上下文或者专门定义方法从子窗体获取返回数据

Boolean isCancel =
(Boolean)uiObj.getUIContext().get(\"dialog\_isCancel\");

**if**(isCancel==**null** \|\| isCancel.booleanValue())

**return**;

[HashMap]{.underline} [result]{.underline} = ([HashMap]{.underline})
uiObj.getUIContext().get(\"result\");

}

### 子窗体接收参数

// 子窗体在onLoad方法中可从上下文获取父窗体传递的数据

**public** **void** onLoad() **throws** Exception

{

**super**.onLoad();

// 尝试从上下文获取开始和截止时间

Date beginDate = (Date) getUIContext().get(\"rqContract\_beginDate\");

Date endDate = (Date) getUIContext().get(\"rqContract\_endDate\");

kdpBeginDate.setValue(beginDate);

kdpEndDate.setValue(endDate);

}

自定义BOTP函数
--------------

### 开发FormulaFunction类

BOS
Java中新增Java类，实现com.kingdee.bos.service.formula.api.IFormulaFunctions接口，按照下例编写代码，最重要的方法如下：

**public** Object evalFunction(String func, [List]{.underline}
paramList) **throws** KScriptException

{

**if**(func == **null** \|\| paramList == **null**)

**return** **null**;

Context ctx = **null**;

**if**(paramList.size()\>0 && paramList.get(0) **instanceof** Context)

ctx = (Context)paramList.get(0);

**else**

ctx = ContextUtils.*getContextFromSession*();

//判断用户是选了哪个公式

**try**{

// 多账号经销商获取主客户资料，

**if**(\"\_\_BOTGetParentCustomer\".equals(func))

{

**int** index = 1;

String custNumber = getIDStringFromObject(paramList.get(index++));

String strProp = getStringFromParams(paramList, index++);

String orgNumber = getStringFromParams(paramList, index++);

String bizTypeNumber = getStringFromParams(paramList, index++);

**return** \_\_BOTGetParentCustomer(ctx, custNumber, strProp, orgNumber,
bizTypeNumber);

}

//
根据费用类型获取预算项目，传递参数：费用类型ID或编码；返回结果：预算项目编码

**else** **if**(\"\_\_BOTGetBudgetItem\".equals(func))

{

String easNumber = getIDStringFromObject(paramList.get(1));

String typeNumber = getIDStringFromObject(paramList.get(2));

**return** \_\_BOTGetBudgetItem(ctx, typeNumber, easNumber);

}

// 获取当前帐套名称，返回结果：预算项目编码

**else** **if**(\"\_\_BOTGetContext\".equals(func))

{

String param = getIDStringFromObject(paramList.get(1));

**return** \_\_BOTGetContext(ctx, param);

}

**else**

**return** **null**;

}

**catch**(Exception e)

{

**throw** **new** KScriptException(\"1001\", **null**, e.getMessage(),
e);

}

}

### 在Entity上注册FormulaFunction类

在来源单据entity或目标单据entity上注册类，添加扩展属性billFormulaClass

![](media/media/image138.png){width="5.435416666666667in"
height="3.713888888888889in"}

多级基础资料
------------

### 多级基础资料模板

![](media/media/image139.png){width="4.683333333333334in"
height="3.475in"}

### 关键属性

多级基础资料的实体有一个共同的父实体TreeBase，其中的属性含义如下：

-   ![](media/media/image140.png){width="1.96875in"
    height="1.7520833333333334in"}isLeaf：是否叶子节点；

-   level：层级，根节点的层级是1；

-   longNumber：长编码，从根节点到当前节点路径上的所有节点的编码用"!"分隔连接的字符串，示例：03!03.20!03.20.01

-   displayName：长名称，从根节点到当前节点路径上的所有节点的名称用"\_"分隔连接的字符串，示例：施工建设阶段\_勘察设计管理\_设计文件内部审批要件

长编码在SQL和代码中常用于：判断节点是否属于某个父节点，获取节点所有的下级节点。示例：

where (job.FLongNumber=CT\_HPJ\_ProjPlanJob.FLongNumber

or LEFT(job.FLongNumber, LENGTH(CT\_HPJ\_ProjPlanJob.FLongNumber)+1)

> =CONCAT(CT\_HPJ\_ProjPlanJob.FLongNumber,\'!\'))

套打数据源开发
--------------

为单据套打打印提供数据源，套打数据源的开发请参考

### 默认单据套打方法

在单据的UI抽象类的两个方法

-   actionPrint\_actionPerformed(ActionEvent)

-   actionPrintPreview\_actionPerformed(ActionEvent)

其中构建数据源的代码为：com.kingdee.bos.ctrl.kdf.data.impl.BOSQueryDelegate
data = new
com.kingdee.eas.framework.util.CommonDataProvider(idList,getTDQueryPK());

### 员工花名册套打方法

com.kingdee.eas.hr.emp.client.EmployeeRosterListUI.execKDFAllSelectionActionNew()

其中的数据源com.kingdee.eas.hr.emp.client.[]{#OLE_LINK85
.anchor}EmployeeDetailNoteDataProvider，具有非常复杂的多数据源的取数逻辑，开发人员可以借鉴参考

### 费用申请单套打方法

com.kingdee.eas.cp.bc.client.OtherExpenseEditUI.methodForPrint(ActionEvent,
boolean)

其中的数据源com.kingdee.eas.framework.print.MultiDataSourceProviderProxy，能够带审批信息打印，开发人员可以借鉴参考

元数据开发
----------

本文开始的章节就重点说明BOS开发一个非常重要的特点是"MDA模型驱动"，模型是单据所具有的各种元素的描述，这些描述不仅仅在建模时有用，在运行时同样可以通过元数据引擎获取到，开发者可以基于模型取得单据具有的诸如属性、功能、实现类等等信息。

### 元数据引擎

com.kingdee.bos.metadata.util.MetaDataLoader提供了运行时获取各种元数据的方法

以下给出元数据应用案例：

### 获取Entity及其Bean

已知单据的BosType获取其控制器Bean，类似于SaleOrderFactory.getLocalInstance(ctx)，但是并不是在代码中指定，而是动态根据BosType获取，可用于很多公共处理方法的设计开发中。

示例代码如下，该方法首先根据BosType获取entity元数据，在查找其工厂类的全名：

**protected** ICoreBase getBizInterface(Context ctx, BOSObjectType
bosType)

**throws** BOSException, EASBizException

{

**try**{

元数据信息

EntityObjectInfo billEntity = MetaDataLoader.*getEntity*(ctx, bosType);

获取接口工厂

String strClsFactory = billEntity.getBusinessImplFactory();

反射

[Class]{.underline} clsFactory = Class.*forName*(strClsFactory);

获取

[]{#_Toc487979299 .anchor}Method method =
[clsFactory.getMethod(\"getLocalInstance\",
Context.**class**)]{.underline};

调用工厂产生接口

ICoreBase iCoreBase = (IObjectBase) method.invoke(clsFactory, ctx);

**return** iCoreBase;

}**catch** (ClassNotFoundException e) {

**throw** **new** BOSException(e);

} **catch** (SecurityException e) {

**throw** **new** BOSException(e);

} **catch** (NoSuchMethodException e) {

**throw** **new** BOSException(e);

} **catch** (IllegalAccessException e) {

**throw** **new** BOSException(e);

} **catch** (IllegalArgumentException e) {

**throw** **new** BOSException(e);

} **catch** (InvocationTargetException e) {

**throw** **new** BOSException(e);

}

}

### 构造Entity对应的值对象

> 已知Entity元数据，创建一个新的值对象。
>
> **public** **static** IObjectValue getObjectValueInfo(EntityObjectInfo
> entity)
>
> **throws** EASBizException, BOSException

{

**try**

{

[Class]{.underline} [clazz]{.underline} =
Class.*forName*(entity.getObjectValueClass());

IObjectValue billInfo = (IObjectValue)clazz.newInstance();

**return** billInfo;

} **catch** (ClassNotFoundException e) {

**throw** **new** BOSException(e);

} **catch** (InstantiationException e) {

**throw** **new** BOSException(e);

} **catch** (IllegalAccessException e) {

**throw** **new** BOSException(e);

}

}

### 检索Entity中的属性

遍历Entity中的所有属性（包括DEP中增加的属性）

**public** **static** **void** buildModelFileter(Context ctx,
IObjectValue billInfo)

{

[]{#OLE_LINK59 .anchor}EntityObjectInfo entity =
MetaDataLoader.*getEntity*(ctx, billInfo.getBOSType());

PropertyCollection coll = entity.getPropertiesRuntime();

**for**(**int** i=0; i\<coll.size(); i++)

{

PropertyInfo property = coll.get(i);

// 关联属性解析

**if**(property **instanceof** LinkPropertyInfo)

{

LinkPropertyInfo linkProperty = (LinkPropertyInfo)property;

EntityObjectInfo [supplierEntity]{.underline} =
linkProperty.getRelationship().getSupplierObject();

......

}

// 自有属性解析

**else**

{

OwnPropertyInfo ownProperty = (OwnPropertyInfo) property;

// 多语言属性解析

**if**(ownProperty.isMultilingual())

{

ColumnInfo [column]{.underline} = ownProperty.getMappingField();

> ......

}

// 非多语言属性解析

**else**

{

BOSObjectType [type]{.underline} = ownProperty.getBOSType();

> ......

}

}

}

}

权限检查
--------

单据的标准功能权限由框架负责检查和控制，开发人员不需要干预。有些场合中，可能需要自定义特殊权限项，然后在代码中执行权限检查。下面的代码给出调用权限平台执行权限检查的示例：

**public** **static** **void** checkPermissionItem([Map]{.underline}
uiContext, String permissionItem) **throws** Exception

{

IObjectPK userPK = (IObjectPK)uiContext.get(\"USER.PK\");

IObjectPK orgPK = (IObjectPK)uiContext.get(\"ORG.PK\");

IMetaDataPK metaPK = (IMetaDataPK)uiContext.get(\"METADATA.PK\");

Boolean orgExtFromCtx = (Boolean)uiContext.get(\"ORGEXT\");

**if**(orgExtFromCtx == **null**)

orgExtFromCtx = Boolean.*FALSE*;

PermissionHelper.*checkFunctionPermission*(userPK, orgPK, metaPK,
**null**, permissionItem, orgExtFromCtx.booleanValue(), uiContext);

}

自动编码
--------

在单据的EditUI抽象类里会有调用编码平台的方法setAutoNumberByOrg(String)，开发人员可参考学习。勾选了![](media/media/image141.png){width="2.5in"
height="0.23958333333333334in"}的单据发布后，其AbstractControllerBean中也会加入通过编码平台自动获取编码的方法，开发人员可以参考学习：

**protected** **void** setAutoNumberByOrg(Context
ctx,com.kingdee.eas.framework.ObjectBaseInfo model,String orgType)

{

String sysNumber = **null**;

**try**

{ //不为空，不为null，组织类型不为null

**if** (!StringUtils.*isEmpty*(orgType) &&
!\"NONE\".equalsIgnoreCase(orgType) &&
ContextUtil.*getCurrentOrgUnit*(ctx,
OrgType.*getEnum*(orgType))!=**null**)

{

sysNumber = FrameWorkUtils.*getCodeRuleServer*(ctx,model,
ContextUtil.*getCurrentOrgUnit*(ctx,
OrgType.*getEnum*(orgType)).getString(\"id\"));

}

**else** **if**
(com.kingdee.eas.util.app.ContextUtil.*getCurrentOrgUnit*(ctx) !=
**null**)

{

sysNumber = FrameWorkUtils.*getCodeRuleServer*(ctx,model,
ContextUtil.*getCurrentOrgUnit*(ctx).getString(\"id\"));

}

**if** (!StringUtils.*isEmpty*(sysNumber)) {

model.setString(\"number\",sysNumber);

}

}

**catch** (Exception e) {}

}

产品报表分析
------------

EAS财务、供应链、生成等很多模块的标准产品报表，业务逻辑复杂，在设计开发中大量用到临时表进行计算。某些场合需要分析这些报表的计算过程时就非常难以跟踪。

值得欣慰的是，总部提供了执行过程跟踪工具，使用方法：

A.  在报表弹出过滤查询界面后按【[]{#OLE_LINK75
    .anchor}Ctrl+shift+alt+\]】会弹出查询跟踪界面，执行录制功能；然后关闭工具正常完成报表查询。\]

![](media/media/image142.png){width="6.40625in"
height="3.467361111111111in"}

A.  报表查询完成后，重新按【Ctrl+shift+alt+\]】，在跟踪器上点击【停止】，然后点击【查看】

![](media/media/image143.png){width="6.4118055555555555in"
height="2.917361111111111in"}

A.  在弹出的"详细信息"页面上就可以看到报表执行过程中所调用的服务端控制器及其方法，以及执行过程中的时间耗费。结合BOS反编译代码分析和跟踪调试，可以找出报表的计算逻辑。

![](media/media/image144.png){width="6.410416666666666in"
height="3.678472222222222in"}

 EAS产品改造开发
================

元数据改造
----------

以下针对标准产品数据的二次开发可以在DEP中完成：

-   标准产品增加字段

-   实体增加功能

-   UI调整界面布局和样式，增加按钮和Action

-   增加Query连接对象和查询字段

-   Function增加功能描述

-   增加自定义权限

常规EAS项目，绝大部分标准产品元数据改造可在DEP中完成。

EditUI/ListUI.java扩展
----------------------

通过窗体工厂UIFactory加载的窗体，包括所有的EditUI和ListUI，BOS提供了扩展继承的机制。

新建一个类从某个EditUI/ListUI继承，保持包路径完全一致，类名为：\[UI类名\]CTEx
，或者\[UI类名\]PIEx。示例：扩展com.kingdee.eas.sd.sale.client.SaleOrderEditUI类，新建com.kingdee.eas.sd.sale.client.SaleOrderEditUIPIEx，父类为SaleOrderEditUI类。

关于扩展类如何在运行时加载生效，开发人员可以参考com.kingdee.bos.ui.face.AbstractUIFactory类的方法createUIObjectNoInit。

在扩展类里，可以扩展标准产品原有方法修改或添加功能。示例代码：

ControllerBean.java扩展
-----------------------

对标准产品已有的ControllerBean进行扩展的方法：

-   新增ControllerBeanEx类，保持包路径完全一致，父类为原ControllerBean，例如扩展com.kingdee.eas.sd.sale.app.SaleOrderControllerBean，新增com.kingdee.eas.sd.sale.app.SaleOrderControllerBeanEx，父类为SaleOrderControllerBean

-   实体添加controllerBeanEx扩展属性，value=\[扩展类的包路径和类目\]。对于EAS7.0及后续版本，可以在DEP中修改entity添加该扩展属性，避免了在BOS中修改元数据产生的二开冲突。

![](media/media/image147.png){width="5.275in" height="3.08125in"}

示例代码：

DEP脚本扩展
-----------

DEP引入的实体、EditUI、ListUI，可以对大部分框架方法添加前置/后置脚本进行扩展。脚本使用JavaScript语法，使用rhino脚本引擎。

脚本中可以调用EAS中任何Java类的public方法！

更多脚本开发说明请参考总部相关文档。

### pluginCtx.getUI()

该方法总部文档没有说明却非常常用，用于UI中获取当前UI对象。

### UI脚本示例

// 工作流审批界面中在值对象中设置审批是否通过标志，以便服务端进行判断

获取界面的属性

var approveIsPass =[]{#OLE_LINK86 .anchor}
pluginCtx.getUIContext().get(\"approveIsPass\");

if(approveIsPass!=null)

设置当前窗体的属性值

pluginCtx.getUI().getDataObject().put(\"multiApprove\_approveIsPass\",
approveIsPass);

### entity脚本示例

// 工作流提交执行合同相关检查

获取环境上下文

var ctx=pluginCtx.getContext();

获取方法

var model=[]{#OLE_LINK60 .anchor}methodCtx.getParamValue(1);

获取关联信息

var
helper=com.kingdee.eas.hefei.contface.helper.app.BizBillHelper.getIntance(ctx,
model);

判断合同信息

if(helper.getContractInfo()==null)

throw new com.kingdee.eas.framework.bireport.BireportException(

com.kingdee.eas.framework.bireport.BireportException.SELF\_INFO,

new Array(\"单据没有关联合同\"));

helper.checkContractBill4WF();

DEP+BOS的功能扩展
-----------------

DEP脚本具有强大的代码扩展能力，但是缺点也很明细：没有代码语法检查、调试不方便。
因此在DEP脚本中编写大量的脚本代码并不是一个明智的做法。

作者在长时间的开发中总结了一套有效方法：大量的核心代码仍然在BOS
Java中进行开发，通过DEP脚本把开发代码和产品模块进行联结。

### UI界面/实体方法扩展

例如增加save/submit/delete/audit/unAudit这些方法的前置逻辑或后置逻辑，示例：

![](media/media/image149.png){width="6.409027777777778in"
height="2.2631944444444443in"}

在BOS中新增了BizBillHelper辅助类，基于合同检查应付金额的合同逻辑代码，实际上是在checkContractBill()方法中完成，DEP脚本仅仅起到了把应付单提交和合同检查进行联结的功能。

获取公共的方法来进行操作

Dep只负责获取参数

这个方法的另一个好处是代码重用，如果客户有多个UI或Entity都存在类似的处理逻辑，则所有需要引用的地方，都只需要写简单的一句脚本即可。而不是到处拷贝粘贴大量的脚本，即繁杂混乱又容易出错。

### UI界面增加控件

例如增加按钮、文本框、标签等，可视化建模部分在DEP模型设计中完成，

当需要设置这些控件的样式时：可以在BOS
Java中开发独立的辅助类方法，例如设置单据新增的项目合同F7控件样式：ProjectUIHelper.setContractF7()，通过方法参数把DEP中的F7控件及其它必须的数据传递给BOS
Java。

#### UI ToolBar增加按钮

ToolBar增加按钮不需要复杂的定位设置，作者还有更为简单的方法，把Button和Action的开发全部放到BOS
Java中实现，UI只需要简单调用即可

在某个合同接口案例中，客户要求在7张单据的列表/编辑界面（14个UI）都要增加合同相关的按钮（大约5个），如果手工在DEP中新增，需要增加70的Button和Action。

-   开发Button对应的Action类

![](media/media/image150.png){width="6.415972222222222in"
height="2.7284722222222224in"}

-   开发工具类，向参数传递过来的UI对象添加合同系列按钮

![](media/media/image151.png){width="6.416666666666667in"
height="3.0416666666666665in"}

-   DEP中为需要添加按钮的UI界面，在onload后置脚本中添加调用的脚本代码

![](media/media/image152.png){width="6.415277777777778in"
height="3.061111111111111in"}

-   最终效果

所有的Action实现代码只有一份，所有UI只需要一句简单脚本调用即可。

### UI界面Java引用控件

DEP中新增的控件，可能会被UIPIEx的其它方法引用。案例：某客户销售订单进行深度定制开发，增加了很多字段和控件，并且参与到物料控制、价格控制等核心业务逻辑中。

![](media/media/image153.png){width="6.4125in" height="2.39375in"}

这些控件必须能够被SaleOrderEditUIPIEx引用，因此需要设计一种方法，把DEP里增加的控件传送到Java中。

-   SaleOrderEditUIPIEx增加用于指向控件对象的类成员变量

**public** **class** SaleOrderEditUIPIEx **extends** SaleOrderEditUI {

[]{#_Toc487979317 .anchor}// 定义EAS80升级后增加的DEP控件对象

**protected** KDBizPromptBox prmtcustomFundType;

**protected** KDBizPromptBox prmtGreeBizType;

**protected** KDBizPromptBox prmtzhuHaiBizType;

**protected** KDBizPromptBox prmtcuprice;

-   SaleOrderEditUIPIEx增加方法，接受DEP控件并且赋值给上述类成员变量

//用于DEP调用，把动态控件传递到代码中

public void []{#OLE_LINK87 .anchor}setDEPComponents(Object object) {

HashMap components = (HashMap) object;

prmtcustomFundType = (KDBizPromptBox)
components.get(\"prmtcustomFundType\");

prmtGreeBizType = (KDBizPromptBox) components.get(\"prmtGreeBizType\");

prmtzhuHaiBizType = (KDBizPromptBox)
components.get(\"prmtzhuHaiBizType\");

prmtcuprice = (KDBizPromptBox) components.get(\"prmtcuprice\");

}

-   DEP中，SaleOrderEditUI在OnLoad方法增加前置脚本，调用setDEPComponents把控件传给Java

[]{#OLE_LINK76 .anchor} //把动态控件传递到代码中

> var components=new java.util.HashMap();
>
> components.put(\"prmtcustomFundType\",
> pluginCtx.getKDBizPromptBox(\"prmtcustomFundType\"));
>
> components.put(\"prmtGreeBizType\",
> pluginCtx.getKDBizPromptBox(\"prmtGreeBizType\"));
>
> components.put(\"prmtzhuHaiBizType\",
> pluginCtx.getKDBizPromptBox(\"prmtzhuHaiBizType\"));
>
> components.put(\"prmtcuprice\",
> pluginCtx.getKDBizPromptBox(\"prmtcuprice\"));
>
> pluginCtx.getUI().setDEPComponents(components);

![](media/media/image154.png){width="6.417361111111111in"
height="2.1194444444444445in"}

 产品和错误分析
===============

产品分析
--------

### 客户端日志

适用于：运行时打开客户端界面，通过日志找到所执行对应的Java类。本方法适用于快速找到标准产品UI界面对应的Java类。

EAS中95%
以上的UI界面由窗体工厂（UIFactory）负责加载，UIFactory加载窗体时，会在控制台或日志中明确输出所加载窗体的Java包路径和类名。

示例：打开销售订单列表界面时的控制台日志：

![](media/media/image155.png){width="6.384722222222222in"
height="3.3020833333333335in"}

如果是在正式客户端，可以查看日志文件：as\\client\\logs\\client.log和log4j.log

已知特殊情形：ListUI中的自定义查询面板、MsgBox消息框等窗体，不是由UIFactory加载，不适用于本方法。

### 主菜单

适用于：通过数据库中的主菜单，找到所执行的Java类

EAS系统主菜单存储于数据库表：[]{#OLE_LINK61
.anchor}T\_PM\_MainMenuItem，该表的FUiClassName字段保持了菜单项对应的Java类。示例：

[]{#OLE_LINK77 .anchor}select FNumber, FName\_L2, FUiClassName from
T\_PM\_MainMenuItem

where FName\_L2 like \'%采购订单%\'

![](media/media/image156.png){width="6.413888888888889in"
height="1.3055555555555556in"}

### 线程挂起

适用于：客户端弹出**模态对话框**时，通过线程执行堆栈找到对应的代码点。
适用于产品分析、客户端的信息、警告或错误分析。

示例：user用户执行费用报销单的新增报错，当弹出对话框时，切记不要点确定消除对话框！转到BOS的调试透视图，在"调试"视图中，找到客户端进程，一般模态界面对应的线程名为"Thread
\[AWT-EventQueue-2\]"（如果不是可尝试其它线程），右键暂挂，

![](media/media/image157.png){width="4.795138888888889in"
height="2.9458333333333333in"}

![](media/media/image158.png){width="5.707638888888889in"
height="2.995138888888889in"}

![](media/media/image159.png){width="5.565972222222222in"
height="3.326388888888889in"}

经分析可知，是BizCollCoreBillEditUI的构造方法对用户类型进行检查。

### 方法断点

适用于：明确知道某个操作执行必然调用的方法，希望了解执行过程的来龙去脉。该方法对于学习EAS产品框架有非常好的帮助。

操作：在该方法上加"方法断点"，捕获断点后，可在"调试"视图中观察执行过程。

示例：希望了解ListUI上点击【新增】按钮弹出EditUI的过程，可在EditUI的构造方法或onLoad方法上打断点，观察执行栈

![](media/media/image160.png){width="6.4125in"
height="3.439583333333333in"}

### 人为制造阻塞或异常

当从确定的入口分析代码执行过程非常困难时（执行链非常长，调用的方法或跟踪的代码太多），可以在某个确定的过程点打断点，或者制造异常来观察异常堆栈。

示例1：分析销售订单的锁库功能，以便为二开单据增加类似的锁库功能。从UI入口到服务端执行分析，由于供应类的服务端大量使用适配器的机制，静态代码无法追踪，动态执行也非常困难。由于明确知道锁库必定会更新即时库存表T\_IM\_Inventory中的锁库数量，因此可以采用以下办法之一：

1)  如果是Oracle数据库，使用PLSQL提前更新对应的数据，并且不要提交事务。使EAS订单锁库执行到表更新时被阻塞。然后挂起服务端线程，观察执行过程，优先挂起名称类似"\[RPC-XXX\]"的线程

2)  修改T\_IM\_Inventory表中锁库数量字段名，使EAS订单锁库执行到表更新时，抛出SQLException，观察错误堆栈，得到方法执行过程。

用法2：分析客户端和服务端间的方法调用过程。客户端调用服务端方法，用断点阻塞服务端进程，然后挂起客户端线程，观察客户端执行路径

### 类加载断点

分析产品时，明确知道某个类会被加载，可以加"类加载断点"观察Java类何时何处被加载。由于JVM中每个Java类只会加载一次，因此该方法用处并不大。

在分析底层一些配置、缓存的加载过程时，可配合使用该方法。

错误分析
--------

### 错误堆栈

Java异常处理时打印出来的异常堆栈，对于异常分析来说是如获珍宝，相比其他语言开发是非常幸福的。如下图这样的详细的错误报告，非常容易就可以找到错误发生点，甚至可以分析方法执行路径学习产品开发设计方法。

![](media/media/image161.png){width="6.409722222222222in"
height="2.091666666666667in"}

也有很多异常的错误对象并非如此直观，这和开发人员写代码时对异常的处理有关。示例：

}**catch** (SQLException e){

**异常处理1：throw** **new** BOSException(\"数据库发生异常:\" +
e.getMessage());

**异常处理2：throw** **new** BOSException(e);

}

异常处理1打印的堆栈，只能追踪到所在行代码，但是e从何而来则无法输出，因为没有为BOSException提供cause（原因），原因被开发人员"隐瞒了"。

异常处理2打印的堆栈，除了BOSException，还会打印SQLException，SQLException是BOSException的cause（原因）。

带有Cause的异常打印示例：

![](media/media/image162.png){width="6.417361111111111in"
height="3.234722222222222in"}

带有Cause的异常分析可能也更需要细心和经验，在实际的EAS错误中，可能最后抛给用户的异常，是经过层层包装转发，Cause已经嵌套很深。遇到这种情况，开发人员可以找到比较原始的Cause，结果下一节所说的异常断点，通常可以快速定位错误。

另外，有时嵌套的Cause，其最原始的Exception可能并不真的是异常发生点，例如上图，直观看异常产生于SQLDiagnostic.addDiagnostic方法：

[java.sql.SQLException]{.underline}: 对象名
\'T\_PRJ\_ProjectPlanEntry1\' 无效。

at
net.sourceforge.jtds.jdbc.SQLDiagnostic.addDiagnostic([SQLDiagnostic.java:372]{.underline})

但是实际上该方法并没有问题，产生问题的原因是交给该方法执行的SQL语句（也就是参数或数据）有问题，真正错误源头在这个错误堆栈里无法看到！数据或参数的错误就需要开发人员真正仔细分析了。

### 异常断点使用

对于分析数据异常具有显著的作用，通过异常断点可以捕获异常最初抛出的运行时点，结合跟踪执行和数据观察分析，找出异常原因。

在调试或Java透视图下，点击菜单"运行------添加Java异常断点"

![](media/media/image163.png){width="6.409722222222222in"
height="3.6958333333333333in"}

如果在异常抛出的路径上存在异常类型转换或重新封装，例如以下代码：

**try**{

> ......

}**catch** (Exception e){

**throw** **new** HeFeiBizException(HeFeiBizException.ERROR,**new**
Object\[\]{\"数据错误\"});

}

Try方法体中如果发生类型任何异常，最终被转换为HeFeiBizException返回，在EAS提供的错误日志中只会出现HeFeiBizException异常，但是try方法体中到底哪一行代码发什么了什么样的异常无法直接看到。

建议开发人员在BOS快测中，可以先打HeFeiBizException的异常断点，当运行到catch方法体内时，可以选择
}**catch** (Exception e){ 中的变量 e
按【ctrl+shift+i】，观察e的具体类型，这时有两种办法继续向前跟踪：

-   在"显示"视图中，输入 e.printStackTrace();
    按【ctrl+shift+i】执行（执行前先清空服务端和客户端控制台的日志，便于观察），然后到控制台查看打印出来的错误日志；

-   观察的变量 e
    的异常类型（class）后，再加上该类型的异常断点，重新走一遍重现异常的操作，抓住
    e 最初抛出的位置。

跟踪调试
--------

### 调试视图

分析当前断点的执行路径，该视图对于学习EAS产品来说，是一个非常强悍的利器。

例如开发者如果想知道当双击EAS主菜单某个菜单，例如"销售订单新增"，我们知道该菜单一定会调用SaleOrderEditUI.class，那么我们可以在该类的构造方法或者onLoad方法上打上方法断点，然后双击"销售订单新增"直至断点被捕获，在调试视图中可以观察到从最初菜单被点击直至断点被捕获的最完整准确的执行路径！

![](media/media/image164.png){width="6.416666666666667in"
height="2.223611111111111in"}

切换到大纲视图，找到onLoad()方法，从右键菜单中找到并点击【切换方法断点】

![](media/media/image165.png){width="6.411111111111111in"
height="2.21875in"}

切换到EAS客户端，找到并执行"销售订单新增"，BOS会捕获到SaleOrderEditUI的onLoad方法断点。

![](media/media/image166.png){width="6.415972222222222in"
height="2.723611111111111in"}

观察"调试"视图，这里列出了执行到断点的完整路径，可以从中找出EAS是如何一步一步从菜单点击执行到SaleOrderEditUI.onLoad()。在执行堆栈任一行上，都可以点击反编译对应的class，都可以根据反编译代码对类的内部变量、局部变量进行观察。

在本案例中，有两行代码开发应当给予足够的关注：

-   UIFactoryHelper.initUIObject(String, Map, Map, String) 行： 296

-   UINewTabFactory.create(String, Map, Map, String) 行： 110

绝大多数EAS界面的加载和初始化，都由这两个类负责完成，包括前面所描述的EditUI和ListUI的扩展机制都可以在这里找到答案。

### 表达式视图

设置一个变量或计算式，在单步执行时观察变化，对于分析产品数据何时何地发生改变具有很大帮助

应用示例：编辑界面某个控件值在打开单据时发生不和预期的改变，可以在构造方法、onLoad方法、loadFields这些方法上打上断点，在表达式视图中添加所关注的数据，例如
txtproject.getText()，在单步执行过程中观察何时何处发生的改变。

### 显示视图

可以在断点处分析变量、表达式，可以执行一个语句获取结果，甚至可以改变线程里的对象数据！

使用用法是：在显示视图中自行输入变量名或者Java语句，选中后按【ctrl+shift+i】执行

![](media/media/image167.png){width="6.409027777777778in"
height="4.345138888888889in"}

#### 深度应用示例1

观察执行过程中的数据库表、临时表数据。后台方法需要更新数据库的在执行过程中几乎都是带事务属性的，有时还会创建临时表。在代码跟踪分析过程中，由于事务未结束，从数据库层根本看不到数据变化，特别是临时表事务结束后通常都会释放掉，无法再数据库层进行跟踪分析。而在断点位置，在显示视图里执行一句com.kingdee.eas.util.app.DbUtil.executeQuery(ctx,
\"select \... from \....\") 即可轻松获取所需数据。

#### 深度应用示例2

执行过程中改变数据，修改执行路径。示例：EAS的元数据加载和很多参数启用了缓存机制，当我们需要观察元数据和参数如何加载时，这些缓存就成了最大障碍。这时可以在适当的地方打上断点，在从缓存获取数据前，在显示视图里执行一个缓存清除语句，例如cacheXXX.clear()
即可清空运行时的缓存，强迫系统去加载数据。

### 变量视图

观察类变量的数据，对于分析标准产品具有帮助。在某些class反编译的源码不能使用时，可以借助该视图观察类对象的数据。

 EAS接口开发
============

[]{#OLE_LINK82
.anchor}异构系统间的集成分为：数据集成、功能集成、流程集成、界面集成。

实际开发中，EAS和异构系统之间需求最多的是数据集成，本章节阐述的也只针对数据集成。其它3中集成在现有技术下要么很难实现、要么实现成本非常高，很少有客户强行去做。

数据流向
--------

接口按数据流方向分为：

EAS输出给第三方（EAS输出），EAS输出比较简单，需要完成的开发内容有：

-   物理通道的设计和实现，运行平台选择

-   数据交换的格式和内容约定

<!-- -->

-   第三方输出给EAS（EAS输入），由于涉及从外部接入数据到EAS系统，其开发内容和开发成本都远高于EAS输出接口，通常还需要完成以下开发内容：

    -   基础数据映射：解决异构系统之间关于基础资料名称编码的差异

    -   基础数据转换和检查：接受的基础数据文本描述符号，检查并转换为EAS的基础数据对象

    -   业务数据检查：接受的外部数据，检查其数据是否符合EAS业务要求；外部系统不能提供的但是EAS要求必须录入的数据如何计算补充

    -   业务数据保存和确认：分析EAS对数据的业务处理（保存、提交、审核或核准）要求及是否存在上下游关联业务的特殊要求，接受的外部数据如何满足EAS系统的这些要求，外部系统不能提供的部分，需要自己准确分析后进行补充处理

物理连接
--------

主要有以下技术实现方式：

-   数据库连接：在数据库层进行连接和数据交换，由数据库负责安全和权限控制，适用于可直接访问对方数据库的场合，开发成本低容易实现

-   WebService：通过WebService进行连接和数据交换，由EAS服务器或其它WebService平台负责安全和权限控制，适用于数据库不能直连，可通过网络访问EAS服务的场合，开发成本高

-   HTTP连接：通过HTTP协议进行连接，和WebService原理相似。

-   文本文件（Excel文件）：通过文件传递数据，适用于数据库和EAS服务均无法访问的场合，开发成本高并且用户使用不方便

前三种方式一般需要开发的内容有：

### 连接配置

建立关于外部数据库或WebService连接方式的配置信息。作为一名合格的开发人员，不应当把对方接口的连接方式写死到代码里，传统开发中可能会放在配置文件或者数据库表中，BOS开发中可以用BOS新建相应的连接配置基础资料。保存连接的URL、数据库类型/WebService方法、用户名、密码等信息，提供连接测试功能。有时可能会需要按照组织、业务类型等设置不同的连接信息。

WebService连接配置案例：

![](media/media/image168.png){width="6.411111111111111in"
height="2.2597222222222224in"}

### 连接实现

构建外部数据库或WebService连接实现的底层代码，提供给业务层调用。

#### SQL Server连接示例

**public** **class** ExternDBUtil {

//获取数据库连接参数(客户端)

**public** **static** DBConnectParms getDBParms4Test() **throws**
BOSException

{

DBConnectParms connectParms=**new** DBConnectParms();

connectParms.setHost(\"192.168.21.53\");

cnnectParms.setPort(\"1521\");

connectParms.setDBName(\"eas\");

connectParms.setUser(\"sa\");

connectParms.setPassword(\"\");

**return** connectParms;

}

//创建[sqlserver]{.underline}数据库连接

**private** **static** Connection ConnectSQLServerDB([]{#OLE_LINK62
.anchor}DBConnectParms connectParms) **throws** BOSException

{

**if**(connectParms==**null**)

**throw** **new** BOSException(\"K3数据库连接参数未指定\");

Connection connection=**null**;

**try** {

//加载JDBC驱动

Class.*forName*(\"net.sourceforge.jtds.jdbc.Driver\");

String url=\"jdbc:jtds:sqlserver://\" + connectParms.getHost() + \":\" +
connectParms.getPort() + \"/\" + connectParms.getDBName();

支持驱动

DriverManager.*registerDriver*(**new**
net.sourceforge.jtds.jdbc.Driver());

connection=DriverManager.*getConnection*(connectParms.getUser(),

connectParms.getPassword(),password);

**return** connection;

} **catch** (ClassNotFoundException e) {

**throw** **new** BOSException(e);

} **catch** (SQLException e) {

**throw** **new** BOSException(e);

}**finally**{

SQLUtils.*cleanup*(rs, statement, connection);

}

}

**public** **static** JdbcRowSet executeQuery(DBConnectParms params,
String sql) **throws** BOSException

{

Connection connection = **null**;

Statement statement= **null**;

java.sql.ResultSet rs = **null**;

JdbcRowSet jdbcrowset = **null**;

**try**{

> 连接

connection=*ConnectSQLServerDB*(params);

会话

> statement = connection.createStatement();
>
> 执行

rs = statement.executeQuery(sql);

获取结果

JdbcRowSet rowset = **new** JdbcRowSet();

填充 rowset.populate(rs);

jdbcrowset = rowset;

**return** jdbcrowset;

}**catch**(SQLException exc){

**throw** **new** BOSException(\"Sql3 execute exception : \" + sql,
exc);

}**finally**{

SQLUtils.*cleanup*(rs, statement, connection);

}

}

**public** **static** **void** execute(DBConnectParms params, String
sql) **throws** BOSException

{

Connection connection = **null**;

Statement statement= **null**;

**try**{

connection=*ConnectSQLServerDB*(params);

statement = connection.createStatement();

statement.execute(sql);

}**catch**(SQLException exc){

**throw** **new** BOSException(\"Sql3 execute exception : \" + sql,
exc);

}**finally**{

SQLUtils.*cleanup*(**null**, statement, connection);

}

}

#### 第三方WebService连接示例

**public** **class** ContfaceAppHelper {

**public** **static** String call(String url, String qName, String
method, String requestXml)

**throws** BOSException, EASBizException

{

**try**{

org.apache.axis.client.Service service = **new** Service();

org.apache.axis.client.Call call = (Call) service.createCall();

//直接引用远程的[wsdl]{.underline}文件

String wsdlUrl = url + \"?wsdl\";

call.setTargetEndpointAddress(wsdlUrl);

//设置调用方法，WSDL里面描述的接口方法名称

call.setOperationName(**new** QName(qName, method));

//设置调用方法的接口参数类型

call.addParameter(\"strXml\",

[]{#OLE_LINK63 .anchor}org.apache.axis.encoding.XMLType.*XSD\_STRING*,

javax.xml.rpc.ParameterMode.*IN*);

//设置接口方法的返回类型

call.setReturnType([]{#OLE_LINK64
.anchor}org.apache.axis.encoding.XMLType.*XSD\_STRING*);

根据请求参数获取返回值？？？？

String responseXml = (String)call.invoke(**new**
Object\[\]{requestXml});

**return** responseXml;

}**catch** ([]{#OLE_LINK65 .anchor}ServiceException e){

**throw** **new** BireportException(BireportException.*SELF\_INFO*,

**new** Object\[\]{e.getMessage()});

}**catch** (RemoteException e){

**throw** **new** BireportException(BireportException.*SELF\_INFO*,

**new** Object\[\]{\"连接合同接口失败: \" + e.getMessage()});

}

}

#### EAS WebService连接示例

// 根据连接配置，创建一个远程调用

public static org.apache.axis.client.Call
getRemoteCall(EasWsConnInfoInfo easConn)

throws BOSException, EASBizException

{

try{

org.apache.axis.client.Service service = new
org.apache.axis.client.Service();

org.apache.axis.client.Call call = (org.apache.axis.client.Call)
service.createCall();

//直接引用远程的wsdl文件

String ws\_login = easConn.getWsAddress()+\"/EASLogin?wsdl\";

call.setTargetEndpointAddress(ws\_login);

//设置调用方法，WSDL里面描述的接口方法名称

call.setOperationName(\"login\");

//设置调用方法的接口参数类型

call.removeAllParameters();

call.addParameter(\"userName\", XMLType.XSD\_STRING, ParameterMode.IN);

call.addParameter(\"password\", XMLType.XSD\_STRING, ParameterMode.IN);

call.addParameter(\"slnName\", XMLType.XSD\_STRING, ParameterMode.IN);

call.addParameter(\"dcName\", XMLType.XSD\_STRING, ParameterMode.IN);

call.addParameter(\"language\", XMLType.XSD\_STRING, ParameterMode.IN);

call.addParameter(\"dbType\", XMLType.XSD\_INT, ParameterMode.IN);

//设置接口方法的返回类型

call.setReturnType(new javax.xml.namespace.QName(\"urn:client\",
\"WSContext\"));

> //返回类

call.setReturnClass(WSContext.class);

call.setReturnQName(new javax.xml.namespace.QName(\"\",
\"loginReturn\"));

//准备本次方法调用的参数

> //设置不至于报错

String password =
(easConn.getPassword()==null?\"\":easConn.getPassword());

Object\[\] params = new Object\[\]{

easConn.getUserName(), password,

\"eas\", easConn.getDcNumber(), \"l2\",

easConn.getDatabaseType().getValue()

};

WSContext context = (WSContext) call.invoke(params);

if(context.getSessionId()==null)

throw new JIPBizException(JIPBizException.ERROR, new
Object\[\]{\"连接\"+easConn.getName()+\"时登陆失败\"});

return call;

}catch (RemoteException e) {

throw new BOSException(e);

}catch (ServiceException e) {

throw new BOSException(e);

}

}

// 注销WebService会话

public static void remoteLogout(org.apache.axis.client.Call call,
EasWsConnInfoInfo easConn)

{

try{

//直接引用远程的wsdl文件

String ws\_login = easConn.getWsAddress()+\"/EASLogin?wsdl\";

call.setTargetEndpointAddress(ws\_login);

//设置调用方法，WSDL里面描述的接口方法名称

call.setOperationName(\"logout\");

//设置调用方法的接口参数类型

call.removeAllParameters();

call.addParameter(\"userName\", XMLType.XSD\_STRING, ParameterMode.IN);

call.addParameter(\"slnName\", XMLType.XSD\_STRING, ParameterMode.IN);

call.addParameter(\"dcName\", XMLType.XSD\_STRING, ParameterMode.IN);

call.addParameter(\"language\", XMLType.XSD\_STRING, ParameterMode.IN);

//设置接口方法的返回类型

call.setReturnType(XMLType.XSD\_BOOLEAN);

//准备本次方法调用的参数

Object\[\] params = new Object\[\]{

easConn.getUserName(), \"eas\", easConn.getDcNumber(), \"l2\",

};

Boolean success = false;

success = (Boolean)call.invoke(params);

if(success.booleanValue())

System.out.println(\"logout from \" + ws\_login + \" successed.\");

else

System.out.println(\"logout from \" + ws\_login + \" failed.\");

}catch (RemoteException e) {

e.printStackTrace();

}

}

-   WSContext示例：

-   调用EAS WebService方法示例：

EasWsConnInfoInfo easConn = (EasWsConnInfoInfo)
params.get(\"EasWsConnInfoInfo\");

//模拟第三方通过WebService调用EAS接口

Call call = **null**;

**try**{

call = EasWebServiceHelper.*getRemoteCall*(easConn);

String address = easConn.getWsAddress()+\"/WSJsonFaceFacade?wsdl\";

//调用远程添加凭证方法

call.setTargetEndpointAddress(address);

> 设置要调用的方法

call.setOperationName(\"readJson\");

call.removeAllParameters();

call.addParameter(\"jBill\",
org.apache.axis.encoding.XMLType.*XSD\_STRING*,
javax.xml.rpc.ParameterMode.*IN*);

call.setReturnType(org.apache.axis.encoding.XMLType.*XSD\_STRING*);

String result = (String)call.invoke(**new** String\[\]{strJson});

**return** result;

}**catch** (RemoteException e) {

e.printStackTrace();

**throw** **new** JIPBizException(JIPBizException.*ERROR*, **new**
Object\[\]{\"需要连接\"+easConn.getName()+\"，但是无法连接所需的WEB服务\"});

}**finally**{

**if**(call!=**null**)

EasWebServiceHelper.*remoteLogout*(call, easConn);

}

#### HTTP连接示例

public String invokeHttp(String mapkey, String param) throws IOException

{

InputStream is = null;

OutputStream out = null;

try{

String uri = shccConfig.getDescription() + \"?random=\" + Math.random();

URL url = new URL(uri);

HttpURLConnection conn = (HttpURLConnection) url.openConnection();

conn.setRequestMethod(\"POST\");

conn.setDoInput(true);

conn.setDoOutput(true);

conn.setRequestProperty(\"Content-Type\",
\"application/json;charset=utf-8\");

conn.setReadTimeout(1000 \* 60 \* 3);

conn.setConnectTimeout(1000 \* 60 \* 3);

conn.setRequestProperty(\"Connection\", \"keep-alive\");

conn.setRequestProperty(\"mapkey\", mapkey);

out = conn.getOutputStream();

byte\[\] b = new byte\[1024\];

int size = 0;

out.write(param.getBytes(\"UTF-8\"));

out.flush();

out.close();

is = conn.getInputStream();

ByteArrayOutputStream ba = new ByteArrayOutputStream();

while ((size = is.read(b)) != -1)

ba.write(b, 0, size);

String result = new String(ba.toByteArray(), \"UTF-8\");

return result;

}finally{

if(is != null)

try{is.close();}catch (IOException e){e.printStackTrace();}

if(out != null)

try{out.close();}catch (IOException e){e.printStackTrace();}

}

}

#### EAS外部数据源

EAS的扩展报表平台集成有一个比较完善的外部数据库连接工具

![](media/media/image170.png){width="4.893055555555556in"
height="1.9784722222222222in"}

![](media/media/image171.png){width="6.411111111111111in"
height="3.2958333333333334in"}

-   列表界面：com.kingdee.eas.rpts.ctrlreport.client.OutDBCenterListUI

-   编辑界面：com.kingdee.eas.rpts.ctrlreport.client.OutDBCenterEditUI

-   连接配置表：T\_CTR\_ExtReportOutDB

-   数据连接工具类：com.kingdee.bos.ctrl.common.datacenter.DataCenterConnUtil

运行平台
--------

WebService方式搭建的接口，需要运行在一个中间件服务器中，中间件服务器可以选择：

-   EAS平台：和EAS服务集成在一起，可以方便的调用EAS平台的各种功能和业务模块。但是必须为外部系统调用服务提供专用的登录账号，会消耗EAS并发许可，调用前必须先调用login服务登录，调用完成后要调用logout注销，较为麻烦，适用于需要调用EAS业务模块、EAS平台组件的接口。

-   第三方平台开发和运行：使用第三方中间件独立搭建WebService接口，例如Tomcat，和EAS服务完全无关，仅在数据层和EAS集成。优点是开发成本较低、部署和调整方便，缺点是不能调用EAS强大的业务组件和业务逻辑实现。适用于简单的EAS数据输出接口。

接口内容
--------

-   对于数据库连接的数据交换，通常是给出数据字典即可。复杂的EAS数据，可在数据库层开发若干视图，把要集成的数据进行初步的集成和简化后提供给第三方。

-   对于Excel文件，双方需要约定数据的命名、类型、Excel文件样式。

-   对于WebService和很棒文件传递的接口，就需要约定的交换数据的内容格式。目前主流的内容格式技术有：XML、JSON，基于这两种技术，需要开发：

    -   对象格式化：把EAS对象转换为XML或JSON的方法

    -   对象反格式化：把XML或JSON数据转换为EAS对象的方法

### XML格式

可使用成熟的org.[]{#OLE_LINK66
.anchor}dom4j组件，完成XML文件或字符流到DOM对象的转换和读取。开发人员仍然需要开发EAS对象和DOM模型的转换解析功能。

用XML传递数据库结果集时，可以使用标准Java的javax.sql.rowset.WebRowSet

### XML开发示例

// 把一个功能调用命令封装成符合约定的XML查询请求

**public** **static** String getInvokeXml(String command,
[HashMap]{.underline} params)

{

Document document = DocumentHelper.*createDocument*();

Element root = document.addElement(\"invoke\");

root.addElement(\"command\").setText(command);

**if**(params!=**null**)

{

Element element\_datas = root.addElement(\"inputdata\");

> //回

**for**([Entry]{.underline} entry:
[(Set\<Entry\>)params.entrySet()]{.underline})

{

String key = entry.getKey().toString();

String value = \"\";

> 判断是否为空

**if**(entry.getValue()!=**null**)

> 赋值

value = entry.getValue().toString();

> 添加进文档中

element\_datas.addElement(key).setText(value);

}

}

将文件转换文String返回

**return** document.[]{#OLE_LINK81 .anchor}asXML();

}

// 执行WebService调用

**public** **static** String call(String url, String qName, String
method, String requestXml)

**throws** BOSException, EASBizException

{

**try**

{

org.apache.axis.client.Service service = **new** Service();

org.apache.axis.client.Call call = (Call) service.createCall();

//直接引用远程的[wsdl]{.underline}文件

String wsdlUrl = url + \"?wsdl\";

call.setTargetEndpointAddress(wsdlUrl);

//设置调用方法，WSDL里面描述的接口方法名称

call.setOperationName(**new** QName(qName, method));

//设置调用方法的接口参数类型

call.addParameter(\"strXml\", []{#OLE_LINK67
.anchor}org.apache.axis.encoding.XMLType.*XSD\_STRING*,
javax.xml.rpc.ParameterMode.*IN*);

//设置接口方法的返回类型

call.setReturnType(org.apache.axis.encoding.XMLType.*XSD\_STRING*);

> 返回结果

String responseXml = (String)call.invoke(**new**
Object\[\]{requestXml});

**return** responseXml;

}

**catch** (ServiceException e)

{

**throw** **new** BireportException(BireportException.*SELF\_INFO*,
**new** Object\[\]{e.getMessage()});

}

**catch** (RemoteException e)

{

**throw** **new** BireportException(BireportException.*SELF\_INFO*,
**new** Object\[\]{\"连接合同接口失败: \" + e.getMessage()});

}

}

// 执行远程SQL查询，返回结果集

**public** **static** WebRowSet query(String url, String qName, String
sql)

**throws** BOSException, EASBizException

{

String requestXml = *getQueryXml*(sql);

String responseXml = *call*(url, qName, \"query\", requestXml);

**if**(responseXml==**null**)

**throw** **new** BireportException(BireportException.*SELF\_INFO*,
**new** Object\[\]{\"合同接口查询错误: 未返回任何结果\"});

**try**

{

> 解析xml

Document document = DocumentHelper.*parseText*(responseXml);

Element root = document.getRootElement();

// 结果分析处理

**if**(root.element(\"exception\")==**null**)

{

Element element = root.element(\"webRowSet\");

**if**(element==**null**)

**throw** **new** BireportException(BireportException.*SELF\_INFO*,
**new** Object\[\]{\"合同接口查询错误: 未返回查询结果\"});

> //文档

Document tmp\_doc = DocumentHelper.*createDocument*();

tmp\_doc.setRootElement((Element)element.clone());

// Document转换为字符流, 从字符流解析得到WebRowSet

javax.sql.rowset.WebRowSet rowSet = **new**
com.sun.rowset.WebRowSetImpl();

rowSet.readXml(**new** StringReader(tmp\_doc.asXML()));

**return** rowSet;

}

**Else** // 转入异常处理

{

String errMsg = root.element(\"exception\").elementText(\"message\");

**throw** **new** BireportException(BireportException.*SELF\_INFO*,
**new** Object\[\]{\"合同接口查询错误: \" + errMsg});

}

}

**catch** (DocumentException e)

{

**throw** **new** BireportException(BireportException.*SELF\_INFO*,

**new** Object\[\]{\"解析返回结果时发生文档格式错误: \" +
e.getMessage()});

}

**catch** (SQLException e)

{

**throw** **new** BireportException(BireportException.*SELF\_INFO*,

**new** Object\[\]{\"解析返回结果时发生数据错误: \" + e.getMessage()});

}

}

// 执行远程功能调用，返回结果Map

**public** **static** [HashMap]{.underline} invoke(String url, String
qName, String command, [HashMap]{.underline} params)

**throws** BOSException, EASBizException

{

// 构造查询请求并调用服务

String requestXml = *getInvokeXml*(command, params);

String responseXml = *call*(url, qName, \"invoke\", requestXml);

**if**(responseXml==**null**)

**throw** **new** BireportException(BireportException.*SELF\_INFO*,
**new** Object\[\]{\"合同接口调用功能错误: 未返回任何结果\"});

**try**

{

Document document = DocumentHelper.*parseText*(responseXml);

Element root = document.getRootElement();

// 结果分析处理

**if**(root.element(\"exception\")==**null**)

{

Element element\_datas = root.element(\"outdata\");

[HashMap]{.underline} outdata = **new** [HashMap]{.underline}();

[]{#_Toc487979343 .anchor}Iterator\<Element\> iterator =
[element\_datas.elementIterator()]{.underline};

**while**(iterator.hasNext())

{

Element element = iterator.next();

String key = element.getName();

String value = element.getText();

[outdata.put(key, value)]{.underline};

}

**return** outdata;

}

// 转入异常处理

**else**

{

String errMsg = root.element(\"exception\").elementText(\"message\");

**throw** **new** BireportException(BireportException.*SELF\_INFO*,
**new** Object\[\]{\"合同接口执行功能错误: \" + errMsg});

}

}

**catch** (DocumentException e)

{

**throw** **new** BireportException(BireportException.*SELF\_INFO*,

**new** Object\[\]{\"解析返回结果时发生文档格式错误: \" +
e.getMessage()});

}

}

### Json格式

可使用成熟的org.json组件，完成JSON字符流到JSON对象的转换和读取。开发人员仍然需要开发EAS对象和JSON模型的转换解析功能。

BOS提供了com.kingdee.bos.json.JSONUtils工具类，对JSON开发提供了有限的支持。

### Json开发示例

// 构造一个JSon对象，将来转换为字符串向第三方输出

JSONObject result = **new** JSONObject();

// JSON加入一个普通的键值对

result.put(\"number\", \"001\");

// JSON加入一个数组对象

//JSON数组

JSONArray list = **new** JSONArray();

list.put(\"001\");

list.put(\"002\");

result.put(\"entry\", list);

// JSON加入另一个JSON对象（相当于加入一个map结构对象）

JSONObject params = **new** JSONObject();

params.put(\"project\", \"马钢接口\");

params.put(\"developer\", \"kingdee\");

params.put(\"user\", \"MaGang\");

result.put(\"params\", params);

// JSON对象转换为String

output = result.toString();

// 输入字符串转换为JSon对象

JSONObject input = **new** JSONObject(output);

// JSON对象获取键值对

String [number]{.underline} = input.getString(\"number\");

// JSON对象获取数组

JSONArray list2 = input.getJSONArray(\"entry\");

list2.getString(0);

// JSON对象获取JSON对象（相当于获取一个map结构对象）

JSONObject params2 = input.getJSONObject(\"params\");

String [project]{.underline} = params2.getString(\"project\");

String [developer]{.underline} = params2.getString(\"developer\");

String [user]{.underline} = params2.getString(\"user\");

### 数据格式转换

从接口接收的字符串数据，转换为正确的Java数据类型，开发人员可参考使用：

-   com.kingdee.bos.dao.ormapping.impl.ImplUtils

-   com.kingdee.util.TypeConversionUtils

基础数据体系
------------

通过异构系统传递数据的各方，对于交换数据所引用的基础数据的定义必须保持一致从而能够相互识别，例如客户供应商、物料、组织、人员等等。

### 基础数据映射

业务系统数据的集成必须以基础数据一致或可转换为前提。如果异构系统间的基础数据完全一致，或者可通过某种规则进行简单转换，那么可以省却本节步骤，否则必须通过基础数据映射表解决该问题。

开发者需要开发一张基础资料映射表业务单据，提供基本的数据维护、检查和权限控制，需要开发数据转换的基础层功能。为了方便用户使用可能需要提供Excel批量导入功能，有时甚至需要通过接口从第三方系统引入外部基础数据。

### 基础数据转换

外部系统接收的业务数据中，可能包含众多以字符串描述的基础数据（例如组织编码、人员编码、客户编码、物料编码、计量单位名称等等），在EAS中需要转换为对象或者对象ID，在转换前还需要检查其对应的基础数据是否存在。

开发人员可能为这些基础数据逐项开发检查和转换功能，但是当基础数据非常多时，例如：凭证、收付款、合同、订单等可能具有数十几个数据项的业务单据时，工作量就会变得很大。

如果开发通用数据转换功能，则需要注意有些基础数据会需要其它条件共同进行筛选。例如凭证科目，仅通过科目编码并不能唯一正确的找到对应的EAS数据，还必须通过财务组织进行筛选。

业务数据处理
------------

### 业务数据检查

接受的外部数据，检查其数据是否符合EAS业务要求；外部系统不能提供的但是EAS要求必须录入的数据如何计算补充

### 业务数据确认

分析EAS对数据的业务处理（保存、提交、审核或核准）要求及是否存在上下游关联业务的特殊要求，接受的外部数据如何满足EAS系统的这些要求，外部系统不能提供的部分，需要自己准确分析后进行补充处理

Excel导入导出
-------------

在EAS中表格数据右键导出为Excel是控件级功能，因此所有单据的列表界面和编辑界面表格都支持导出为Excel文件，所见即所得。因此EAS中通常不需要开发EAS导出Excel功能。

EAS也提供了基于Excel引入数据的平台级功能，即引入引出工具，但是该工具只能解决一部分业务需求，开发者还会经常遇到Excel数据引入EAS的开发。

### 业务及设计

在EAS中常见的Excel导入需求有：

-   基础数据的导入，例如：价格政策、客户区域关系、非标准业务的组织关系等等，这类数据结构通常比较简单，导入后直接保存到数据库，建议通过Bean来保存数据不要直接写数据库。

-   单据分录的导入，例如：合同资源清单、客户余额调整分录等等，这些数据通常在保存、审核时会存在导入后的用户确认、二次计算等等，并且后台存在各种检查校验。这类导入做方案时，建议把导入数据填充到单据分录表格中，不要直接保存，由用户自己执行单据的保存提交操作。

### Excel工具类

EAS和BOS开发环境已经集成了Excel的操作工具类，Excel2003及以前版本的工具类为：

-   org.apache.poi.hssf.usermodel.HSSFCell;

-   org.apache.poi.hssf.usermodel.HSSFRow;

-   org.apache.poi.hssf.usermodel.HSSFSheet;

-   org.apache.poi.hssf.usermodel.HSSFWorkbook;

Excel2007及以后版本的工具类为：

-   org.apache.poi.xssf.usermodel.XSSFCell;

-   org.apache.poi.xssf.usermodel.XSSFRow;

-   org.apache.poi.xssf.usermodel.XSSFSheet;

-   org.apache.poi.xssf.usermodel.XSSFWorkbook;

### Excel导入完整案例

该案例包包含：

-   从Excel2003、2007读取数据的工具类：Excel2003Util、Excel2007Util、ExcelUtils、FileFilterImpl

-   单据或基础资料导入数据的辅助类，提供直接以按钮挂到单据界面方法：ExcelDataImporter

-   利用辅助类完成单据和基础资料导入数据的具体案例：BudgetAdjustExcelImporter，PricePolicyExcelImporter

### Excel导入代码示例

**import** java.io.File;

**import** javax.swing.filechooser.FileFilter;

**public** **class** FileFilterImpl **extends** FileFilter

{

**protected** String ends;

**protected** String description;

**public** FileFilterImpl(String ends, String description)

{

**this**.ends = ends.toLowerCase(); // 设置文件后缀

**this**.description = description; // 设置文件描述文字

}

// 只显示符合扩展名的文件，目录全部显示

**public** **boolean** accept(File file)

{

**if** (file.isDirectory())

**return** **true**;

String fileName = file.getName();

**if** (fileName.toLowerCase().endsWith(**this**.ends))

**return** **true**;

**return** **false**;

}

**public** String getDescription()

{

**return** **this**.description;

}

**public** String getEnds()

{

**return** **this**.ends;

}

}

**public** **class** [Excel2003Util]{.underline} **implements**
Serializable, ExcelUtils {

**protected** HSSFWorkbook workBook = **null**;

**protected** HSSFSheet sheet = **null**;

**protected** **int** rowCount = 0;

**protected** **int** colCount = 0;

**protected** InputStream fis = **null**;

**private** [Excel2003Util()]{.underline} {}

**public** Excel2003Util(String fileName, String sheetName) **throws**
Exception

{

**if** (StringUtils.*isEmpty*(fileName))

**throw** **new** EASBizException(EASBizException.*CHECKBLANK*, **new**
Object\[\]{\"文件名称\"});

// 打开Excel文件

fis = **new** FileInputStream(**new** File(fileName));

workBook = **new** HSSFWorkbook(fis);

**if** (StringUtils.*isEmpty*(sheetName))

sheet = workBook.getSheetAt(0);

**else**

sheet = workBook.getSheet(sheetName);

**if** (sheet == **null**)

**throw** **new** EASBizException(EASBizException.*CHECKBLANK*, **new**
Object\[\]{\"Excel文件中的工作簿\"});

[]{#_Toc487979358 .anchor}// 计算行数和列数

rowCount = sheet.getLastRowNum() - sheet.getFirstRowNum() + 1;

**for**(**int** i=0; i\<rowCount && colCount\>0; i++)

{

**if** (sheet.getRow(i) != **null**)

colCount = sheet.getRow(i).getLastCellNum();

}

}

**public** String getCellData(**int** rowNum, **int** colNum)

{

**if** (rowNum\>=rowCount \|\| sheet.getRow(rowNum)==**null** \|\|
colNum\>=colCount)

**return** \"\";

HSSFRow row = sheet.getRow(rowNum);

HSSFCell cell = row.getCell(colNum);

**return** ExcelUtil.*getCellValue*(cell); //
Excel2003以下读取单元格数据

// return ExcelXUtil.getCellValue(cell); // Excel2007以上读取单元格数据

}

**public** **int** getRowCount()

{

**return** rowCount;

}

**public** **int** getColCount()

{

**return** colCount;

}

**public** **void** close() **throws** Exception

{

**try** {**if** (fis != **null**)fis.close();}

**catch** (Exception e) {}

}

}

// 导入Excel文件数据的方法

**public** **void** importData() **throws** Exception

{

editData = uiObj.editData;

// 选择Excel文件对话框

KDFileChooser choose = **new** KDFileChooser();

choose.addChoosableFileFilter(**new** FileFilterImpl(\".xls\",
\"excel97-2003(.xls)\"));

choose.addChoosableFileFilter(**new** FileFilterImpl(\".xlsx\",
\"excel(.xlsx)\"));

**int** result = choose.showOpenDialog(uiObj);

**if** (result != 0 \|\| choose.getSelectedFile() == **null**)

**return**;

[]{#_Toc487979359 .anchor}// 获取所选文件名称

String fileName = choose.getSelectedFile().getName();

ExcelUtils excelUtils = **null**;

**if**(fileName.endsWith(\".xls\"))

excelUtils = **new**
Excel2003Utils(choose.getSelectedFile().getAbsolutePath());

**else** **if**(fileName.endsWith(\".xlsx\"))

excelUtils = **new**
Excel2007Utils(choose.getSelectedFile().getAbsolutePath());

**else**

**throw** **new** XxglException(XxglException.ERROR,**new**
Object\[\]{\"只能打开Excel文件\"});

// 按行读取数据

**for** (**int** i = 1; i \< excelUtils.getRowCount(); i++)

{

......

// 读取每一列数据

**for** (**int** j = 0; j \< excelUtils.getColCount(); j++)

{

String value = excelUtils.getCellData(i, j);

......

}

}

}

关于EIP平台
-----------

EAS7.0及后续版本提供了一个接入外部数据的平台：EIP外部数据转换平台，其机制是外部数据先进入临时表，然后通过B
OTP转换生成所需的业务单据。在这过程中，基础资料映射和转换也是比不可少，该平台提供了基础数据映射关系管理工具。

EIP平台适合处理的业务：第三方数据在数据库层把数据提供给EAS，EAS定时读取形成EAS数据。可以几乎不做开发，通过实施配置就能把外部数据引入EAS。

目前该平台需要付费使用，开发顾问做接口时可参考该平台的设计方法和部分模块。

关于平台更多的技术资料请自行到Mykingdee或BOS开发者论坛中获取。

 EAS工作流
==========

总体介绍
--------

EAS的工作流系统包含了3部分：工作流设计工具，工作流运行引擎，工作流运行期管理工具。开发人员可参看EAS专门的工作流系统手册进行深入学习和研究，本章节从开发者的角度对工作流作快速介绍，达到快速简单应用的目的。

工作流中的几个概念：

-   工作流设计模型：开发人员进行工作流开发的成果，可能是未完工的模型；

-   工作流定义：EAS运行时真正投入使用的流程定义，工作流设计模型校验无错误，发布后会自动生成对应的工作流定义；

-   工作流实例：EAS单据提交后，如果符合工作流启动条件，会为此单据生成一个工作流实例，工作流实例和启动时的工作流定义的流程是一致的。

-   活动节点：工作流实例中，处于活动状态的节点；

-   审批结果：工作流流程的审批节点，审批人做出的审批意见和结果。

工作流的设计开发在BOS开发工具中完成，运行测试和监控维护在EAS客户端进行。BOS提供了"工作流连接"和"工作流编辑"两个透视图，用于建立到EAS服务器的连接，和进行工作流设计开发。工作流连接和编辑前，必须启动EAS应用服务器，部分版本的EAS必须启动BIM服务。

工作流的模型、定义、示例等等，全部保存在数据库中，和数据库帐套相关。

工作流模型设计开发
------------------

以设计一条常见的简单工作流为例，帮助学习者快速掌握常见工作流模型设计方法。关于过多知识和技能的深入学习，请参考总部标准文档。

以下仅说明常见开发注意事项

### 自动审核节点参与人

此自动节点是工作流引擎后台自动处理，调用节点绑定的单据功能（一般是单据审核功能），引擎会按照此处传递的参与人构造上下文中的当前用户变量。在单据审核的功能中，一般会加入如下代码，从上下文中获取当前用户，并设置为单据的审核人。

**protected** **void** \_audit(Context ctx, IObjectValue model,
IObjectPK pk) **throws** BOSException, EASBizException {

**if** (pk == **null**)

**hrow** **new** HeFeiBizException(HeFeiBizException.*NULL\_BILL\_ID*);

BizAcctAdjustBillInfo billInfo =
(BizAcctAdjustBillInfo)checkDBStatus(ctx, pk.toString(),
BillStatusEnum.*save*, **true**);

checkBillFields(ctx, billInfo);

billInfo.setAuditTime(**new** Date());

**billInfo.setAuditor((UserInfo)ctx.get(\"UserInfo\"));**

billInfo.setBaseStatus(BillStatusEnum.*audited*);

**this**.\_update(ctx, **new** ObjectUuidPK(billInfo.getId()),
billInfo);

writeBackAfterBillAudit(ctx, billInfo);

}

### 提交单据进入工作流

注意不要用user这类没有绑定职员的用户测试工作流，工作流引擎会抛出没有对应职员的异常，单据不会启动工作流实例。

注意：工作流设计的变更不会影响已经启动的工作流实例，如果希望单据按更新后的流程走，必须终止现有流程实例，重新提交单据重启启动工作流。

如果当前用户对应多个匹配的工作流定义，EAS会按照提交节点参与人的范围，自窄而宽的优先选择工作流。

工作流状态图
------------

在单据、消息中心、工作流管理等界面下，都可以通过相应的按钮，打开工作流（实例）的状态图，在状态图中常见的查询和管理操作有（受权限控制）

### 查看流程属性

对开发人员来说很重要**，这里可以看到流程中各种变量的值**，对于流程走向、执行的错误分析极为重要；另外可以对流程执行【挂起】【撤销挂起】【终止】操作；

### 错误日志

**对开发人员非常重要**，工作流引擎运行在服务端，流程执行过程中发生的异常无法反馈给客户端，只能通过日志记录进行分析。常见的如：自动节点执行功能代码时发生异常、活动没有参与人等等。

![](media/media/image173.png){width="5.15625in" height="5.1875in"}

![](media/media/image174.png){width="3.834722222222222in"
height="2.748611111111111in"}

![](media/media/image175.png){width="5.90625in"
height="2.9583333333333335in"}

![](media/media/image176.png){width="6.416666666666667in"
height="2.2916666666666665in"}

![](media/media/image177.png){width="6.416666666666667in"
height="3.90625in"}

单据审批界面
------------

![](media/media/image178.png){width="6.409722222222222in"
height="3.96875in"}

开发人员必须清楚：**单据的审批界面和单据界面是不同的界面对象**，系统首先是打开了审批处理界面（MultiApproveUI），然后又根据审批任务关联的单据打开了对应的单据UI（例如：TravelOrderBillEditUI），并嵌入到MultiApproveUI中。

注意：审批界面的工具栏并不是单据界面的工具栏，点击【提交】操作时，首先是执行了MultiApproveUI的提交操作，当操作传到服务端MultiApproveControllerBean后，其对应的\_submit方法会寻找单据对应的服务端ControlleanBean并调用\_submit(Context
ctx, IObjectValue model)方法

### 业务单据操作集成

EAS提供了接口，可以在审批界面工具栏集成单据UI的按钮。在单据EditUI中加入如下代码，把需要集成到审批界面的按钮加入返回结果即可。但是不推荐开发人员这么做！

public List mergeMultiApproveButton() {

List bnList = new ArrayList();

bnList.add(this.btnSave);

return bnList;

}

单据流程检查
------------

当单据提交进入工作流以后，除了流程的当前处理人在消息中心中对单据进行处理，应当禁止其他用户操作单据，例如对单据进行：保存、提交、删除、审核/反审核等。EAS系统本身没有提供这个逻辑的实现，因此开发人员需要自己增加。示例代码：

**public** **static** **void** checkBillWorkFlow(Context ctx, String
billId)

**throws** BOSException, EASBizException

{

**if**(StringUtils.*isEmpty*(billId)) **return**;

StringBuffer sql = **new** StringBuffer()

.append(\"select p.fstate from T\_WFR\_ProcInstBizObj pb \\n\")

.append(\"inner join T\_WFR\_ProcInst p on pb.fprocinstid=p.fprocinstid
\\n\")

.append(\"where pb.fbizobjid=\'\").append(billId)

.append(\"\' and p.fstate like \'open.%\' \\n\");

IRowSet rs = com.kingdee.eas.util.app.DbUtil.*executeQuery*(ctx,
sql.toString());

**if**(rs.size()\>0)

**throw** **new**
HeFeiBizException(HeFeiBizException.*BILL\_IN\_WORKFLOW*);

}

此方法可做成公共方法，在所有单据的业务方法中进行调用检查。

 EAS单据转换
============

EAS单据转换为ERP中不同业务单据按照业务流向进行串联提供了完整的平台，包括以下部分：

-   转换规则配置：配置上游业务单据到下游业务单据的转换规则，主要是：下游单据的数据转换和计算规则、可参与转换的上游单据条件、分组和汇总规则，转换过程控制参数等

-   转换关系记录：记录具有关联关系的上游单据和下游单据

-   转换引擎：按照预定义的转换规则和指定的上游单据，执行单据转换，生成下游单据

-   界面操作：用户可以执行的单据转换相关操作：关联生成、上查和下查

-   上下游业务检查和控制：该逻辑的实现由开发人员通过Java代码实现

BOTP业务案例
------------

### 案例及设计

ERP业务流中，上游业务一般都会对下游业务具有约束控制作用。本文以采购订单生成采购入库业务为例，这是最常见的业务案例代表：

-   7月1日2张已确认的采购订单

    -   单据001采购物料如下：

        -   行1：打印纸 100包 已入库0，未入库100

        -   行2：墨盒10个 已入库0，未入库10

    -   单据002采购物料如下：

        -   行1：鼠标20个 已入库0，未入库20

        -   行2：U盘20个 已入库0，未入库20

        -   行3：打印纸 50包 已入库0，未入库50

-   7月5日到货：打印纸20包，墨盒10个，U盘5个。库管员做采购入库单，选择"001单行1，001单行2，002单行2"，关联生成采购入库单，录入实际入库数量，保存提交并审核确认。

    -   在审核确认时，系统需要执行对采购订单的反写更新：

        -   单据001行1： 已入库20，未入库80

        -   单据001行2： 已入库10，未入库0

        -   单据002行2： 已入库5，未入库15

对于某些具有行状态的单据分录，由于单据001行2的未入库数量已经为0，即采购完成，因此行状态应当设为关闭。

-   在审核反写完成后，系统应当检查的被反写采购分录的执行数量："已入库数量"不能大于"数量"20，"未入库"不能小于"0"

<!-- -->

-   7月6日到货：打印纸50包，
    U盘15个。库管员做采购入库单，选择"002单行2，002单行3"关联生成采购入库单，录入实际入库数量，保存提交并审核确认。系统反写和检查逻辑同上，如果具有订单分录具有行状态，则应当设置002单行2、行3的状态为"关闭"

-   7月7日库管员发现7月5日录入的采购入库单数量填写错误，需要取消重做。库管员找到已审核的7月5日入库单，执行反审核。

    -   反审核仍然要反写采购订单并执行检查，但是数值必须取反。如果订单分录行状态是"关闭"则应当将其打开，一般是设置为"审核"

    -   反审核后，库管员修改、保存、提交、审核入库单。审核时执行反写和检查逻辑

-   7月10日到货：鼠标20个。库管员做采购入库单，选择"002单行1"关联生成采购入库单，录入实际入库数量，保存提交并审核确认。

    -   审核时执行的反写和检查逻辑同上

    -   截止现在002单所有行的入库全部完成，应当设置整张单据的状态为"已关闭"，表明采购订单以及全部执行完成。

> 该案例的开发设计中，有以下值得注意的问题：

### 反写和检查点

一般BOTP的关联反写和检查都放在目标单据的审核和反审核方法中，其含义是当下游业务确认时才执行反写和检查。

在某些应用中（极少），可能需要在保存的时候进行反写，删除时撤销反写，此时开发人员需要注意，因为单据的保存操作可以反复执行，必须解决重复反写的问题。

### 上下游关系获取

目标单据向源单反写和检查时，必须能够找到对应的源单据。EAS提供了[]{#OLE_LINK68
.anchor}T\_BOT\_Relation表记录源单和目标单关系，但是一般开发中，更倾向于使用单据自带的sourceBillID属性，该属性需要在BOTP转换规则中进行配置。

### 按分录控制

几乎很少会遇到纯单据到单据的关联生成，正如本案例，在ERP中更多遇到的是用户选择多张源单据同时下推生成目标单据，或者用户只选择一直单据的部分分录行下推目标单据。

因此在ERP中处理关联业务时，更多的是按明细分录行进行反写和检查。这也要求在记录上下游关系时，更重要的是记录上下游分录的关系。

### 分组合并的限制

EAS的BOTP平台提供了对下推生成的目标单据进行分组合并的功能，如果目标单据需要对源单进行反写控制，那么本文不建议使用合并功能，你无法把合并后的执行数据分拆到多个来源。

如果一定既要合并又要反写，那就需要用户和开发者共同确认一种分拆执行数据的策略，并且需要建立单据的核销关系表，以便下游业务取消（反审核）时能够正确的撤销已反写数据

### 反写和检查的顺序

在本案例的反写和检查设计中，本文先执【反写】行后执行【检查】，该方式前提是审核和反审核的代码执行必须处于数据库事务中。

按照常规思路，先检查后反写似乎更为合理并且效率更高（减少数据库操作）。但是EAS的应用通常是面向大型集团企业，很多业务都存在并发执行的可能性。先检查后执行就可能会产生数据错误，先反写后检查在逻辑上可以避免这种错误。

转换规则
--------

### 单头转换规则

![](media/media/image179.png){width="6.415972222222222in"
height="4.1125in"}

配置下游单据头字段的取数规则。

请注意，所有EAS单据都具有一个字段"原始单据ID/sourceBillID/FSourceBillID"，用来记录当前单据关联的来源单据。因此一般会为目标单据的"原始单据ID"字段配置BOTP公式，取来源单据的ID。

![](media/media/image180.png){width="6.4125in"
height="0.9111111111111111in"}

### 分录转换规则

配置下游单据分录的取数规则。下表中的一行表示来源单据分录的每一行分录，将会产生一行目标单据分录，如果此处配置N行则每一行来源分录将产生N行目标分录。

请注意，通常EAS开发中，目标单据的分录，都会增加字段"来源分录ID"用来记录当前分录关联的来源分录，需要配置BOTP公式取来源分录的ID。

![](media/media/image181.png){width="6.408333333333333in"
height="1.4222222222222223in"}

### 分组规则和数值合计

表示依据来源单据产生的目标单据和分录集合，按照指定的字段或字段组合进行分组合并；数值合计定义合并过程中哪些字段进行SUM操作。

![](media/media/image182.png){width="6.4118055555555555in"
height="1.775in"}

![](media/media/image183.png){width="6.408333333333333in"
height="1.7048611111111112in"}

### 规则过滤和单据过滤

定义能够参与单据转换的来源单据的过滤条件。

-   规则过滤：如果用户所选的单据集合中，存在不满足条件的单据或分录，则本次BOTP操作被禁止；

-   单据过滤：在EAS8.0以前的版本中，称为"数据过滤"，如果用户所选的单据集合中，存在不满足条件的单据或分录，则这些单据和分录会被筛除，剩下符合条件的单据和分录进行转换。

![](media/media/image184.png){width="6.414583333333334in"
height="3.040277777777778in"}

### BOTP公式平台

在目标单据的取数定义中，除了可以简单取来源单据的字段或者取固定值，还可以通过公式平台定义计算公式。

注意：公式语言中的语句需要以分号";"结尾，切换到"脚本查看"页签中如果存在中文，说明公式不正确。

![](media/media/image185.png){width="6.415277777777778in"
height="3.609722222222222in"}

-   支持常用的条件判断、加减乘除、逻辑判断等；

-   支持通过函数计算，系统提供了预置的常用函数，同时支持在BOS中用Java开发自定义的函数，自定义BOTP函数的方法请参考前面的章节《自定义BOTP函数》

![](media/media/image186.png){width="5.188194444444444in"
height="2.0104166666666665in"}

### 组织隔离

用户可以在各业务组织下创建单独所需要的BOTP规则。

在使用时，系统会加载"当前组织＋根组织"下的BOTP规则，其他组织的规则不可见。建议实施和开发人员配置规则时，尽量在根组织下配置，以便全集团可见可用。

转换关系记录
------------

> 源单据和通过BOTP创建的目标单据之间的关联关系，EAS本身提供了记录表如下：

-   系统BOTP关系表：T\_BOT\_Relation和T\_BOT\_RelationEntry

在很多场合下，例如：反写和检查、多业务环节的报表取数等，通过系统关系表取数需要花费的代码开销较大，本文建议通过下游单据的表头sourceBillID和分录增加的专门字段例如[]{#OLE_LINK69
.anchor}srcEntryID来记录上下游单据和分录的关联关系，减少代码和执行开销。

-   自建上下游关系：sourceBillId或srcEntryID

注意：由于系统关系表已经内置一些必要的索引，在某些数据量大的场合，可能基于系统关系表检索上下游关系比基于自建上下游关系检索的效率更高。建议必要时为自建上下游关系字段也建立索引。

界面操作
--------

所有业务单据的列表界面ListUI和编辑界面EditUI，都内置了以下操作：

-   【上查】：查询当前单据对应的来源业务单据

-   【下查】：查询当前单据已生成的下游业务单据。上查和下查都是基于T\_BOT\_Relation寻找上下游单据

-   【关联生成】：对当前所选单据执行创建下游单据的操作，会弹出对话框由用户选择想要创建的下游单据类型和使用的BOTP规则

![](media/media/image187.png){width="6.416666666666667in"
height="2.770138888888889in"}

![](media/media/image188.png){width="6.407638888888889in"
height="2.922222222222222in"}

![](media/media/image189.png){width="3.689583333333333in"
height="1.6777777777777778in"}

反写和检查控制
--------------

> 请参考前面章节中的《controllerbean.java------代码示例：\_audit》。
>
> 对其中的方法和注意事项进行说明：

### 方法事务属性

本文要求，所有涉及数据库数据修改的方法，哪怕方法内仅有一个数据库修改语句，但是由于存在被其它方法嵌套调用的可能，也必须保证方法具有事务属性，设置方法是在entity上把方法的事务属性设为Required。

### 源单数据更新

示例代码如下：

// 按分录反写来源项目计划分录及业务控制检查

ProjectReportEntryInfo entryInfo = **null**;

IProjectPlanEntry [iPlanEntry]{.underline} =
ProjectPlanEntryFactory.*getLocalInstance*(ctx);

String sql = \"update T\_PRJ\_ProjectPlanEntry set FIsReported=1,
FReportedManday=IsNull(FReportedManday,0)+? where FID=?\";

**for**(**int** i=0; i\<billInfo.getEntrys().size(); i++)

{

entryInfo = billInfo.getEntrys().get(i);

**if**(entryInfo.getSrcEntryID()==**null**)

**continue**;

// throw new EASBizException(EASBizException.CHECKBLANK, new Object\[\]{

> \"第\"+(i+1)+\"行分录不是BOTP生成的\"});

//用SQL反写（推荐）

com.kingdee.eas.util.app.DbUtil.*execute*(ctx, sql,

**new** Object\[\]{entryInfo.getManday(), entryInfo.getSrcEntryID()});

// 上游业务检查：累计汇报人天不能超过计划人天

String selSql = \"select FReportedManday, FManday from
T\_PRJ\_ProjectPlanEntry where FID=? and FReportedManday\>FManday\";

IRowSet rowSet = com.kingdee.eas.util.app.DbUtil.*executeQuery*(ctx,

selSql, **new** Object\[\]{entryInfo.getSrcEntryID()});

**try**

{

**if**(rowSet.next())

{

**throw** **new** EASBizException(EASBizException.*CHECKBLANK*,

**new**
Object\[\]{\"来源计划的累计汇报人天（\"+rowSet.getString(1)+\"）超出计划人天（\"+rowSet.getString(2)+\"）\"});

}

}

**catch** (SQLException e)

{

// 必须注意！！！异常必须抛出！！！

e.printStackTrace();

**throw** **new** BOSException(e);

}

}

}

代码调用BOTP平台
----------------

有些业务中，客户要求或者业务要求自动依据源单据下推目标单据，自动保存和处理目标单据，这时开发人员要在Java代码中自己调用BOTP引擎执行单据转换。开发人员需要：

-   获取需要转换的源单据

-   根据目标单据获取合适的BOTP规则

-   调用BOTP引擎，以参数形式传递源单和BOTP规则，执行单据转换

-   从转换结果中获取目标单据，执行业务处理。必要时需要在代码中调用BOTP平台功能保存上下游单据的关联关系

> 示例代码如下：

**public** **static** **void** createChargeBill(Context ctx, IObjectPK
pk, **boolean** isSave)

**throws** BOSException, EASBizException

{

ObjectUuidPK pk2 = **new** ObjectUuidPK(pk.toString());

// 获取源单值对象

IObjectValue model = **null**;

调用代码账单控制器

CoreBillBaseController controller =
(CoreBillBaseController)EJBFactory.*getBusinessController*(ctx,
pk2.getObjectType());

**try** {

> 获取员账单基础集合

CoreBillBaseCollection coll = controller.getCoreBillBaseCollection(ctx);

**if**(coll.size()\>0)

model = coll.getObject(0);

**else**

**throw** **new**
HeFeiBizException(HeFeiBizException.*ERROR\_ON\_METHOD*, **new**
Object\[\] {\"创建预算台账记账单\", \"源单已经被删除\"});

[]{#_Toc487979393 .anchor}} catch (RemoteException e) {

**throw** **new** BOSException(e);

}

// 获取可用的BOTP规则

BOTMappingInfo mapping = BOTMappingHelper.*getMapping*(ctx, model,
\"3C185590\", **null**);

[]{#_Toc487979394 .anchor}// 获取BOTP引擎服务实例

IBTPManager ibtpManager = BTPManagerFactory.*getLocalInstance*(ctx);

[]{#_Toc487979395 .anchor}// 执行BOTP转换

BTPTransformResult btpResult =
ibtpManager.transform((CoreBillBaseInfo)model, mapping);

// 获取转换结果

新集合

IObjectCollection destCol = btpResult.getBills();

预算转变表

BudgetChargeBillInfo chargeBill =
(BudgetChargeBillInfo)destCol.getObject(0);

[]{#_Toc487979396 .anchor}// 保存生成的目标单据及BOTP关联关系

ibtpManager.saveRelations(chargeBill,
btpResult.getBOTRelationCollection());

}

 EAS扩展报表
============

> EAS扩展报表菜单：

-   ~~商业分析------扩展报表中心------报表平台------报表工具~~

-   商业分析------其他报表工具------报表服务平台------扩展报表

数据集和扩展报表按照组织进行隔离。开发人员在报表中心增加的数据集和扩展报表，保存时取当前组织作为所属组织，未来如果在其他组织下进入报表中心将看不到这些数据集和扩展报表。

由于扩展报表本身已经具有子系统树，可以按系统设计和保存报表。按组织隔离将会导致难以找到过去开发或者别人开发的报表，因此本文建议，**所有扩展报表开发，默认都在根组织下进行**。

开发方法概述
------------

### 报表开发步骤

![](media/media/image190.png){width="6.4125in"
height="2.720138888888889in"}

-   切换到根组织，进入扩展报表开发界面，在左侧选取合适的子系统路径

-   在"SQL数据集"目录下，增加报表所需的所有数据源定义

-   在"扩展报表"目录下，设计报表界面

### 数据源设计方法

金蝶扩展报表UI设计器提供了如：Group、Sum、Select等一系列强大的公式，可以在UI中实现对数据集进行分组统计、多数据源拼接等功能。因此对于很多复杂的数据源，开发者就不需要追求在SQL数据集中一次性加工完成。

对于来源多个业务系统的性质差异很大的数据，可以分为多个数据源，然后在UI界面中用公式进行拼接；对于需要汇总的数据，也可以利用UI界面的汇总公式辅助完成。

![](media/media/image191.png){width="6.4118055555555555in"
height="2.875in"}

SQL数据集开发
-------------

### 参数设计

参数是最终用户通过报表查询数据时，点击【新增数据集】，切换到"参数"页签，为数据源增加参数。

各类型参数的控件类型、设置及其它简单属性请开发者自己理解和尝试。

参数设置好以后，可以点击【预览】看一下运行时界面。

![](media/media/image192.png){width="6.4125in"
height="3.167361111111111in"}

### SQL设计

切换到"查询"页签，勾选"自定义查询"，直接写K-SQL语句

![](media/media/image193.png){width="6.413888888888889in"
height="3.5055555555555555in"}

-   SQL里引用参数，需要在参数名称前加@

-   日期型参数引入SQL，应当符合KSQL的日期语法格式

### 预览

> 点击【预览】，输入参数，可查看执行结果

![](media/media/image194.png){width="6.409027777777778in"
height="2.6118055555555557in"}

点击【当前执行SQL】可以查看经过参数拼接后的实际执行SQL。

### 组织范围控制

最终用户使用报表查询数据时，应当按照用户的组织权限进行范围隔离。例如：员工统计表具有"所属组织"参数，是报表主业务组织数据，该参数一定是必填项。那么当A部门经理查询员工时，应当控制其不能选择没有权限的B、C、D......组织。

常用的解决方法是：

-   为行政组织单独开发一个按当前用户范围获取可用组织的数据源

![](media/media/image195.png){width="6.410416666666666in"
height="1.4180555555555556in"}

> []{#_Toc487979406 .anchor}SELECT FID, FName\_l2, FNumber, FLongNumber
>
> FROM T\_Org\_Admin org
>
> where FName\_l2 like \'%@name%\' and FNumber like \'%@number%\'
>
> and []{#OLE_LINK70 .anchor}exists (select 1 from T\_PM\_OrgRange r
>
> where r.FUserID=\'@ExtRptCurrentUserInfoID\' and org.FID=r.FOrgID)
>
> Order by FNumber

-   员工统计表的"所属组织F7"使用"SQL数据集"类型，数据源设为上一步开发的SQL数据集

![](media/media/image196.png){width="6.410416666666666in"
height="2.15625in"}

### 参数的关联控制

### 自定义参数插件

有些场合下，报表界面的多个参数间具有更为复杂细致的联动要求，这是需要开发独立的参数插件Java类。开发者可以参考总部提供的参数插件开发文档和示例。

Java数据源
----------

EAS中某些业务的数据存在动态表、动态列的情形，例如员工薪酬、生产成本等，这些表无法使用静态SQL获取所需数据，EAS为开发者提供了执行[]{#OLE_LINK71
.anchor}存储过程返回结果、代码返回SQL或数据集的方法。新建存储过程的方法开发者可自行结合存储过程的相关知识进行研究学习，本节介绍Java数据集的开发方法。

### 新增数据源定义

![](media/media/image198.png){width="6.410416666666666in"
height="3.196527777777778in"}

![](media/media/image199.png){width="6.410416666666666in"
height="1.2416666666666667in"}

-   配置提供SQL语句或结果集的Java类全路径

-   设置好数据源所需的查询参数，点击预览，如果执行正确就能够看到数据集以及得到输出字段

### 开发Java数据源

请参考总部给出的文档：

[]{#_1561268271 .anchor}

示例代码（com.kingdee.eas.fm.liquid.client.StockAnalysisDataSet）：

**public** **class** StockAnalysisDataSet **extends**
AbstractJavaDataSet

{

**public** IRowSet\[\] getCustomRowSet(Window parent, String
otherDataCenter) **throws** Exception

{

[Map]{.underline} filter = **new** [HashMap]{.underline}();

[filter.put(\"queryDate\",
**this**.filterParamMap.get(\"queryDate\"))]{.underline};

**if** (**this**.filterParamMap.get(\"parentCompanyId\") != **null**)

[filter.put(\"parentCompanyId\",
(String)**this**.filterParamMap.get(\"parentCompanyId\"))]{.underline};

**if**
(![(FMHelper.~~isEmpty~~(**this**.filterParamMap.get(\"queryCycle\")))]{.underline})

[filter.put(\"queryCycle\",
(String)**this**.filterParamMap.get(\"queryCycle\"))]{.underline};

IRowSet irs =
FundStockFacadeFactory.*getRemoteInstance*().getStockAnalysis(filter);

**return** **new** IRowSet\[\]{irs};

}

**public** [Map]{.underline} getOutputParam() **throws** Exception

{

[HashMap]{.underline} outputParamMap = **new** [HashMap]{.underline}();

[outputParamMap.put(\"count\", \"2\")]{.underline};

[outputParamMap.put(\"pi\", \"3.14159\")]{.underline};

[outputParamMap.put(\"dateFrom\", \"2009-09-09\")]{.underline};

[outputParamMap.put(\"dateTimeFrom\", \"2009-09-09
09:09:09\")]{.underline};

[outputParamMap.put(\"timeFrom\", \"09:09:09\")]{.underline};

**return** outputParamMap;

}

}

报表界面
--------

> 扩展报表界面核心是通过大量的公式进行取数、计算、样式控制。

第一次接触扩展报表的开发者，请使用报表向导增加一些简单的列表型、分组汇总型、交叉分析型的报表，观察、学习、尝试报表公式的使用方法。

金蝶总部提供了丰富的扩展报表设计开发文档，开发者可以下载学习。

下面介绍扩展报表可以实现的核心功能：

-   向导功能：新建扩展报表，点击菜单"文件------新建报表向导"

-   分组统计：Group公式用于对数据源数据进行分组，统计函数用于数据统计分析

-   多数据源：一张扩展报表可包含多个数据源，多个数据源可以用于

    -   生成动态列

    -   多业务数据拼接成一张完整的报表

-   报表联查：设置某个单元格点击后联查其他报表或业务单据，通常用于"汇总表------明细表------业务单据"这样一个报表穿透查询体系

-   发布和权限控制：做好的扩展报表可以发布到EAS主菜单，并且设置报表的查询、打印权限

![](media/media/image201.png){width="6.409722222222222in"
height="3.1569444444444446in"}

 EAS基础数据
============

组织
----

EAS组织管理模块的系统主菜单路径：【基础数据管理】【组织架构】【组织单元】。

组织的元数据：com.kingdee.eas.basedata.org.app.FullOrgUnit，数据库表：T\_ORG\_BaseUnit。

### 管理单元（CU）

管理单元的元数据：com.kingdee.eas.basedata.org.app.CtrlUnit，数据库表：[]{#OLE_LINK72
.anchor}T\_ORG\_CtrlUnit

EAS管理单元维护需要用Administrator登录，系统主菜单路径：【基础数据管理】【组织架构】【管理单元】。

管理单元是一种特殊的组织，提供对基础资料数据、业务单据数据的逻辑隔离。默认情况下，不同的管理单元的数据，在EAS客户端相互间不可见。对于大型集团公司，实施顾问一般会把整个集团公司作为根级CU，各个分子公司作为下级CU，整个CU是一个树状多级数据结构。

EAS模型（单据和基础资料）的实体一般都是从ObjectBase实体集成，ObjectBase实体中有一个名称为
cu 的属性，对应的数据库字段是
FControlUnitID，记录了数据所属的管理单元。EAS运行时，单据和基础资料的管理单元的赋值由系统完成。在单据和基础资料的列表界面中，系统提供了按管理单元隔离数据的方法，观察ListUI.class的方法getDefaultCUFilter（EAS8.0之前）：

***protected** **final** FilterInfo getDefaultCUFilter(**boolean**
isIgnore)*

*{*

*......*

*filter.getFilterItems().add(**new** FilterItemInfo(\"CU.id\",
SysContext.getSysContext().getCurrentCtrlUnit().getId().toString(),
CompareType.EQUALS));*

*......*

*}*

可以看到所有列表UI的基类已经实现了按CU过滤数据的功能。对于一些系统公共的基础资料数据并不需要按CU过滤，例如：价格类型、销售类型、业务类型等等，可以覆盖重写此方法。或者重写isIgnoreCUFilter方法去除管理单元过滤：

***protected boolean isIgnoreCUFilter()***

***{***

***return false;***

***}***

### 业务组织

大型企业会按职责和业务范围划分很多职能部门，例如办公室、财务部、人力资源部、采购部、销售部、生产部等等，EAS中为对这些部门赋予相应的业务属性，财务部具有财务业务属性，采购部具有采购业务属性，销售部具有销售业务属性等等。相应的，EAS的组织基础资料就具有各种业务属性，这和小型软件中单一的行政组织架构有着很大的区别。

组织的业务属性是有区别的，下图是EAS的行政组织、财务组织属性和库存组织属性

![](media/media/image202.png){width="5.791666666666667in"
height="2.5694444444444446in"}

![](media/media/image203.png){width="5.789583333333334in"
height="1.6298611111111112in"}

![](media/media/image204.png){width="5.790972222222222in"
height="1.00625in"}

各业务组织的上下级关系体系是独立的，例如财务组织上下级关系体系和行政组织上下级关系体系是两个不同体系的关系划分。

存在这种情形，一个部门具有多种业务属性，例如设一个独立的行政部门"物资部"，既管采购又管库存，这样物资部就具有采购组织、库存组织、行政组织多种业务属性。

EAS中业务组织及实体定义：

  -------------- ------------------------------------------------------ ----------------------
  **业务组织**   **实 体**                                              **数据库表**
  行政组织单元   com.kingdee.eas.basedata.org.app.AdminOrgUnit          T\_ORG\_Admin
  财务组织单元   com.kingdee.eas.basedata.org.app.CompanyOrgUnit        T\_ORG\_Company
  HR组织单元     com.kingdee.eas.basedata.org.app.HROrgUnit             T\_ORG\_HRO
  销售组织单元   com.kingdee.eas.basedata.org.app.SaleOrgUnit           T\_ORG\_Sale
  库存组织单元   com.kingdee.eas.basedata.org.app.StorageOrgUnit        T\_ORG\_Storage
  采购组织单元   com.kingdee.eas.basedata.org.app.PurchaseOrgUnit       T\_ORG\_Purchase
  成本中心       com.kingdee.eas.basedata.org.app.CostCenterOrgUnit     T\_ORG\_CostCenter
  利润中心       com.kingdee.eas.basedata.org.app.ProfitCenterOrgUnit   T\_ORG\_ProfitCenter
  质检组织       com.kingdee.eas.basedata.org.app.QualityOrgUnit        T\_ORG\_Quality
  -------------- ------------------------------------------------------ ----------------------

#### 单据的组织隔离

EAS80框架生成的ListUI抽象类会自动添加按用户组织范围隔离的过滤条件，可以满足绝大部分单据的隔离需求。新建一个销售业务单据并发布，观察ListUI抽象类方法

***protected** FilterInfo getDefaultFilterForQuery()*

*{*

*......*

*FilterInfo otherFilter =
com.kingdee.eas.framework.FrameWorkUtils.getF7FilterInfoByAuthorizedOrg(com.kingdee.eas.basedata.org.OrgType.getEnum(\"Sale\"),\"saleOrgUnit.id\",**true**);*

***if** (otherFilter != **null**) {*

> *......*
>
> *filter.mergeFilter(otherFilter, \"AND\");*
>
> *......*

*}*

***return** filter;*

*}*

#### 新增单据获取主业务组织

EAS80框架生成的EditUI抽象类会自动添加按当前单据主业务组织属性获取业务组织的方法，可以满足绝大部分单据的隔离需求。示例代码（获取财务组织）：

**protected** com.kingdee.bos.dao.IObjectValue createNewData()

{

......

**if**
(com.kingdee.eas.common.client.SysContext.getSysContext().getCurrentOrgUnit(com.kingdee.eas.basedata.org.OrgType.getEnum(\"Company\"))
!= **null** &&
com.kingdee.eas.common.client.SysContext.getSysContext().getCurrentOrgUnit(com.kingdee.eas.basedata.org.OrgType.getEnum(\"Company\")).getBoolean(\"isBizUnit\"))//是否实体组织

objectValue.put(\"company\",com.kingdee.eas.common.client.SysContext.getSysContext().getCurrentOrgUnit(com.kingdee.eas.basedata.org.OrgType.getEnum(\"Company\")));

......

**return** objectValue;

}

可以简化为：

**protected** com.kingdee.bos.dao.IObjectValue createNewData()

{

......

OrgUnitInfo company = SysContext.getSysContext().getCurrentFIUnit();

if (company != null)

[]{#OLE_LINK73 .anchor}billInfo.setCompany(company);

return objectValue;

......

}

### 实体组织和虚体组织

业务组织分为（示例：A分公司及其下属的财务部和采购部）：

-   实体组织：是真实执行相应业务职能的部门，例如：A分公司下的财务部是实体财务组织，B分公司下的采购部是实体采购组织......；

-   虚体组织是实体组织之上（上级），从外部看也具有业务职能，但是执行者不是其自身，而是其下级组织；例如：A分公司具有财务业务和采购业务，但是具体执行是财务部和采购部，"A分公司"这个组织并不做具体业务，因此是虚体财务组织和虚体采购组织。

EAS中虚体组织往往位于实体业务组织上级，常用于做各业务部门数据的统计分析。一般实际业务处理在实体业务组织下进行，属性isBizUnit标识组织是否实体组织。

#### 新增单据限制实体组织

一般情形下，应当限制新增单据的主业务组织必须是实体组织，可以在EditUI的createNewData()方法中增加检查，示例：

**protected** com.kingdee.bos.dao.IObjectValue createNewData()

{

......

CompanyOrgUnitInfo companyOrg =
SysContext.getSysContext().getCurrentFIUnit();

**if**(companyOrg==**null** \|\| !companyOrg.isIsBizUnit())

{

MsgBox.showError(\"请切换到实体财务组织下增加单据\");

SysUtil.abort();

}

......

}

### 组织委托关系

企业经营管理中，既有业务和职能的划分，又存在相互间的协作，例如一个完整的采购流程，需要的业务环节有：采购、收货、验收、入库、付款、入账，这些环节涉及到不同的业务和部门，这时需要明确某个业务在下一个环节的流向（部门），以下图为例（黑色是行政关系，红色是资金流，蓝色是物流）：

EAS中组织间的这些协作关系，以组织委托关系的形式进行记录。EAS组织委托关系是在组织单元的业务属性中定义，在【基础数据管理】【组织架构】【全局委托关系】中可以统一查询。

设置组织委托关系：在组织基础资料的业务属性卡里设置，如下图：

![](media/media/image205.png){width="6.417361111111111in"
height="3.2729166666666667in"}

-   组织委托关系元数据：com.kingdee.eas.basedata.org.app.OrgUnitRelation

-   数据库表：T\_ORG\_UnitRelation。

![](media/media/image206.png){width="6.415277777777778in"
height="2.558333333333333in"}

开发人员做跨部门业务系统模块时，应当了解和遵循这种委托关系。例如销售订单，订单有发货组织和仓库字段，一般需要根据订单的销售组织，找到委托的库存组织，以此作为默认值进行填写，用户也可以自行修改。这种委托关系在有些业务中是强控的，在另外一些业务中可能是不控制的，需要视具体需求分析确定。

一个默认的规则是：企业各种业务处理需要在相应的业务组织下进行，例如销售订单只能在销售组织而不是库存组织下进行新增和维护。也有例外，有的模块为了用户处理方便，提供了自动从当前组织（依据委托关系）自动寻找对应的业务组织的功能。

#### 获取委托到当前组织的来源组织

-   示例：已知当前财务组织ID，获取委托到当前组织的销售组织

[[]{#OLE_LINK13 .anchor}]{#OLE_LINK12 .anchor}OrgUnitCollection
collection = OrgUnitRelationFactory.getLocalInstance(ctx).getFromUnit(

toOrgUnitId, OrgType.COMPANY\_VALUE, OrgType.SALE\_VALUE);

#### 获取当前组织的委托目标组织

-   示例：已知当前销售组织ID，取财务委托的目标组织

OrgUnitCollection collection =
OrgUnitRelationFactory.getLocalInstance(ctx).getToUnit(

fromOrgUnitId, OrgType.SALE\_VALUE, OrgType.COMPANY\_VALUE);

[]{#_Toc325093741 .anchor}

用户
----

![](media/media/image207.png){width="6.415277777777778in"
height="3.16875in"}

### 用户类型

EAS用户和人员是两个不同的概念和对象。EAS用户分为如下几种类型：

-   职员用户：用户账号必须和一个职员进行关联；

-   客户用户：用户账号必须和一个客户进行关联；

-   供应商用户：用户账号必须和一个供应商进行关联；

-   系统管理员：账号所有系统管理权限，但是不具有业务权限；

-   其他用户：账户不和上述其他对象管理。

### 缺省组织

决定了用户登录EAS后，默认所在的组织

### 用户组织范围

![](media/media/image208.png){width="6.407638888888889in"
height="1.8979166666666667in"}

![](media/media/image209.png){width="5.238888888888889in"
height="2.1333333333333333in"}

表示企业中某个特定用户具有业务执行和查看权限的组织范围，其作用体现：

-   用户首先需要分配组织范围，然后才能在各组织下分配具体的功能权限

-   用户组织范围决定用户在EAS中能够切换和进入哪些业务组织

[]{#OLE_LINK74
.anchor}用户组织范围元数据com.kingdee.eas.base.permission.OrgRange，数据表T\_PM\_OrgRange

通常在做扩展报表时，开发人员需要依据T\_PM\_OrgRange限定所取数据的组织范围，或者在报表过滤界面中可选择的组织范围。

### 用户功能权限

EAS的功能权限是三维的：组织+权限项+用户

![](media/media/image210.png){width="4.164583333333334in"
height="2.839583333333333in"}

分配权限时需要注意"组织"，权限项有业务属性，如果权限项的业务属性和组织的业务属性不一致，那么在"可授权"的权限项里将看不到该权限项。

用户权限的其它常用分配方法：

-   批量分配和取消权限

-   增加角色，为角色分配权限项，然后为用户分配角色

-   数据授权：权限项需要支持数据授权，然后在"安全管理------权限管理------授权规则"里设置数据权限规则，然后在权限分配的数据授权里添加规则。更多使用方法请参考相关文档

EAS职员和职位
-------------

-   [[[]{#OLE_LINK16 .anchor}]{#OLE_LINK15 .anchor}]{#OLE_LINK14
    .anchor}职员元数据和表：com.kingdee.eas.basedata.person.Person，T\_BD\_Person

-   职位元数据和表：com.kingdee.eas.basedata.org.Position，T\_ORG\_Position

-   职员和职位关系表：com.kingdee.eas.basedata.org.PositionMember，T\_ORG\_PositionMember

EAS中的人员基础信息中没有所属部门。实施人员会为人员分配职位，每个职位有所属部门。一个人员可能会有多个职位，其中有且仅有一个职位是主要职位。一般来说，开发人员可以根据人员的主要职位的所在部门确定人员所属部门。

select p.fname\_l2, p.fnumber, org.FNumber, org.FName\_l2

from T\_BD\_Person p

inner join T\_ORG\_PositionMember pm on pm.FPersonID=p.FID and
pm.FIsPrimary=1

inner join T\_ORG\_Position pos on pm.FPositionID=pos.FID

inner join t\_org\_admin org on pos.FAdminOrgUnitID=org.FID

 物料和客商
-----------

### 基本信息

-   物料元数据：com.kingdee.eas.basedata.master.material.app.Material，数据表：T\_BD\_Material

-   客户元数据：com.kingdee.eas.basedata.master.cssp.app.Customer，数据表：T\_BD\_Customer

-   供应商元数据：com.kingdee.eas.basedata.master.cssp.app.Supplier，数据表：T\_BD\_Supplier

![](media/media/image211.png){width="5.058333333333334in"
height="4.136805555555555in"}

### 多标准分类

物料和客商可以按照基本分类进行多级分类，此外还可以自定义新的分类标准，对已有的物料和客商进行多种标准分类。例如客户基础资料，用户一般会按照所在地域分类，也可能需要按照注册资金规模分类、按照经济性质分类、按照合作关系分类等等，这样在后期对业务数据进行统计分析时，能够按照各种分类标准进行统计。

-   [[]{#OLE_LINK17 .anchor}]{#OLE_LINK18
    .anchor}物料分类标准：com.kingdee.eas.basedata.master.material.MaterialGroupStandard，T\_BD\_MaterialGroupStandard

-   物料分类类目：com.kingdee.eas.basedata.master.material.MaterialGroup，T\_BD\_MaterialGroup

-   物料分类明细：com.kingdee.eas.basedata.master.material.MaterialGroupDetial，T\_BD\_MaterialGroupDetial

-   [[[[]{#OLE_LINK19 .anchor}]{#OLE_LINK20 .anchor}]{#OLE_LINK22
    .anchor}]{#OLE_LINK21
    .anchor}客户供应商分类标准：com.kingdee.eas.basedata.master.cssp.CSSPGroupStandard，T\_BD\_CSSPGroupStandard

-   客户供应商分类类目：com.kingdee.eas.basedata.master.cssp.CSSPGroup，T\_BD\_CSSPGroup

-   []{#OLE_LINK23
    .anchor}客户供分类明细：com.kingdee.eas.basedata.master.cssp.CustomerGroupDetail，T\_BD\_CustomerGroupDetail

-   供应商分类明细：com.kingdee.eas.basedata.master.cssp.SupplierGroupDetail，T\_BD\_SupplierGroupDetail

### 多业务属性

物料和客商除了基本的信息以外，在不同的业务中还具有相应的属性，例如物料，除了物料自有属性，当物料应用在库存业务中具有例如安全库存、库存上限、保质期等，当用于销售业务中时具有参考价格、税种税率等，这些属性针对不同的物料、不同的业务组织，设置也可能不相同。开发人员应当熟悉物料和客商大约具有的各种业务属性，在实际开发工作中进行灵活应用。

![](media/media/image212.png){width="6.410416666666666in"
height="2.922222222222222in"}

![](media/media/image213.png){width="5.2375in"
height="2.296527777777778in"}

![](media/media/image214.png){width="5.466666666666667in"
height="1.8104166666666666in"}

![](media/media/image215.png){width="5.509027777777778in"
height="2.7243055555555555in"}

### 组织隔离和共享

物料和客商相对于普通的基础资料来说，有个重要的功能，用户能够维护和管理物料客商的共享范围，用户可以在某个CU中建立基础资料，然后分配到其他CU，再为CU中的各业务组织分配基础资料。

一般认为，在物料客商的各业务属性页签中，如果维护了某个组织的业务属性并且启用，则该物料客商对于该组织可用，开发人员引用基础资料并做组织范围限定时，应当遵循这些设置和规则。常用物料客商业务属性元数据和表如下：

-   物料财务属性：com.kingdee.eas.basedata.master.material.MaterialCompanyInfo，T\_BD\_MaterialCompanyInfo

-   物料采购属性：com.kingdee.eas.basedata.master.material.MaterialPurchasing，T\_BD\_MaterialPurchasing

-   物料销售属性：com.kingdee.eas.basedata.master.material.MaterialSales，T\_BD\_MaterialSales

-   物料库存属性：com.kingdee.eas.basedata.master.material.MaterialInventory，T\_BD\_MaterialInventory

-   客户财务属性：com.kingdee.eas.basedata.master.cssp.CustomerCompanyInfo，T\_BD\_CustomerCompanyInfo

-   客户销售属性：com.kingdee.eas.basedata.master.cssp.CustomerSaleInfo，T\_BD\_CustomerSaleInfo

-   供应商财务属性：com.kingdee.eas.basedata.master.cssp.SupplierCompanyInfo，T\_BD\_SupplierCompanyInfo

-   供应商采购属性：com.kingdee.eas.basedata.master.cssp.SupplierPurchaseInfo，T\_BD\_SupplierPurchaseInfo

### 物料计量单位

> EAS中每个物料可用的计量单位及其转换系数，有专门的定义。

![](media/media/image216.png){width="5.065972222222222in"
height="2.526388888888889in"}

开发人员做涉及物料计量单位控制及数量转换时，应当遵循该定义。

-   计量单位元数据及表：com.kingdee.eas.basedata.assistant.MeasureUnit，T\_BD\_MeasureUnit

-   物料计量单位元数据及表：com.kingdee.eas.basedata.master.material.MultiMeasureUnit，T\_BD\_MultiMeasureUnit

### 物料辅助属性

辅助属性用于细分物料类型。在大型企业ERP系统中，物料是一个核心数据，在财务、进销存、生产等非常多的业务中会引用到。如何划分物料需要综合各业务环节需求，例如：

-   财务中需要设置"计算机"物料核算企业"计算机"每年的采购、销售金额；

-   对于采购业务来说，"计算机"显然过于泛泛，可能需要更为明细的物料设置，例如划分为"笔记本计"、"台式机"、"服务器"、"PC"等等

-   如果是一家PC销售企业，对于销售业务来说，还需要更为明细的物料划分，例如"DELL笔记本"、"联想台式机"、"IBM3300服务器"等等

> 如果物料设置过于明细，那么对于财务、采购来说就非常冗杂，做报表分析会很麻烦。

辅助属性提供了一种在物料设置之外的类型细分方法（也可以理解为规格型号），以平衡企业各业务环节的物料设置需求。

![](media/media/image217.png){width="5.561805555555556in"
height="3.276388888888889in"}

-   辅助属性元数据及表：com.kingdee.eas.basedata.master.material.AsstAttrValue，T\_BD\_AsstAttrValue

-   物料辅助属性元数据及表：com.kingdee.eas.basedata.master.material.MaterialAsstAttrValue，T\_BD\_MaterialAsstAttrValue

仓库和库存
----------

核算项目
--------

> 用于财务凭证按对象进行辅助记账，标准产品预置了一些常用基础资料作为核算项目。

![](media/media/image218.png){width="6.4125in"
height="2.854861111111111in"}

### 自定义辅助核算项目

> 树形基础资料，用于标准产品基础资料外其他仅用于财务核算用的核心对象定义。

-   [[]{#OLE_LINK28 .anchor}]{#OLE_LINK29
    .anchor}自定义核算项目元数据和表：com.kingdee.eas.basedata.master.auxacct.GeneralAsstActType，T\_BD\_GeneralAsstActType

-   自定义核算项目类别元数据和表：com.kingdee.eas.basedata.master.auxacct.GeneralAsstActTypeGroup，T\_BD\_GeneralAsstActTypeGroup

### 添加非标核算项目

> 把二次开发添加的基础资料作为财务核算项目，以下开发资料来自总部给出的文档。

[]{#_1560939133 .anchor}

其他业务知识
------------

### 税率税额

-   价格或不含税价格，金额或不含税金额，一般属性名为：price，amount

-   税率，税额，一般属性名为：taxRate，tax

-   含税价格，含税金额，一般属性名为：taxPrice，taxAmount

注意在EAS供应链和财务模块中，关于含税金额和税额属性的名称并不相同，开发者应自己从entity元数据中查询。

计算方法可以参考

-   com.kingdee.eas.scm.common.client.helper.UiHandlingHelper

-   com.kingdee.eas.scm.common.client.helper.SaleUiHandlingHelper.SaleUiHandlingHelper

基本公式：

-   含税价格＝不含税价格×税率／100

-   含税金额＝含税价格×数量

### 价格和折扣

-   折扣方式，一般属性名为discountType，由DiscountModeEnum定义

![](media/media/image220.png){width="3.4159722222222224in"
height="0.40625in"}

-   单位折扣额或折扣率，一般属性名为：discount

-   折扣额，一般属性名为：dicountAmount

-   实际单价、实际含税单价，即扣除折扣额的单价，一般属性名为：actualPrice，actualTaxPrice

计算方法可以参考

-   com.kingdee.eas.scm.common.client.helper.UiHandlingHelper

-   com.kingdee.eas.scm.common.client.helper.SaleUiHandlingHelper.SaleUiHandlingHelper

> 基本公式：

-   计算单位折扣额/率：折扣额＝价格－实际价格，折扣率＝折扣额／价格×100

-   计算折扣金额：折扣金额＝折扣额×数量＝折扣率／100×数量

### 数量计量

-   计量单位、数量，一般的EAS业务单据支持多计量单位，用户录入单据时可以指定自己想要的计量单位及数量。一般属性名称为：unit、qty

-   基本计量单位、基本数量，物料基础资料中会设置基本计量单位，一般的EAS单据中也会有根据基本计量单位换算出来的基本数量。一般属性名称为：baseUnit、baseQty

-   辅助计量单位、辅助数量，很多供应链单据中设置有辅助计量单位和辅助数量，提供计量单位之外的第二种计量方式，但是在实际业务中应用并不多。一般属性名称为：assistUnit、assistQty

如果用户业务中存在同一个物料可能会使用多计量单位，那么相关的统计报表获取数量数据时，应当统一取基本计量单位数量字段，避免计量单位不一致造成统计数据错误

计量单位换算处理可以参考

-   com.kingdee.eas.scm.common.client.helper.UiHandlingHelper

### 币别和金额

-   本位币：当前财务组织或者所委托的财务组织，确定记账使用的基础货币，例如"人民币"

-   原币：当前业务记录使用的货币，例如"美元"

-   原币金额，也就是业务单据的普通金额

-   本位币金额，即原币金额按照汇率转换得到的本位币货币金额，一般属性名中包含"local"，例如：localAmount、localTaxAmount。

如果用户业务中涉及到外币，那么相关的统计报表获取金额数据时，应当统一取本位币类型的金额字段，避免币种不一致造成统计数据错误

 WAFII开发
==========

开发文档：http://waf2.kingdee.com:6888/waf2help/

WAFII BOS快测URL

http://localhost:56898/myweb/webframework/management/index.do?method=init

http://127.0.0.1:56898/myweb/webframework/management/index.do?method=init

  {#section-1 .ListParagraph}
=
