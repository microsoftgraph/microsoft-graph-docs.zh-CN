---
title: 向服务主体授予 appRoleAssignment
description: 向服务主体授予应用程序角色分配。
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 8e8bc455f8b04e4a78bfcad1795917350ec8b86b
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2020
ms.locfileid: "44382656"
---
# <a name="grant-an-approleassignment-to-a-service-principal"></a>向服务主体授予 appRoleAssignment

命名空间：microsoft.graph

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将应用程序角色分配给客户端服务主体。

分配给服务主体的应用程序角色也称为 "[应用程序权限](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types)"。 可以通过应用角色分配或通过[许可体验](https://docs.microsoft.com/azure/active-directory/develop/application-consent-experience)直接授予应用程序权限。

若要向客户端服务主体授予应用程序角色分配，您需要三个标识符：

- `principalId`：要 `id` 向其分配应用角色的客户端服务主体的。
- `resourceId`： `id` `servicePrincipal` 定义了应用程序角色（应用程序权限）的资源（API）。
- `appRoleId`： `id` `appRole` 要分配给客户端服务主体的（在资源服务主体上定义）的。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | AppRoleAssignment、Directory.accessasuser.all、all 和的所有子目录    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|Application | AppRoleAssignment、所有的目录读写。 |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignments
```

> [!NOTE]
> 作为一种最佳做法，我们建议通过[ `appRoleAssignedTo` _资源_服务主体的关系](serviceprincipal-post-approleassignedto.md)创建应用程序角色分配，而不是 `appRoleAssignments` 分配的用户、组或服务主体的关系。

## <a name="request-headers"></a>请求头

| 名称       | 说明|
|:-----------|:----------|
| Authorization | Bearer {token}。必需。  |
| Content-type | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供[appRoleAssignment](../resources/approleassignment.md)对象的 JSON 表示形式。

## <a name="response"></a>响应

如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[appRoleAssignment](../resources/approleassignment.md)对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面是一个请求示例。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_create_approleassignment"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignments
Content-Type: application/json
Content-Length: 110

{
  "principalId": "principalId-value",
  "resourceId": "resourceId-value",
  "appRoleId": "appRoleId-value"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-create-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-create-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-create-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


在此示例中， `{id}` 和 `{principalId-value}` 都是 `id` 分配的客户端服务主体，也是 `{resoruceId}` `id` 资源服务主体（API）的。

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
