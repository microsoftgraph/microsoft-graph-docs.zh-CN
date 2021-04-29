---
title: 向服务主体授予 appRoleAssignment
description: 向服务主体授予应用角色分配。
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: e8021b9bcc96e0a70a139e5d4fd1597f186ab20b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054418"
---
# <a name="grant-an-approleassignment-to-a-service-principal"></a>向服务主体授予 appRoleAssignment

命名空间：microsoft.graph


向客户端服务主体分配一个应用角色。

分配给服务主体的应用角色也被称为[应用程序权限](/azure/active-directory/develop/v2-permissions-and-consent#permission-types)。 应用程序权限可以通过应用角色分配直接授予，或通过[协议体验](/azure/active-directory/develop/application-consent-experience)授予。

若要向客户端服务主体授予应用角色分配，需使用三个标识符：

- `principalId`： 或要向其分配应用角色的客户端服务主体的 `id`。
- `resourceId`：已定义应用角色（应用程序权限）的资源 `servicePrincipal` (API) 的 `id`。
- `appRoleId`：要分配给客户端服务主体的 `appRole`（在资源服务主体上定义）的 `id`。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | AppRoleAssignment.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | AppRoleAssignment.ReadWrite.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignments
```

> [!NOTE]
> 最佳做法是，建议通过 [`appRoleAssignedTo`_资源_ 服务主体](serviceprincipal-post-approleassignedto.md)的关系（而不是通过分配的用户、组或服务主体的`appRoleAssignments`关系）创建应用角色分配。

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
  "name": "serviceprincipal_create_approleassignment"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/9028d19c-26a9-4809-8e3f-20ff73e2d75e/appRoleAssignments
Content-Type: application/json

{
  "principalId": "9028d19c-26a9-4809-8e3f-20ff73e2d75e",
  "resourceId": "8fce32da-1246-437b-99cd-76d1d4677bd5",
  "appRoleId": "498476ce-e0fe-48b0-b801-37ba7e2685c6"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-create-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-create-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-create-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-create-approleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


请注意，在本示例中，请求 URL (`9028d19c-26a9-4809-8e3f-20ff73e2d75e`) 中用作服务主体 **id** 的值与正文中的 **principalId** 属性相同。**resourceId** 的值是资源服务主体（该 API）的 **id**。

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#appRoleAssignments/$entity",
  "id": "2jLOj0YSe0OZzXbR1Gd71fDqFUrPM1xIgUfvWBHJ9n0",
  "createdDateTime": "2021-02-15T16:39:38.2975029Z",
  "appRoleId": "498476ce-e0fe-48b0-b801-37ba7e2685c6",
  "principalDisplayName": "Fabrikam App",
  "principalId": "9028d19c-26a9-4809-8e3f-20ff73e2d75e",
  "principalType": "ServicePrincipal",
  "resourceDisplayName": "Microsoft Graph",
  "resourceId": "8fce32da-1246-437b-99cd-76d1d4677bd5"
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
