---
title: 还原 ListItem 的以前版本
description: 将 ListItem 的以前版本还原为当前版本。 这将使用以前版本的内容创建一个新版本，但保留项的所有现有版本。
localization_priority: Normal
ms.prod: sharepoint
author: ''
doc_type: apiPageType
ms.openlocfilehash: c6109575256ed6a90019b4da1d88723a163569b1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511668"
---
# <a name="restore-a-previous-version-of-a-listitem"></a>还原 ListItem 的以前版本

命名空间：microsoft.graph

将 ListItem 的以前版本还原为当前版本。 这将使用以前版本的内容创建一个新版本，但保留项的所有现有版本。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|            权限类型             |         权限（从最低特权到最高特权）          |
| :------------------------------------- | :----------------------------------------------------------- |
| 委派（工作或学校帐户）     | Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All |
| 委派（个人 Microsoft 帐户） | 无                                                          |
| 应用程序                            | Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a>请求正文

无需请求正文。

## <a name="example"></a>示例

本示例还原由 `{item-id}` 和 `{version-id}` 标识的 listItem 的一个版本。


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite sites.readwrite.all", "target": "action", "tags": "service.graph service.sharepoint" } -->

```http
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/restore-item-version-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/restore-item-version-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/restore-item-version-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/restore-item-version-listitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a>响应

如果成功，该 API 调用会返回 `204 No Content`。

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
  ]
} -->
