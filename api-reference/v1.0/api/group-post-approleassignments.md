---
title: 向组授予 appRoleAssignment
description: 向组授予应用角色分配。
ms.localizationpriority: high
doc_type: apiPageType
ms.prod: groups
author: psignoret
ms.openlocfilehash: 0138fee6bd43e6d15a7f75d4d24baee90e53986c
ms.sourcegitcommit: 4ff6e89e89178cbd5aef8aa019e714d95817fae4
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2022
ms.locfileid: "65016937"
---
# <a name="grant-an-approleassignment-to-a-group"></a>向组授予 appRoleAssignment

命名空间：microsoft.graph

使用此 API 将应用角色分配给组。 该组的所有直接成员都将被视为已分配。 若要向组授予应用角色分配，需使用三个标识符：

- **principalId**：要向其分配应用角色的 **组** 的 ID。
- **resourceId**：已定义应用角色的资源 **servicePrincipal** 的 ID。
- **appRoleId**：要分配给组的 **appRole** （在资源服务主体上定义）的 ID。

要[使用组来管理对应用程序的访问](/azure/active-directory/users-groups-roles/groups-saasapps)，可能还需要其他许可证。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | AppRoleAssignment.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | AppRoleAssignment.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->
```http
POST /groups/{groupId}/appRoleAssignments
```

> [!NOTE]
> 最佳做法是，建议通过 _资源_ 服务主体的 `appRoleAssignedTo` 关系（而不是通过分配的用户、组或服务主体的 `appRoleAssignments` 关系）创建应用角色分配。

## <a name="request-headers"></a>请求标头

| 名称       | 说明|
|:-----------|:----------|
| Authorization | Bearer {token}。必需。  |
| Content-type | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供 [appRoleAssignment](../resources/approleassignment.md) 对象的 JSON 表示形式。

下表显示了创建 [appRoleAssignment](../resources/approleassignment.md) 时所需的属性。 根据需要为 **appRoleAssignment** 指定其他可写属性。

| 属性 | 类型 | 说明 |
|--|--|--|
| appRoleId | Guid | 分配给主体的 [应用角色](../resources/approle.md)的标识符 (**id**)。 必须在资源应用程序的服务主体 (**resourceId**) 上的 **appRoles** 属性中公开此应用角色。 如果资源应用程序尚未声明任何应用角色，则可以指定默认应用角色 ID `00000000-0000-0000-0000-000000000000`，以表示将主体分配给资源应用，但没有任何特定应用角色。 |
| principalId | Guid | [ 组的唯一标识符（**ID**）](../resources/group.md)被授予应用角色。 |
| resourceId | Guid | 已为其分配的资源 [服务主体](../resources/serviceprincipal.md)的唯一标识符 (**id**)。 |


## <a name="response"></a>响应

如果成功，此运营商将在响应正文中返回 `201 Created` 响应代码和 [appRoleAssignment](../resources/approleassignment.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面是一个请求示例。 在此示例中，URL 中的 ID 和 **principalId** 的值都将是已分配组的 ID。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_create_approleassignment_1"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/7679d9a4-2323-44cd-b5c2-673ec88d8b12/appRoleAssignments
Content-Type: application/json

{
  "principalId": "7679d9a4-2323-44cd-b5c2-673ec88d8b12",
  "resourceId": "076e8b57-bac8-49d7-9396-e3449b685055",
  "appRoleId": "00000000-0000-0000-0000-000000000000"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-create-approleassignment-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-create-approleassignment-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-create-approleassignment-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-create-approleassignment-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/group-create-approleassignment-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/group-create-approleassignment-1-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>响应

下面是一个响应示例。 

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('7679d9a4-2323-44cd-b5c2-673ec88d8b12')/appRoleAssignments/$entity",
  "id": "pNl5diMjzUS1wmc-yI2LEkGgWqFFrFdLhG2Ly2CysL4",
  "deletedDateTime": null,
  "appRoleId": "00000000-0000-0000-0000-000000000000",
  "createdDateTime": "2021-02-19T17:55:08.3369542Z",
  "principalDisplayName": "Young techmakers",
  "principalId": "7679d9a4-2323-44cd-b5c2-673ec88d8b12",
  "principalType": "Group",
  "resourceDisplayName": "Yammer",
  "resourceId": "076e8b57-bac8-49d7-9396-e3449b685055"
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
