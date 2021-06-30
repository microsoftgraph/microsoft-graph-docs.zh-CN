---
title: cloudPcAuditEvent：getAuditActivityTypes
description: 按租户 ID 获取审核活动类型。
author: ecmadao
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: a6e5fd01d0b2100affa6b5d89c43a50cddbaa533
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211221"
---
# <a name="cloudpcauditevent-getauditactivitytypes"></a>cloudPcAuditEvent：getAuditActivityTypes

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

按租户 ID 获取审核活动类型。

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型| 权限（从最低特权到最高特权） |
|:---|:---|
|委派（工作或学校帐户）|CloudPC.Read.All、CloudPC.ReadWrite.All|
|委派（个人 Microsoft 帐户） | 不支持。|
|应用程序|CloudPC.Read.All、CloudPC.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码 `200 OK` 和 String 集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "cloudpcauditevent_getauditactivitytypes"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/auditEvents/getAuditActivityTypes
```

### <a name="response"></a>响应


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Edm.String)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    "Get Audit Activity Types value"
  ]
}
```
