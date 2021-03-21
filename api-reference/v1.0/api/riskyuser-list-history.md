---
title: 列表历史记录
description: 从历史记录导航属性获取 riskyUserHistoryItems。
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: fb7f5d900ad66a56421db7b0cbf6161aaa0cf460
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959429"
---
# <a name="list-history"></a>列表历史记录
命名空间：microsoft.graph

从历史记录导航属性获取 riskyUserHistoryItems。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户） | IdentityRiskyUser.Read.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | IdentityRiskyUser.Read.All |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/riskyUsers/{riskyUserId}/history
GET /identityProtection/riskyUsers/{riskyUserId}/history/{riskyUserHistoryItemId}/history
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持一些 OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "get_riskyuserhistoryitem_2"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/{riskyUserId}/history
```


### <a name="response"></a>响应
**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.riskyUserHistoryItem)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.riskyUserHistoryItem",
      "id": "5e1d812e-812e-5e1d-2e81-1d5e2e811d5e",
      "isDeleted": "Boolean",
      "isProcessing": "Boolean",
      "riskLastUpdatedDateTime": "String (timestamp)",
      "riskLevel": "String",
      "riskState": "String",
      "riskDetail": "String",
      "userDisplayName": "String",
      "userPrincipalName": "String",
      "userId": "String",
      "initiatedBy": "String",
      "activity": {
          "riskEventTypes": [],
          "detail": "userPerformedSecuredPasswordReset"
      }
    }
  ]
}
```


