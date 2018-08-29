---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 获取驱动器
ms.openlocfilehash: 4c77a1ef801fa65edf77376d421cafa3ff79f3d4
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2018
ms.locfileid: "23269430"
---
# <a name="get-drive"></a>获取驱动器

检索 [Drive](../resources/drive.md) 资源的属性和关系。

驱动器是文件系统的顶级容器，例如 OneDrive 或 SharePoint 文档库。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All    |
|应用程序 | Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All |

## <a name="get-current-users-onedrive"></a>获取当前用户的 OneDrive

可以通过 `me` 单一实例访问登录用户的驱动器（如果使用委派身份验证）。

如果未设置用户的 OneDrive，但用户有使用 OneDrive 的许可，那么在使用委派身份验证时，该请求将自动设置用户驱动器。

### <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive
```

## <a name="get-a-users-onedrive"></a>获取用户的 OneDrive

若要访问用户的 OneDrive 或 OneDrive for Business，应用必须请求对 User 资源获取 **drive** 关系。

如果未设置用户的 OneDrive，但用户有使用 OneDrive 的许可，那么在使用委派身份验证时，该请求将自动设置用户驱动器。

### <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all", "tags": "service.graph" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```

### <a name="path-parameters"></a>路径参数

| 参数名称 | 值  | 说明                                       |
|:---------------|:-------|:--------------------------------------------------|
| _idOrUserPrincipalName_     | string | 必需。 拥有 OneDrive 的用户对象的标识符。 |

## <a name="get-the-document-library-associated-with-a-group"></a>获取与组关联的文档库

若要访问组的默认文档库，你的应用程序应请求组中的 **drive** 关系。

### <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all", "tags": "service.graph" } -->

```http
GET /groups/{groupId}/drive
```

### <a name="path-parameters"></a>路径参数

| 参数名称 | 值  | 说明                                       |
|:---------------|:-------|:--------------------------------------------------|
| _groupId_      | string | 必需。 拥有文档库的组的标识符。 |

## <a name="get-the-document-library-for-a-site"></a>获取某个站点的文档库

为了访问[站点的](../resources/site.md)默认文档库，你的应用程序应请求站点中的 **drive** 关系。

### <a name="http-request"></a>HTTP 请求

```http
GET /sites/{siteId}/drive
```

### <a name="path-parameters"></a>路径参数

| 参数名称 | 值  | 说明                                       |
|:---------------|:-------|:--------------------------------------------------|
| _siteId_       | string | 必需。 包含文档库的站点的标识符。 |

## <a name="get-a-drive-by-id"></a>根据 ID 获取驱动器

如果你有某个驱动器的唯一标识符，则可以直接从顶级驱动器集合来访问它。

### <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}
```

### <a name="path-parameters"></a>路径参数

| 参数名称 | 值  | 说明                                       |
|:---------------|:-------|:--------------------------------------------------|
| _driveId_      | string | 必需。 请求获取的驱动器的标识符。 |

## <a name="optional-query-parameters"></a>可选的查询参数

这些方法支持 [$select 查询参数][odata-query-parameters]塑造响应。

## <a name="http-response"></a>HTTP 响应

每个方法将在响应正文中返回匹配驱动器的 [Drive 资源][drive-resource]。

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.drive", "truncated": true, "name": ["get-drive-by-id", "get-drive-by-group", "get-drive-by-user", "get-drive-default"] } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "b!t18F8ybsHUq1z3LTz8xvZqP8zaSWjkFNhsME-Fepo75dTf9vQKfeRblBZjoSQrd7",
    "driveType": "business",
    "owner": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "Ryan Gregg"
        }
    },
    "quota": {
        "deleted": 256938,
        "remaining": 1099447353539,
        "state": "normal",
        "total": 1099511627776
    }
}
```

### <a name="error-response-codes"></a>错误响应代码

如果驱动器不存在且无法自动设置（当使用委派身份验证），将返回 `HTTP 404` 响应。

[drive-resource]: ../resources/drive.md
[odata-query-parameters]: ../../../concepts/query_parameters.md

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "suppressions": [
      "Warning: /api-reference/v1.0/api/drive_get.md:
        Unable to map some markdown elements into schema.
            Unmapped methods:
        get-drive-default, get-drive-by-user, get-drive-by-group, get-drive-by-id
            Unmapped tables:
        Permissions - AuthScopes, Path parameters - PathParameters, Path parameters - PathParameters, Path parameters - PathParameters, Path parameters - PathParameters"
  ],
  "tocPath": "Drives/Get drive"
} -->
