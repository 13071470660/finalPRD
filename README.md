# 食别PRD
- 20*20：[点击直接查看（无法自动播放ppt和音频）](https://kdocs.cn/l/svedM7voS?f=111)或[下载ppt](https://github.com/13071470660/finalPRD/blob/master/2020.pptx)
## 一、价值主张设计
- 一句话价值主张：为用户提供便捷的菜品记录体验，用户不需要打字输入菜单，只需要对着餐盘拍一张照片，就可以记录这一顿饭所吃的菜品和热量。
- 一分钟价值主张：为用户提供便捷的菜品记录体验和识别不认识的菜品、果蔬体验，用户不需要打字输入菜单，只需对着餐盘拍一张照片或上传菜品照片，应用可通过菜品识别功能自动返回菜品信息，包括菜名、卡路里、营养成分等，用户只需选择份量（如半碗），系统可自动推算该份量的卡路里数并记录。若识别有误，用户可以便捷地选择系统选出的其他三个相似菜品作为纠正，系统可通过用户的纠正反馈加强识别能力，提高识别准确率。

### 产品概述
用户可以使用该应用记录每日食谱，通过拍照识别当天菜品，记录自己的饮食习惯和营养摄入，或者在生活中遇到不认识的美食、果蔬，也可使用该应用拍照识别一下，就可以得知菜品的相关信息，包括名称、热量、营养价值、不适人群等。该应用帮助用户记录饮食、识别菜品的同时，还会推荐健康的饮食搭配。

### 加值宣言
1. 百度AI菜品识别api
- 用户不需要打字输入菜单，只需要对着餐盘拍一张照片，就可以记录这一顿饭所吃的菜品和热量。
- 用户在生活中遇到不认识的美食，可使用该应用拍照识别一下，就可以得知菜品的相关信息，包括名称、热量、营养价值、不适人群等
- 百度菜品识别api可识别超过9千种菜品，准确识别图片中的菜品名称、位置，并获取百科信息。
2. 百度AI果蔬识别api
- 根据拍摄照片，识别图片中果蔬名称，帮助用户识别日常生活中遇到的不认识的果蔬，可结合识别结果进一步为用户提供营养价值、搭配禁忌，果蔬推荐等相关信息。

### 核心价值
用户可以通过识别菜品，得知“这是什么菜？吃这个会不会胖？我能不能吃？我能吃多少？”并且用户只需通过“拍一张照片”的方式即可快速记录自己的饮食包括热量、营养物质等的摄入。

### 目标用户
- 有减肥需求的人
- 追求养生、健康生活的人
- 患有三脂高等方面身体不适人群
- 需要自己下厨但是对食材不了解的厨房新手
 
### 用户痛点
- 现有的饮食记录app一般采用用户自行手动打字输入菜品的方式来记录饮食，菜品输入记录的操作虽不算繁琐，但由于每日需记录饮食的次数约3次，不便的打字输入记录方式多少令用户感到麻烦，很难令用户养成习惯，甚至放弃记录。
- 想保持饮食健康但不知道如何搭配食物，面对美食不知道它的热量、成分是否符合健康需求、可以吃多少？
- 用户在生活中会遇到不认识的菜品、果蔬，想了解其热量、营养、成分、不适人群等。
- 出于身体健康方面的限制，很多食物不能多食，但是不知如何分辨哪些食材是禁忌多食的

### AI概率性考量
![](https://upload-images.jianshu.io/upload_images/9457515-f78f5005601a86ee.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![](https://upload-images.jianshu.io/upload_images/9457515-2829f6f4b1097012.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

百度菜品识别api精确度有待考量。图一上传图片为红丝绒蛋糕，返回结果置信度首位“千层”明显错误，但候补有出现“蛋糕”等类似菜品；图二上传图片实为姜撞奶，返回结果为置信度第一为双皮奶，并且没有出现“姜撞奶”这一推测结果。在菜品之间相似度高的情况下，容易出现识别不精确的现象。
## 需求列表与人工智能API加值
使用场景 | 用户需求 | 重要性  | 技术 |  
-|-|-|-
用户饭前拍照记录菜单 | 记录自己的饮食习惯，计算每日摄入的热量、营养等 | 非常重要 | 百度AI菜品识别api |
用户在生活中会遇到不了解的菜品 | 了解其热量、营养成分、不适人群等，并分析自己是否可以吃，能吃多少 | 非常重要 | 百度AI菜品识别api|
用户在生活中会遇到不认识的果蔬 | 了解其热量、营养成分、不适人群等，并分析自己是否可以吃，能吃多少 | 重要 | 百度AI果蔬识别api|

## 二、原型
- [产品原型](http://nfunm033.gitee.io/food_separation)
-----
1.记录模块

![](https://upload-images.jianshu.io/upload_images/9457515-e9e7e436fe509c75.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![](https://upload-images.jianshu.io/upload_images/9457515-4cea0d3b737af773.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![](https://upload-images.jianshu.io/upload_images/9457515-0acaf61f507cb749.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![](https://upload-images.jianshu.io/upload_images/9457515-4ddc2ab0fb49e965.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

2.搜索模块

![](https://upload-images.jianshu.io/upload_images/9457515-5c77292e4c0da31b.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

3.我模块

![](https://upload-images.jianshu.io/upload_images/9457515-2bc6e75669a3c321.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![](https://upload-images.jianshu.io/upload_images/9457515-ce77564fd112dcf5.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![](https://upload-images.jianshu.io/upload_images/9457515-d6453159ddce4a8e.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

### 产品结构图
1.  产品功能结构图

![](https://upload-images.jianshu.io/upload_images/9457515-f859324fd4000690.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


2. 产品流程图

![](https://upload-images.jianshu.io/upload_images/9457515-f9964a615b3f4bbd.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)



## 三、API的运用
### 三家菜品识别api的运用尝试：
#### 1. 百度-菜品识别
- [接口文档](https://ai.baidu.com/ai-doc/IMAGERECOGNITION/Kk3bcxbxj)
- 接口描述：该请求用于菜品识别。即对于输入的一张图片（可正常解码，且长宽比适宜），输出图片的菜品名称、卡路里信息、置信度。
- 接口地址：https://aip.baidubce.com/rest/2.0/image-classify/v2/dish
- 请求方式：POST
- 输入：
```
请求示例：
# encoding:utf-8

import requests
import base64

request_url = "https://aip.baidubce.com/rest/2.0/image-classify/v2/dish"
# 二进制方式打开图片文件
f = open('[本地文件]', 'rb')
img = base64.b64encode(f.read())

params = {"image":img,"top_num":5}
access_token = '[调用鉴权接口获取的token]'
request_url = request_url + "?access_token=" + access_token
headers = {'content-type': 'application/x-www-form-urlencoded'}
response = requests.post(request_url, data=params, headers=headers)
if response:
    print (response.json())
```

- 输出：
```
返回示例：
HTTP/1.1 200 OK
x-bce-request-id: 73c4e74c-3101-4a00-bf44-fe246959c05e
Cache-Control: no-cache
Server: BWS
Date: Tue, 18 Oct 2016 02:21:01 GMT
Content-Type: application/json;charset=UTF-8
{
	"log_id": 7357081719365269362,
	"result_num": 5,
	"result": [
	{
		"calorie": "119",
		"has_calorie": true,
		"name": "酸汤鱼",
		"probability": "0.396031"
		"baike_info": {
			"baike_url": "http://baike.baidu.com/item/%E9%85%B8%E6%B1%A4%E9%B1%BC/1754055",
			"description": "酸汤鱼，是黔桂湘交界地区的一道侗族名菜，与侗族相邻的苗、水、瑶等少数民族也有相似菜肴，但其中以贵州侗族酸汤鱼最为有名，据考证此菜肴最早源于黎平县雷洞镇牙双一带。制作原料主要有鱼肉、酸汤、山仓子等香料。成菜后，略带酸味、幽香沁人、鲜嫩爽口开胃，是贵州“黔系”菜肴的代表作之一。这道菜通常先自制酸汤，之后将活鱼去掉内脏，入酸汤煮制。"
		}
	},
	{
		"calorie": "38",
		"has_calorie": true,
		"name": "原味黑鱼煲",
		"probability": "0.265432",

	},
	{
		"calorie": "144",
		"has_calorie": true,
		"name": "椒鱼片",
		"probability": "0.0998993"
	},
	{
		"calorie": "98",
		"has_calorie": true,
		"name": "酸菜鱼",
		"probability": "0.0701917"
	},
	{
		"calorie": "257.65",
		"has_calorie": true,
		"name": "柠檬鱼",
		"probability": "0.0471465"
	}]
}
```



#### 2. 京东人工智能开放平台-菜品识别
- [接口文档](https://aidoc.jd.com/image/food.html)
- 接口描述：菜品识别API为用户提供菜品识别功能，输入一张菜品图片，返回识别结果——具体菜名及识别所用时间。
- 接口地址：https://aiapi.jd.com/jdai/FoodApi
- 请求方式：POST
- 输入：
```
请求示例：
import wx_sdk

url = 'https://aiapi.jd.com/jdai/FoodApi'
bodyStr = '{"image":"xxx"}' #输入菜品图片
params = { 
    'appkey' : 'your appkey',
    'secretkey' : 'your secretKey'
}

response = wx_sdk.wx_post_req( url, params, bodyStr=bodyStr )
print( response.text )
```
- 输出：
```
返回示例：
{
    "code": "10000",
    "charge": false,
    "remainTimes": 4998,
    "remainSeconds": -1,
    "msg": "查询成功",
    "result": {
               "message":"ok ",
               "status": 1000,
               "used_time": 606 
               "result": "红烧肉"
    }
}
```

#### 3. 北京安捷智合科技-菜品识别
- [接口文档](https://market.aliyun.com/products/57124001/cmapi032952.html?spm=5176.10695662.1996646101.searchclickresult.4b6b8814HdOH7o&aly_as=jDNHy0xE#sku=yuncode2695200001)
- 接口描述:使用人工智能算法，自动根据图像识别菜品，可识别数千种菜品。
- 接口地址：http://dish.market.alicloudapi.com/detection/dish
- 请求方式：POST
- 输入：
```
请求示例：
import urllib, urllib2, sys


host = 'http://dish.market.alicloudapi.com'
path = '/detection/dish'
method = 'POST'
appcode = '你自己的AppCode'
querys = ''
bodys = {}
url = host + path

bodys['image'] = '''image'''
post_data = urllib.urlencode(bodys)
request = urllib2.Request(url, post_data)
request.add_header('Authorization', 'APPCODE ' + appcode)
//根据API的要求，定义相对应的Content-Type
request.add_header('Content-Type', 'application/x-www-form-urlencoded; charset=UTF-8')
response = urllib2.urlopen(request)
content = response.read()
if (content):
    print(content)
```

- 输出：
```
返回示例：
{
  "result": [
    {
      "score": "0.82971",
      "has_calorie": true,
      "calorie": "41",
      "name": "炒青菜"
    },
    {
      "score": "0.085715",
      "has_calorie": true,
      "calorie": "35",
      "name": "白灼菜心"
    },
    {
      "score": "0.084575",
      "has_calorie": true,
      "calorie": "-1",
      "name": "时令蔬菜"
    }
  ]
}
```


### 三家API比较分析：

**1. [百度菜品识别api](https://ai.baidu.com/tech/imagerecognition/dish)**
- **返回信息**：菜名，每100g的卡路里含量，置信度，百科词条名称、图片链接、内容描述，百度百科页面链接
- **产品定价**：![](https://upload-images.jianshu.io/upload_images/9457515-004bbcf01329e6b2.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

**2. [京东人工智能开放平台-菜品识别API](http://neuhub.jd.com/market/api/87)**
- **返回信息**：单个菜名
- **产品定价**：免费试用

**3. [北京安捷智合科技-菜品识别API](https://market.aliyun.com/products/57124001/cmapi032952.html?spm=5176.10695662.1996646101.searchclickresult.4b6b8814HdOH7o&aly_as=jDNHy0xE#sku=yuncode2695200001)**
- **返回信息**：菜名，置信度，卡路里
- **产品定价**：![](https://upload-images.jianshu.io/upload_images/9457515-3f17816a4793bc59.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

#### 对比分析：
- 从功能上看，能返回卡路里含量的有百度菜品API和北京安捷智合科技-菜品识别API，而京东人工智能开放平台-菜品识别API只能返回单个菜品名称。并且，百度菜品识别API还可以返回百科词条名称、图片链接、内容描述，百度百科页面链接等信息。
- 从性价比上看，百度菜品识别API提供的信息更多，价格也相对北京安捷智合科技-菜品识别API来说较低。

### 百度-果蔬识别：
- [接口文档](https://ai.baidu.com/tech/imagerecognition/ingredient)
- 接口描述:使用人工智能算法，自动根据图像识别菜品，可识别数千种菜品。
- 接口地址：https://aip.baidubce.com/rest/2.0/image-classify/v1/classify/ingredient
- 请求方式：POST
- 输入：
```
请求示例：
# encoding:utf-8

import requests
import base64

'''
细粒度图像识别
'''

request_url = "https://aip.baidubce.com/rest/2.0/image-classify/v1/classify/ingredient"
# 二进制方式打开图片文件
f = open('[本地文件]', 'rb')
img = base64.b64encode(f.read())

params = {"image":img}
access_token = '[调用鉴权接口获取的token]'
request_url = request_url + "?access_token=" + access_token
headers = {'content-type': 'application/x-www-form-urlencoded'}
response = requests.post(request_url, data=params, headers=headers)
if response:
    print (response.json())
```

- 输出：
```
返回示例：
HTTP/1.1 200 OK
x-bce-request-id: 73c4e74c-3101-4a00-bf44-fe246959c05e
Cache-Control: no-cache
Server: BWS
Date: Tue, 18 Oct 2016 02:21:01 GMT
Content-Type: application/json;charset=UTF-8
{
    "log_id": 1091287364,
    "result_num": 20,
    "result": [
        {
            "name": "非果蔬食材",
            "score": 0.99999988079071
        },
        {
            "name": "油菜",
            "score": 1.1175458780599e-8
        },
        {
            "name": "蛇果",
            "score": 7.2776291659693e-9
        },
        {
            "name": "国光苹果",
            "score": 5.6971951600815e-9
        },
        {
            "name": "海枣",
            "score": 4.2508210285064e-9
        },
        {
            "name": "琼瑶浆葡萄",
            "score": 4.1451895249622e-9
        },
        {
            "name": "京锐号辣椒",
            "score": 3.9915102334476e-9
        },
        {
            "name": "冬瓜",
            "score": 3.3611948779821e-9
        },
        {
            "name": "长江豆",
            "score": 2.9944848822794e-9
        },
        {
            "name": "黑加仑",
            "score": 2.7750137743254e-9
        },
        {
            "name": "面包果",
            "score": 2.3357531464541e-9
        },
        {
            "name": "椰子",
            "score": 1.9741890344704e-9
        },
        {
            "name": "美人瓜",
            "score": 1.9319581490151e-9
        },
        {
            "name": "莲藕",
            "score": 1.759222323372e-9
        },
        {
            "name": "黑奥林",
            "score": 1.7266311713726e-9
        },
        {
            "name": "芥菜",
            "score": 1.6180708994895e-9
        },
        {
            "name": "样芹菜",
            "score": 1.5472728653876e-9
        },
        {
            "name": "篙巴",
            "score": 1.4084827748562e-9
        },
        {
            "name": "花生",
            "score": 1.3972580870103e-9
        },
        {
            "name": "魁绿猕猴桃",
            "score": 1.3920842256709e-9
        }
    ]
}
```

- 产品定价
![](https://upload-images.jianshu.io/upload_images/9457515-a22d3e949617d899.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


##### [更多API使用示例](http://nfunm033.gitee.io/apifinal/)

### 使用后风险报告
>在第三届图像识别竞赛WebVision中，阿里AI以82.54%的识别准确率击败了来自世界各地的 150 多支队伍，获得了冠军，同时也将万物识别领域的历史纪录提升了3个百分点。 BigVideo和华为云分别获得第二名和第三名。[（查看原文）](https://t.cj.sina.com.cn/articles/view/6502270080/18390c48001900n5nh?from=tech&sudaref=www.baidu.com&display=0&retcode=0)
![](https://upload-images.jianshu.io/upload_images/9457515-7886642fbbabc269.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

>目前，人类对ImageNet图像的识别错误率大约在5%，微软的人工智能系统的错误率为4.94%，谷歌为4.8%。百度如今已将这一错误率进一步降至4.58%，实现了质的飞跃。
百度之所以能够在ImageNet测试中取得佳绩，依靠的是一种名为“深度学习”的算法。“深度学习”是近几年出现的一类新的人工智能技术，计算机学习了更多人类的神经系统。百度近年频繁在人工智能领域加大投资，目前已经建立了巨大的神经网络，也是世界上第一个建立“深度学习”的神经网络的公司，这就犹如火箭引擎，而目前大数据呈几何式增长，为火箭提供燃料。[（查看原文）](http://science.china.com.cn/2015-05/14/content_7905687.htm)

百度的图像识别技术打败微软和谷歌，将错误率降至4.58%，并且拥有成熟先进的“深度学习”算法，令百度在人工智能领域成就突出，但在“图像识别”领域，百度依然存在一些抢镜对手，如阿里AI、BigVideo和华为云。

即使从图像识别的准确率来说，百度不敌阿里AI、BigVideo和华为云，但是百度在图片识别的基础上推出了更细类的“菜品识别”“果蔬识别”，在此app上运用时，识别结果更加精准，返回信息更加全面。

一旦返回的第一结果有误，还可根据置信度排名，列出前3种菜品供用户选择更正，免去用户手动输入更正菜名的麻烦，在优化用户体验的同时，帮助提升图像识别的能力。

百度菜品识别的缺陷是：只能识别单一菜品、无法估计图像中菜品的体积。
