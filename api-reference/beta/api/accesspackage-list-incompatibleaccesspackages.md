---
title: 列出不兼容的AccessPackages
description: 检索访问权限与特定访问包不兼容的访问包的列表。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c78226a7f131e6e8d5259edb6972ff506c2a8b81
ms.sourcegitcommit: e7cfc67ac8fa2ccf895ca7a8d5f640fb99237928
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2022
ms.locfileid: "65102932"
---
# <a name="list-incompatibleaccesspackages"></a>列出不兼容的AccessPackages

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索 [在 accessPackage](../resources/accesspackage.md) 上标记为不兼容的 [accessPackage](../resources/accesspackage.md) 对象的列表。  

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleAccessPackages
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持通过大型响应进行服务器端分页的 OData 查询参数。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| Authorization | 持有者 \{token\}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [accessPackage](../resources/accesspackage.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "get_incompatibleaccesspackages"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleAccessPackages
```

### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackage",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "c0a74b4d-2694-4d5d-a964-1bee4ff0aaf2",
      "catalogId": "c955f54f-e248-4155-b314-0bdd63f5aae9",
      "displayName": "accesspackage"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List incompatibleAccessPackages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

