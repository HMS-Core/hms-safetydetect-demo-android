# SafetyDetect UserDetect Server Sample

English | [中文](https://github.com/HMS-Core/hms-safetydetect-demo-java/blob/master/SafetyDetect-UserDetect-Sample/SafetyDetect-UserDetect-Server-Sample/README_ZH.md)


## Table of Contents

 * [Introduction](#introduction)
 * [Installation](#installation)
 * [Configuration ](#configuration )
 * [Supported Environments](#supported-environments)
 * [Sample Code](#sample-code)
 * [License](#license)


## Introduction
SafetyDetect UserDetect Server Sample provides sample program to obtain the detection result.

## Getting Started
Before using SafetyDetect UserDetect Server Sample code, check whether java environment and Maven has been installed.
Decompress the SafetyDetect UserDetect Server sample code package.

## Supported Environments
Java 1.7 or a later version is recommended.

## Configuration
No additional configuration is required.

## Sample Code
Perform the following steps on the server:
1. Obtain an access token.
2. Call the cloud-side API to obtain the detection result.

The procedure is as follows:
Obtain an access token.
For details, please refer to Open Platform Authentication.
Call the cloud-side API to obtain the detection result. The following is a request example:

```json
POST https://hirms.cloud.huawei.com/rms/v1/userRisks/verify?appId=123456 HTTP/1.1
Content-Type: application/json;charset=utf-8
{
    "accessToken":"AAWWHI94sgUR2RU5_P1ZptUiwLq7W8XWJO2LxaAPuXw4_HOJFXnBlN-q5_3bwlxVW_SHeDPx_s5bWW-9DjtWZsvcm9CwXe1FHJg0u-D2pcQPcb3sTxDTJeiwEb9WBPl_9w",
    "response":"bc9d6e73-b422-4d7c-8464-2a8b5ad5b525"
}
```
More API information please visit 
https://developer.huawei.com/consumer/en/doc/development/HMS-Guides/SafetyDetectUserDetectDevelopment 

##  License
SafetyDetect UserDetect Server Sample is licensed under the [Apache License, version 2.0](http://www.apache.org/licenses/LICENSE-2.0).

