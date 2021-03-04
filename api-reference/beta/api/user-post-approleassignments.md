---
title: 向用户授予 appRoleAssignment
description: 向用户授予应用角色分配。
localization_priority: Priority
doc_type: apiPageType
ms.prod: users
author: psignoret
ms.openlocfilehash: 6c3ff85213332b5cc6a1585834d0b2a52c0c6fce
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444754"
---
# <a name="grant-an-approleassignment-to-a-user"></a>向用户授予 appRoleAssignment

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用此 API 将应用角色分配给用户。 若要向用户授予应用角色分配，需使用三个标识符：

- `principalId`：要向其分配应用角色的用户的 `id`。
- `resourceId`：已定义应用角色的资源 `servicePrincipal` 的 `id`。
- `appRoleId`：要分配给用户的 `appRole`（在资源服务主体上定义）的 `id`。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | AppRoleAssignment.ReadWrite.All、Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | AppRoleAssignment.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/appRoleAssignments
```

> [!NOTE]
> 最佳做法是，建议通过 _资源_ 服务主体的 `appRoleAssignedTo` 关系（而不是通过分配的用户、组或服务主体的 `appRoleAssignments` 关系）创建应用角色分配。

## <a name="request-headers"></a>请求标头

| 名称       | 说明|
|:-----------|:----------|
| Authorization | Bearer {token}。必需。  |
| Content-Type | application/json. Required. |

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
  "name": "user_create_approleassignment"
}-->

```http
POST https://graph.microsoft.com/beta/users/cde330e5-2150-4c11-9c5b-14bfdc948c79/appRoleAssignments
Content-Type: application/json

{
  "principalId": "cde330e5-2150-4c11-9c5b-14bfdc948c79",
  "resourceId": "8e881353-1735-45af-af21-ee1344582a4d",
  "appRoleId": "00000000-0000-0000-0000-000000000000"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-create-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-create-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-create-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-create-approleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


在此示例中，`{id}` 和 `{principalId-value}` 均为已分配用户的 `id`。

### <a name="response"></a>响应

下面是一个响应示例。 

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('cde330e5-2150-4c11-9c5b-14bfdc948c79')/appRoleAssignments/$entity",
  "id": "5TDjzVAhEUycWxS_3JSMeY-oHkjrWvBKi7aIZwYGQzg",
  "deletedDateTime": null,
  "appRoleId": "00000000-0000-0000-0000-000000000000",
  "createdDateTime": "2021-02-15T10:31:53.5164841Z",
  "principalDisplayName": "Megan Bowen",
  "principalId": "cde330e5-2150-4c11-9c5b-14bfdc948c79",
  "principalType": "User",
  "resourceDisplayName": "dxprovisioning-graphapi-client",
  "resourceId": "8e881353-1735-45af-af21-ee1344582a4d"
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


