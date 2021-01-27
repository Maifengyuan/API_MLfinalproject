# API_MLfinalproject
API课程期末项目产品文档
</br>
</br>

## 文档简介：
本文档主要描述“看见”小程序的功能需求及其设计，目的在于清晰的定义各个模块的需求细节及逻辑流程，并清晰、有层次的定义页面原型中各个模块的内容来源和相关的逻辑。
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
|最后修订日期|2021-01-22|
|展示视频|[智能APP加值产品报告](https://www.bilibili.com/video/BV1tV411q7V8/)；[原型交互视频](https://pan.baidu.com/s/1BtCCNX1Z1OjBrKPxmQRIOQ)网盘提取码: 8jet |
</br>

## 文档版本信息
|序号|开发版本号|修订人|修订日期|备注|
| --- | --- | --- | --- | --- |
|1|s1.0|麦锋源|2020-12-19|创建文档，初步确定产品定位与核心价值|
|2|s1.1|麦锋源|2020-12-21|添加价值主张画布和产品结构流程图|
|3|s1.2|麦锋源|2020-12-22|添加产品功能和信息结构图以及总体流程图|
|4|s1.3|麦锋源|2020-12-23|添加功能列表|
|5|s1.4|麦锋源|2020-12-29|添加数据流程图，完善产品特色|
|6|s1.5|麦锋源|2021-1-3|对API应用平台进行实践分析，构建对比数据|
|7|s1.6|麦锋源|2021-1-5|添加用户浏览社区内容用例图|
|8|s1.7|麦锋源|2021-1-10|将价值主张画布更改为用户画像，添加API代码示例：通用物体与场景识别|
|9|s1.8|麦锋源|2021-1-11|完善图像识别技术api的代码示例对比|
|10|s1.9|麦锋源|2021-1-16|添加智能API加值说明|
|11|s2.0|麦锋源|2021-1-20|添加原型图链接与相关说明|
|12|s2.1|麦锋源|2021-1-22|上传项目展示视频|
</br>

## 目录

|MVP加/价值主张宣言|问题需求|界面流程及关键智能交互|数据流程及关键智能API使用|其他|
| --- | --- | --- | --- | --- |
|[MVP价值宣言](#chapter1) |[使用情景](#chapter3)|[用户体验/旅程](#chapter8)|[数据流程分析和界面流程](#chapter11)|[总结与感谢](#chapter14)|
|[产品概述](#chapter1) |[用户画像](chapter4)|[界面设计可取性](#chapter9)|[数据流设计可取性](#chapter12)|[参考材料](#chapter15)|
|[产品简介](#chapter2) |[需求列表](#chapter5)|[界面流程及关键智能交互](#chapter10)|[代码及数据展示加值](#chapter13)|[内容汇总](#chapter16)|
|---------------------|[API智能加值](#chapter6)|--------------------|---------------------|---------------------|
|---------------------|[利害分析](#chapter7)|---------------------|---------------------|---------------------|

</br>
</br>

## 产品介绍

<div align=center><img src="https://github.com/Maifengyuan/API_MLfinalproject/blob/main/img/%E7%9C%8B%E8%A7%81logo.png" width="400" height="400" alt="logo"></div>

<h3 id="chapter1">一、产品概述</h3>
本产品将致力于服务视力障碍人群，通过图像识别和智能语音技术，对被拍摄的事物进行识别后输出语音描述，并对用户进行解释说明，最大化满足视力障碍人士对新事物的认知、分享以及平等拓展社会人际关系的需求，为用户提供无障碍体验，创造有价值的沟通社区，为视障人士打开更丰富、多彩的世界。

<br/>

#### MVP加值说明（融合人工智能API）
|问题情境|解决方案|
| --- | --- |
|无法看见眼前的事物，并对其做出行为判断|API——物体识别与场景识别+语音合成：对被拍摄事物进行分析，通过语言的方式实时输出给用户|
|无法正常通过图片或视频读取社交信息|API-图像识别+语言合成：对离线图像进行分析，并通过语言输出给用户|
|分享个人日志|API——语言转写+NLP：将用户输入的语言转换成文本存入发布信息中|
|简化使用操作|API——人脸识别+语音识别：辅助用户高校、安全使APP|

</br>
</br>

<h3 id="chapter2">二、产品简介</h3>

- 定位：针对视障群体打造的一款结合摄影、创作和分享的APP“看见”，运用图形识别技术，解读像素背后所蕴含的真谛，创造出社会人文价值。
- 特色：产品以智能、无障碍为主要价值导向，将图像识别、NLP技术的与机器学习-决策服务相融合，为视障人群带来最舒适、最贴心的使用体验。此外，产品将贯彻“Less is more”的设计理念，将极简的风格渲染至产品的每一处细节，打破传统影音软件多元素泛滥的外表，使得产品始终聚焦在核心功能的设计上，优化用户在无障碍与流畅性等方面的使用体验。

</br>
</br>

<h3 id="chapter4">三、问题需求</h3>

![用户画像](img/User_Portrait.png)

“手机产商们总是竭力地优化着99%的体验，但总有人愿意去解决着1%的问题。无障碍模式往往被藏在设置界面里的角落，但它却是最具有人文关怀的功能”，这一定程度上代表APP“看见”的这一类产品。那些边缘的需求或许不及大众产品的所创造的商业价值，相对没有庞大的受众与支持，但这些往往是被我们所忽视人类社会最具温暖的东西。科技发展目的是为了人类更好的生活，既然如此，给予特殊群体更多的帮助和温暖也应贯彻每个交互产品的核心价值。基于这个理念，“看见”将价值主张聚焦于视障人群，希望能突破正常生活温暖的包裹，去拥抱那些仍在寒风中行走的人。

<br/>
<br/>

<h3 id="chapter3">四、使用情景</h3>

#### 使用情境说明
“看见APP”的使用情境涵盖视障群体的日常生活，包括社交、出行、导航、记录生活等。下方用例图主要以两个使用情境做具体说明：
<br/>
1. 用户从注册成为应用的浏览者到内容的创作者的过程；
2. 用户通过APP寻求帮助，达到方便规划出行的目的。

<div align=center><img src="https://github.com/Maifengyuan/API_MLfinalproject/blob/main/img/Use_Case.jpg" width="750" height="800" alt="用例图"></div>

<br/>
<br/>

<h3 id="chapter5">五、需求列表</h3>

#### 关键API使用与
将智能API加值融入具体功能解决视障人士使用互联网产品是存在的难题
1. 图片信息难以获取——图像识别
2. 读屏反馈缺陷——语音识别+语音合成
3. 数据准确性——NLP文本处理技术
4. 安全与验证——面部识别
5. 兼容性——插件模式

![需求列表](img/Function_list.png)


<br/>
<br/>

<h3 id="chapter6">六、API智能加值</h3>


<br/>
<br/>

<h3 id="chapter7">七、利害分析</h3>
“看见”APP优化了视障群体在使用社交产品时的体验，同时内容分析平台承载内容创作者、商品销售者与用户三种角色，产品通过远程内容和生活服务吸引用户，流量的增加促进企业合作，产生的红利将内容输出者与产品绑定，形成一条受收益链。

1. 人工智能类型
APP使用人工智能相关服务均为弱人工智能，所有智能API都面向指定任务，不具有自我认知能力，其能力覆盖面较小
2. 系统性偏差
API分析结果并不能确保百分之百的准确性，信息识别结果会存在一定误导性和偏差，需要人工对内容数据进行后期审核

<br/>
<br/>

<h3 id="chapter8">八、用户体验/旅程分析</h3>

![用户体验/旅程](img/user_travel.png)

<br/>
<br/>

<h3 id="chapter9">九、界面设计可取性</h3>

1. 用户可欲性
APP所使用的关键API加值有明确的使用目标和领域，针对图像和文本内容的输出、图像识别以及生活出行规划都提供了便捷的使用方案，极大优化了视障群体生活所需的各个方面

2. 技术可行性
针对视障群体对于信息获取效率与社区需求，APP结合图像识别、语音合成、语音识别等API服务，优化产品在服务端迈向智能。

3. 商业可行性
“看见”APP利用多种针对性强且成本较低的API功能实现产品服务，对于智能识图和智能出行等方面与其他互联网公司进行合作能创造一定的共同价值。

![商业模式](img/Business_Model.png)

<br/>


<h3 id="chapter12">十、数据流设计可取性</h3>

<div align=center><img src="https://github.com/Maifengyuan/API_MLfinalproject/blob/main/img/Data_flowchart.jpg" width="600" height="800" alt="数据流"></div>

1. 用户可欲性
APP使用方式简单，因为针对视障人群有特殊设计，使得整体操作可以完全依靠手势和语音反馈完成，APP对不同用户使用体验在设置模块增加了个性化的操作模式，以达到最佳的无障碍沟通与APP使用。此外，通过智能语音助手可以快速帮助用户完成出行安排等工作。

2. 技术可行性
针对视障群体对于信息获取效率与社区需求，APP结合图像识别、语音合成、语音识别等API服务，优化产品在服务端迈向智能。

3. 商业可行性
APP以提高视障群体的生活品质为主要目标，在公益方面会达到一定的影响力，切合了社会进步所需要的人文关怀方向，通过科技为人类创造美好生活。

<br/>
<br/>

<h3 id="chapter10">十一、界面流程及关键智能交互</h3>

[产品原型图在线浏览](https://modao.cc/app/f83ebdfdc74e882f158a6cfadd000e95d9ba5d4a/embed/v2)

![原型界面设计](img/Interface_design.jpg)

<br/>
<br/>

<h3 id="chapter11">十二、数据流程分析和界面流程</h3>

#### 功能结构

<div align=center><img src="https://github.com/Maifengyuan/API_MLfinalproject/blob/main/img/Functional_str.jpg" width="450" height="750" alt="功能结构"></div>

***

#### 信息结构

<div align=center><img src="https://github.com/Maifengyuan/API_MLfinalproject/blob/main/img/Information_str.jpg" width="450" height="850" alt="信息结构"></div>


</br>
<br/>

<h3 id="chapter13">十三、代码及数据展示加值</h3>

产品结合图像识别、语言合成等智能API，进一步简化用户在使用产品时所需要操作步骤，通过简单的指控，智能语音系统与对用户的脸部识别完成登入、浏览、分析等功能，最大程度满足无障碍使用体验。

#### 通用物体识别与场景识别技术
- 以百度和讯飞两个平台图像识别API服务技术实践得出的比对结果

|对比项|百度|讯飞|
|---|---|---|
|代码示例-图像识别技术：场景与物体识别|[百度api代码示例](https://github.com/Maifengyuan/API_MLfinalproject/blob/main/code/%E7%99%BE%E5%BA%A6-%E9%80%9A%E7%94%A8%E7%89%A9%E4%BD%93%E5%92%8C%E5%9C%BA%E6%99%AF%E8%AF%86%E5%88%AB.ipynb)|[讯飞api代码示例](https://github.com/Maifengyuan/API_MLfinalproject/blob/main/code/%E8%AE%AF%E9%A3%9E-%E5%9C%BA%E6%99%AF-%E7%89%A9%E4%BD%93-%E5%9C%BA%E6%89%80%E8%AF%86%E5%88%AB.ipynb)|

<h4>场景识别实践结果</h4>

<div align=center><img src="https://github.com/Maifengyuan/API_MLfinalproject/blob/main/img/ptest05.jpg" width="500" height="450" alt="场景识别材料"></div>

1. 百度场景识别API返回参数

```
{'log_id': 5712521386408023851,
 'result_num': 5,
 'result': [{'score': 0.358338, 'root': '建筑-其他', 'keyword': '居民楼'},
  {'score': 0.253114, 'root': '自然风景-天空', 'keyword': '天空'},
  {'score': 0.17113, 'root': '建筑-现代建筑', 'keyword': '剧院/博物馆/礼堂'},
  {'score': 0.088515, 'root': '自然风景-其他', 'keyword': '风景'},
  {'score': 0.006694, 'root': '植物-树', 'keyword': '树'}]}
```

2. 讯飞场景识别API返回参数

```
{'code': 0,
 'data': {'fileList': [{'label': 9,
    'labels': [9, 3, 11, 18, 10],
    'name': 'test01.jpg',
    'rate': 0.9986672401428223,
    'rates': [0.9986672401428223,
     0.0010075508616864681,
     0.0002714783186092973,
     3.254865441704169e-05,
     1.3011311239097267e-05],
    'review': False}],
  'reviewCount': 0,
  'topNStatistic': [{'count': 1, 'label': 9}]},
 'desc': 'success',
 'sid': 'tup000011d5@dxb9d81358500b000100'}
```

|参数|返回值|说明|
| --- | --- | --- |
|label|9| 对应场景：山峰|
|labels|9,3,11,18,10|表示前5个最可能场景的label，分别是山峰，草地，森林，其他场景，湖|
|rate|0.99|介于0-1间的浮点数，表示该图像被识别为某个分类的概率值，概率越高、机器越肯定|
|rates|0.99,0.001,0.0002,3.25,1.3|labels对应，前5个最可能场景对应得分|
|review|False|返回true时存在偏差，可信度较低，返回false时可信度较高|

```
{"place":[{
    "entity":[{
        "id":32,"name":"street",
        "score":0.83509528636932373
        }],
     "frameID":0,"startTimeOffset":0.0}]
 }
```

|参数|返回值|说明|
| --- | --- | --- |
|id/name|32,street|识别结果：街道|
|score|0.83|置信度|

<br/>

<h4>物体识别实践结果</h4>

<div align=center><img src="https://github.com/Maifengyuan/API_MLfinalproject/blob/main/img/stest02.jpg" width="500" height="350" alt="物体识别材料"></div>

1. 百度物体识别API返回参数

```
{'log_id': 6639343850218473740,
 'result_num': 5,
 'result': [{'score': 0.31101, 'root': '商品-电脑办公', 'keyword': '笔记本电脑'},
  {'score': 0.230072, 'root': '商品-数码产品', 'keyword': '台式电脑'},
  {'score': 0.155608, 'root': '商品-家用电器', 'keyword': '音箱'},
  {'score': 0.076702, 'root': '商品-电脑办公', 'keyword': '键盘'},
  {'score': 0.001803, 'root': '商品-电脑办公', 'keyword': '电脑'}]}
```

2. 讯飞物体识别API返回参数

```
{'code': 0,
 'data': {'fileList': [{'label': 19903,
    'labels': [19903, 18881, 1314, 4760, 3042],
    'name': 'stest02.jpg',
    'rate': 0.26318418979644775,
    'rates': [0.26318418979644775,
     0.043663863092660904,
     0.03755110874772072,
     0.027026833966374397,
     0.023022780194878578],
    'review': True}],
  'reviewCount': 1,
  'topNStatistic': [{'count': 1, 'label': 19903}]},
 'desc': 'success',
 'sid': 'tup000011dc@dx680d13585d5b1aba00'}
```

|参数|返回值|说明|
| --- | --- | --- |
|label|19903| 对应物体：老鼠；分类：物品|
|labels|19903, 18881, 1314, 4760, 3042|表示前5个最可能场景的label，分别是老鼠，笔记本，无线局域网络，外围设备，计算机鼠标|
|rate|0.26|介于0-1间的浮点数，表示该图像被识别为某个分类的概率值，概率越高、机器越肯定|
|rates|0.26,0.043,0.037,0.027,0.023|labels对应，前5个最可能场景对应得分|
|review|True|返回true时存在偏差，可信度较低，返回false时可信度较高|

<br/>

|实践结果分析|百度|讯飞|
|---|---|---|
|效果对比：场景识别|对于场景识别所使用的图像，我们能直观的看到两排偏橙色的教学楼、中间的绿树、人行道与远处的山和泛黄的天空，这是对于视觉正常的人所能达到的直观感受，在百度API返回的结果中，场景中除了街道，存在的四个主要部分都能基本正确的识别出来，这一点要优于讯飞API。但在具体描述（keyword）准确率不高，但这一点相比讯飞有了更具象的说明|讯飞API对于识别需要结合场景识别与场所识别返回的结果，并没有识别出建筑，但相比百度API识别到了街道|
|效果对比：物体识别|物体识别选用了一张主体明显的图片，包括笔记本电脑、蓝牙耳机和鼠标。百度API一次返回五个识别结果，匹配的对象包括两个（笔记本电脑、键盘），耳机错误识别成音响，其次没有识别出鼠标，结果的准确率与实际图片存在差距|讯飞API返回的结果包括鼠标，笔记本，无线局域网络，外围设备，计算机鼠标，其中结果和百度都存在一个特点，因为主题少于结果参数个数值，会出现重复的结果参数，此外相比于百度并没有识别出耳机|
|性价比衡量|免费调用量日均主要是500次，开通按量后付费调用失败不计费[百度ai开放平台图像识别产品价格](https://ai.baidu.com/ai-doc/IMAGERECOGNITION/rk3bcxa9e)|免费调用量日均主要是500次，附加90天10万次的体验包，若是付费的话分为三个套餐，1万服务量350元/年；10万服务量3200/年；100万服务量30000元/年[讯飞开放平台图像识别产品价格](https://www.xfyun.cn/services/site_identification?target=price)|
|服务评估|仅有api文档且无示例代码，应用场景和参数不完整，无法进行进一步开发调用|[具有详细的说明](https://www.xfyun.cn/services/wordRecg)及[api调用教程](https://www.xfyun.cn/doc/words/wordRecg/API.html#%E6%8E%A5%E5%8F%A3%E8%AF%B4%E6%98%8E),且参数划分完整，提供业务参数，可扩展性强|

- 总结：利用场景/物体识别API的最终目的是将正常视觉所能传达的信息以语音描述的方式完美呈现给视障人群，所以对API最基础的衡量首先需要看图片内容识别的匹配程度，结合场景与物体识别，以基础的API调用测试，两个平台的的准确率相差甚少，但百度API做了更加细分的处理，在对主题目标进行识别后，还进行了细分标签的判断，例如将建筑具体到剧院/博物馆/礼堂。这一点上百度API占优势。物体识别两个平台的准确率较为相似，但实践中只对百度对通用物体和场景的API功能进行调用，此外百度提供的识别还包括很多细分类别，这一点上百度显然投入更多，相比较与讯飞更有优势。

<div align=center><img src="https://github.com/Maifengyuan/API_MLfinalproject/blob/main/img/baidu.jpg" width="500" height="300" alt="百度图像识别功能列表"></div>

<br/>

#### 文本处理技术
- 以百度和讯飞两个平台API服务技术实践得出的比对结果

|对比项|百度|讯飞|
|---|---|---|
|代码示例：自然语言处理（NLP）|[百度-NLP](https://github.com/Maifengyuan/API_MLfinalproject/blob/main/code/%E7%99%BE%E5%BA%A6-%E8%AF%AD%E9%9F%B3%E5%90%88%E6%88%90.ipynb)|[讯飞-NLP](https://github.com/Maifengyuan/API_MLfinalproject/blob/main/code/%E8%AE%AF%E9%A3%9E-NLP%E6%8A%80%E6%9C%AF%E5%AE%9E%E8%B7%B5.ipynb)|


> 功能涵盖：文本标签、文本分类、文本纠错、摘要提取、情感分析、发布者地址识别

<h4>语言合成实践结果</h4>
以下主要通过文本纠错以及情感分析做功能分析，其余内容请通过上方的代码链接查看详情

1. 百度-NLP返回参数

- 文本纠错

```
result03 = baidu_amend(text="明明明白白白的原因，但明明就想让白白把事情说的明明白白")
result03gbk = str(result03,encoding="GBK")
result03dict =json.loads(result03gbk)
result03dict
```
```
{'log_id': 2247225581012071484,
 'item': {'vec_fragment': [{'ori_frag': '的',
    'begin_pos': 44,
    'correct_frag': '得',
    'end_pos': 46}],
  'score': 2.20157,
  'correct_query': '明明明白白白的原因，但明明就想让白白把事情说得明明白白'},
 'text': '明明明白白白的原因，但明明就想让白白把事情说的明明白白'}
```

这里故意刁难了下纠错功能，但API仍然从复杂难懂的语句中抽出了错误用词（vec_fragment），将“的”改正为“得”

***

- 情感分析
```
result06 = baidu_sentiment(text="我不送彩礼，丈母娘不高兴了，我送彩礼，媳妇不独立了，我都不知道该保大还是保小？")
result06gbk = str(result06,encoding="GBK")
result06dict =json.loads(result06gbk)
result06dict
```
```
{'log_id': 6752814638925151352,
 'text': '我不送彩礼，丈母娘不高兴了，我送彩礼，媳妇不独立了，我都不知道该保大还是保小？',
 'items': [{'positive_prob': 0.00176568,
   'confidence': 0.996076,
   'negative_prob': 0.998234,
   'sentiment': 0}]}
```

|参数|描述|结果说明|
| --- | --- | --- |
|log_id|请求唯一标识码|6752814638925151352|
|sentiment|表示情感极性分类结果，0:负向，1:中性，2:正向|负向|
|confidence|表示分类的置信度，取值范围[0,1]||0.99，置信度高|
|positive_prob|表示属于积极类别的概率 ，取值范围[0,1]|0.99|
|negative_prob|表示属于消极类别的概率，取值范围[0,1]|0.001|

2. 讯飞-NLP返回参数（输入内容与百度NLP相同）
- 文本纠错
```
response==>>
{"header":{"code":0,"message":"success","sid":"ase000e57ed@hu17732669b6f0210882"},"payload":{"result":{"compress":"raw","encoding":"utf8","format":"json","seq":"0","status":"3","text":"eyJjaGFyIjogW10sICJ3b3JkIjogW10sICJyZWR1bmQiOiBbWzMsICLnmb0iLCAiIiwgInJlZHVuZCJdXSwgIm1pc3MiOiBbXSwgIm9yZGVyIjogW10sICJkYXBlaSI6IFtdLCAicHVuYyI6IFtdLCAiaWRtIjogW10sICJvcmciOiBbXSwgImxlYWRlciI6IFtdLCAibnVtYmVyIjogW119"}}}
text==>>
{"char": [], "word": [], "redund": [[3, "白", "", "redund"]], "miss": [], "order": [], "dapei": [], "punc": [], "idm": [], "org": [], "leader": [], "number": []}
```

|参数|描述|结果说明|
| --- | --- | --- |
|char/word|别字纠错|无|
|redund|语法纠错-冗余：[2, ‘CD’, ‘R’, ‘redund’]] --> [位置，原文本，纠错后文本，类型] |删除第三个“白”|
|miss|语法纠错-缺失|无|
|order|语法纠错-乱序|无|
|dapei|搭配纠错|无|
|punc|标点纠错|无|
|idm|成语纠错|无|
|org|机构名纠错|无|
|leader|领导人职称纠错|无|
|number|数字纠错|无|

***

- 情感分析

```
{"code":"0","data":{"score":0.1486,"sentiment":-1},"desc":"success","sid":"ltp0079c9ee@dx65e5136833261aba00"}
```

|参数|描述|结果说明|
| --- | --- | --- |
|score|分类对应得分，范围 0-1|0.14|
|sentiment|情感极性分类结果，0：中性；1：褒义；-1：贬义|贬义|

<br/>

|实践结果分析|百度|讯飞|
|---|---|---|
|效果对比|在文本纠错上，使用了较难理解的话来衡量两种NLP对于文本的细节处理，结果显示百度准确率略高。在情感分析上都能识别出偏负面的情感，差异不大。但讯飞NLP对于文本纠错的分析上涵盖的内容要比百度NLP多，潜力更大|
|性价比衡量|每日 50000 次免费调用量，开通按量后付费。调用失败不计费[百度ai开放平台手写字api产品价格](https://ai.baidu.com/ai-doc/OCR/9k3h7xuv6)|免费次数为90天10万服务量，若是付费的话分为三个套餐，1万服务量350元/年；10万服务量3200/年；100万服务量30000元/年[讯飞开放平台手写字api](https://www.xfyun.cn/services/wordRecg)|
|服务评估|仅有api文档且无示例代码，应用场景和参数不完整，无法进行进一步开发调用|[具有详细的说明](https://www.xfyun.cn/services/wordRecg)及[api调用教程](https://www.xfyun.cn/doc/words/wordRecg/API.html#%E6%8E%A5%E5%8F%A3%E8%AF%B4%E6%98%8E),且参数划分完整，提供业务参数，可扩展性强|

- 总结：
因为应用需要不断将语音内容和文本内容进行转换，所以对于文本分析的准确性来说十分重要，因为服务用于用户的日常生活，所以即使是绕口令也要保证精确，从对比结果的分析得出，百度NLP技术对于语言的把握性更强，但对于后期的内容分析，讯飞提供的数据会更加多样化，除去近似的产品性价比，讯飞未来运用的潜力会更大，有助于减少人工的分析。

</br>
<br/>

<h3 id="chapter16">十四、内容汇总</h3>
</br>

- 独特非重复有效外连URL：23
- 高水平原创图表：10

***

<h3 id="chapter14">十五、总结与感谢</h3>
这次的文档我参考了很多专业的产品文档与过去学长/学姐的案例，相比他们我在文档中增加了很多文字阐述，我认为自己的优势是绘制流程图，这一方面我有提前做过很多功课，所以上手和流程思维会稍快一些。这使得文档整体的呈现风格偏故事化，这在一定程度上有违于规范的产品文档，偏向个性化。但作为课程实践，我认为这样有利于运用自己的所学所想去表达产品思维，我更希望将这作为一个作品展示。<br/>
不过纵观自己的产品文档，也有不少缺陷：

- 工具运用：
1. [会议桌](https://app.huiyizhuo.com/login?redirect=https%3A%2F%2Fapp.huiyizhuo.com%2F)
2. [Process On](https://www.processon.com/)
3. [墨刀](https://modao.cc/dashboard)
4. [Canva可画](https://www.canva.cn/folder/all-designs)

<h3 id="chapter15">十六、参考材料</h3>

|来源|作者|标题|链接|
| --- | --- | --- | --- |
|环球网|秦璐敏|《中国视障群体约1731万人 30岁以下年轻人占23.5%》|[](https://china.huanqiu.com/article/9CaKrnKl9mV)|
|2016年中国互联网视障用户基本情况报告|中国信息无障碍产品联盟|《中国互联网视障用户基本情况报告》|[](http://www.199it.com/archives/460010.html)|
|时代数据|郑艺阳|《中国有1730万盲人，为什么我们很少看到他们！》|[](https://baijiahao.baidu.com/s?id=1647725605829566019&wfr=spider&for=pc)|
|2019腾讯发布|腾讯X信息无障碍研究会|《视障人士在线社交报告》|[报告链接](http://www.siaa.org.cn/media/1/%E8%A7%86%E9%9A%9C%E4%BA%BA%E5%A3%AB%E5%9C%A8%E7%BA%BF%E7%A4%BE%E4%BA%A4%E6%8A%A5%E5%91%8A_%E5%9B%BE%E6%96%87%E7%89%88_.pdf)|
|中国信息无障碍产品联盟秘书处|中国信息无障碍产品联盟|《中国互联网视障用户基本情况报告》|[报告链接](http://www.siaa.org.cn/media/1/%E4%B8%AD%E5%9B%BD%E4%BA%92%E8%81%94%E7%BD%91%E8%A7%86%E9%9A%9C%E7%94%A8%E6%88%B7%E5%9F%BA%E6%9C%AC%E6%83%85%E5%86%B5%E6%8A%A5%E5%91%8A.pdf)|
|图书馆论坛|丁亚茹，肖鹏|《国外视障人群信息行为研究综述》|[论文链接](http://qikan.cqvip.com/Qikan/Article/Detail?id=7002561077)|
|Bilibili视频|up：六分超超|《这才是iPhone的最强功能，不接受反驳——视觉无障碍功能体验》|[视频链接](https://www.bilibili.com/video/av202959101)|
