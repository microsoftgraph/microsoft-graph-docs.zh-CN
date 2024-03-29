---
author: JeremyKelley
description: 跟踪随时间推移在驱动器项目及其子项中的更改。
ms.date: 09/10/2017
title: 'driveItem: delta'
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 3ca8c95a2d14ca8c5cc81c710b72b618430e7380
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019925"
---
# <a name="driveitem-delta"></a>driveItem: delta

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

跟踪随时间推移在 [driveItem](../resources/driveitem.md) 及其子项中的更改。

应用程序首先调用不带任何参数的 `delta`。服务开始枚举驱动器的层次结构，返回项目页面和 `@odata.nextLink` 或 `@odata.deltaLink`，如下所述。应用程序应该使用 `@odata.nextLink` 继续调用，直到不再返回 `@odata.nextLink`，或响应内容为空更改集。

接收完所有更改后，可将这些更改应用于本地状态。若要在将来检查更改，请通过上一响应中的 `@odata.deltaLink` 再次调用 `delta`。

返回具有 [`deleted` 方面](../resources/deleted.md) 的已删除邮件。应从本地状态中删除设置此属性的项目。 

**注意：** 如果在同步所有更改后文件夹为空，则仅应在本地删除此文件夹。

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
GET /drives/{drive-id}/root/delta
GET /groups/{groupId}/drive/root/delta
GET /me/drive/root/delta
GET /sites/{siteId}/drive/root/delta
GET /users/{userId}/drive/root/delta
```

## <a name="function-parameters"></a>函数参数

| 参数   | 类型  | 说明                                                                                                                          |
|:-------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| 令牌  | 字符串 | 可选。 如果未指定，则枚举层次结构的当前状态。 如果为 `latest`，则返回具有最新增量令牌的空响应。 如果为之前的增量令牌，则返回自该令牌起的新状态。

## <a name="optional-query-parameters"></a>可选查询参数

此方法支持使用 `$select`、`$expand` 和 `$top` [OData 查询参数](/graph/query-parameters)自定义响应。

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [DriveItem](../resources/driveitem.md) 资源集合。

除了 DriveItems 集合，此响应还包括以下属性之一：

| 名称                 | 值  | 说明                                                                                                                                      |
|:---------------------|:-------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| **@odata.nextLink**  | url    | 如果当前集有其他更改，用来检索下一可用更改页的 URL。                                        |
| **@odata.deltaLink** | url    | 返回当前所有更改后返回的 URL，而不是 **@odata.nextLink**。用于在将来读取下一组更改。  |

## <a name="examples"></a>示例

### <a name="example-1-initial-request"></a>示例 1：初始请求

下面是一个如何调用此 API 以建立本地状态的示例。

#### <a name="request"></a>请求

下面是一个初始请求的示例。


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "get_item_delta_first" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/root/delta
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-delta-first-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-delta-first-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-delta-first-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-delta-first-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面是一个响应示例。

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true, "scope": "file.read" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "0123456789abc",
            "name": "folder2",
            "folder": { }
        },
        {
            "id": "123010204abac",
            "name": "file.txt",
            "file": { }
        },
        {
            "id": "2353010204ddgg",
            "name": "file5.txt",
            "deleted": { }
        }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/drive/delta(token=1230919asd190410jlka)"
}
```

此响应包含第一页的更改，**@odata.nextLink** 属性指示当前的项目集中有更多项目。在检索完所有项目页之前，你的应用程序应继续请求 **@odata.nextLink** 的 URL 值。

### <a name="example-2-last-page-in-a-set"></a>示例 2：集合中的最后一页

下面是一个如何调用此 API 以更新本地状态的示例。

#### <a name="request"></a>请求

下面是一个初始请求之后的请求示例。


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "get_item_delta_last" }-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/root/delta(token='1230919asd190410jlka')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-delta-last-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-delta-last-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-delta-last-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-delta-last-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面是一个响应示例。

<!-- { "blockType": "response", "truncated": true, "@odata.type": "Collection(microsoft.graph.driveItem)", "scope": "file.read" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "0123456789abc",
            "name": "folder2",
            "folder": { },
            "deleted": { }
        },
        {
            "id": "123010204abac",
            "name": "file.txt",
            "file": { }
        }
    ],
    "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/drive/root/delta?(token='1230919asd190410jlka')"
}
```

此响应表示名为 `folder2` 的项目已被删除，并在初始请求和此请求之间添加或修改了 `file.txt` 项目以更新本地状态。

最后一页的项目将包括 **@odata.deltaLink** 属性，此属性提供的 URL 以后可用于检索自当前项目集起的更改。

可能会发生本服务无法为特定标记提供更改列表的情况（例如，如果客户端在连接断开很长时间后尝试重新使用旧标记，或如果服务器状态已更改并需要新标记）。在这些情况下，本服务将返回带有错误响应的 `HTTP 410 Gone` 错误（包含以下错误代码之一）和 `Location` 标头（包含从头开始全新的增量枚举的新 nextLink）。完成全部枚举后，将返回的项目与本地状态进行比较，并遵循以下说明。

| 错误类型                       | 说明                                                                                                                                                                                                                    |
|:---------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `resyncChangesApplyDifferences`  | 如果确定上次同步时服务与你的本地更改保持同步，请将任意本地项目替换为服务器的版本（包括删除）。上载服务器并不知道的任意本地更改。 |
| `resyncChangesUploadDifferences` | 上载服务未返回的任意本地项目，并上载与服务器版本不同的任意文件（如果不知道哪个是最新的，请保留两份）。                                       |

### <a name="example-3-retrieving-the-current-deltalink"></a>示例 3：检索当前 deltaLink

在某些情况下，请求当前 deltaLink 值可能非常有用（无需首先枚举驱动器中已有的所有项）。

如果应用只需了解更改，不需要了解现有项，这将非常有用。若要检索最新的 deltaLink，请使用查询字符串参数 `?token=latest` 调用 `delta`。

> **注意：** 如果尝试维护文件夹或驱动器中项目的完整本地表示形式，则必须使用 `delta` 进行初始枚举。
如果在枚举期间发生任何写入操作，则无法保证其他方法（例如通过文件夹的 `children` 集合分页）返回每一个项目。 使用 `delta` 是确保读取所需全部数据的唯一方法。

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "get-delta-latest", "scope": "files.read", "target": "action" } -->

```msgraph-interactive
GET /me/drive/root/delta?token=latest
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-delta-latest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-delta-latest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-delta-latest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-delta-latest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [ ],
    "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/drive/root/delta?token=1230919asd190410jlka"
}
```

### <a name="example-4-retrieving-delta-results-using-a-timestamp"></a>示例 4：使用时间戳检索增量结果

在某些情况下，客户端可能知道某个特定时间之前的驱动器状态，但没有该时间点的 deltaLink。 在这种情况下，客户端可以使用 URL 编码时间戳作为 `token` 查询字符串参数的值调用 `delta`，例如 `?token=2021-09-29T20%3A00%3A00Z` 或“?token=2021-09-29T12%3A00%3A00%2B8%3A00”。

仅 OneDrive for Business 和 SharePoint 支持使用时间戳代替令牌。

> **注意：** 客户端应尽可能使用 `delta` 查询提供的 deltaLink，而不是生成自己的令牌。 仅当 deltaLink 未知时才应使用此功能。


#### <a name="request"></a>请求



# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "get-delta-timestamp", "scopes": "files.read", "tags": "service.graph", "target": "action" } -->

```msgraph-interactive
GET /me/drive/root/delta?token=2021-09-29T20%3A00%3A00Z
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-delta-timestamp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-delta-timestamp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-delta-timestamp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-delta-timestamp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>响应

<!-- { "blockType": "response", "truncated": true, "@odata.type": "Collection(microsoft.graph.driveItem)", "scope": "file.read" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "0123456789abc",
            "name": "folder2",
            "folder": { },
            "deleted": { }
        },
        {
            "id": "123010204abac",
            "name": "file.txt",
            "file": { }
        }
    ],
    "@odata.deltaLink": "https://graph.microsoft.com/v1.0/me/drive/root/delta?(token='1230919asd190410jlka')"
}
```

## <a name="remarks"></a>注解

* 增量源显示每项的最新状态，而不是每个更改的最新状态。如果项目重命名两次，它只显示一次并且使用最新名称。
* 出于各种原因，同一项可能在增量源中出现不止一次。你应使用最后一次出现的项目。
* 项目中的 `parentReference` 属性将不包括 **路径** 的值。之所以出现这种情况，是因为重命名文件夹不会导致从 **delta** 返回文件夹的任何后代。**使用增量时应始终按 id 跟踪项目**。
* Delta 查询不会返回某些 DriveItem 属性，具体取决于操作和服务类型，如下表所示。

    **OneDrive for Business**
    
    | 操作类型 | Delta 查询忽略的属性 |
    |---------|----------|
    | 创建/修改 | `ctag` |
    | 删除 | `ctag`, `name` |


    **OneDrive（消费者）**
    
    | 操作类型 | Delta 查询忽略的属性 |
    |---------|----------|
    | 创建/修改 | 不适用 |
    | 删除 | `ctag`, `size` |

## <a name="scanning-permissions-hierarchies"></a>扫描权限层次结构

默认情况下，增量查询响应将包含查询中所有项目的发生了更改的共享信息，即使这些项目从其父级继承了权限，本身没有直接的共享更改。 这通常会导致后续调用，获取每个项目的权限详细信息，而不只是共享信息发生更改的项目。 通过向增量查询请求添加 `Prefer: hierarchicalsharing` 标头，能够帮助你更好地了解权限更改的发生方式。

如果提供了 `Prefer: hierarchicalsharing` 标头，将返回以下对象的共享信息：权限层次结构的根以及明确具有共享更改的项目。 如果共享更改是从某个项目中删除共享，你会发现一个空的共享 facet，用以区分从其父级继承的项目和唯一但没有共享链接的项目。 你还将在未共享用于建立初始作用域的权限层次结构的根处看到这个空的共享 facet。

在许多扫描场景中，你可能会对权限的更改特别感兴趣。 若要在增量查询响应中明确哪些更改是由权限更改造成的，可提供 `Prefer: deltashowsharingchanges` 标头。 当提供此标头时，由于权限更改而出现在增量查询响应中的所有项目都将具有 `@microsoft.graph.sharedChanged":"True"` OData 注释。 此功能适用于 SharePoint 和 OneDrive for Business 帐户，但不适用于 OneDrive 消费者版本的帐户。

> **注意：** 为了使用 `Prefer: deltashowsharingchanges` 标头，你需要使用 `Prefer: deltashowremovedasdeleted` 和 `Prefer: deltatraversepermissiongaps`。 这些标头值可以在一个标头中连接在一起：`Prefer: deltashowremovedasdeleted, deltatraversepermissiongaps, deltashowsharingchanges`。

## <a name="error-responses"></a>错误响应

除了上面详述的重新同步错误之外，还请参阅[错误响应][error-response]，详细了解错误返回方式。

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Sync changes from the service to your client state.",
  "keywords": "sync,delta,changes,$delta",
  "section": "documentation",
  "tocPath": "Items/Sync changes",
  "suppressions": [
  ]
}
-->


