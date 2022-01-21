---
title: 为服务主体授予 appRoleAssignment
description: 为服务主体授予应用角色分配。
ms.localizationpriority: high
doc_type: apiPageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 833a4c4c147535a8c96c9d881c75d01faf9ee6b3
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62105359"
---
# <a name="grant-an-approleassignment-for-a-service-principal"></a>为服务主体授予 appRoleAssignment

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将资源服务主体的应用角色，分配给用户、组或客户端服务主体。

分配给服务主体的应用角色也被称为[应用程序权限](/azure/active-directory/develop/v2-permissions-and-consent#permission-types)。 应用程序权限可以通过应用角色分配直接授予，或通过[协议体验](/azure/active-directory/develop/application-consent-experience)授予。

若要授予应用角色分配，需使用三个标识符：

- `principalId`： **用户** 的 `id`，**组** 或要向其分配应用程序角色的客户端 **servicePrincipal**。
- `resourceId`：已定义应用角色的资源 **servicePrincipal** 的 `id`。
- `appRoleId`： **appRole** 中的 `id`来分配给用户、组或服务主体。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | AppRoleAssignment.ReadWrite.All 和 Application.Read.All、AppRoleAssignment.ReadWrite.All 和 Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | AppRoleAssignment.ReadWrite.All 和 Application.Read.All、AppRoleAssignment.ReadWrite.All 和 Directory.Read.All、Application.ReadWrite.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignedTo
```

## <a name="request-headers"></a>请求标头

| 名称       | 说明|
|:-----------|:----------|
| Authorization | Bearer {token}。必需。  |
| Content-type | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供 [appRoleAssignment](../resources/approleassignment.md) 对象的 JSON 表示形式。

## <a name="response"></a>响应

如果成功，此运营商将在响应正文中返回 `201 Created` 响应代码和 [appRoleAssignment](../resources/approleassignment.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面是一个请求示例。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_create_approleassignedto"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/9028d19c-26a9-4809-8e3f-20ff73e2d75e/appRoleAssignedTo
Content-Type: application/json

{
  "principalId": "33ad69f9-da99-4bed-acd0-3f24235cb296",
  "resourceId": "9028d19c-26a9-4809-8e3f-20ff73e2d75e",
  "appRoleId": "ef7437e6-4f94-4a0a-a110-a439eb2aa8f7"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-create-approleassignedto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-create-approleassignedto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-create-approleassignedto-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-create-approleassignedto-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/serviceprincipal-create-approleassignedto-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/serviceprincipal-create-approleassignedto-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


在此示例中，`{id}` 和 `{resourceId-value}` 是资源服务主体的 `id`，`{principalId}` 是分配的用户、组或客户端服务主体的 `id`。

### <a name="response"></a>响应

下面是一个响应示例。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#servicePrincipals('9028d19c-26a9-4809-8e3f-20ff73e2d75e')/appRoleAssignedTo/$entity",
  "id": "-WmtM5na7Uus0D8kI1yylpU9Mdo0Pb9OoBJvd3T5eKc",
  "deletedDateTime": null,
  "appRoleId": "ef7437e6-4f94-4a0a-a110-a439eb2aa8f7",
  "creationTimestamp": "2021-02-15T16:14:59.8643039Z",
  "principalDisplayName": "Parents of Contoso",
  "principalId": "33ad69f9-da99-4bed-acd0-3f24235cb296",
  "principalType": "Group",
  "resourceDisplayName": "Fabrikam App",
  "resourceId": "9028d19c-26a9-4809-8e3f-20ff73e2d75e"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
