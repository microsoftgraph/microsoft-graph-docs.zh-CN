---
title: '创建 oAuth2PermissionGrant (委派权限授予) '
description: 创建表示委派权限授予的 oAuth2PermissionGrant 对象。
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: dc32f5ba7ff9ed0ac412bc0257e9dc4c0d345dca
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129658"
---
# <a name="create-oauth2permissiongrant-a-delegated-permission-grant"></a>创建 oAuth2PermissionGrant (委派权限授予) 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建由 [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) 对象表示的委派权限授予。

委派权限授予授权表示客户端应用程序) 的客户端服务主体 (代表已登录用户的 API) 访问代表 API) 的资源服务主体 (，以访问已授予的委派权限限制的访问级别。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | DelegatedPermissionGrant.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Directory.ReadWrite.All |

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

下表显示创建 [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md)时所需的属性。

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
| clientId | 字符串 | **授权** 在访问 API [](../resources/serviceprincipal.md)时代表已登录用户操作的应用程序的客户端服务主体的 ID。 必需。  |
| consentType | String | 指示是否向客户端应用程序授予了模拟所有用户或仅模拟特定用户的授权。 *AllPrincipals* 指示对模拟所有用户的授权。 *主体* 指示对模拟特定用户的授权。 管理员可以代表所有用户授予同意。 在某些情况下，可能会授权非管理员用户代表自己同意某些委派权限。 必需。  |
| principalId | String | 当 **consentType** [为 Principal](../resources/user.md)时，客户端有权访问资源的用户的 **ID。**  如果 **consentType** 为 *AllPrincipals，* 则此值为 null。 当 **consentType** 为 Principal 时 *是必需的*。 |
| resourceId | String | **有权访问** 的资源 [服务主体](../resources/serviceprincipal.md)的 ID。 这标识了客户端有权尝试代表登录用户调用的 API。 |
| scope | String | 委派权限声明值的列表（以空格分隔）应包含在 API (访问令牌) 。 例如，`openid User.Read GroupMember.Read.All`。 每个声明值都应与资源服务主体 的 **publishedPermissionScopes** 属性中列出的 API 定义的委派权限之一的值 [字段匹配](../resources/serviceprincipal.md)。 |
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
  "clientId": "clientId-value",
  "consentType": "consentType-value",
  "principalId": "principalId-value",
  "resourceId": "resourceId-value",
  "scope": "scope-value",
  "startTime": "2016-10-19T10:37:00Z",
  "expiryTime": "2016-10-19T10:37:00Z"
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
  "id": "id-value",
  "clientId": "clientId-value",
  "consentType": "consentType-value",
  "principalId": "principalId-value",
  "resourceId": "resourceId-value",
  "scope": "scope-value",
  "startTime": "2016-10-19T10:37:00Z",
  "expiryTime": "2016-10-19T10:37:00Z"
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


