---
author: rahmit
ms.author: rahmit
ms.date: 09/10/2018
title: 发布页面
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: d9bf699c0038e785a11560ee7326cfb2324345f3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335886"
---
# <a name="sitepage-publish"></a>sitePage: 发布

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

发布[sitePage][]资源的最新版本, 使页面的版本可供所有用户使用。 如果该页面已签出, 请签入该页面并发布它。 如果页面已签出到此 API 的调用方, 则会自动签入并发布该页面。

[sitePage]: ../resources/sitepage.md

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | Files.ReadWrite、Files.ReadWrite.All    |
|应用程序 | Files.ReadWrite.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{siteId}/pages/{pageId}/publish
```

## <a name="request-body"></a>请求正文

此邮件没有请求正文。 发送的任何请求正文都将被忽略。

## <a name="response"></a>响应

如果成功，该 API 调用会返回 `204 No Content`。

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```


<!--
{
  "type": "#page.annotation",
  "description": "Publish a page.",
  "keywords": "publish page",
  "section": "documentation",
  "tocPath": "Pages/Publish",
  "suppressions": []
}
-->
