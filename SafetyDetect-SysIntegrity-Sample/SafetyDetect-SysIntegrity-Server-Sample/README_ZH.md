# SafetyDetect SysIntegrity Server Sample

[English](https://github.com/HMS-Core/hms-safetydetect-demo-java/blob/master/SafetyDetect-SysIntegrity-Server-Sample/README.md) | 中文

## 目录

 * [介绍](#介绍)
 * [运行步骤](#运行步骤)
 * [支持环境](#支持环境)
 * [示例代码](#示例代码)
 * [许可证](#许可证)


## 介绍
SafetyDetect SysIntegrity Server Sample 提供了在服务端验证结果的示例代码。
## 运行步骤
在运行SafetyDetect SysIntegrity Server Sample之前，请检查是否安装Java以及Maven。

## 支持环境
Java 1.7 及以上

## 示例代码

1. 解析JWS，获取header，payload，signature。
2. 从header中获取证书链，使用HUAWEI CBG root证书对其进行验证。
3. 校验证书链中的叶证书域名，域名：sysintegrity.platform.hicloud.com。
4. 从signature中获取签名，校验其签名。
5. 从payload中获取完整性验证结果，格式和样例摘录如下：
```json
{
    "advice":"RESTORE_TO_FACTORY_ROM",
    "apkCertificateDigestSha256":[
        "yT5JtXRgeIgXssx1gQTsMA9GzM9ER4xAgCsCC69Fz3I="
    ],
    "apkDigestSha256":"6Ihk8Wcv1MLm0O5KUCEVYCI/0KWzAHn9DyN38R3WYu8=",
    "apkPackageName":"com.huawei.hms.safetydetectsample",
    "basicIntegrity":false,
    "nonce":"R2Rra24fVm5xa2Mg",
    "timestampMs":1571708929141
}
```
更多信息请访问
https://developer.huawei.com/consumer/cn/doc/development/HMS-Guides/SafetyDetectSysIntegrityDevelopment 

##  许可证
此代码已获得 [Apache License, version 2.0](http://www.apache.org/licenses/LICENSE-2.0).

