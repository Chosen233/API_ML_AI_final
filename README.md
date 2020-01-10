# 项目名称：培英

# 产品说明文档

| Title | Content |
| --- | --- |
| 发布日期| 2019/12/10 |
| 项目名称| 培英 |
| 项目状态| 已完成 |
| 项目所有者| 蔡晓晨 |
| 项目设计师| 蔡晓晨 |
| 项目开发者| 蔡晓晨 |
| 项目测试者| 蔡晓晨|

## 目录
- [价值主张设计](#价值主张设计) 
    - [加值宣言](#加值宣言)
    - [核心价值](#核心价值)
    - [用户痛点](#用户痛点)
    - [人工智能概率性与用户痛点](#人工智能概率性与用户痛点)   
    - [需求列表与人工智能API加值](#需求列表与人工智能API加值) 
- [原型](#原型)
    - [交互及界面设计](#交互及界面设计)
    - [信息设计](#信息设计)
    - [原型文档](#原型文档)
- [API](#API产品使用关键AI或机器学习之API的输出入展示)
    - [API1.使用水平](#API1使用水平)
    - [API2.使用比较分析](#API2使用比较分析)
    - [API3.使用后风险报告](#API3使用后风险报告)

## 产品定位

“培英”是帮助英语水平处于入门水平的初学者的教育类软件，皆在培养用户学习英语的兴趣。

*   对象为英语处于入门水平的初学者，基础较差。

## 项目背景

*   随着社会竞争的加强，学习和掌握一门外语成为人们热衷的加分项，不少家长都有意识去培养孩子学习英语的兴趣。
*  家长自己不懂如何去培养孩子学习英语的兴趣，强迫孩子死记硬背容易弄巧成拙。

*   通过对一系列的教育类APP调查，几乎所有的教育类APP都没有一款是针对入门初学者设计的APP。



## 目标

*   通过使用百度AI的通用物体与图像识别和有道智云API，把用户拍下来的照片进行识别并翻译成英语单词。
*   把翻译的单词积累下来可以回顾


# 价值主张设计

## 加值宣言

本产品皆在通过使用百度AI开放平台的通用物体与图像识别和有道智云API来实现对照片进行识别及翻译，培养孩子学习的兴趣，满足好奇心。

*   （主要）百度AI开放平台的通用物体与图像识别对本产品加值部分在于：根据数千个可识别对象、生物、风景，接口返回识别内容。
*   （辅助）有道智云API对本产品加值部分在于：根据上一步识别出的内容进行翻译。

## 核心价值

*   着重于当前家长想要培养孩子学习英语的兴趣，提供给用户识别图像翻译单词的功能，以求用户在使用过程中参与感和乐趣能激发学习英语单词的动力。


## 用户痛点

*   家长想培养孩子学习英语的兴趣却不知道该如何下手
*   家长想检验孩子英语口语的水平，可是自身英语水平也很一般。
*   找不到一款适合儿童学习英语使用的教育类app。
*   百度翻译中的实物翻译的流程较繁琐

## 人工智能概率性与用户痛点
####可能导致识别失败的因素及其如何解决：
* 无法检测出物体
解决方式：弹出提示“无法识别内容”，帮助用户重新返回到拍摄页面进行再次拍摄-识别。
* 物体识别出错或不匹配—
解决方式：
a.用户可通过滑动卡片，选择性添加识别对象的单词及中文意思
b.创建一个用户界面，指引人们在运行之前确保摄像头画面中已经出现了要识别的目标

## 需求列表与人工智能API加值

 需求列表

| # | 用户案例 | 重要性 | 笔记 | 技术 |
| --- | --- | --- | --- | --- |
| 1 | 林妈妈的儿子问她吃的水果用英语该怎么读 | 极其重要 | 核心功能 | 分析图像 |
| 2 | 小明要准备一个英语朗诵比赛，但是他不确定自己读音标不标准 | 重要 | 核心功能 | 口语测评 |


# 原型
## 产品架构图
![](https://i.loli.net/2020/01/10/YbPlquSBIoiRtvU.png)


## 交互及界面设计
- [培英产品原型](https://k3j4yj.axshare.com)，若该链接加载过慢，请[点击此处](http://nfunm001.gitee.io/e.qpp)

- 百度AI通用物体和场景识别API：识别照片主体内容，返回名称。
- 有道智云AI文本翻译API：根据返回的名称翻译成英语单词。
![输入图片说明](https://i.loli.net/2020/01/07/YQM1ls4jxqwiDc9.png)

## 信息设计
![](https://i.loli.net/2020/01/09/h76HJZMEdN2USnI.png)
![](https://i.loli.net/2020/01/09/Cn2AXEgu8dGTvR5.png)
![](https://i.loli.net/2020/01/09/UY6rhfmIzV3gSNF.png)
![](https://i.loli.net/2020/01/09/U53vizJNGgFcbaV.png)
![](https://i.loli.net/2020/01/09/U53vizJNGgFcbaV.png)
![](https://i.loli.net/2020/01/09/hKjrpBbtGIUvFMO.png)
![](https://i.loli.net/2020/01/09/N6Tqc4F3dAnPyXe.png)
![](https://i.loli.net/2020/01/09/itmScTfVFzqPNae.png)

## 原型文档
* [培英产品原型](https://k3j4yj.axshare.com)
* [培英产品原型下载](https://gitee.com/NFUNM001/e.qpp)

# API产品使用关键AI或机器学习之API的输出入展示
## API1使用水平
#### 百度AI通用物体与图像识别
* 输入
```
# encoding:utf-8
import requests 

# client_id 为官网获取的AK， client_secret 为官网获取的SK
host = 'https://aip.baidubce.com/oauth/2.0/token?grant_type=client_credentials&client_id=XtxocZFz4nIKzPyME6QtunyF&client_secret=NyfS6nELlg71kYoDRujgXF7jw5ILZyqe'
response = requests.get(host)
if response:
    print(response.json())
```
* 输出
```
{'refresh_token': '25.9b57acdc18563c73298b9d80272d2f4b.315360000.1892305426.282335-18081781', 'expires_in': 2592000, 'session_key': '9mzdA5rh5spnaTEx7qFHWhkPxb+P3XEzxkndRYKP+RrEr8NvDKkSCT4x9r9cukFb031H6lIe8a/GgiXnlq7HEtTuUt1x4g==', 'access_token': '24.805ba36f70a4d0e6d743401eb732d35c.2592000.1579537426.282335-18081781', 'scope': 'public vis-classify_dishes vis-classify_car brain_all_scope vis-classify_animal vis-classify_plant brain_object_detect brain_realtime_logo brain_dish_detect brain_car_detect brain_animal_classify brain_plant_classify brain_ingredient brain_advanced_general_classify brain_custom_dish brain_poi_recognize brain_vehicle_detect brain_redwine brain_currency brain_vehicle_damage wise_adapt lebo_resource_base lightservice_public hetu_basic lightcms_map_poi kaidian_kaidian ApsMisTest_Test权限 vis-classify_flower lpq_开放 cop_helloScope ApsMis_fangdi_permission smartapp_snsapi_base iop_autocar oauth_tp_app smartapp_smart_game_openapi oauth_sessionkey smartapp_swanid_verify smartapp_opensource_openapi smartapp_opensource_recapi fake_face_detect_开放Scope vis-ocr_虚拟人物助理 idl-video_虚拟人物助理', 'session_secret': 'ae8de328be480b79cdcab9ac5bfb8eec'}
```

* 输入
```
# encoding:utf-8

import requests
import base64


···
通用物体和场景识别
'''

request_url = "https://aip.baidubce.com/rest/2.0/image-classify/v2/advanced_general"
# 二进制方式打开图片文件
f = open('C:/Users/29552/Desktop/what.jpg', 'rb')
img = base64.b64encode(f.read())

params = {"image":img}
access_token = '24.805ba36f70a4d0e6d743401eb732d35c.2592000.1579537426.282335-18081781'
request_url = request_url + "?access_token=" + access_token
headers = {'content-type': 'application/x-www-form-urlencoded'}
response = requests.post(request_url, data=params, headers=headers)
if response:
    print (response.json())
```
* 输出
```
{'log_id': 9095107985145517526, 'result_num': 5, 'result': [{'score': 0.746256, 'root': '非自然图像-书籍封面', 'keyword': '书籍'}, {'score': 0.584855, 'root': '人物-人物特写', 'keyword': '人物特写'}, {'score': 0.426847, 'root': '人物-人物特写', 'keyword': '鬓发'}, {'score': 0.267823, 'root': '人物-人物特写', 'keyword': '美女'}, {'score': 0.100517, 'root': '人物-人物特写', 'keyword': '女人'}]}
```


## API2使用比较分析
#### 百度AI——通用物体和场景识别

**API性价比方面**：

*   免费调用量500次/天 ，且付费后，每日免费调用额度仍保留；

*   可选择“按调用量付费”进行API调用；

*   [百度AI——通用物体和场景识别——产品定价](https://ai.baidu.com/tech/imagerecognition/general)

**API成熟度方面**：

*   准确性高：基于百度海量数据，利用深度学习技术及高精度算法不断迭代模型，准确率业界领先

*   标签体系丰富：可识别出10万+物体及场景标签，并在不断丰富中，持续提供更精细的识别服务

*   简单易用：支持标准化接口封装，调用简单，只需上传单张图片，即可获取识别结果

*   [百度AI——通用物体和场景识别——产品优势](https://ai.baidu.com/tech/imagerecognition/general)

#### （2）竞争对手分析：阿里云——图像识别

**API性价比方面**：

*   API前5000次调用免费仅限首次购买资源包的用户。

*   采用购买按月（自然月）预付费资源包的计费方式，计费方式单一；

*   [阿里云——图像识别——产品定价](https://help.aliyun.com/document_detail/53386.html?spm=a2c4g.11174283.3.2.3cc81039M0w0uA)

**API成熟度方面**：

*   识别精准度高：图像识别等算法精度处于业内领先水平

*   识别效率高：支持实时识别

*   [阿里云——图像识别——产品优势](https://data.aliyun.com/product/image?spm=5176.10695662.1141443.1.35af6a39VVvSsT&aly_as=VV3agq85)

#### [](https://github.com/Liaojunjie2333/final#3%E6%80%BB%E7%BB%93)（3）总结

*   **性价比方面**，百度AI开放平台的API调用性价比较高。第一，其给予每天一定的免费调用次数，且购买服务后免费次数依然保留。第二，可选择“按调用量付费”进行API调用，提供这样的选择无疑更加灵活。

*   **成熟度方面**，百度和阿里都有着各自的产品优势、技术优势，但百度在图像识别方面的产品相比较而言更多，有理由相信百度在这方面更加的有经验优势。


## API3使用后风险报告
所使用的API类别：**通用物体和场景识别**

##### 输入输出的限制
* access_token的有效期为30天，切记需要每30天进行定期更换，或者每次请求都拉取新token

##### 目前和未来发展性

*   通用物体和场景识别这样的api在实际使用当中有时出现识别不准，图片内容有多个物体而没有正确识别主体。

* 一张肉眼很容易就判断出内容的图片，可能因为噪点的问题而导致识别不准。所以我们做图像识别的产品有风险，产品设计要考虑风险，我们做这件事就要考虑用技术的时候，用对地方很重要，用错地方就会很大的风险。


#### API市场竞争程度

*   目前API市场上，提供“图像识别”这一类型的API接口服务的公司还是比较多的，竞争剧烈，百度、阿里、腾讯和微软等等都有在做

*   每一个都有各自的优势，没有哪一家能够做到真正的压制，消费者根据自身的需求去选择不同的产品。

