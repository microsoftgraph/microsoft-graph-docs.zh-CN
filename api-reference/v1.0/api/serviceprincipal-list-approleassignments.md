---
title: 列出向服务主体授予的 appRoleAssignment
description: 检索向服务主体授予的应用角色分配列表。
ms.localizationpriority: high
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: e14378d9333572e4ae2fdda31e3c8dfcb865591b
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2022
ms.locfileid: "62878370"
---
# <a name="list-approleassignments-granted-to-a-service-principal"></a>列出向服务主体授予的 appRoleAssignment

命名空间：microsoft.graph


检索已向服务主体授予的 [appRoleAssignment](../resources/approleassignment.md) 列表。

分配给服务主体的应用角色也被称为[应用程序权限](/azure/active-directory/develop/v2-permissions-and-consent#permission-types)。 应用程序权限可以通过创建应用角色分配直接授予，或通过[协议体验](/azure/active-directory/develop/application-consent-experience)授予。

>**注意**，此请求可能具有最近授予或删除的应用角色分配的复制延迟。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Application.Read.All、Directory.Read.All、Application.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All  |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Application.Read.All、Directory.Read.All、Application.ReadWrite.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/appRoleAssignments
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。

## <a name="request-headers"></a>请求标头

| 名称           | 说明                |
|:---------------|:---------------------------|
| Authorization  | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [appRoleAssignment](../resources/approleassignment.md) 对象集合。

## <a name="example"></a>示例

### <a name="request"></a>请求

以下是请求检索已分配给服务主体的应用角色的请求示例。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_get_approleassignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/8e881353-1735-45af-af21-ee1344582a4d/appRoleAssignments
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-get-approleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-get-approleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-get-approleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-get-approleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/serviceprincipal-get-approleassignments-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/serviceprincipal-get-approleassignments-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面是一个响应示例。 

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#appRoleAssignments",
  "value": [
    {
      "id": "UxOIjjUXr0WvIe4TRFgqTY4z9Wu5KxpBtlEpoTGjw-A",
      "createdDateTime": "2021-02-02T04:22:45.4980259Z",
      "appRoleId": "e2a3a72e-5f79-4c64-b1b1-878b674786c9",
      "principalDisplayName": "dxprovisioning-graphapi-client",
      "principalId": "8e881353-1735-45af-af21-ee1344582a4d",
      "principalType": "ServicePrincipal",
      "resourceDisplayName": "Microsoft Graph",
      "resourceId": "fea94d6d-b5bf-44d2-a887-4f72a8d74f44"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List appRoleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
