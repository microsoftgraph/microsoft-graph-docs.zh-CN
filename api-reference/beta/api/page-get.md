---
title: 获取页面
description: 检索 page 对象的属性和关系。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: b4138c46a4717db4590d0e929518e1f8df2893ed
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337815"
---
# <a name="get-page"></a>获取页面

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索[page](../resources/onenotepage.md)对象的属性和关系。

**获取页面信息**

按页面标识符访问页面的元数据:

```
GET /me/onenote/pages/{id}
```

**获取页面内容**

您可以使用页面的`content`终结点获取页面的 HTML 内容:

```
GET /me/onenote/pages/{id}/content[?includeIDs=true]
GET /me/onenote/pages/{id}/$value[?includeIDs=true]
```

`includeIDs=true`查询选项用于[更新页面](../api/page-update.md)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | 请参阅 "注意,"、"注释"、"全部"、"全部"、"写"    |
|委派（个人 Microsoft 帐户） | 注意: Read、notes。读写    |
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
此方法支持`select`和`expand` [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应。

默认响应将展开`parentSection`并选择节的`id`、 `name`和`self`属性。 页面`expand`的`parentNotebook`有效值为和`parentSection`。

## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |
| 接受 | string | `application/json` |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功, 此方法在响应`200 OK`正文中返回响应代码和[onenotePage](../resources/onenotepage.md)对象。
## <a name="example"></a>示例
##### <a name="request"></a>请求
下面是一个请求示例。
 <!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/onenote/pages/{id}
```
##### <a name="response"></a>响应
下面是一个响应示例。 注意: 为简洁起见, 此处显示的响应对象将被截断。 将从实际调用中返回所有属性。
 <!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 312

{
  "title": "title-value",
  "createdByAppId": "createdByAppId-value",
  "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
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
<!--
{
  "type": "#page.annotation",
  "description": "Get page",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
