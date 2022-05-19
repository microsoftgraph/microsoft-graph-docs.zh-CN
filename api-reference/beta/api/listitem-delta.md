---
author: learafa
description: 获取新创建、更新或删除的列表项，而无需对整个项集合执行完整读取。
title: lisItem： delta
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: def214ca5ba9d633ba9835d3678350fd9cf6e04a
ms.sourcegitcommit: 562dc670cea411de0ecc232840ce1c650abbe34c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2022
ms.locfileid: "65549630"
---
# <a name="listitem-delta"></a>listItem： delta

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取新创建、更新或删除的 [列表项](../resources/listitem.md) ，而无需对整个项集合执行完整读取。

一开始，应用不使用任何参数调用 `delta`。
该服务开始枚举列表的层次结构、返回项目的页面，以及 **@odata.nextLink** 或 **@odata.deltaLink**。
应用应继续使用 **@odata.nextLink** 调用，直到看到 **@odata.deltaLink** 返回。

收到所有更改后，可以将其应用到本地状态。
若要检查将来的更改，请使用上一响应中的 **@odata.deltaLink** 再次调用`delta`。

增量源显示每项的最新状态，而不是每个更改的最新状态。 如果某个项重命名了两次，则它只会显示一次，其最新名称。
由于各种原因，同一项可能多次出现在增量源中。 应使用最后一次出现的项。

已删除的项随 [已删除的方面](../resources/deleted.md)一起返回。 已删除指示项目已删除且无法还原。
应从本地状态中删除具有此属性的项。

> **注意：** 仅当文件夹在同步所有更改后为空时，才应在本地删除该文件夹。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Sites.Read.All、Sites.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。   |
|应用程序 | Sites.Read.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /sites/{siteId}/lists/{listId}/items/delta
```

## <a name="query-parameters"></a>查询参数

在请求 URL 中，可以包含以下可选查询参数。

| 参数    | 类型   | 说明                                                                                                                          |
|:-------------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| 令牌        | 字符串 | 可选。 如果未指定，则枚举层次结构的当前状态。 如果 `latest`返回具有最新增量令牌的空响应。 如果是以前的增量令牌，则返回自该令牌以来的新状态。|

此方法支持使用 `$select`、`$expand` 和 `$top` [OData 查询参数](/graph/query-parameters)自定义响应。

## <a name="request-headers"></a>请求标头

|标头       |值                    |
|-------------|-------------------------|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [listItem](../resources/listitem.md) 对象集合。

除了 **listItem** 对象的集合外，响应还将包含以下属性之一。

| 名称                 | 值  | 说明                                                                                                                                      |
|:---------------------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| **@odata.nextLink**  | URL    | 如果当前集有其他更改，用来检索下一可用更改页的 URL。                                        |
| **@odata.deltaLink** | URL    | 返回当前所有更改后返回的 URL，而不是 **@odata.nextLink**。用于在将来读取下一组更改。  |

在某些情况下，服务将返回一个 `410 Gone` 响应代码，其中包含错误响应，其中包含以下错误代码之一，以及包含 `Location` 启动新增量枚举的新 `nextLink` 标头。 例如 (，如果客户端在断开连接很长时间后尝试重复使用旧令牌，或者服务器状态已更改并且需要) 新令牌，则会发生这种情况。

完成完整枚举后，将返回的项目与本地状态进行比较，并根据错误类型按照说明进行操作。

| 错误类型                       | 说明                                                                                                                               |
|:---------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------|
| `resyncChangesApplyDifferences`  | 将任何本地项替换为服务器 (的版本，包括删除) （如果在上次同步时确保服务是最新的本地更改）。 上载服务器并不清楚的任意本地更改。 |
| `resyncChangesUploadDifferences` | Upload服务未返回的任何本地项，并上传与服务器版本不同的任何项 (如果你不确定哪个项目更最新) ，则保留这两个副本。                                       |

除了重新同步错误以及有关如何返回错误的更多详细信息，请[参阅 Microsoft Graph错误响应和资源类型][error-response]。

## <a name="examples"></a>示例

### <a name="example-1-initial-request"></a>示例 1：初始请求

下面是初始请求的示例，演示如何调用此 API 来建立本地状态。

#### <a name="request"></a>请求

下面是初始请求的示例。

<!-- { "blockType": "request", "name": "get_listItem_delta_first" } -->

```http
GET https://graph.microsoft.com/beta/sites/contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE/lists/22e03ef3-6ef4-424d-a1d3-92a337807c30/items/delta
```

#### <a name="response"></a>响应

下面是一个响应示例，其中包含更改的第一页和 **@odata.nextLink** 属性，该属性指示当前项集中不再有项目可用。 在检索完所有项目页之前，你的应用程序应继续请求 **@odata.nextLink** 的 URL 值。

<!-- { "blockType": "response", "name": "get_listItem_delta_first", "@odata.type": "microsoft.graph.listItem", "isCollection": true, "truncated": true, "scope": "site.read" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "createdDateTime": "2020-06-02T22:46:58Z",
            "eTag": "\"{12AD05BB-59B8-43AA-9456-77C44E9BC066},756\"",
            "id": "1",
            "lastModifiedDateTime": "2021-10-14T23:27:27Z",
            "webUrl": "http://contoso.sharepoint.com/Shared%20Documents/TestFolder",
            "createdBy": {
                "user": {
                    "displayName": "John doe",
                }
            },
            "parentReference": {
                "id": "1",
                "path": "Shared%20Documents",
                "siteId": "12AD05BB-59B8-43AA-9456-77C44E9BC066"
            },
            "contentType": {
                "id": "0x00123456789abc",
                "name": "Folder"
            }
        },
        {
            "createdDateTime": "2020-06-02T22:46:58Z",
            "eTag": "\"{12AD05BB-59B8-43AA-9456-77C44E9BC067},756\"",
            "id": "2",
            "lastModifiedDateTime": "2021-10-14T23:27:27Z",
            "webUrl": "http://contoso.sharepoint.com/Shared%20Documents/TestItemA.txt",
            "createdBy": {
                "user": {
                    "displayName": "John doe",
                }
            },
            "parentReference": {
                "id": "2",
                "path": "Shared%20Documents",
                "siteId": "12AD05BB-59B8-43AA-9456-77C44E9BC066"
            },
            "contentType": {
                "id": "0x00123456789abc",
                "name": "Document"
            }
        },
        {
            "createdDateTime": "2020-06-02T22:46:58Z",
            "eTag": "\"{12AD05BB-59B8-43AA-9456-77C44E9BC068},756\"",
            "id": "3",
            "lastModifiedDateTime": "2021-10-14T23:27:27Z",
            "webUrl": "http://contoso.sharepoint.com/Shared%20Documents/TestItemB.txt",
            "createdBy": {
                "user": {
                    "displayName": "John doe",
                }
            },
            "parentReference": {
                "id": "3",
                "path": "Shared%20Documents",
                "siteId": "12AD05BB-59B8-43AA-9456-77C44E9BC066"
            },
            "contentType": {
                "id": "0x00123456789abc",
                "name": "Document"
            }
        }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/beta/sites/contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE/lists/22e03ef3-6ef4-424d-a1d3-92a337807c30/items/delta?token=1230919asd190410jlka"
}
```

### <a name="example-2-last-page-request"></a>示例 2：最后一页请求

下面是一个请求示例，其中显示了集内的最后一页以及如何调用此 API 来更新本地状态。

#### <a name="request"></a>请求

下面是初始请求之后的请求示例。

<!-- { "blockType": "request", "name": "get-listItem-delta-last" }-->

```http
GET https://graph.microsoft.com/beta/sites/contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE/lists/22e03ef3-6ef4-424d-a1d3-92a337807c30/items/delta?token=1230919asd190410jlka
```

#### <a name="response"></a>响应

下面是一个响应示例，指示已删除命名 `TestItemB.txt` 的项，并且在初始请求和此请求之间添加或修改了该项 `TestFolder` 以更新本地状态。

最后一页的项目将包括 **@odata.deltaLink** 属性，此属性提供的 URL 以后可用于检索自当前项目集起的更改。


<!-- { "blockType": "response", "name": "get-listItem-delta-last", "truncated": true, "@odata.type": "microsoft.graph.listItem", "isCollection": true,  "scope": "site.read" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
       {
            "createdDateTime": "2020-06-02T22:46:58Z",
            "eTag": "\"{12AD05BB-59B8-43AA-9456-77C44E9BC066},756\"",
            "id": "1",
            "lastModifiedDateTime": "2016-03-21T20:01:37Z",
            "webUrl": "http://contoso.sharepoint.com/Shared%20Documents/TestFolder",
            "createdBy": {
                "user": {
                    "displayName": "John doe",
                }
            },
            "parentReference": {
                "id": "1",
                "path": "Shared%20Documents",
                "siteId": "12AD05BB-59B8-43AA-9456-77C44E9BC066"
            },
            "contentType": {
                "id": "0x00123456789abc",
                "name": "Folder"
            }
        },
        {
            "id": "3",
            "parentReference": {
                "siteId": "12AD05BB-59B8-43AA-9456-77C44E9BC066"
            },
            "contentType": {
                "id": "0x00123456789abc",
                "name": "Document"
            },
            "deleted": {"state": "deleted"}
        }
    ],
    "@odata.deltaLink": "https://graph.microsoft.com/beta/sites/contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE/lists/22e03ef3-6ef4-424d-a1d3-92a337807c30/items/delta?token=1230919asd190410jlka"
}
```

### <a name="example-3-delta-link-request"></a>示例 3：增量链接请求

在某些情况下，在不首先枚举列表中的所有项的情况下请求当前 `deltaLink` 值可能很有用。 如果你的应用只想了解更改，并且不需要了解现有项目，这会很有用。
若要检索最新`deltaLink`信息，请使用查询字符串参数`?token=latest`调用`delta`。

#### <a name="request"></a>请求

请求示例如下所示。

<!-- { "blockType": "request", "name": "get-delta-latest", "scope": "sites.read", "target": "action" } -->

```http
GET /sites/contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE/lists/22e03ef3-6ef4-424d-a1d3-92a337807c30/items/delta?token=latest
```

#### <a name="response"></a>响应

下面展示了示例响应。

<!-- { "blockType": "response", "name": "get-delta-latest", "isEmpty": true, "@odata.type": "microsoft.graph.listItem", "isCollection": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [ ],
    "@odata.deltaLink": "https://graph.microsoft.com/beta/sites/contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE/lists/22e03ef3-6ef4-424d-a1d3-92a337807c30/items/delta?token=1230919asd190410jlka"
}
```

## <a name="see-also"></a>另请参阅
[使用增量查询跟踪 Microsoft Graph 数据更改](/graph/delta-query-overview)

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Sync changes from the service to your client state.",
  "keywords": "sync,delta,changes,$delta",
  "section": "documentation",
  "tocPath&quot;: &quot;ListItem/Get delta"
} -->
