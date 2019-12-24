# 项目名称：培英

# 产品说明文档

| Title | Content |
| --- | --- |
| 发布日期| 2019/12/10 |
| 项目名称| 培英 |
| 项目状态| 进行中 |
| 项目所有者| 蔡晓晨 |
| 项目设计师| 蔡晓晨 |
| 项目开发者| 蔡晓晨 |
| 项目测试者| 蔡晓晨|


## 产品定位

“培英”是帮助英语水平处于入门水平的初学者的教育类软件，皆在培养用户学习英语的兴趣。

*   对象为英语处于入门水平的初学者，基础较差。

## 背景

*   随着社会竞争的加强，学习和掌握一门外语成为人们热衷的加分项，不少家长都有意识去培养孩子学习英语的兴趣。
*  家长自己不懂如何去培养孩子学习英语的兴趣，强迫孩子死记硬背容易弄巧成拙。

*   通过对一系列的教育类APP调查，几乎所有的教育类APP都没有一款是针对入门初学者设计的APP。



## 目标

*   通过使用计算机视觉——分析图像和有道智云API，把用户拍下来的照片进行识别并翻译成英语单词。
*   把翻译的单词积累下来可以回顾


# 价值主张设计

## 加值宣言

本产品皆在通过使用计算机视觉——分析图像和有道智云API来实现对照片进行识别及翻译，培养孩子学习的兴趣，满足好奇心。

*   （主要）微软Azure中的计算机视觉——分析图像对本产品加值部分在于：根据数千个可识别对象、生物、风景，接口返回识别内容。
*   （辅助）有道智云API对本产品加值部分在于：根据上一步识别出的内容进行翻译。

## 核心价值

*   分析图像：最小可用产品为拍照／上传图片，检测用户上传的图片，返回单词内容。
*   口语评测：使用腾讯云——智聆口语评测提供用户检验口语是否标准。

## 用户痛点

*   家长想培养孩子学习英语的兴趣却不知道该如何下手
*   家长想检验孩子英语口语的水平，可是自身英语水平也很一般。
*   找不到一款适合儿童学习英语使用的教育类app。
*   百度翻译中的实物翻译的流程较繁琐

## 人工智能概率性与用户痛点(进行中）
####可能导致识别失败的因素及其如何解决：
* 无法检测出物体
解决方式：弹出提示“无法检测出物体”，帮助用户重新返回到拍摄页面进行再次拍摄-识别。
* 物体识别出错或不匹配—
解决方式：
a.用户可通过滑动卡片，选择性添加识别对象的单词及中文意思
b.创建一个用户界面，指引人们在运行之前确保摄像头画面中已经出现了要识别的目标

## 需求列表与人工智能API加值

## 需求列表

| # | 用户案例 | 重要性 | 笔记 | 技术 |
| --- | --- | --- | --- | --- |
| 1 | 林妈妈的儿子问她吃的水果用英语该怎么读 | 极其重要 | 核心功能 | 分析图像 |
| 2 | 小明要准备一个英语朗诵比赛，但是他不确定自己读音标不标准 | 重要 | 核心功能 | 口语测评 |




# PART3 API产品使用关键AI或机器学习之API的输出入展示
· 输入
```
# encoding:utf-8
import requests 

# client_id 为官网获取的AK， client_secret 为官网获取的SK
host = 'https://aip.baidubce.com/oauth/2.0/token?grant_type=client_credentials&client_id=XtxocZFz4nIKzPyME6QtunyF&client_secret=NyfS6nELlg71kYoDRujgXF7jw5ILZyqe'
response = requests.get(host)
if response:
    print(response.json())
```
· 输出
```
{'refresh_token': '25.9b57acdc18563c73298b9d80272d2f4b.315360000.1892305426.282335-18081781', 'expires_in': 2592000, 'session_key': '9mzdA5rh5spnaTEx7qFHWhkPxb+P3XEzxkndRYKP+RrEr8NvDKkSCT4x9r9cukFb031H6lIe8a/GgiXnlq7HEtTuUt1x4g==', 'access_token': '24.805ba36f70a4d0e6d743401eb732d35c.2592000.1579537426.282335-18081781', 'scope': 'public vis-classify_dishes vis-classify_car brain_all_scope vis-classify_animal vis-classify_plant brain_object_detect brain_realtime_logo brain_dish_detect brain_car_detect brain_animal_classify brain_plant_classify brain_ingredient brain_advanced_general_classify brain_custom_dish brain_poi_recognize brain_vehicle_detect brain_redwine brain_currency brain_vehicle_damage wise_adapt lebo_resource_base lightservice_public hetu_basic lightcms_map_poi kaidian_kaidian ApsMisTest_Test权限 vis-classify_flower lpq_开放 cop_helloScope ApsMis_fangdi_permission smartapp_snsapi_base iop_autocar oauth_tp_app smartapp_smart_game_openapi oauth_sessionkey smartapp_swanid_verify smartapp_opensource_openapi smartapp_opensource_recapi fake_face_detect_开放Scope vis-ocr_虚拟人物助理 idl-video_虚拟人物助理', 'session_secret': 'ae8de328be480b79cdcab9ac5bfb8eec'}
```

· 输入
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
· 输出
```
{'log_id': 9095107985145517526, 'result_num': 5, 'result': [{'score': 0.746256, 'root': '非自然图像-书籍封面', 'keyword': '书籍'}, {'score': 0.584855, 'root': '人物-人物特写', 'keyword': '人物特写'}, {'score': 0.426847, 'root': '人物-人物特写', 'keyword': '鬓发'}, {'score': 0.267823, 'root': '人物-人物特写', 'keyword': '美女'}, {'score': 0.100517, 'root': '人物-人物特写', 'keyword': '女人'}]}
```

## 使用水平 输入+输出
1、产品使用到的API展示
Azure-标记图像api
有道志云-翻译API
我爱背单词-单词集API

