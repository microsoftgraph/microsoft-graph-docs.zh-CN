---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 列出驱动器
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: ae97b3aecea005b06748874e5f4c527b934ea2a7
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272882"
---
# <a name="list-available-drives"></a>列出可用的驱动器

检索可用于目标用户、组或[站点](../resources/site.md)的 [Drive](../resources/drive.md) 资源列表。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All    |
|应用程序 | Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All |

## <a name="list-a-groups-drives"></a>列出组的驱动器

若要列出某个组的文档库，应用应请求组中的 **drives** 关系。

### <a name="http-request"></a>HTTP 请求

<!-- {"blockType": "request", "name": "group-list-drives", "scopes": "groups.read.all", "tags": "service.graph" } -->

```http
GET /groups/{groupId}/drives
```
#### <a name="sdk-sample-code"></a>SDK 示例代码
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/group-list-drives-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/group-list-drives-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Objective-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/group-list-drives-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="list-a-sites-drives"></a>列出站点的驱动器

若要列出某个站点的文档库，应用应请求站点中的 **drives** 关系。

<!-- {"blockType": "request", "name": "site-list-drives", "scopes": "sites.read.all", "tags": "service.graph" } -->

```http
GET /sites/{siteId}/drives
```
#### <a name="sdk-sample-code"></a>SDK 示例代码
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/site-list-drives-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/site-list-drives-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Objective-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/site-list-drives-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="list-a-users-drives"></a>列出用户的驱动器

<!-- {"blockType": "request", "name": "user-list-drives", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /users/{userId}/drives
```
#### <a name="sdk-sample-code"></a>SDK 示例代码
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/user-list-drives-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/user-list-drives-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Objective-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user-list-drives-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="list-the-current-users-drives"></a>列出当前用户的驱动器

<!-- {"blockType": "request", "name": "enum-drives", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drives
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持使用 `$expand`、`$select`、`$skipToken`、`$top` 和 `$orderby` [OData 查询参数](/graph/query-parameters)自定义响应。


## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Drive](../resources/drive.md) 对象集合。

<!-- { "blockType": "response", 
       "@odata.type": "Collection(microsoft.graph.drive)",
       "name": ["group-list-drives", "site-list-drives", "user-list-drives", "enum-drives"],
       "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "942CAEB0-13AE-491B-85E4-7557CDC0F25F",
      "driveType": "documentLibrary",
      "name": "Shared Documents",
      "owner": {
        "user": {
          "id": "AE2A1EE9-81A7-423C-ABE4-B945F47509BB",
          "displayName": "Ryan Gregg"
        }
      }
    },
    {
      "id": "C1CD3ED9-0E98-4B0B-82D3-C8FB784B9DCC",
      "driveType": "documentLibrary",
      "name": "Contoso Project Files",
      "owner": {
        "user": {
          "id": "406B2281-18E8-4416-9857-38C531B904F1",
          "displayName": "Daron Spektor"
        }
      }
    }
  ]
}
```
#### <a name="sdk-sample-code"></a>SDK 示例代码
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/enum-drives-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/enum-drives-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Objective-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/enum-drives-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="remarks"></a>说明

大多数用户将只有一个 Drive 资源。

组和站点可使用多个 Drive 资源。

默认情况下将隐藏包含 [system][] Facet 的 Drive。
若要列出它们，请在 `$select` 语句中包含 `system`。

[system]: ../resources/systemfacet.md

<!-- {
  "type": "#page.annotation",
  "description": "List the available drives for a user, group, or site.",
  "keywords": "drive,onedrive.drive,list drives",
  "section": "documentation",
  "tocPath": "Drives/List drives",
  "suppressions": [
    "Error: /api-reference/v1.0/api/drive-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/drive-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/drive-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/drive-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/drive-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/drive-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/drive-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/drive-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/drive-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
