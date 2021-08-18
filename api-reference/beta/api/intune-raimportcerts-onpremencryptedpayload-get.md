---
title: 获取 onPremEncryptedPayload
description: 读取 onPremEncryptedPayload 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f7eaf4e63ac842f16524e4418b23aa56c7b124d76f953e4e613cdca143e1fce1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54145640"
---
# <a name="get-onpremencryptedpayload"></a>获取 onPremEncryptedPayload

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

读取 [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) 对象的属性和关系。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /onPremEncryptedPayloads/{onPremEncryptedPayloadsId}
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
GET https://graph.microsoft.com/beta/onPremEncryptedPayloads/{onPremEncryptedPayloadsId}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 834

{
  "value": {
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
}
```




