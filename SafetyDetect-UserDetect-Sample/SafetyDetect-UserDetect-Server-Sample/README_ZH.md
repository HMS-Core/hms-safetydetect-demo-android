# SafetyDetect UserDetect Server Sample

[English](https://github.com/HMS-Core/hms-safetydetect-demo-java/blob/master/SafetyDetect-UserDetect-Sample/SafetyDetect-UserDetect-Server-Sample/README.md) | 中文


## 目录

 * [介绍](#介绍)
 * [运行步骤](#运行步骤)
 * [支持环境](#支持环境)
 * [示例代码](#示例代码)
 * [许可证](#许可证)


## 介绍
SafetyDetect UserDetect Server Sample提供了获取服务端结果的示例代码.

## 运行步骤
在运行SafetyDetect UserDetect Server Sample之前，请检查是否安装Java以及Maven。
## 支持环境
Java 1.7 及以上

## 示例代码
服务端主要分为两步：
1. 获取accessToken。
2. 调用云侧API获取检测结果。

具体步骤如下：
获取accessToken.
详细请参见[开放平台鉴权相关内容描述](https://developer.huawei.com/consumer/cn/doc/HMSCore-Guides-V5/open-platform-oauth-0000001050123437-V5)。
调用云侧API获取检测结果：调用云侧获取结果。消息请求示例如下所示:

```json
POST https://hirms.cloud.huawei.com/rms/v1/userRisks/verify?appId=123456 HTTP/1.1
Content-Type: application/json;charset=utf-8
{
    "accessToken":"AAWWHI94sgUR2RU5_P1ZptUiwLq7W8XWJO2LxaAPuXw4_HOJFXnBlN-q5_3bwlxVW_SHeDPx_s5bWW-9DjtWZsvcm9CwXe1FHJg0u-D2pcQPcb3sTxDTJeiwEb9WBPl_9w",
    "response":"bc9d6e73-b422-4d7c-8464-2a8b5ad5b525"
}
```
更多信息请访问
https://developer.huawei.com/consumer/cn/doc/development/HMS-Guides/SafetyDetectUserDetectDevelopment 

##  许可证
此示例代码已获得 [Apache License, version 2.0](http://www.apache.org/licenses/LICENSE-2.0).

