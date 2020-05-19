---
title: 向用户授予 appRoleAssignment
description: 向用户授予应用程序角色分配。
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 665f73533499b17727b07102a97aef1589f2100a
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290684"
---
# <a name="grant-an-approleassignment-to-a-user"></a>向用户授予 appRoleAssignment

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用此 API 将应用程序角色分配给用户。 若要向用户授予应用程序角色分配，需要三个标识符：

- `principalId`：要 `id` 向其分配应用程序角色的用户。
- `resourceId`： `id` `servicePrincipal` 定义了应用程序角色的资源的。
- `appRoleId`： `id` `appRole` 要分配给用户的（在资源服务主体上定义）的。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | AppRoleAssignment、Directory.accessasuser.all 和所有    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | AppRoleAssignment |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/appRoleAssignments
```

> [!NOTE]
> 作为一种最佳做法，我们建议通过 `appRoleAssignedTo` _资源_服务主体的关系创建应用程序角色分配，而不是 `appRoleAssignments` 分配的用户、组或服务主体的关系。

## <a name="request-headers"></a>请求标头

| 名称       | 说明|
|:-----------|:----------|
| Authorization | Bearer {token}。必需。  |
| Content-Type | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供[appRoleAssignment](../resources/approleassignment.md)对象的 JSON 表示形式。

## <a name="response"></a>响应

如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[appRoleAssignment](../resources/approleassignment.md)对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面是一个请求示例。

<!-- {
  "blockType": "request",
  "name": "user_create_approleassignment"
}-->

```http
POST https://graph.microsoft.com/beta/users/{id}/appRoleAssignments
Content-Type: application/json
Content-Length: 110

{
  "principalId": "principalId-value",
  "resourceId": "resourceId-value",
  "appRoleId": "appRoleId-value"
}
```

在此示例中， `{id}` 和 `{principalId-value}` 都是 `id` 分配的用户的。

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
Content-length: 253

{
  "id": "id-value",
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "principalType": "principalType-value",
  "principalId": "principalId-value",
  "principalDisplayName": "principalDisplayName-value",
  "resourceId": "resourceId-value",
  "resourceDisplayName": "resourceDisplayName-value"
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
