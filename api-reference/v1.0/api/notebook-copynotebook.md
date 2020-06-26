---
title: 笔记本： copyNotebook
description: 将笔记本复制到目标文档库中的 "笔记本" 文件夹。 如果文件夹不存在，则创建该文件夹。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 5f10c39cbb53da9329d11ee0724f716c28871813
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44892456"
---
# <a name="notebook-copynotebook"></a>笔记本： copyNotebook

命名空间： microsoft. graph 将笔记本复制到目标文档库中的 "笔记本" 文件夹。 如果文件夹不存在，则创建该文件夹。

对于复制操作，请遵循异步调用模式：首先调用复制操作，然后轮询操作终结点以获取结果。

## <a name="permissions"></a>权限
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | Notes.Create、Notes.ReadWrite    |
|应用程序 | Notes.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {token}. Required. |
| Content-Type | string | `application/json` |

## <a name="request-body"></a>请求正文
在请求正文中，提供一个 JSON 对象，其中包含您的操作所需的参数。 如果无需，可以发送空正文。

| 参数    | 类型   |说明|
|:---------------|:--------|:----------|
|groupId|String|要复制到的组的 id。 仅在复制到 Microsoft 365 组时使用。|
|renameAs|String|副本的名称。 默认值为现有项目的名称。 |

## <a name="response"></a>响应

如果成功，此方法将返回 `202 Accepted` 响应代码和 `Operation-Location` 标头。 轮询操作-位置终结点以[获取复制操作的状态](onenoteoperation-get.md)。

## <a name="example"></a>示例
下面是一个如何调用此 API 的示例。
##### <a name="request"></a>请求
下面是一个请求示例。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "notebook_copynotebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/copyNotebook
Content-type: application/json
Content-length: 108

{
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/notebook-copynotebook-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/notebook-copynotebook-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/notebook-copynotebook-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/notebook-copynotebook-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>响应
下面是一个响应示例。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebook: copyNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
