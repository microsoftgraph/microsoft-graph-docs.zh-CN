---
title: 获取页面
description: 检索 page 对象的属性和关系。
ms.localizationpriority: medium
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 06463449255e5dd10fbfb142832bc480498e0df0
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60945077"
---
# <a name="get-page"></a>获取页面

命名空间：microsoft.graph

检索 page 对象的属性 [和](../resources/page.md) 关系。

**获取页面信息**

按页面标识符访问页面元数据：

```
GET /me/onenote/pages/{id}
```

**获取页面内容**

可以使用页面的 `content` 终结点获取页面的 HTML 内容：

```
GET /me/onenote/pages/{id}/content[?includeIDs=true]
GET /me/onenote/pages/{id}/$value[?includeIDs=true]
```

查询 `includeIDs=true` 选项用于更新 [页面](../api/page-update.md)。

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | Notes.Read、Notes.ReadWrite    |
|应用程序 | Notes.Read.All、Notes.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages/{id}
GET /users/{id | userPrincipalName}/onenote/pages/{id}
GET /groups/{id}/onenote/pages/{id}
GET /sites/{id}/onenote/pages/{id}
```
## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 `select` 和 `expand` [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。

默认响应将 `parentSection` 展开并选择节的 、 和 `id` `name` `self` 属性。 页面 `expand` 的有效值为 `parentNotebook` 和 `parentSection` 。

## <a name="request-headers"></a>请求头
| 名称       | 类型 | 说明|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |
| 接受 | string | `application/json` |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [page](../resources/page.md) 对象。
## <a name="example"></a>示例
##### <a name="request"></a>请求
下面是一个请求示例。
 <!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
##### <a name="response"></a>响应
下面是一个响应示例。 注意：为简洁起见，将截断此处所示的响应对象。 将从实际调用中返回所有属性。
 <!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "title": "title-value",
  "createdByAppId": "createdByAppId-value",
  "links": {
    "oneNoteClientUrl": {
      "href": "href-value"
    },
    "oneNoteWebUrl": {
      "href": "href-value"
    }
  },
  "contentUrl": "contentUrl-value",
  "content": "content-value",
  "lastModifiedDateTime": "2016-10-19T10:37:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
