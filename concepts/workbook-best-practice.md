---
title: Microsoft Excel API 的最佳实践Graph
description: 列出 Microsoft Excel API 的最佳实践和Graph
author: grangeryy
ms.localizationpriority: medium
ms.prod: excel
ms.openlocfilehash: 17833cacc58ddc431e1488826391e5eb36ee06b8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59142339"
---
# <a name="best-practices-for-working-with-the-excel-api-in-microsoft-graph"></a>在 Microsoft Excel 中处理 Graph API 的最佳实践

本文提供有关在 Microsoft Excel 中处理 Graph。

## <a name="manage-sessions-in-the-most-efficient-way"></a>以最有效的方式管理会话

如果你在一定时间内进行多个呼叫，我们建议你创建一个会话，并传递每个请求的会话 ID。 若要表示 API 中的会话，请使用 `workbook-session-id: {session-id}` 标头。 通过执行此操作，你可以最Excel使用应用程序 API。

以下示例演示如何将新数字添加到表中，然后使用这种方法在工作簿中查找一条记录。

### <a name="step-1-create-a-session"></a>步骤 1：创建会话

#### <a name="request"></a>请求

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/createSession
Content-type: application/json
Content-length: 52

{
  "persistChanges": true
}
```
#### <a name="response"></a>响应

下面是一个成功响应。

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "persistChanges": true
}
```

### <a name="step-2-add-a-new-row-to-the-table"></a>步骤 2：向表中添加新行

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
Content-length: 42

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
Content-length: 0

{
}
```

#### <a name="response"></a>响应

```http
HTTP/1.1 204 No Content
```

有关详细信息，请参阅创建[会话和](/graph/api/workbook-createsession?view=graph-rest-1.0)[关闭会话](/graph/api/workbook-closesession?view=graph-rest-1.0)。

## <a name="working-with-apis-that-take-a-long-time-to-complete"></a>使用需要很长时间才能完成的 API

您可能会注意到，某些操作需要不确定的时间才能完成;例如，打开一个大型工作簿。 在等待这些请求的响应时，很容易命中超时。 为了解决此问题，我们提供长时间运行的操作模式。 使用此模式时，无需担心请求超时。

目前，Microsoft Excel API 中的会话Graph已启用长时间运行的操作模式。 此模式涉及以下步骤：

1. 向 `Prefer: respond-async` 请求添加标头，以指示在加入会话时这是一个长时间运行的操作。
2. 长时间运行的操作将返回 响应 `202 Accepted` 以及 Location 标头，以检索操作状态。 如果会话创建在几秒后完成，它将返回常规创建会话响应，而不是使用长时间运行的操作模式。
3. 通过 `202 Accepted` 响应，您可以在指定位置检索操作状态。 操作状态值包括 `notStarted` `running` 、、 `succeeded` 和 `failed` 。
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
长时间运行的操作模式将返回 `202 Accepted` 类似于以下内容的响应。

```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
Content-type: application/json

{
}
```

在某些情况下，如果创建在几秒内成功，它不会进入长时间运行的操作模式;相反，它将作为常规创建会话返回，并且成功的请求将返回 `201 Created` 响应。

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "persistChanges": true
}
```

以下示例显示请求失败时的响应。

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


使用长时间运行的操作模式，可以通过以下请求获取指定位置的创建状态。 建议的轮询状态的间隔约为 30 秒。 最大间隔不应超过 4 分钟。

#### <a name="request"></a>请求

```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
{
}
```

#### <a name="response"></a>响应

下面是操作的状态为 时的响应 `running` 。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": {operation-id},
    "status": "running"
}
```

下面是操作状态为 时的响应 `succeeded` 。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": {operation-id},
    "status": "succeeded",
    "resourceLocation": "https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/sessionInfoResource(key='{key}')
}
```

下面是操作状态为 时的响应 `failed` 。

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

有关错误的更多详细信息，请参阅错误 [代码](workbook-error-codes.md#error-code)。

### <a name="acquire-session-information"></a>获取会话信息

#### <a name="request"></a>请求

状态为 `succeeded` 时，可以通过类似如下的请求获取创建的 `resourceLocation` 会话信息。

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

>**注意：** 获取会话信息取决于初始请求。 如果初始请求未返回响应正文，则无需获取结果。
