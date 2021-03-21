---
title: 获取历史记录
description: 读取 riskyUserHistoryItem 对象的属性和关系。
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: f3af631bc0c49d6b0ea2a71325df2b559917a2e2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959520"
---
# <a name="get-history"></a>获取历史记录
命名空间：microsoft.graph

读取 [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) 对象的属性和关系。


>**注意：** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | IdentityRiskyUser.Read.All、IdentityRiskUser.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | IdentityRiskyUser.Read.All、IdentityRiskUser.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/riskyUsers/{userId}/history
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

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "get_riskyuserhistoryitem_1"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history
```


### <a name="response"></a>响应
**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUserHistoryItem"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": 
  {
    "@odata.type": "#microsoft.graph.riskyUserHistoryItem",
    "id": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69",
    "isDeleted": false,
    "isGuest": false,
    "isProcessing": false,
    "riskLevel": "none",
    "riskState": "remediated",
    "riskDetail": "userPerformedSecuredPasswordReset",
    "riskLastUpdatedDateTime": "2019-05-03T03:50:34.9565578Z",
    "userDisplayName": "Allan Deyoung",
    "userPrincipalName": "AllanD@contoso.OnMicrosoft.com",
    "userId": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69",
    "initiatedBy": "68ca8ec0-11f8-456b-a785-70d9936650d5",
    "activity": {
      "@odata.type": "microsoft.graph.riskUserActivity"
    }
  }
}
```


