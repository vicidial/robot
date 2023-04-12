# jiqiren.github.io



1,vicidial sip robot 对接阿里云智能对话机器人(云小蜜)产品架构图


![89d6bf6c31bfb638009c5db0c9b0bf10](https://user-images.githubusercontent.com/19338645/231347530-614ea60b-6139-4cb4-9335-f7b984fcd945.png)

2,阿里云智能对话机器人 电话号码收集配置:
![img_v2_6753a023-bf08-4b44-a980-3dd969cc7eag](https://user-images.githubusercontent.com/19338645/231347659-01d71f97-df99-4586-9aa9-35dd375bcf3b.jpg)

3,sip对接参数:

* exten => _xxxxxxxx, n, SIPAddHeader(X-AliyunIVR-ConversationId:${UNIQUEID})
* exten => _xxxxxxxx, n, SIPAddHeader(X-AliyunIVR-CallingNumber:${CallerID)})

4,机器人对接参数:
* 电话号码收集:
{action:"CollectedNumber",broadcast:""}
* 挂机:
{action:"hangUp",broadcast:"感谢您的来电,再见"}
* 转人工:
{action:"transferToAgent",broadcast:"正在为您转接人工服务,请稍等"}


微信号联系: vicidial
