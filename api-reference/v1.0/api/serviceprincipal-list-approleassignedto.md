---
title: 为服务主体授予的列表 appRoleAssignments
description: 检索为服务主体授予的应用程序角色分配的列表。
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 17916fb43cbe8d994a54cd1d52e5b2378bc3050a
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44288696"
---
# <a name="list-approleassignments-granted-for-a-service-principal"></a>为服务主体授予的列表 appRoleAssignments

命名空间：microsoft.graph

检索已授予给定资源服务主体的用户、组或客户端服务主体的[appRoleAssignment](../resources/approleassignment.md)列表。

例如，如果资源服务主体是 Microsoft Graph API 的服务主体，这将返回所有已向其授予了对 Microsoft Graph 的仅限应用程序权限的服务主体。

如果资源服务主体是向用户和组授予应用程序角色的应用程序，这将返回为此应用程序分配的应用程序角色的所有用户和组。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | "AppRoleAssignment"、"全部"、"全部"、"Directory.accessasuser.all"、"全部"、"全部"、"directory"  |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | "AppRoleAssignment"、"全部"、"全部"、"全部"、"全部"、"目录" |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/appRoleAssignedTo
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

如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[appRoleAssignment](../resources/approleassignment.md)对象集合。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面的示例演示了检索已授予给定资源服务主体的应用程序角色分配的请求。

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_get_approleassignedto"
}-->

```http
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/appRoleAssignedTo
```

### <a name="response"></a>响应

下面是一个响应示例。 

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 306

{
  "value": [
    {
      "creationTimestamp": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "principalDisplayName": "principalDisplayName-value",
      "principalId": "principalId-value",
      "principalType": "principalType-value",
      "resourceDisplayName": "resourceDisplayName-value"
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
