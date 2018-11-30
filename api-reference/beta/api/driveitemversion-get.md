---
title: 获取 DriveItemVersion 资源（预览）
description: 检索 DriveItem 的某个特定版本的元数据。
ms.openlocfilehash: c78a81d1a5428bbb969f8761b238655ab7919e5a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043278"
---
# <a name="get-a-driveitemversion-resource-preview"></a>获取 DriveItemVersion 资源（预览）

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

检索 [DriveItem](../resources/driveitem.md) 的某个特定版本的元数据。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All    |
|应用程序 | Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All |


## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}
GET /me/drive/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}
```

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [DriveItemVersion](../resources/driveitemversion.md) 对象。


## <a name="example"></a>示例

本示例检索当前用户驱动器中的文件的版本。

### <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "request", "name": "get-single-version", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}
```

### <a name="response"></a>响应

这将返回版本的集合：

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItemVersion", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "D4990684-58CE-4FAB-9B87-D6C49E74F298",
    "lastModifiedBy": {
    "user": {
        "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
        "displayName": "Ryan Gregg"
    }
    },
    "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
    "size": 123
}
```

## <a name="remarks"></a>注解

OneDrive 不保留文件以前版本的完整元数据。

当应用检索文件的可用版本列表时，将返回 [DriveItemVersion](../resources/driveitemversion.md) 资源，它提供有关特定版本的可用信息。


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
