---
title: Microsoft Graph 中的 Excel Api 的最佳实践
description: 在 Microsoft Graph 中列出 Excel Api 的最佳实践和示例
author: grangeryy
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: d824cf89a07c81bae3a2e129896da9af282be49c
ms.sourcegitcommit: bbff139eea483faaa2d1dd08af39314f35ef48ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/08/2020
ms.locfileid: "46598573"
---
# <a name="best-practices-for-working-with-the-excel-api-in-microsoft-graph"></a>在 Microsoft Graph 中使用 Excel API 的最佳实践

本文提供了有关在 Microsoft Graph 中使用 Excel Api 的建议。

## <a name="manage-sessions-in-the-most-efficient-way"></a>以最有效的方式管理会话

如果您在一定时间内进行了多次调用，我们建议您创建一个会话并将会话 ID 传递给每个请求。 若要表示 API 中的会话，请使用 `workbook-session-id: {session-id}` 标头。 通过执行此操作，您可以以最有效的方式使用 Excel Api。

下面的示例演示如何使用此方法向表中添加新数字，然后在工作簿中查找一条记录。

### <a name="step-1-create-a-session"></a>步骤1：创建会话

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

以下是成功的响应。

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "persistChanges": true
}
```

### <a name="step-2-add-a-new-row-to-the-table"></a>步骤2：向表中添加新行

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

### <a name="step-3-look-up-a-value-in-the-updated-table"></a>步骤3：在更新后的表格中查找值

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

### <a name="step-4-close-the-session-after-all-the-requests-are-completed"></a>步骤4：在所有请求都完成后关闭会话

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

有关更多详细信息，请参阅[创建会话](/graph/api/workbook-createsession?view=graph-rest-1.0)和[关闭会话](/graph/api/workbook-closesession?view=graph-rest-1.0)。

## <a name="working-with-apis-that-take-a-long-time-to-complete"></a>使用需要很长时间才能完成的 Api

您可能会注意到，某些操作需要的时间不确定，无法完成。例如，打开一个大型工作簿。 在等待对这些请求的响应时，很容易就会遇到超时。 若要解决此问题，我们提供了长期运行的操作模式。 使用此模式时，无需担心请求的超时。

目前，Microsoft Graph 中的会话创建 Excel API 启用了长时间运行的操作模式。 此模式涉及以下步骤：

1. 将 `Prefer: respond-async` 标头添加到请求，以指示在你为会话发货时，它是一个长时间运行的操作。
2. 长时间运行的操作将返回 `202 Accepted` 响应以及位置标头以检索操作状态。 如果会话创建在几秒内完成，它将返回常规的 create session 响应，而不是使用长时间运行的操作模式。
3. 通过 `202 Accepted` 响应，可以在指定位置检索操作状态。 操作状态值包括 `notStarted` 、 `running` 、 `succeeded` 和 `failed` 。
4. 操作完成后，可以通过成功响应中的指定 URL 获取会话创建结果。

下面的示例使用长时间运行的操作模式创建会话。

### <a name="initial-request-to-create-session"></a>创建会话的初始请求

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/worksheets({id})/createSession
Prefer: respond-async
Content-type: application/json
{
    "persistChanges": true
}
```

### <a name="response"></a>响应

长时间运行的操作模式将返回 `202 Accepted` 如下所示的响应。

```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
Content-type: application/json

{
}
```

在某些情况下，如果创建在几秒后成功，则不会进入长时间运行的操作模式;相反，它作为常规创建会话返回，成功的请求将返回 `201 Created` 响应。

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "persistChanges": true
}
```

下面的示例演示请求失败时的响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

```http
HTTP/1.1 500 Internal Server Error
Content-type: application/json
{
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


### Poll status of the long-running create session

With the long-running operation pattern, you can get the creation status at specified location by using the following request. The suggested interval to poll status is around 30 seconds. The maximum interval should be no more than 4 minutes.

```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
{
}
```

以下是操作状态为时的响应 `running` 。

```http
HTTP/1.1 200 OK
Content-type: application/json
{
    "id": {operation-id},
    "status": "running"
}
```

以下是操作状态为时的响应 `succeeded` 。

```http
HTTP/1.1 200 OK
Content-type: application/json
{
    "id": {operation-id},
    "status": "succeeded",
    "resourceLocation": "https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/sessionInfoResource(key='{key}')
}
```

以下是操作状态为时的响应 `failed` 。

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

有关错误的更多详细信息，请参阅[错误代码](/concepts/workbook-error-codes.md)

### <a name="acquire-session-information"></a>获取会话信息

使用的状态 `succeeded` ，您可以通过 `resourceLocation` 与以下内容类似的请求来获取创建的会话信息。

```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/sessionInfoResource(key='{key}')
{
}
```

以下是答复。

```http
HTTP/1.1 200 OK
Content-type: application/json
{
    "id": "id-value",
    "persistChanges": true
}
```

>**注意：** 获取会话信息取决于初始请求。 如果初始请求不返回响应正文，则无需获取结果。
