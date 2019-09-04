---
title: 列出 riskyUsers
description: 检索**riskyUser**对象集合的属性和关系。
localization_priority: Normal
author: cloudhandler
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 76cba3d86b17445828a34e93653d5f8849affb12
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36722578"
---
# <a name="list-riskyusers"></a>列出 riskyUsers

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索**riskyUser**对象集合的属性和关系。

>**注意:** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | IdentityRiskyUser.Read.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | IdentityRiskyUser.Read.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /riskyUsers
```
## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持`$filter`自定义查询响应。 请参阅本主题后面的示例。 

## <a name="request-headers"></a>请求标头
| 名称      |说明|
|:----------|:----------|
| Authorization  | Bearer {token}。必需。 |
| Workbook-Session-Id  | 用于确定是否保留更改的工作簿会话 ID。 可选。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功, 此方法在响应`200 OK`正文中返回响应代码和[riskyUser](../resources/riskyuser.md)对象集合。

## <a name="examples"></a>示例
### <a name="example-1-list-risky-users"></a>示例 1: 列出有风险的用户
#### <a name="request"></a>请求
下面是一个请求示例。

# <a name="httptabhttp"></a>[HTTP.SYS](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_riskyusers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/riskyUsers
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-riskyusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-riskyusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目标-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-riskyusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应
下面是一个响应示例。
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.riskyUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
        {
            "id": "c2b6c2b9-dddc-acd0-2b39-d519d803dbc3",
            "riskLastUpdatedDateTime": "2016-01-29T20:03:57.7872426Z",
            "isGuest": true,
            "isProcessing": true,
            "isDeleted": true,
            "riskDetail": "adminConfirmedSigninCompromised",
            "riskLevel": "high",
            "riskState": "atRisk",
            "userDisplayName": "Alex Wilbur",
            "userPrincipalName": "alexw@contoso.com"
        }
    ]
}
```

### <a name="example-2-list-risky-users-and-filter-the-results"></a>示例 2: 列出有风险的用户并筛选结果
#### <a name="request"></a>请求
下面的示例演示如何使用`$filter`来获取其聚合风险级别为中的 riskyUser 的集合。


# <a name="httptabhttp"></a>[HTTP.SYS](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_filter_riskyusers"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/beta/riskyUsers?$filter=riskLevel eq microsoft.graph.riskLevel'medium'
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-filter-riskyusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-filter-riskyusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目标-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-filter-riskyusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应
下面是一个响应示例。
<!-- {
  "blockType": "response",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.riskyUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "c2b6c2b9-dddc-acd0-2b39-d519d803dbc3",
            "riskLastUpdatedDateTime": "2018-09-22T00:04:49.1195968Z",
            "isGuest": false,
            "isProcessing": true,
            "isDeleted": false,
            "riskDetail": "none",
            "riskLevel": "medium",
            "riskState": "atRisk",
            "userDisplayName": "Alex Wilbur",
            "userPrincipalName": "alexw@contoso.com",
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
