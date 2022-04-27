---
title: " (委派的权限授予) 创建 oAuth2PermissionGrant"
description: 创建一个 oAuth2PermissionGrant 对象，表示委派的权限授予。
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 150b501fd5fd1d751fdbdd3dfdc204ea863b6e2f
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2022
ms.locfileid: "65060687"
---
# <a name="create-oauth2permissiongrant-a-delegated-permission-grant"></a> (委派的权限授予) 创建 oAuth2PermissionGrant

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建由 [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) 对象表示的委派权限授予。

委托的权限授权授权客户端服务主体 (表示客户端应用程序) ，以代表已登录用户访问代表 API) 的资源服务主体 (访问受授予的委派权限限制的访问级别。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | DelegatedPermissionGrant.ReadWrite.All、Directory.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | DelegatedPermissionGrant.ReadWrite.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /oauth2PermissionGrants
```

## <a name="request-headers"></a>请求标头

| 名称       | 类型 | 说明 |
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

在请求正文中，提供 [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) 对象的 JSON 表示形式。

下表显示了创建 [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) 时所需的属性。

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
| clientId | 字符串 | 应用程序的客户端 [服务主体](../resources/serviceprincipal.md)**的 ID**，该应用程序有权在访问 API 时代表已登录用户执行操作。 必需。  |
| consentType | String | 指示是否授予客户端应用程序模拟所有用户或仅特定用户的授权。 *AllPrincipals* 指示授权模拟所有用户。 *主体* 指示授权模拟特定用户。 管理员可以代表所有用户授予同意。 在某些情况下，对于某些委派的权限，非管理员用户可能有权代表自己同意。 必需。  |
| principalId | String | 当 **consentType** 为 *主体* 时，客户端有权访问资源的 [用户](../resources/user.md) **ID**。 如果 **consentType** 为 *AllPrincipals* ，则此值为 null。 如果 **consentType** 是主体，则为必需 *。* |
| resourceId | String | 有权访问权限的资源 [服务主体](../resources/serviceprincipal.md)的 **ID**。 这将标识客户端有权代表已登录用户尝试调用的 API。 |
| scope | String | 委托权限的声明值的空格分隔列表，应包含在资源应用程序的访问令牌中， (API) 。 例如，`openid User.Read GroupMember.Read.All`。 每个声明值应与由 API 定义的委托权限之一的 **值** 字段匹配，该权限在资源 [服务主体](../resources/serviceprincipal.md)的 **publishedPermissionScopes** 属性中列出。 |
| startTime | DateTimeOffset | 目前，将忽略开始时间值，但需要一个值。 必需。 |
| expiryTime | DateTimeOffset | 目前，将忽略结束时间值，但需要一个值。 必需。 |

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 200 系列响应代码和新的 [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_oAuth2PermissionGrant"
}-->

```http
POST https://graph.microsoft.com/beta/oauth2PermissionGrants
Content-Type: application/json

{
    "clientId": "ef969797-201d-4f6b-960c-e9ed5f31dab5",
    "consentType": "AllPrincipals",
    "resourceId": "943603e4-e787-4fe9-93d1-e30f749aae39",
    "scope": "DelegatedPermissionGrant.ReadWrite.All",
    "startTime": "2022-03-17T00:00:00Z",
    "expiryTime": "2023-03-17T00:00:00Z"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-oauth2permissiongrant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/post-oauth2permissiongrant-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/post-oauth2permissiongrant-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant"
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#oauth2PermissionGrants/$entity",
    "clientId": "ef969797-201d-4f6b-960c-e9ed5f31dab5",
    "consentType": "AllPrincipals",
    "expiryTime": "2023-03-17T00:00:00Z",
    "id": "l5eW7x0ga0-WDOntXzHateQDNpSH5-lPk9HjD3Sarjk",
    "principalId": null,
    "resourceId": "943603e4-e787-4fe9-93d1-e30f749aae39",
    "scope": "DelegatedPermissionGrant.ReadWrite.All",
    "startTime": "2022-03-17T00:00:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update oAuth2PermissionGrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


