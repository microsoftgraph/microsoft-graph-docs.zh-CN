---
title: 列出 userCredentialUsageDetails
description: 获取给定租户的 userCredentialUsageDetails 对象列表。
ms.localizationpriority: medium
author: besiler
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 3b2efb78529fe0a066ce17f1306574f5ff5f7691
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61011065"
---
# <a name="list-usercredentialusagedetails"></a>列出 userCredentialUsageDetails

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取给定 [租户的 userCredentialUsageDetails](../resources/usercredentialusagedetails.md) 对象列表。 详细信息包括用户信息、重置状态和失败原因。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | Reports.Read.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用                            | Reports.Read.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /reports/userCredentialUsageDetails
```

## <a name="optional-query-parameters"></a>可选的查询参数

此函数支持可选的 OData 查询参数 **$filter。** 你可以将 **$filter** [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) 资源的以下一个或多个属性。

| 属性 | 说明和示例 |
|:--------- |:----------- |
| 功能 | 按要注册的使用情况数据类型 (重置) 。 例如：`/reports/userCredentialUsageDetails?$filter=feature eq 'registration'`。 支持的筛选器运算符： `eq` |
| userDisplayName | 按用户筛选显示名称。 例如：`/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`。 支持的筛选器运算符： `eq` 和 `startswith()` 。 支持不区分大小写。 |
| userPrincipalName  | 按用户主体名称进行筛选。 例如：`/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`。    支持的筛选器运算符： `eq` 和 `startswith()` 。 支持不区分大小写。 |
| isSuccess | 按活动状态筛选。 例如：`/reports/userCredentialUsageDetails?$filter=isSuccess eq true`。 支持的筛选器运算符： `eq` 和 `orderby` 。 |
| authMethod  | 按注册期间使用的身份验证方法进行筛选。 例如：`/reports/userCredentialUsageDetails?$filter=authMethod eq microsoft.graph.usageAuthMethod'email'`。 支持的筛选器运算符 `eq` ：。 |
| failureReason | 如果活动失败， (失败原因筛选) 。 例如：`/reports/userCredentialUsageDetails?$filter=failureReason eq 'Contoso'`。 支持的筛选器运算符： `eq` 和 `startswith()` 。 支持不区分大小写。 |


## <a name="request-headers"></a>请求头

| 名称      |说明|
|:----------|:----------|
| Authorization | 持有者 {token} |
| Content-Type | application/json |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) 对象集合。

## <a name="examples"></a>示例

以下示例演示如何调用此 API。

### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_usercredentialusagedetails"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/userCredentialUsageDetails
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-usercredentialusagedetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-usercredentialusagedetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-usercredentialusagedetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-usercredentialusagedetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-usercredentialusagedetails-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。 所有属性都从实际调用中返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userCredentialUsageDetails",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/reports/$metadata#Collection(microsoft.graph.getUserCredentialUsageDetails)",
  "value":[
    {
      "id" : "id-value",
      "feature":"registration",
      "userPrincipalName":"userPrincipalName-value",
      "userDisplayName": "userDisplayName-value",
      "isSuccess" : true,
      "authMethod": "email",
      "failureReason": "User contacted an admin after trying the email verification option",
      "eventDateTime" : "2019-04-01T00:00:00Z"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List userCredentialUsageDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


