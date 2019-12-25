---
title: 列出 credentialUserRegistrationDetails
description: 获取给定租户的 credentialUserRegistrationDetails 对象的列表。
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: 527576eb416c4459ac8c1e5612d1a33c77c4204c
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868882"
---
# <a name="list-credentialuserregistrationdetails"></a>列出 credentialUserRegistrationDetails

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取给定租户的[credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md)对象的列表。

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
GET /reports/credentialUserRegistrationDetails
```

## <a name="optional-query-parameters"></a>可选查询参数

此函数支持可选的 OData 查询参数 **$filter**。 您可以对[credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md)资源的以下一个或多个属性应用 **$filter** 。

| 属性 | 说明和示例 |
| --------- | ----------------------- |
| userDisplayName | 按用户名称筛选。 例如：`/reports/credentialUserRegistrationDetails?$filter=userDisplayName eq 'Contoso'`。 支持的筛选器`eq`运算符： `startswith()`和。 支持不区分大小写。 |
| userPrincipalName | 按用户主体名称筛选。 例如：`/reports/credentialUserRegistrationDetails?$filter=userPrincipalName eq 'Contoso'`。 支持的筛选器`eq`运算符`startswith()`：和。 支持不区分大小写。 |
| authMethods | 按注册过程中使用的身份验证方法进行筛选。 例如：`/reports/credentialUserRegistrationDetails?$filter=authMethods/any(t:t eq microsoft.graph.registrationAuthMethod'email')`。 支持的筛选器`eq`运算符：。 |
| isRegistered | 筛选已注册自助密码重置（SSPR）的用户。 例如：`/reports/credentialUserRegistrationDetails?$filter=isRegistered eq true`。 支持的筛选器`eq`运算符：。 |
| isEnabled | 筛选已启用 SSPR 的用户。 例如：`/reports/credentialUserRegistrationDetails?$filter=isEnabled eq true`。 支持的 filtter 运算符`eq`：。 |
| isCapable | 筛选已准备好执行密码重置或多重身份验证（MFA）的用户。 例如：`/reports/credentialUserRegistrationDetails?$filter=isCapable eq true`。 支持的筛选器运算符：`eq` |
| isMfaRegistered | 筛选已注册进行 MFA 的用户。 例如：`/reports/credentialUserRegistrationDetails?$filter=isMfaRegistered eq true`。 支持的筛选器`eq`运算符：。 |

## <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| Authorization | 持有者 {token} |
| Content-Type | application/json |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应`200 OK`正文中返回响应代码和[credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md)对象集合。

## <a name="examples"></a>示例

以下示例演示如何调用此 API。

### <a name="request"></a>请求

下面展示了示例请求。

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_credentialuserregistrationdetails"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/credentialUserRegistrationDetails
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-credentialuserregistrationdetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-credentialuserregistrationdetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-credentialuserregistrationdetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面是一个响应示例。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。 所有属性都是从实际调用返回的。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.credentialUserRegistrationDetails",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/reports/$metadata#Collection(microsoft.graph.credentialUserRegistrationDetails)",
  "value":[
    {
      "id" : "id-value",
      "userPrincipalName":"userPrincipalName",
      "userDisplayName": "userDisplayName-value",
      "authMethods": ["email", "mobileSMS"],
      "isRegistered" : false,
      "isEnabled" : true,
      "isCapable" : false,
      "isMfaRegistered" : true
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List credentialUserRegistrationDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
