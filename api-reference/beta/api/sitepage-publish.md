---
author: rahmit
ms.author: rahmit
ms.date: 09/10/2018
title: 发布页面
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5a00a69542c2b59b1b268433b08656c87d194feb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507528"
---
# <a name="sitepage-publish"></a>sitePage： 发布

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

发布[sitePage][]资源，使页面的版本可供所有用户的最新版本。 如果页已签出，签入此页面并将其发布。 如果页已签出到此 api 呼叫者，页是自动签入，然后发布。

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

此消息没有请求正文。 发送任何请求正文将被忽略。

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
  "suppressions": [
    "Error: /api-reference/beta/api/sitepage-publish.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
