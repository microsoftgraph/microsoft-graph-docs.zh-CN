---
title: 处理长时间运行的操作（测试）
description: 本文会介绍处理长时间运行的操作。
localization_priority: Normal
author: daspek
ms.openlocfilehash: 273299b13be423cf3e6ae625226efff5fef40f8f8ba06f787d0ba9ab29ba5211
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54146205"
---
# <a name="working-with-long-running-actions-beta"></a>处理长时间运行的操作 (beta)


某些 API 响应完成所需的时间不确定。
Microsoft Graph 可能会使用长时间运行操作模式，而不是等待操作完成之后再返回响应。
此模式为你的应用提供了一种轮询长时间运行的操作的状态更新的方法，无需任何等待操作完成的请求。

常规模式包括以下步骤：

1. 应用请求通过 API 执行长时间运行的操作。 API 接受操作，并返回 `202 Accepted` 响应以及 API URL 的 Location 头，以便检索操作状态报告。
2. 应用请求获取操作状态报告 URL，然后收到包含长时间运行的操作进度的 [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) 响应。
3. 长时间运行的操作完成。 
4. 应用再次请求获取操作状态报告 URL ，然后收到显示操作已完成状态的 [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) 响应。

## <a name="initial-action-request"></a>初始操作请求

让我们来逐步完成 [DriveItem 复制](/graph/api/driveitem-copy?view=graph-rest-beta)示例方案。
在此方案中，应用请求复制包含大量数据的文件夹。
因为数据量较大，所以此请求可能需要几秒钟才能完成。


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "lro-copy-item-example", "scopes": "files.readwrite" } -->

```http
POST https://graph.microsoft.com/beta/me/drive/items/{folder-item-id}/copy
Content-Type: application/json

{
  "parentReference": {
    "path": "/drive/root:/Documents"
  },
  "name": "Copy of LargeFolder1"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/lro-copy-item-example-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/lro-copy-item-example-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/lro-copy-item-example-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


API 予以响应，指明已接受此操作，并返回用于检索长时间运行的操作状态的 URL。

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 202 Accepted
Location: https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

**注意：** 返回的位置 URL 可能不在 Microsoft Graph API 终结点上。

在很多情况下，请求到此结束，因为复制操作的完成无需应用执行其他任何工作。
不过，如果应用需要显示复制操作的状态，或确保其正确完成，可以使用监视器 URL。

## <a name="retrieve-a-status-report-from-the-monitor-url"></a>通过监视器 URL 检索状态报告

为了检查复制操作的状态，应用会请求获取上一响应中返回的 URL。 *注意：* 此请求无需验证，因为这是原始调用方专属的短期 URL。 

<!-- { "blockType": "request", "opaqueUrl": true, "name": "lro-check-status", "scopes": "files.readwrite" } -->

```http
GET https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

服务响应返回的信息指明长时间运行的操作仍在进行中：

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.asyncJobStatus" } -->

```http
HTTP/1.1 202 Accepted
Content-type: application/json

{
  "operation": "ItemCopy",
  "percentageComplete": 27.8,
  "status": "inProgress"
}
```

此信息可用于向用户提供复制操作的最新进度。 应用可以继续轮询监视器 URL，以请求获取状态更新并跟踪操作进度。

## <a name="retrieve-a-completed-status-report-from-the-monitor-url"></a>通过监视器 URL 检索已完成状态报告

几秒钟后，复制操作完成。 当应用向监视器 URL 发出请求时，响应返回的是重定向到操作的最终结果。

<!-- { "blockType": "request", "opaqueUrl": true, "name": "lro-check-status-complete", "scopes": "files.readwrite" } -->

```http
GET https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

完成操作后，监视器服务的响应将返回结果的 resourceId。

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.asyncJobStatus" } -->

```http
HTTP/1.1 202 Accepted
Content-type: application/json

{
    "percentageComplete": 100.0,
    "resourceId": "01MOWKYVJML57KN2ANMBA3JZJS2MBGC7KM",
    "status": "completed"
}
```

## <a name="retrieve-the-results-of-the-completed-operation"></a>检索已完成的操作的结果

完成作业后，监视器 URL 返回结果的 resourceId，在此例中为原始项的新副本。
可以使用 resourceId 处理此新项，例如：


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "lro-copy-item-example-complete",
  "scopes": "files.readwrite"
} -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{item-id}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/lro-copy-item-example-complete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/lro-copy-item-example-complete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/lro-copy-item-example-complete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "",
    "name": "Copy of LargeFolder1",
    "folder": { },
    "size": 12019
}
```

## <a name="supported-resources"></a>支持的资源

以下 API 方法支持长时间运行的操作

| **资源** | **API** |
|:------ | :------ |
| DriveItem | [Copy](/graph/api/driveitem-copy?view=graph-rest-beta) |

## <a name="prerequisites"></a>先决条件

查询长时间运行的操作的状态也需要执行长时间运行的操作所需的相同[权限](./permissions-reference.md)。




<!-- {
  "type": "#page.annotation",
  "description": "Monitor the progress of long-running actions in the API.",
  "keywords": "monitor,long,running,operation,action",
  "section": "documentation",
  "suppressions": [
    "Error: lro-check-status:
      Unable to locate a definition for resource type: microsoft.graph.asyncJobStatus",
    "Error: lro-check-status-complete:
      Unable to locate a definition for resource type: microsoft.graph.asyncJobStatus"
  ],
  "tocPath": "Concepts/Long running actions"
} -->
