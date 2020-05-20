---
title: servicePrincipal：添加所有者
description: 使用此 API 添加服务主体的所有者。
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 9a02be5cfddd17c3623d6504cbdadb33580abf4d
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289479"
---
# <a name="serviceprincipal-add-owner"></a>servicePrincipal：添加所有者

命名空间：microsoft.graph

使用此 API 添加[servicePrincipal](../resources/serviceprincipal.md)的所有者。

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  Directory.accessasuser.all 和所有目录。全部，全部。    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Application.readwrite.ownedby 和 "全部读取"。全部、全部读取全部和全部读取全部。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/owners/$ref

```
## <a name="request-headers"></a>请求标头
| 名称       | 说明|
|:-----------|:----------|
| Authorization | Bearer {token}。必需。  |
| Content-Type | application/json. Required. |

## <a name="request-body"></a>请求正文
在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `204 No Content` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。

## <a name="examples"></a>示例
### <a name="request"></a>请求
下面是一个请求示例。

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_serviceprincipal"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
    "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```

在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。
### <a name="response"></a>响应
下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
