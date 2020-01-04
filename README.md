## “时光机” 产品PRD
| 发布日期 | 2019.12.6 
| :-----| ----: 
| 产品名称 |  “时光机”强联系社交平台
| 完成进度 | 进行中
| 文件主人 | 王鹏杰
| 设计者| 王鹏杰
| 开发者| 王鹏杰
# PRD 价值主张设计 15%
#### 需求背景
- 目前互联网上的许多社交软件，类似于微信和QQ，都是致力于维系用户间的弱联系，工作上的加一下，遇到一个有趣的陌生人也加一下，大家都抱着“加了微信，有了联系以后拜托什么事情也方便”这样的心态增加自己好友列表中的好友。但是毫无疑问的是，随着微信中的称不上熟人的陌生人的增加，微信从一开始设定的强化朋友间联系的作用也在不断缩小。而这种相对于“弱联系”的强联系的小圈子文化，恰恰是市场所缺乏的。
- 时光机最吸引人的不是去到未来，而是回到过去。本产品旨在为用户建造一个熟人间的小圈子，让感情历久弥新，不让好兄弟、好闺蜜尘封在冗长的电话簿中，只是一行单调乏味的数字，或者是那些记不真切的会议。并且在此基础上，为用户提供找回失去的“记忆”，重新将人与人之间脆弱的维系链接起来，从无联系到弱联系，从弱联系变成强联系。
## PRD1.加值宣言 3%
一款轻社交智能相册管理产品
###### 重要：
- 运用人脸识别API中的人脸对比服务，在用户上传图片后，自动匹配参与该事件的成员并以特定的时间点予以推送。
- 运用人脸识别API中的人脸搜索服务，当用户上传小时候的照片时，找到其他用户上传的图片中的用户的肖像，通过找相似照片的方式，结合用户提供的生平信息予以匹配。
###### 次要
- 运用人脸识别API中的人脸检测，当用户使用APP时，需进行人脸验证，人脸检测记录用户特征，能够很好的保护用户相册隐私。
#### 核心功能：
- 个人智能云相册，定时自动推送，自动生成用户的照片画廊。

## PRD2.核心价值 3%
- （最小可行性产品）用户可以上传自己所拍摄的照片分享给自己认为最要好的朋友，可以特别标注这是个值得纪念的日子，而在往后的每一年，这一天拍摄的照片或者短视频，我们都会以推送的方式，给参与这项事件的用户。而后加入时光机且同样是参与该事件的用户，我们同样会推送。通过此举反复强化用户之间的联系。

## PRD3.核心价值与用户痛点 3%
- 在时光机使用之初的注册阶段，用户就要进行人脸检测，这里就要用到百度人脸识别API人脸检测服务，我们记录了用户的人脸数据，而此后再使用百度人脸识别API中人脸对比的服务，来决定推送对象。
- 而在第二阶段，当数据库中拥有了足够的人脸对比数据时，用户可以通过上传自己小时候或者年代较为久远的照片，形成一个以时间为顺序的画廊。而用户可以标识自己的画像，通过百度人脸识别api中的人脸搜索api，将其他用户照片中的你相匹配，如若这些人的身份被推测为你的同学或者朋友，会将其推送给用户，用户选择是重新建立，或者不建立，或者用其他社交软件加其好友。

## PRD4.人工智能概率性与用户痛点 3%
### 百度AI-人脸识别API-——产品优势
- 人脸识别技术国际领先，识别准确率超过99%，在多个国际公开竞赛中排名第一
- 依托百度深度学习实验室的技术实力，提供稳定、精确的大流量服务，支持毫秒级的识别响应、弹性灵活的高并发承载及99.99%的可靠性保障
- 人脸库支持百万级别的搜索管理。
- 具有活体检测功能，标准化接口封装，提供丰富的HTTP SDK，接入简单，快速上手。

### 可能发生的问题
- 录入人像模糊无法识别。
- 拍摄者手机摄像头出现问题。
- 加了扭曲特效或色彩异常（黑白）的照片或无法识别。
- 网络异常。
### 总结：
- 【时光机智能相册管理】APP运用人脸识别API，自动整理人像照片，在特殊日子予以推送，并记录拍摄相片最多的日子予以记录，本身登陆需要人脸验证进入相册，私密性高，同时又兼顾社交功能，用户能够将自己的相册大批量分享给朋友，亦能在朋友生日时生成相关的照片回味。
- 时光机一项特色功能就是找回以前的朋友，原理就是利用百度人脸识别API中强大的百万级别人脸识别，找到位于其他用户相册中出现的你的脸，进行人脸匹配和信息匹配，而后推荐（可关闭）。
- 在用户上传照片时可能会因为照片的质量问题而无法识别，但是百度人脸识别API可以通过更改图片质量以及活体检测设置来一定程度上保证API可匹配照片。

## PRD5.需求列表与人工智能API加值 3%

| 需求 | API | 重要程度 
| :-----| ----: | ----: 
| 移动端相册保存管理 |  百度人脸识别API人脸对比服务|重要
| 确定照片中的人并匹配用户 |  百度人脸识别API人脸搜索服务|重要
| 在其他用户的相册中找到另一用户用户的脸 | 百度人脸识别API人脸搜索服务|重要
| 相册主人信息录入 |  百度人脸识别API人脸检测服务|次要
| 私密相册主人登入 |  百度人脸识别API人对比测服务|次要

#### 产品定位：
- 轻社交相册管理软件，维系用户与自己小圈子的亲密度

#### 目标用户：
- 有管理相册需求群体，例如班级、家族内，兄弟闺蜜间。

#### 适用场景
- 场景一： 老庞过生日时，APP推送提示给老庞的朋友老王，APP自动生成一个仅包含有老庞相片的画廊，当老王点赞并送上祝福后，（如果老王的相册中有老庞与他的合照）APP会增添老王与老庞的照片加入这个画廊。
- 场景二： 同学聚会过了一年后，“时光机”推送当日拍摄上传的视频以及图片，给去年视频以及相册中所有参与过的用户。
#### 用户需求
- 需求一：移动端相册保存管理
- 需求二：记录好友生日以及公共纪念日（如国庆节、劳动节），个人纪念日（结婚纪念、毕业纪念）等特殊日子提示。
- 需求三：通过信息匹配（如上传同一张照片，或不同照片上出现的同一个人），找到以前失去联系的熟人。

## 原型 20%
原型1.交互及界面设计 5%

原型2.信息设计 5%

原型3.原型文档 5%

原型4.口头操作说明 5%
### 使用者交互与设计（axure产品原型）
[原型](http://jackonz2017.gitee.io/shiguangji-yuanxing/#g=1&p=%E9%A6%96%E9%A1%B5)

## API1.使用水平 5%
### 可用API
· 人脸搜索API
#### 使用水平
##### 人脸搜索API使用测试
- 接口描述：也称为1：N识别，在指定人脸集合中，找到最相似的人脸；
- 进行人脸查找相关操作前，需要进行人脸库操作。
##### 百度AI开放平台-人脸识别API
##### 百度人脸库架构
```
|- 人脸库(appid)
   |- 用户组一（group_id）
      |- 用户01（uid）
         |- 人脸（faceid）
      |- 用户02（uid）
         |- 人脸（faceid）
         |- 人脸（faceid）
         ....
       ....
   |- 用户组二（group_id）
   |- 用户组三（group_id）
   ....
```
##### 关于人脸库的设置限制：
- 每个开发者账号可以创建100个appid；
- 每个appid对应一个人脸库，且不同appid之间，人脸库互不相通；
- 每个人脸库下，可以创建多个用户组，用户组（group）数量没有限制；
- 每个用户组（group）下，可添加无限个user_id，无限张人脸（注：为了保证查询速度，单个group中的人脸容量上限建议为80万）；
- 每个用户（user_id）所能注册的最大人脸数量20；

###### 输入：
```
# encoding:utf-8

import requests

'''
人脸搜索
'''

request_url = "https://aip.baidubce.com/rest/2.0/face/v3/search"

params = {"image":img2, "image_type": "BASE64","group_id_list":"group_repeat,group_233","quality_control":"LOW","liveness_control":"NORMAL"}
access_token = '[24.da074e3129df6a4bf7ae2bad20f070c0.2592000.1579701470.282335-18089226]'
request_url = request_url + "?access_token=" + access_token
headers = {'content-type': 'application/json'}
response = requests.post(request_url, data=params, headers=headers)
if response:
    print (response.json())
```
###### 输出：
```
{'error_code': 0, 'error_msg': 'SUCCESS', 'log_id': 12012575550, 'timestamp': 1577115260, 'cached': 0, 'result': {'face_token': 'a43d347463854de0a38185db6c3b845f', 'user_list': [{'group_id': 'group_repeat', 'user_id': 'jackchan', 'user_info': 'abc', 'score': 96.868911743164}]}}
```
##### Face++旷视AI开放平台-人脸识别API
#####  Face++人脸库架构
```
|- 人脸库(faceset)
   |- 用户组一（faceset_token）
      |- 用户01（face_tokens）
      |- 用户02（face_tokens）
      ....
   |- 用户组二（faceset_token）
   |- 用户组三（faceset_token）
   ....
```
##### 关于人脸库的设置限制：
- 创建一个人脸的集合 FaceSet，用于存储人脸标识 face_token。一个 FaceSet 能够存储10000个 face_token。

###### 输入：
```
# -*- coding: utf-8 -*-
import urllib.request
import urllib.error
import time

http_url = ' https://api-cn.faceplusplus.com/facepp/v3/search'
key = "IpRO_fXwnvj7aVk83DWwTQpBBZ3HSoz1"
secret = "F6MBfAY8TBAiiiszvJxA0g32ooMxq98b"
filepath = r"C:\Users\王鹏杰\Desktop\2019~2020课程\API\2.jpg"

boundary = '----------%s' % hex(int(time.time() * 1000))
data = []
data.append('--%s' % boundary)
data.append('Content-Disposition: form-data; name="%s"\r\n' % 'api_key')
data.append(key)
data.append('--%s' % boundary)
data.append('Content-Disposition: form-data; name="%s"\r\n' % 'api_secret')
data.append(secret)
data.append('--%s' % boundary)
data.append('Content-Disposition: form-data; name="%s"\r\n' % 'faceset_token')
data.append(faceset_token)
data.append('--%s' % boundary)
fr = open(filepath, 'rb')
data.append('Content-Disposition: form-data; name="%s"; filename=" "' % 'image_file')
data.append('Content-Type: %s\r\n' % 'application/octet-stream')
data.append(fr.read())
fr.close()
data.append('--%s' % boundary)
data.append('Content-Disposition: form-data; name="%s"\r\n' % 'return_landmark')
data.append('1')
data.append('--%s' % boundary)
data.append('Content-Disposition: form-data; name="%s"\r\n' % 'return_attributes')
data.append(
    "gender,age,smiling,headpose,facequality,blur,eyestatus,emotion,ethnicity,beauty,mouthstatus,eyegaze,skinstatus")
data.append('--%s--\r\n' % boundary)

for i, d in enumerate(data):
    if isinstance(d, str):
        data[i] = d.encode('utf-8')

http_body = b'\r\n'.join(data)

# build http request
req = urllib.request.Request(url=http_url, data=http_body)

# header
req.add_header('Content-Type', 'multipart/form-data; boundary=%s' % boundary)

try:
    # post data to server
    resp = urllib.request.urlopen(req, timeout=5)
    # get response
    qrcont = resp.read()
    # if you want to load as json, you should decode first,
    # for example: json.loads(qrount.decode('utf-8'))
    print(qrcont.decode('utf-8'))
except urllib.error.HTTPError as e:
    print(e.read().decode('utf-8'))
#  仅仅支持10000张人脸图搜索
```
###### 输出：
```
{"image_id": "0oAp+twc6E/BUVGBGX22wQ==", "faces": [{"face_rectangle": {"width": 130, "top": 99, "left": 140, "height": 130}, "face_token": "9239735ccf3bb2519fdd59c7a2e722d8"}], "time_used": 375, "thresholds": {"1e-3": 62.327, "1e-5": 73.975, "1e-4": 69.101}, "request_id": "1577167555,6d93fed6-ff77-4465-b877-5b57bb19cd1e", "results": [{"confidence": 92.464, "user_id": "", "face_token": "fb68dfa143702e180cf6cbf7ee400534"}]}
```

## API2.使用比较分析 5%
##### 百度人脸搜索API与FACE++人脸搜索API对比
|| 人脸库 | 人脸搜索准确率 |
|--------|:-----:|:-----:|
| 百度| 百度的人脸库可进行80万张图片的人脸检索 | 96.868911743164 |
| FACE++ | FACEset可进行1万张图片的人脸检索 | 92.464% |

## API3.使用后风险报告 5%

## API4.加分项 3%
