---
author: JeremyKelley
description: 在新的父项下或使用新名称异步创建 [driveItem] [item-resource] 的副本 (包括任何子级)。
ms.date: 09/10/2017
title: 复制文件或文件夹
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 22cb3f59b8db2ad6f884940df1acce9aab6b6b6a
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416842"
---
# <a name="copy-a-driveitem"></a>复制 DriveItem

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

以异步方式在新父项下或使用新名称创建一个 [driveItem][item-resource] 副本（包括任何子项）。

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
POST /drives/{driveId}/items/{itemId}/copy
POST /groups/{groupId}/drive/items/{itemId}/copy
POST /me/drive/items/{item-id}/copy
POST /sites/{siteId}/drive/items/{itemId}/copy
POST /users/{userId}/drive/items/{itemId}/copy
```

### <a name="request-body"></a>请求正文

在请求正文中，提供具有以下参数的 JSON 对象。


| 名称            | 值                                          | 说明                                                                                                 |
|:----------------|:-----------------------------------------------|:------------------------------------------------------------------------------------------------------------|
| parentReference | [ItemReference](../resources/itemreference.md) | 可选。引用在其中创建副本的父项。                                         |
| name            | string                                         | 可选。副本的新名称。如果未提供新名称，将同一名称用作原始名称。    |

**注意：**_parentReference_ 应包括目标文件夹的 `driveId` 和 `id` 参数。

## <a name="example"></a>示例

本示例将由 `{item-id}` 标识的文件复制到使用 `driveId` 和 `id` 值标识的文件夹。
该文件的新副本将被命名为 `contoso plan (copy).txt`。


# <a name="httptabhttp"></a>[HTTP.SYS](#tab/http)
<!-- { "blockType": "request", "name": "copy-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/copy
Content-Type: application/json

{
  "parentReference": {
    "driveId": "6F7D00BF-FC4D-4E62-9769-6AEA81F3A21B",
    "id": "DCD0D3AD-8989-4F23-A5A2-2C086050513F"
  },
  "name": "contoso plan (copy).txt"
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/copy-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/copy-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目标-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/copy-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a>响应

返回有关如何在接受请求时[监视复制操作进度](/graph/long-running-actions-overview)的详细信息。

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 202 Accepted
Location: https://contoso.sharepoint.com/_api/v2.0/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

`Location` 头值提供的服务 URL 将返回复制操作的最新状态。 可以根据此信息[确定复制操作完成时间](/graph/long-running-actions-overview)。

### <a name="remarks"></a>注解

在许多情况下，复制操作采用异步执行。API 响应仅指明复制操作获得接受还是遭到拒绝（比如说，由于目标文件名已被其他对象使用而遭到拒绝）。

[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
  ]
}
-->
