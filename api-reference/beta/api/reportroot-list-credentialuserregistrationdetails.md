---
title: 列出 credentialUserRegistrationDetails
description: 获取给定租户的 credentialUserRegistrationDetails 对象列表。
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: bf6e99722c44ff0054869056be09314d6befac59
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136666"
---
# <a name="list-credentialuserregistrationdetails"></a>列出 credentialUserRegistrationDetails

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取给定租户 [的 credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) 对象列表。

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

## <a name="optional-query-parameters"></a>可选的查询参数

此函数支持可选的 OData 查询 **参数**$filter。 可以将 **$filter凭据**[UserRegistrationDetails](../resources/credentialuserregistrationdetails.md)资源的以下一个或多个属性应用。

| 属性 | 说明和示例 |
| --------- | ----------------------- |
| userDisplayName | 按用户名筛选。 例如：`/reports/credentialUserRegistrationDetails?$filter=userDisplayName eq 'Contoso'`。 支持的筛选器运算符： `eq` 和 `startswith()` 。 支持不区分大小写。 |
| userPrincipalName | 按用户主体名称进行筛选。 例如：`/reports/credentialUserRegistrationDetails?$filter=userPrincipalName eq 'Contoso'`。 支持的筛选器运算符： `eq` 和 `startswith()` 。 支持不区分大小写。 |
| authMethods | 按注册期间使用的身份验证方法进行筛选。 例如：`/reports/credentialUserRegistrationDetails?$filter=authMethods/any(t:t eq microsoft.graph.registrationAuthMethod'email')`。 支持的筛选器运算符： `eq` . |
| isRegistered | 筛选已注册 SSPR 服务中的自助服务密码重置 (用户) 。 例如：`/reports/credentialUserRegistrationDetails?$filter=isRegistered eq true`。 支持的筛选器运算符： `eq` . |
| isEnabled | 筛选已启用 SSPR 的用户。 例如：`/reports/credentialUserRegistrationDetails?$filter=isEnabled eq true`。 支持的筛选运算符： `eq` . |
| isCapable | 筛选准备在 MFA 服务中执行密码重置或多重 (的用户) 。 例如：`/reports/credentialUserRegistrationDetails?$filter=isCapable eq true`。 支持的筛选器运算符： `eq` |
| isMfaRegistered | 筛选为 MFA 注册的用户。 例如：`/reports/credentialUserRegistrationDetails?$filter=isMfaRegistered eq true`。 支持的筛选器运算符： `eq` . |

## <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| Authorization | 持有者 {token} |
| Content-Type | application/json |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回响应代码 `200 OK` 和 [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) 对象集合。

## <a name="examples"></a>示例

以下示例演示如何调用此 API。

### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_credentialuserregistrationdetails"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/credentialUserRegistrationDetails
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-credentialuserregistrationdetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-credentialuserregistrationdetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-credentialuserregistrationdetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-credentialuserregistrationdetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。 从实际调用中返回所有属性。

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


