---
title: 创建页面
description: 在指定分区中新建页面。
ms.localizationpriority: medium
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 402ff69bf2277e65da2446a02a8e17e792e81e6b
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60926397"
---
# <a name="create-page"></a>创建页面

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在指定分区中新建[页面](../resources/onenotepage.md)。
## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | Notes.Create、Notes.ReadWrite    |
|应用程序 | Notes.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/pages
POST /users/{id | userPrincipalName}/onenote/sections/{id}/pages
POST /groups/{id}/onenote/sections/{id}/pages
POST /sites/{id}/onenote/sections/{id}/pages
```
## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |
| Content-Type | string | HTML 内容（包括多部分请求必备的“演示”部分）的 `text/html` 或 `application/xhtml+xml`。多部分请求使用 `multipart/form-data; boundary=your-boundary` 内容类型。 |

## <a name="request-body"></a>请求正文
在请求正文中，提供页面的 HTML 内容。

正文可以将 HTML 直接置于请求正文中，或者其可以包含多部分消息格式，如示例中所示。如果要发送二进制数据，则必须发送多部分请求。

## <a name="response"></a>响应

如果成功，此方法在 `201 Created` 响应正文中返回 响应代码和新 [onenotePage](../resources/onenotepage.md) 对象。

## <a name="example"></a>示例
##### <a name="request"></a>请求
下面是一个请求示例。

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/me/onenote/sections/{id}/pages
Content-type: multipart/form-data; boundary=MyPartBoundary198374

--MyPartBoundary198374
Content-Disposition:form-data; name="Presentation"
Content-Type:text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with <i>rendered</i> images and an <b>attached</b> file</title>
    <meta name="created" content="2015-07-22T09:00:00-08:00" />
  </head>
  <body>
    <p>Here's an image from an online source:</p>
    <img src="https://..." alt="an image on the page" width="500" />
    <p>Here's an image uploaded as binary data:</p>
    <img src="name:imageBlock1" alt="an image on the page" width="300" />
    <p>Here's a file attachment:</p>
    <object data-attachment="FileName.pdf" data="name:fileBlock1" type="application/pdf" />
  </body>
</html>

--MyPartBoundary198374
Content-Disposition:form-data; name="imageBlock1"
Content-Type:image/jpeg

... binary image data ...

--MyPartBoundary198374
Content-Disposition:form-data; name="fileBlock1"
Content-Type:application/pdf

... binary file data ...

--MyPartBoundary198374--
```
##### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，会将此处所示的响应对象截断。将从实际调用中返回所有属性。<!-- { "blockType": "ignored" } -->
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
  "lastModifiedDateTime": "2016-10-19T10:37:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Page",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


