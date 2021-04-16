---
title: 更新 onPremEncryptedPayload
description: 更新 onPremEncryptedPayload 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 79f08c0136bfd941dcae491bc56d1fd1484ffa73
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868378"
---
# <a name="update-onpremencryptedpayload"></a>更新 onPremEncryptedPayload

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [onPremEncryptedPayload 对象](../resources/intune-raimportcerts-onpremencryptedpayload.md) 的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /onPremEncryptedPayloads/{onPremEncryptedPayloadsId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) 对象的 JSON 表示形式。

下表显示创建 [onPremEncryptedPayload 时所需的属性](../resources/intune-raimportcerts-onpremencryptedpayload.md)。

|属性|类型|说明|
|:---|:---|:---|
|tenantId|Guid|尚未记录|
|userId|Guid|尚未记录|
|deviceId|Guid|尚未记录|
|payloadId|Guid|尚未记录|
|deviceKeyThumbprint|String|尚未记录|
|cert1PayloadUUID|String|尚未记录|
|cert2PayloadUUID|String|尚未记录|
|cert3PayloadUUID|String|尚未记录|
|plistTemplate|String|尚未记录|
|encryptedBlob|二进制|尚未记录|
|payloadVersion|Int32|尚未记录|
|状态|Int32|尚未记录|
|createdTime|DateTimeOffset|尚未记录|
|lastModifiedTime|DateTimeOffset|尚未记录|
|eTag|String|尚未记录|
|isDeleted|Boolean|尚未记录|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/onPremEncryptedPayloads/{onPremEncryptedPayloadsId}
Content-type: application/json
Content-length: 781

{
  "@odata.type": "#microsoft.graph.onPremEncryptedPayload",
  "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
  "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
  "deviceId": "6de0af45-af45-6de0-45af-e06d45afe06d",
  "payloadId": "f12f6c03-6c03-f12f-036c-2ff1036c2ff1",
  "deviceKeyThumbprint": "Device Key Thumbprint value",
  "cert1PayloadUUID": "Cert1Payload UUID value",
  "cert2PayloadUUID": "Cert2Payload UUID value",
  "cert3PayloadUUID": "Cert3Payload UUID value",
  "plistTemplate": "Plist Template value",
  "encryptedBlob": "ZW5jcnlwdGVkQmxvYg==",
  "payloadVersion": 14,
  "status": 6,
  "createdTime": "2017-01-01T00:03:18.9597073-08:00",
  "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
  "eTag": "ETag value",
  "isDeleted": true
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 781

{
  "@odata.type": "#microsoft.graph.onPremEncryptedPayload",
  "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
  "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
  "deviceId": "6de0af45-af45-6de0-45af-e06d45afe06d",
  "payloadId": "f12f6c03-6c03-f12f-036c-2ff1036c2ff1",
  "deviceKeyThumbprint": "Device Key Thumbprint value",
  "cert1PayloadUUID": "Cert1Payload UUID value",
  "cert2PayloadUUID": "Cert2Payload UUID value",
  "cert3PayloadUUID": "Cert3Payload UUID value",
  "plistTemplate": "Plist Template value",
  "encryptedBlob": "ZW5jcnlwdGVkQmxvYg==",
  "payloadVersion": 14,
  "status": 6,
  "createdTime": "2017-01-01T00:03:18.9597073-08:00",
  "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
  "eTag": "ETag value",
  "isDeleted": true
}
```




