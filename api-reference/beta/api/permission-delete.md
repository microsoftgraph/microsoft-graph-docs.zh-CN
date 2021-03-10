---
author: JeremyKelley
description: 删除 DriveItem 访问权限。
ms.date: 09/10/2017
title: 删除对项的访问权限
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 69c14288576738b9dfa448cdaefb4b3d2ef87133
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50625373"
---
# <a name="delete-a-sharing-permission-from-a-file-or-folder"></a>从文件或文件夹中删除共享权限

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

删除 [DriveItem](../resources/driveitem.md) 访问权限。

只能删除 **非** 继承的共享权限。
**InheritedFrom** 属性必须为 `null`。

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
DELETE /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
DELETE /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
DELETE /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a>可选的请求标头

| 名称          | 类型   | 说明                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| if-match      | string | 如果包含此请求标头，且提供的 eTag（或 cTag）与项中的当前标记不匹配，则返回 `412 Precondition Failed` 响应，并且不会删除该项。 |


## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="example"></a>示例

本示例从当前用户 OneDrive 的项 {item-id} 中删除标识为 {perm-id} 的权限。


<!-- { "blockType": "request", "name": "delete-permission", "scopes": "files.readwrite" }-->
```http
DELETE https://graph.microsoft.com/beta/me/drive/items/{item-id}/permissions/{perm-id}
```

### <a name="response"></a>响应

<!-- { "blockType": "response", "truncated": false } -->

```http
HTTP/1.1 204 No Content
```

## <a name="remarks"></a>注解

* 具有 `personal`（OneDrive 个人版）**driveType** 的 [驱动器](../resources/drive.md) 无法创建或修改根 DriveItem 上的权限。 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Remove an item's sharing permissions",
  "keywords": "permission, permissions, sharing, remove permissions, delete permissions",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Delete permission",
  "suppressions": [
  ]
}
-->


