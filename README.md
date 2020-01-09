## “时光机” 产品PRD
| 发布日期 | 2019.12.6 
| :-----| ----: 
| 产品名称 |  “时光机”智能云相册
| 完成进度 | 完成
| 文件主人 | 王鹏杰
| 设计者| 王鹏杰
| 开发者| 王鹏杰
[演示PPT](# 时光机智能云相册管理)
# PRD价值主张设计 15%
#### 需求背景
- 目前互联网上的许多社交软件，类似于微信和QQ，都是致力于维系用户间的弱联系，工作上的加一下，遇到一个有趣的陌生人也加一下，大家都抱着“加了微信，有了联系以后拜托什么事情也方便”这样的心态增加自己好友列表中的好友。但是毫无疑问的是，随着微信中的称不上熟人的陌生人的增加，微信从一开始设定的强化朋友间联系的作用也在不断缩小。而这种相对于“弱联系”的强联系的小圈子文化，恰恰是市场所缺乏的。
- 时光机最吸引人的不是去到未来，而是回到过去。本产品旨在为用户建造一个熟人间的小圈子，让感情历久弥新，不让好兄弟、好闺蜜尘封在冗长的电话簿中，只是一行单调乏味的数字，或者是那些记不真切的会议。并且在此基础上，为用户提供找回失去的“记忆”，重新将人与人之间脆弱的维系链接起来，从无联系到弱联系，从弱联系变成强联系。
## PRD1.加值宣言 3%
- 一句话版本：一款轻社交智能云相册管理产品
##### 一分钟版本：
###### 重要：
- 运用人脸识别API中的人脸对比服务，在用户上传图片后，自动匹配参与该事件的成员并以特定的时间点予以推送。
- 运用人脸识别API中的人脸搜索服务，当用户上传小时候的照片时，找到其他用户上传的图片中的用户的肖像，通过找相似照片的方式，结合用户提供的生平信息予以匹配。
###### 次要
- 运用人脸识别API中的人脸检测，当用户使用APP时，需进行人脸验证，人脸检测记录用户特征，能够很好的保护用户相册隐私。
#### 核心功能：
- 个人智能云相册，定时自动推送，自动生成用户的照片画廊。

## PRD2.核心价值 3%
- （最小可行性产品）用户可以上传自己所拍摄的照片分享给自己认为最要好的朋友，可以特别标注这是个值得纪念的日子，而在往后的每一年，这一天拍摄的照片或者短视频，我们都会以推送的方式，给参与这项事件的用户。而后加入时光机且同样是参与该事件的用户，我们同样会推送。通过此举反复强化用户之间的联系。
- 在时光机使用之初的注册阶段，用户就要进行人脸检测，这里就要用到百度人脸识别API人脸检测服务，我们记录了用户的人脸数据，而此后再使用百度人脸识别API中人脸对比的服务，来决定推送对象。
- 而在第二阶段，当数据库中拥有了足够的人脸对比数据时，用户可以通过上传自己小时候或者年代较为久远的照片，形成一个以时间为顺序的画廊。而用户可以标识自己的画像，通过百度人脸识别api中的人脸搜索api，将其他用户照片中的你相匹配，如若这些人的身份被推测为你的同学或者朋友，会将其推送给用户，用户选择是重新建立，或者不建立，或者用其他社交软件加其好友。

## PRD3.核心价值与用户痛点 3%
- 场景一：用户想要快速整理相片。
- 场景二：用户想要纪念重要的人或事。
- 场景三：用户想要保护好自己照片的隐私。
- 场景四：用户即将更换新手机，想要一款专门保存管理相册的云服务器。

## PRD4.人工智能概率性与用户痛点 3%
### 百度AI-人脸识别API-——产品优势
- 人脸识别技术国际领先，识别准确率超过99%，在多个国际公开竞赛中排名第一
- 依托百度深度学习实验室的技术实力，提供稳定、精确的大流量服务，支持毫秒级的识别响应、弹性灵活的高并发承载及99.99%的可靠性保障
- 人脸库支持百万级别的搜索管理。
- 具有活体检测功能，标准化接口封装，提供丰富的HTTP SDK，接入简单，快速上手。

### 可能发生的问题
- 单图多人难以准确检测多个人脸。
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
- 场景三： 某天，老王打开时光机，发觉马上竟然是重要的结婚纪恋日，而自己已经忘记了。
- 场景四： 儿子要结婚了，用户打开时光机从中一次性导出所有关于儿子成长的相片，准备在婚礼当天播放。
- 场景五： 即将毕业，同学们老师间依依不舍，老师将每个人的照片存入相册，每年的这一天，相册里的每一张笑脸的主人都会收到一份名为“学生时代”的画廊，重温过去。

#### 用户需求
- 需求一：移动端相册保存管理
- 需求二：记录好友生日以及公共纪念日（如国庆节、劳动节），个人纪念日（结婚纪念、毕业纪念）等特殊日子提示。
- 需求三：通过信息匹配（如上传同一张照片，或不同照片上出现的同一个人），找到以前失去联系的熟人。

## 原型 20%
原型1.交互及界面设计 5%
- （1）在交互及界面设计的核心交互环节3.2上传图片页面，在上传相片后会首先利用百度人脸识别API中的人脸检测，检测出人脸，再利用人脸对比，检测出人脸的主人，如果为用户好友就为该照片打上标签存入相册，方便日后取用——使用了人脸检测API以及人脸对比API的加值。
输入：批量照片
输出：带有标签的照片

- （2）在交互及界面设计的核心交互环节4.0事件页面，时光机会通过人脸对比筛选出对方相册中你的相片以及你相片中他的照片，生成一个画廊，记叙着双方间的相遇以及大大小小以照片为载体的独特画廊——使用了人脸对比API加值。
输入：批量照片
输出：以人物、事件为主角的画廊

- （3）在交互及界面设计的非核心交互环节3.4时光机页面，添加相片，人脸检测出人脸，选择自己的人脸，而后利用人脸搜索，找到存在于陌生人（即不为好友）相册中，选择你的脸，匹配信息进行随机的好友推荐——使用了人脸检测API以及人脸搜索API的加值。
- 输入：批量照片
- 输出：文字信息

原型2.信息设计 5%
- 产品结构图
![产品结构图.png](https://upload-images.jianshu.io/upload_images/9484392-fcf0b42e3d401a81.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
- 产品功能结构
![产品功能结构图.png](https://upload-images.jianshu.io/upload_images/9484392-5e42555876568488.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
- 产品信息架构
![产品信息架构图.png](https://upload-images.jianshu.io/upload_images/9484392-8a49550b0650f400.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

原型3.原型文档 5%
- [原型](http://jackonz2017.gitee.io/shiguangji-yuanxing/#g=1&p=%E9%A6%96%E9%A1%B5)
- [原型下载](https://gitee.com/jackonz2017/shiguangji-yuanxing)

原型4.口头操作说明 5%
![1_0首页.png](https://upload-images.jianshu.io/upload_images/9484392-fd396ab2715fb292.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![2_0好友.png](https://upload-images.jianshu.io/upload_images/9484392-1e1c3fc741cb07f0.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![3_0相册.png](https://upload-images.jianshu.io/upload_images/9484392-102ea3c1bb3e17b9.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![3_1查看相册.png](https://upload-images.jianshu.io/upload_images/9484392-93d93865bc39e092.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![3_2手动上传图片.png](https://upload-images.jianshu.io/upload_images/9484392-8a247d607fdd46f8.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![3_3新增相册.png](https://upload-images.jianshu.io/upload_images/9484392-74e29618b7caa345.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![3_4时光机.png](https://upload-images.jianshu.io/upload_images/9484392-0eac090e575d3de6.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![4_0事件.png](https://upload-images.jianshu.io/upload_images/9484392-54b61e60e4df11f4.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![4_1搜索.png](https://upload-images.jianshu.io/upload_images/9484392-f32a62334ed56108.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![5_0我.png](https://upload-images.jianshu.io/upload_images/9484392-51d68869a1b6d30c.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

## API1.使用水平 5%
### 可用API
· 人脸搜索API
· 人脸对比API
· 人脸检测API
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
##### 百度人脸识别API与FACE++人脸识别API对比
|| 人脸库 | 人脸搜索准确率 |能否单图多人脸检测|价格|是否有免费配额|人脸搜索是否有成熟案例
|--------|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|
| 百度| 百度的人脸库可进行80万张图片的人脸检索 | 96.868911743164 |实现较为困难 |较为便宜，仅为FACE++一半|是|已有市场案例|
| FACE++ | FACEset可进行1万张图片的人脸检索 | 92.464% |能够实现 |较为昂贵|是|官网未发现市场案例|

### 百度-API性价比方面：
- 具有免费的调用额度，个人用户2QPS，企业用户10QPS。QPS为每秒调用次数，也就是说能限速无限量使用接口。
- 如果账号完成企业认证基础服务API并发支持永久赠送 10QPS，折算成实际业务调用次数，相当于每天：最高免费享用 10QPS 24h 3600s = 864000次 有效调用。
- 准化接口封装，提供丰富的HTTP、SDK，接入简单，快速上手；
- 可查链接：[百度AI-人脸识别-产品价格](https://ai.baidu.com/ai-doc/FACE/Uk37c1m9b)

### 百度-API成熟度：
- 应用案例：通鼎互联、小童科技。
- 支持百万级规模的人脸库管理和搜索，检索速度业内领先，可应对各种业务需求。
- 可视化管理，提供可视化人脸库管理功能，支持人脸组、用户、人脸维度的增、删、改、查操作。
- 高精度稳定服务，万级别人脸库首选识别率高达99%以上，付费用户享受全年服务4个9的 SLA保障，客服响应7*24小时
- 在线调用API，提供在线的人脸搜索接口、人脸库管理组合接口，可以快速集成，达到百万人脸库毫秒级检索速度，实现黑白名单自定义匹配等功能。
- 离线识别SDK，集成到单台硬件设备中，实现1万人以内的小型人脸库快速查找，适用于小区门禁、闸机、企业考勤机等场景。
- 私有化部署，提供一体机和软件部署包两种私有化方案，支持百万级人脸库精准查找，毫秒级搜索结果响应，适用于安防、监控等场景。
- 可查链接：[百度AI-人脸识别-产品优势](https://ai.baidu.com/tech/face/search)

### FACE++-API性价比方面：
- API免费调用额度为3QPS（单月内连续调用十天或调用量超过1万的用户即可获得人脸识别API QPS翻倍至6）人脸稠密关键点识别单独为1。
- SDK 不提供免费使用或免费测试。
- Face 存储有上限：每个用户使用免费服务只能创建 1000个 FaceSet，总计最多存储 100 万个人脸。
- FACE++的人脸识别服务中附加功能选择更多。
- 按量计费，API调用即时扣费，使用多少，支付多少。
- 包时计费，付费时段无限量调用，高量低价享用API服务。
- 授权计费，被授权设备在有效期内可无限量使用SDK服务
- 可查链接：[FACE++-人脸识别-产品价格](https://www.faceplusplus.com.cn/v2/pricing/)

### FACE++-API成熟度：
- 不限人脸数量。
- 多种复杂场景识别。
- 可查链接：[FACE++-人脸识别-产品优势](https://www.faceplusplus.com.cn/v2/pricing/)

### 总结：
- 性价比方面，百度人脸识别API相对于而言，虽然免费的额度较低，但是运营费用更低。
- 成熟度方面，百度人脸识别API已经占有一定的市场，已经生产出类似的产品，说明其成熟度要更胜一筹。
- 但从综合能力上来看，FACE++更胜一筹，因为时光机最重要的功能其实就是人脸对比、人脸检测和人脸搜索，虽然百度人脸识别API在人脸搜索，人脸对比上表现不错，然而相对于FACE++来说，百度人脸检测难以分辨出单张照片中的多个人脸，这是比较百度比较欠缺的部分，然而在身份验证上面，百度却因为“活体检测”有着一定的优势。所以在身份验证上，我们团队选择百度API，而主要功能则是选择FACE++的人脸识别API。

## API3.使用后风险报告 5%
### 面临的挑战
- 由姿态引起的面部变化。人脸识别主要还是根据人的面部特征，表象的特征来进行识别的，所以当你的姿态发生大的变化，面部会发生很大的变化。
- 光照对人脸识别的影响。
- 遮挡等外部干扰，比如一个人戴着墨镜就会把面部的重要信息遮挡住了。
- 因为运动模糊、摄像机没有对焦准确，造成的这种拍照的模糊也会对人脸识别造成影响。
- 人生理上的变化。比如说随着年龄的变化，一个人从少年变成青年，变成老年，他的容貌可能会发生比较大的变化，这也会造成这个表象的变化比较大，从而导致识别率的下降。其次是双胞胎的问题，人脸识别系统究竟能不能正确的识别出来，这个其实在学术界也是有争论的，有一派是认为双胞胎根本不应该靠人脸识别技术进行分辨，它是没法用人脸识别技术来准确进行区分的。
- [参考文献]("https://www.lubanzhang.com/news/industry/187.html")

### 目前和未来发展性
- 基于大数据的大规模人脸检索是人脸识别技术未来发展的重要方向。例如，在公安领域已经进入了大数据时代，出现了传统的技术瓶颈，利用人脸识别技术，利用这些大量的照片数据，提高公安信息化管理水平，是未来人脸识别技术发展的重要方向。
- 深度学习将人脸识别的准确度提升至肉眼级别，大大拓展了2D人脸识别的应用场景，并借助互联网金融爆发的东风，步入金融应用并作为基础设施迅速普及。除此之外，随着互联网金融等业务对身份认证需求的激增，第三方认证服务平台就会出现，基于提供服务的平台型收益模型发展的空间就很大。
- 随着我国城市化进程的加快，社会稳定和城市安全等问题逐渐显现，人脸识别技术是实现安全城市的关键技术。因此，随着智慧城市的大规模建设，人脸识别技术的应用将是未来的一个新趋势。
- 随着面部识别技术的进一步发展，安防行业的快速发展为安全行业开辟了新的市场，同时为面部识别的应用提供了有益的舞台。分析表明，智能视频分析是大安市场未来的方向之一，人脸识别是其中非常重要的技术和应用
- 于人脸识别技术的便利性、安全性，可以作为智能家居的门禁系统和认证系统使用，智能家居和人脸识别技术的融合是未来发展的重点方向。智能家电中的人脸识别技术是融合嵌入式操作系统和内嵌式硬件平台创建的，提升了人脸识别系统与智能家电运用的融合度，具备定义新、应用性强等特性。
- [人脸识别行业发展趋势]("http://www.sohu.com/a/315210405_440324")

### API市场竞争度
- 目前API市场上，提供“人脸识别”这一API接口服务的公司还是比较多的，例如百度、阿里、腾讯、微软、FACE++等等，市场竞争激烈；
- 不同的厂商，人脸识别API也有不同的优缺点，我们只能根据其不同的优点选择API。

## API4.加分项 3%
- [API调用数据ipynb](http://jackonz2017.gitee.io/qimoapi/)
