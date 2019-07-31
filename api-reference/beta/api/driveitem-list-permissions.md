---
author: JeremyKelley
description: 列出 DriveItem 中的有效共享权限。
ms.date: 09/10/2017
title: 列出有权访问文件的权限
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: c3409dc56dbc11f4100d9df54aca44ef54eecaff
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35957071"
---
# <a name="list-sharing-permissions-on-a-driveitem"></a>列出 DriveItem 中的共享权限

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

列出 [DriveItem](../resources/driveitem.md) 中的有效共享权限。

## <a name="access-to-sharing-permissions"></a>访问共享权限

权限集合包括潜在的敏感信息，不可能适用于每个调用方。

* 对于该项目的所有者，将返回所有共享权限。 这包括共有者。
* 对于非所有者的调用方，仅返回应用于调用方的共享权限。
* 对于能够创建共享权限的调用方，仅返回包含机密信息（例如 `shareId` 和 `webUrl`）的共享权限属性。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All    |
|应用程序 | Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/permissions
GET /groups/{group-id}/drive/items/{item-id}/permissions
GET /me/drive/items/{item-id}/permissions
GET /me/drive/root:/{path}:/permissions
GET /sites/{siteId}/drive/items/{itemId}/permissions
GET /users/{userId}/drive/items/{itemId}/permissions
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持使用 `$select` [OData 查询参数](/graph/query-parameters)自定义响应。

## <a name="optional-request-headers"></a>可选的请求标头

| 名称          | 类型   | 说明                                                                                                                                     |
|:--------------|:-------|:------------------------------------------------------------------------------------------------------------------------------------------------|
| if-none-match | string | 如果包含此请求头，且提供的 eTag 与项中的当前 etag 不匹配，则返回 `HTTP 304 Not Modified` 响应。 |

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Permission](../resources/permission.md) 资源集合。

DriveItem 的有效共享权限可能有两个来源：

* 直接对 DriveItem 本身应用的共享权限
* 从 DriveItem 的上级继承的共享权限

调用方可以通过检查 **inheritedFrom** 属性来区分是否为继承权限。此属性是引用从中继承该权限的上级的 [**itemReference**](../resources/itemreference.md) 资源。

对项设置的 SharePoint 权限级别在返回时包含“SP”前缀。 例如，SP.View Only、SP.Limited Access、SP.View Web Analytics Data。 请参阅 [SharePoint 角色完整列表](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1)。

## <a name="example"></a>示例

本示例检索登录用户驱动器中某个项的权限集合。


# <a name="httptabhttp"></a>[HTTP.SYS](#tab/http)
<!-- { "blockType": "request", "name": "get-item-permissions", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/permissions
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-permissions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-permissions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目标-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-permissions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-permissions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

此示例响应包括三个权限，第一个是具有编辑权限的共享链接，第二个是继承自父文件夹用户名为 John 的显式权限，第三个是由一个应用程序创建的读写共享链接。

<!-- {"blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit"
      }
    },
    {
      "id": "2",
      "roles": ["write"],
      "grantedTo": {
        "user": {
          "id": "5D33DD65C6932946",
          "displayName": "John Doe"
        }
      },
      "inheritedFrom": {
        "driveId": "1234567890ABD",
        "id": "1234567890ABC!123",
        "path": "/drive/root:/Documents" }
    },
    {
      "id": "3",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit",
        "application": {
          "id": "12345",
          "displayName": "Contoso Time Manager"
        }
      }
    }
  ]
}
```

## <a name="remarks"></a>注解

不能在 [获取 DriveItem](driveitem-get.md) 的调用过程中或 DriveItem 集合中扩展 DriveItem 的**权限**关系。必须直接访问权限属性。

## <a name="error-responses"></a>错误响应

请参阅[错误响应][error-response]主题，详细了解错误返回方式。

[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "List an item's permissions",
  "keywords": "permission, permissions, sharing",
  "section": "documentation",
  "tocPath": "Sharing/Permissions",
  "suppressions": [
  ]
}
-->
