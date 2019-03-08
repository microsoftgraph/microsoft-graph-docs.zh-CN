---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: 创建 SharePoint 列表
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 7faabe9bddc806d4c416ebed439592ec8630e8af
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481137"
---
# <a name="create-a-new-list"></a>创建新的列表

在 [site][] 中的创建新的 [list][]。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|            权限类型             | 权限（从最低特权到最高特权） |
| :------------------------------------- | :------------------------------------------ |
| 委派（工作或学校帐户）     | Sites.Manage.All                            |
| 委派（个人 Microsoft 帐户） | 不支持。                              |
| 应用程序                            | Sites.ReadWrite.All                         |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

## <a name="request-body"></a>请求正文

在请求正文中，提供要创建的 [list][] 资源的 JSON 表示形式。

## <a name="example"></a>示例

下面的示例展示了如何创建新的泛型列表。

<!-- { "blockType": "request", "name": "create-list", "scopes": "sites.readwrite.all" } -->

```http
POST /sites/{site-id}/lists
Content-Type: application/json

{
  "name": "Books",
  "columns": [
    {
      "name": "Author",
      "text": { }
    },
    {
      "name": "PageCount",
      "number": { }
    }
  ],
  "list": {
    "template": "genericList"
  }
}
```

**注意：** 自定义列都是可选的。

除了此处指定的任何列，还使用引用的**模板**中定义的列创建新列表。
如果未指定 **list** facet 或**模板**，则列表默认为 `genericList` 模板，其中包括“标题”__ 列。

## <a name="response"></a>响应

如果成功，此方法在创建列表的响应正文中返回 [list][]。

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.list", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "22e03ef3-6ef4-424d-a1d3-92a337807c30",
  "createdDateTime": "2017-04-30T01:21:00Z",
  "createdBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "8606e4d5-d582-4f5f-aeba-7d7c18b20cfd"
    }
  },
  "lastModifiedDateTime": "2016-08-30T08:26:00Z",
  "lastModifiedBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "8606e4d5-d582-4f5f-aeba-7d7c18b20cfd"
    }
  }
}
```

**注意：** 为清楚起见，将截断 Response 对象。
实际调用会返回默认属性。

[list]: ../resources/list.md
[site]: ../resources/site.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a new SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "List/Create"
} -->
