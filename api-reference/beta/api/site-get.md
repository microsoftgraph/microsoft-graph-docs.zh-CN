---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 获取 SharePoint 网站
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: bc1f4e478b93472b683cd8249d55a98f751dfaa0
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482285"
---
# <a name="get-a-site-resource"></a>获取网站资源

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索[网站][]资源的属性和关系。**网站**资源表示 SharePoint 中的团队网站。

[网站]: ../resources/site.md

**网站**可按唯一标识符处理，此唯一标识符是下列值的复合 ID：

* 网站集主机名称 (contoso.sharepoint.com)
* 网站集的唯一 ID (GUID)
* 网站的唯一 ID (GUID)

还有一个保留的网站标识符，即 `root`。它经常用于引用给定目标的根网站，如下所示：

* `/sites/root`：租户根网站。
* `/groups/{group-id}/sites/root`：该组的团队网站。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Sites.Read.All、Sites.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Sites.Read.All、Sites.ReadWrite.All |

## <a name="get-the-tenants-root-site"></a>获取租户的根网站

若要访问租户内的根 SharePoint 网站：

<!-- { "blockType": "ignored" } -->

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a>通过相对于服务器的 URL 访问网站

如果你的服务器具有**网站**资源的相对于服务器的 URL，你可以构建请求，如下所示：

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a>访问组团队网站

若要访问组的团队网站：

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a>示例

### <a name="request"></a>请求

<!-- { "blockType": "request", "name": "get-site" } -->

```http
GET /sites/{site-id}
```

### <a name="response"></a>响应

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE",
  "owner": {
    "user": {
      "displayName": "Daron Spektor",
      "id": "5280E7FE-DC7A-4486-9490-E790D81DFEB3"
    }
  },
  "displayName": "OneDrive Team Site",
  "name": "1drvteam",
  "createdDateTime": "2017-05-09T20:56:00Z",
  "lastModifiedDateTime": "2017-05-09T20:56:01Z",
  "webUrl": "https://contoso.sharepoint.com/teams/1drvteam"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Get by ID",
  "suppressions": [
    "Error: /api-reference/beta/api/site-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
