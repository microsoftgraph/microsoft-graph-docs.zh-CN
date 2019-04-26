---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: 从 SharePoint 列表中删除条目
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 36f0c67dada25128cd1a054c066c1d90ccfcbabb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333479"
---
# <a name="delete-an-item-from-a-list"></a>从列表中删除项

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

从 [list][] 中删除项。

[列表]: ../resources/list.md

## <a name="permissions"></a>权限

应用程序必须拥有用户授予的对要删除的项的写入权限，才能删除项。

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Sites.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="optional-request-headers"></a>可选的请求标头

| 名称       | 值 | 说明
|:-----------|:------|:--------------------------------------------------------
| _if-match_ | etag  | 如果包含此请求标头，且提供的 eTag 与项中的当前标记不匹配，则返回 `412 Precondition Failed` 响应，并且不会删除该项。

## <a name="request-body"></a>请求正文

请勿为此方法提供请求正文。

## <a name="example"></a>示例

<!-- { "blockType": "request", "name": "delete-item", "scopes": "files.readwrite" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="response"></a>响应

如果成功，此调用将返回 `204 No Content` 响应，表示资源已被删除，没有可返回的内容。

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Delete",
  "suppressions": []
}
-->
