---
title: 使用 Excel API 的最佳做法
description: 在 Microsoft Graph 中查找有关使用 Excel API 的提示。 了解如何管理会话、使用需要很长时间才能完成的 API，以及如何减少限制错误。
author: grangeryy
ms.localizationpriority: medium
ms.prod: excel
ms.openlocfilehash: 6f2b3a0a9c0213098a9a6a214b03e448050a3a1d
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447021"
---
# <a name="best-practices-for-working-with-the-excel-api"></a>使用 Excel API 的最佳做法

本文提供有关在 Microsoft Graph 中使用 [Excel API](/graph/api/resources/excel) 的建议。

## <a name="manage-sessions-in-the-most-efficient-way"></a>以最有效的方式管理会话

如果在某个时间段内要进行多个调用，建议创建会话，并通过每个请求传递会话 ID。 若要表示 API 中的会话，请使用 `workbook-session-id: {session-id}` 标头。 通过执行此操作，可以以最有效的方式使用 Excel API。

以下示例演示如何使用此方法将新数字添加到表，然后在工作簿中找到一条记录。

### <a name="step-1-create-a-session"></a>步骤 1：创建会话

#### <a name="request"></a>请求

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/createSession
Content-type: application/json

{
  "persistChanges": true
}
```

#### <a name="response"></a>响应

下面是成功的响应。

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "persistChanges": true
}
```

### <a name="step-2-add-a-new-row-to-the-table"></a>步骤 2：向表添加新行

#### <a name="request"></a>请求

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/Table1/rows/add
Content-type: application/json
workbook-session-id: {session-id}

{
  "values": [[“east”, “pear”, 4]]
}
```

#### <a name="response"></a>响应

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "index": 6,
  "values": [[“east”, “pear”, 4]]
}
```

### <a name="step-3-look-up-a-value-in-the-updated-table"></a>步骤 3：在更新的表中查找值

#### <a name="request"></a>请求

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/functions/vlookup
Content-type: application/json
workbook-session-id: {session-id}

{
    "lookupValue":"pear",
    "tableArray":{"Address":"Sheet1!B2:C7"},
    "colIndexNum":2,
    "rangeLookup":false
}
```

#### <a name="response"></a>响应

```http
HTTP code: 200 OK
content-type: application/json

{
    "value": 5
}
```

### <a name="step-4-close-the-session-after-all-the-requests-are-completed"></a>步骤 4：完成所有请求后关闭会话

#### <a name="request"></a>请求

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/closeSession
Content-type: application/json
workbook-session-id: {session-id}

{
}
```

#### <a name="response"></a>响应

```http
HTTP/1.1 204 No Content
```

有关详细信息，请参阅 [“创建会话](/graph/api/workbook-createsession) ”和 [“关闭会话](/graph/api/workbook-closesession)”。

## <a name="work-with-apis-that-take-a-long-time-to-complete"></a>使用需要很长时间才能完成的 API

你可能会注意到，某些操作需要不确定的时间才能完成;例如，打开大型工作簿。 等待对这些请求的响应时，很容易出现超时。 为了解决此问题，我们提供了长时间运行的操作模式。 使用此模式时，无需担心请求超时。

目前，Microsoft Graph 中的会话创建 Excel API 已启用长时间运行的操作模式。 此模式涉及以下步骤：

1. `Prefer: respond-async`将标头添加到请求，以指示在缓存会话时它是一个长时间运行的操作。
2. 长时间运行的操作将返回一个 `202 Accepted` 响应以及一个 Location 标头来检索操作状态。 如果会话创建在几秒内完成，它将返回常规的创建会话响应，而不是使用长时间运行的操作模式。
3. `202 Accepted`通过响应，可以在指定位置检索操作状态。 操作状态值包括`notStarted`、`running`和 `succeeded``failed`.
4. 操作完成后，可以通过成功响应中的指定 URL 获取会话创建结果。

以下示例使用长时间运行的操作模式创建会话。

### <a name="initial-request-to-create-session"></a>创建会话的初始请求

#### <a name="request"></a>请求

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/worksheets({id})/createSession
Prefer: respond-async
Content-type: application/json
{
    "persistChanges": true
}
```

#### <a name="response"></a>响应
长时间运行的操作模式将返回 `202 Accepted` 如下所示的响应。

```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
Content-type: application/json

{
}
```

在某些情况下，如果创建在几秒钟内成功，则不会进入长时间运行的操作模式：相反，它将作为常规创建会话返回，成功的请求将返回 `201 Created` 响应。

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "persistChanges": true
}
```

以下示例演示请求失败时的响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

```http
HTTP/1.1 500 Internal Server Error
Content-type: application/json

{
  "error":{
    "code": "internalServerError",
    "message": "An internal server error occurred while processing the request.",
    "innerError": {
      "code": "internalServerErrorUncategorized",
      "message": "An unspecified error has occurred.",
      "innerError": {
        "code": "GenericFileOpenError",
        "message": "The workbook cannot be opened."
      }
    }
  }
}
```

### <a name="poll-status-of-the-long-running-create-session"></a>长时间运行的创建会话的轮询状态

使用长时间运行的操作模式，可以使用以下请求在指定位置获取创建状态。 建议的轮询状态间隔约为 30 秒。 最大间隔不应超过 4 分钟。

#### <a name="request"></a>请求

```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
{
}
```

#### <a name="response"></a>响应

下面是操作的状态 `running`时的响应。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": {operation-id},
    "status": "running"
}
```

下面是操作状态 `succeeded`时的响应。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": {operation-id},
    "status": "succeeded",
    "resourceLocation": "https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/sessionInfoResource(key='{key}')
}
```

下面是操作状态 `failed`时的响应。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": {operation-id},
  "status": "failed",
  "error":{
    "code": "internalServerError",
    "message": "An internal server error occurred while processing the request.",
    "innerError": {
      "code": ""internalServerErrorUncategorized",
      "message": "An unspecified error has occurred.",
      "innerError": {
        "code": "GenericFileOpenError",
        "message": "The workbook cannot be opened."
      }
    }
  }
}
```

有关错误的更多详细信息，请参阅 [错误代码和消息](workbook-error-codes.md#error-codes-and-messages)。

### <a name="acquire-session-information"></a>获取会话信息

#### <a name="request"></a>请求

如果状态 `succeeded`为，可以通过类似于以下内容的请求获取创建的会话信息 `resourceLocation` 。

```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/sessionInfoResource(key='{key}')
{
}
```

#### <a name="response"></a>响应
以下是答复。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "id-value",
    "persistChanges": true
}
```

> [!NOTE]
> 获取会话信息取决于初始请求。 如果初始请求不返回响应正文，则无需获取结果。

## <a name="reduce-throttling-errors"></a>减少限制错误

Microsoft Graph 中的 Excel API 会影响多个依赖项服务的资源使用情况。 影响可能因不同的请求而异：例如，你可能期望在小型工作簿的单个单元格中更新短字符串比向大型工作簿添加具有复杂公式的大表所消耗的资源更少。

即使具有相同的 API，参数和目标工作簿也会带来显著差异。 因此，Excel API 限制不是使用简单和通用的限制号来定义的，因为它们会导致更严格的限制。 以下最佳做法可帮助你更快地完成任务，减少限制错误。

### <a name="retry-after-header"></a>Retry-After标头

在许多情况下，限制响应包括标 `Retry-After` 头。 尊重标头的值和延迟类似的请求将有助于客户端从限制中恢复。 有关在 Microsoft Graph 中处理来自 Excel API 的错误响应的详细信息，请参阅 [Microsoft Graph 中 Excel API 的错误处理](workbook-error-handling.md)。

### <a name="throttling-and-concurrency"></a>限制和并发

与限制相关的另一个因素是请求并发。 我们建议不要在使用 Excel API 时增加并发性 (例如，将请求并行化到同一工作簿) ，尤其是对于写入请求。 相反，除非存在特定问题，例如与请求执行时间非常短相比，网络开销很大，否则建议在最常见的情况下按顺序使用：对于每个工作簿，仅在收到对当前请求的成功响应后发送下一个请求。

对同一工作簿的并发写入请求通常不会并行运行 (尽管在某些情况下它们确实) ;相反，当请求) 服务器上排队时，它们通常是限制、超时 (的原因，合并冲突 () 和其他类型的故障时涉及并发会话。 它们也会使错误处理复杂化;例如，当收到失败响应时，无法确认其他挂起的请求的状态，这使你难以确定或恢复工作簿的状态。

## <a name="see-also"></a>另请参阅

* [使用 Excel REST API](/graph/api/resources/excel)