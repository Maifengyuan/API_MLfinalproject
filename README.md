# API_MLfinalproject
API课程期末项目产品文档
</br>
</br>

## 文档简介：
本文档主要描述“看见”小程序的功能需求及其设计，目的在于清晰的定义各个模块的需求细节及逻辑流程。目的主要是清晰、有层次的定义页面原型中各个模块的内容来源和相关的逻辑。
</br>
</br>

## 文档使用范围：
此文档主要描述“看见”APP项目中前端页面涉及到的功能点、相对应的后台管理功能支持、以及部分交互细节。本文档主要读者为研发人员、测试人员、市场运营人员、产品经理以及管理人员以及视觉设计师等。
</br>
</br>

## 产品说明
|产品名称|看见|
| --- | --- |
|文件状态|正在修改|
|当前版本|s1.0|
|作者|麦锋源|
|最后修订日期|2020-12-22|
</br>

## 版本信息
|序号|版本号|修订人|修订日期|备注|
| --- | --- | --- | --- | --- |
|1|s1.0|麦锋源|2020-12-19|创建文档，初步确定产品定位与核心价值|
|2|s1.1|麦锋源|2020-12-21|添加价值主张画布和产品结构流程图|
|3|s1.2|麦锋源|2020-12-22|添加产品功能和信息结构图以及总体流程图|
|4|s1.3|麦锋源|2020-12-23|添加功能列表|
|5|s1.4|麦锋源|2020-12-29|添加数据流程图，完善产品特色|
|6|s1.5|麦锋源|2021-1-3|对API应用平台进行实践分析，构建对比数据|
</br>

## 目录
|产品介绍|产品架构|产品功能|项目规划|需求分析
| --- | --- | --- | --- | --- |
|[产品概述](#chapter1) |[功能结构](#chapter5)|[功能列表](#chapter8)|[时间与版本规划](#chapter11)|[需求调研](#chapter14)|
|[产品定位](#chapter2) |[信息结构](#chapter6)|[原型界面](#chapter9)|[成本预算](#chapter12)|[用户评估](#chapter15)|
|[产品特色](#chapter3) |[总体流程](#chapter7)|[数据流与界面](#chapter10)|[风险对策](#chapter13)|[竞品分析](#chapter16)|
|[价值主张](#chapter4) |---------|[用例图](#chapter_case)|[API加值分析](#chapter_key)|[其他](#chapter17)|
</br>
</br>

## 产品介绍
<h3 id="chapter1">一、产品概述</h3>
本产品将致力于服务视力障碍人群，通过图像识别和文字识别技术，对被拍摄的事物进行识别，并对用户进行解释或科普，最大化满足视力障碍人士对新事物的认知、学习、分享产生的需求，为用户提供快捷的查询体验，创造有价值的分享社区，为视障人士打开更有趣、多彩的世界。
</br>
</br>

<h3 id="chapter2">二、产品定位</h3>
针对视障群体打造的一款结合摄影、创作和分享的APP“看见”，运用智能图形识别技术，解读像素背后所蕴含的真谛，通过分享社区创造出“世界就在我眼前”的用户体验。
</br>
</br>

<h3 id="chapter3">三、产品特色</h3>
产品以智能、无障碍为主要价值导向，将图像识别、NLP技术的与机器学习-决策服务相融合，为视障人群带来最舒适、最贴心的使用体验。此外，产品将贯彻“Less is more”的设计理念，将极简的风格渲染至产品的每一处细节，打破传统影音软件多元素泛滥的外表，使得产品始终聚焦在核心功能的设计上，优化用户在便捷性、易操作性等方面的使用体验。
</br>
</br>

<h3 id="chapter4">四、价值主张</h3>

![价值主张画布](img/Value_canvas.jpg)

</br>

## 产品架构
<h3 id="chapter5">五、功能结构</h3>

![功能结构图](img/Functional_structure.jpg)

</br>

<h3 id="chapter6">六、信息结构</h3>

![信息结构图](img/Information_structure.jpg)

</br>

<h3 id="chapter7">七、总体流程</h3>

![产品流程图](img/Flow_Chart.jpg)

</br>

## 产品功能


<h3 id="chapter8">八、功能结构</h3>

![功能列表](img/Function_list.png)

<br/>

<h3 id="chapter9">九、原型图</h3>

<br/>

<h3 id="chapter10">十、数据流与界面</h3>

![数据流程图](img/Data_flowchart.jpg)

<h3 id="chapter_case">十一、用例图</h3>

![内容浏览用例图](img/Use_Case_diagram.jpg)

<h3 id="chapter_key">API加值分析</h3>

#### 图像识别技术
- 以百度和Azure两个平台图像识别API服务技术实践得出的比对结果

|对比项|百度|Azure|
|---|---|---|
|代码示例|[百度-通用物体和场景识别](https://github.com/zhengxiaopingzxp/API_ML_PM_Final_Project/blob/master/code/%E7%99%BE%E5%BA%A6%E6%89%8B%E5%86%99%E5%AD%97api.ipynb)|[Azure-映像说明](https://github.com/zhengxiaopingzxp/API_ML_PM_Final_Project/blob/master/code/%E8%AE%AF%E9%A3%9E%E6%89%8B%E5%86%99%E5%AD%97api.ipynb)|
|效果对比|对于字迹潦草的字体根本无法输出文字，仅使用与字体工整的手写字|对于字迹潦草的字体，仍然能给出部分输出文字，相比百度而已文字的识别准确度也比较高，可查看代码对比|
|精确度对比|[2019-12-09刚刚推出最新版的api文档](https://ai.baidu.com/ai-doc/OCR/hk3h7y2qq)，调用方法和过程比较繁琐，没有给定参考代码，服务刚刚推出，处于起步阶段|[有详细的api调用文档及说明](https://www.xfyun.cn/doc/words/wordRecg/API.html#%E6%8E%A5%E5%8F%A3%E8%AF%B4%E6%98%8E)，并且有相应开发语言的调用示例代码，服务较为成熟|
|性价比衡量|每日 50000 次免费调用量，开通按量后付费。调用失败不计费[百度ai开放平台手写字api产品价格](https://ai.baidu.com/ai-doc/OCR/9k3h7xuv6)|免费次数为90天10万服务量，若是付费的话分为三个套餐，1万服务量350元/年；10万服务量3200/年；100万服务量30000元/年[讯飞开放平台手写字api](https://www.xfyun.cn/services/wordRecg)|
|服务评估|仅有api文档且无示例代码，应用场景和参数不完整，无法进行进一步开发调用|[具有详细的说明](https://www.xfyun.cn/services/wordRecg)及[api调用教程](https://www.xfyun.cn/doc/words/wordRecg/API.html#%E6%8E%A5%E5%8F%A3%E8%AF%B4%E6%98%8E),且参数划分完整，提供业务参数，可扩展性强|

- 总结：

<br/>

#### 文字转语音技术
- 以百度和Azure两个平台文字转语音API服务技术实践得出的比对结果

|对比项|百度|Azure|
|---|---|---|
|代码示例|[百度-语音识别](https://github.com/zhengxiaopingzxp/API_ML_PM_Final_Project/blob/master/code/%E7%99%BE%E5%BA%A6%E6%89%8B%E5%86%99%E5%AD%97api.ipynb)|[Azure-语音识别](https://github.com/zhengxiaopingzxp/API_ML_PM_Final_Project/blob/master/code/%E8%AE%AF%E9%A3%9E%E6%89%8B%E5%86%99%E5%AD%97api.ipynb)|
|效果对比|对于字迹潦草的字体根本无法输出文字，仅使用与字体工整的手写字|对于字迹潦草的字体，仍然能给出部分输出文字，相比百度而已文字的识别准确度也比较高，可查看代码对比|
|精确度对比|[2019-12-09刚刚推出最新版的api文档](https://ai.baidu.com/ai-doc/OCR/hk3h7y2qq)，调用方法和过程比较繁琐，没有给定参考代码，服务刚刚推出，处于起步阶段|[有详细的api调用文档及说明](https://www.xfyun.cn/doc/words/wordRecg/API.html#%E6%8E%A5%E5%8F%A3%E8%AF%B4%E6%98%8E)，并且有相应开发语言的调用示例代码，服务较为成熟|
|性价比衡量|每日 50000 次免费调用量，开通按量后付费。调用失败不计费[百度ai开放平台手写字api产品价格](https://ai.baidu.com/ai-doc/OCR/9k3h7xuv6)|免费次数为90天10万服务量，若是付费的话分为三个套餐，1万服务量350元/年；10万服务量3200/年；100万服务量30000元/年[讯飞开放平台手写字api](https://www.xfyun.cn/services/wordRecg)|
|服务评估|仅有api文档且无示例代码，应用场景和参数不完整，无法进行进一步开发调用|[具有详细的说明](https://www.xfyun.cn/services/wordRecg)及[api调用教程](https://www.xfyun.cn/doc/words/wordRecg/API.html#%E6%8E%A5%E5%8F%A3%E8%AF%B4%E6%98%8E),且参数划分完整，提供业务参数，可扩展性强|

- 总结：

</br>

## 项目规划

<h3 id="chapter11">十二、时间与版本规划</h3>

|版本|时间|详细|
| --- | --- | --- |
|s2.0|1月10日|完成产品文档（包括所有流程图，原型图的设计与代码测试）|
|s2.0|1月14日|完成产品展示|

</br>
<h3 id="chapter12">十三、成本预算</h3>

</br>
<h3 id="chapter13">十四、风险对策</h3>

</br>

## 需求分析

<h3 id="chapter14">十五、需求调研</h3>

</br>
<h3 id="chapter15">十六、用户评估</h3>

#### 用户画像

#### 需求分析

#### 情景假设-系统用例图

</br>
<h3 id="chapter16">十七、竞品分析</h3>
</br>
<h3 id="chapter17">其他</h3>
</br>

#### 关于作者的一些话和展望

#### 参考材料
|来源|作者|标题|链接|
| --- | --- | --- | --- |
|环球网|秦璐敏|《中国视障群体约1731万人 30岁以下年轻人占23.5%》|https://china.huanqiu.com/article/9CaKrnKl9mV|
|2016年中国互联网视障用户基本情况报告|中国信息无障碍产品联盟|《中国互联网视障用户基本情况报告》|http://www.199it.com/archives/460010.html|
|时代数据|郑艺阳|《中国有1730万盲人，为什么我们很少看到他们！》|https://baijiahao.baidu.com/s?id=1647725605829566019&wfr=spider&for=pc|
