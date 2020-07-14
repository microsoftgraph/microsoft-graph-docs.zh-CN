---
title: 获取 raProfileDatabaseEntity
description: 读取 raProfileDatabaseEntity 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5d0dbd34afd108a50a5e91aac414cc19ecd86282
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124241"
---
# <a name="get-raprofiledatabaseentity"></a>获取 raProfileDatabaseEntity

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

读取[raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md)对象的属性和关系。

## <a name="prerequisites"></a>先决条件
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /resourceAccessProfileEntities/{resourceAccessProfileEntitiesId}
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
如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[raProfileDatabaseEntity](../resources/intune-rapolicy-raprofiledatabaseentity.md)对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
GET https://graph.microsoft.com/beta/resourceAccessProfileEntities/{resourceAccessProfileEntitiesId}
```

### <a name="response"></a>响应
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 856

{
  "value": {
    "@odata.type": "#microsoft.graph.raProfileDatabaseEntity",
    "version": 7,
    "isDeleted": true,
    "softDeletedTime": "2016-12-31T23:59:22.6041454-08:00",
    "displayName": "Display Name value",
    "linkedProfileIds": [
      "5b59ac1a-ac1a-5b59-1aac-595b1aac595b"
    ],
    "profileTypeName": "Profile Type Name value",
    "profileBody": "Profile Body value",
    "profileBodyHash": "Profile Body Hash value",
    "platformType": 12,
    "transformedProfileBody": "Transformed Profile Body value",
    "transformedProfileBodyHash": "Transformed Profile Body Hash value",
    "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
    "profileId": "6389d896-d896-6389-96d8-896396d88963",
    "eTag": "ETag value",
    "schemaVersion": "betaStart",
    "lastModified": "2017-01-01T00:03:14.6651031-08:00"
  }
}
```



