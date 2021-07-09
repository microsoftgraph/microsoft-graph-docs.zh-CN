---
title: 使用 JSON 批处理将多个请求合并为一个 HTTP 调用
description: JSON 批处理使你能够通过将多个请求合并为一个单一的 JSON 对象优化应用程序。例如，客户可能希望撰写一个无关的数据视图，例如：
author: davidmu1
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 06ac2bdae205f7525b912c7ea3bd396a2cceae74
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334806"
---
# <a name="combine-multiple-requests-in-one-http-call-using-json-batching"></a>使用 JSON 批处理在一个 HTTP 调用中合并多个请求

通过 JSON 批处理，可通过将多个请求(最多 20 个)合并为一个单一的 JSON 对象来优化应用程序。例如，客户可能希望撰写一个无关数据的视图，例如：

1. 存储在 OneDrive 中的图像
2. 计划任务列表
3. 组日历

将三个单独请求合并到一个单独的批处理请求中可以使应用程序不受重大网络延迟的影响。

> [!VIDEO https://www.youtube-nocookie.com/embed/tzWGOp8zYh8]

## <a name="first-json-batch-request"></a>第一个 JSON 批处理请求

首先，为之前的示例构建 JSON 批处理请求。在这种情况下，单个请求不会以任何方式互相依赖，因此可以按任意顺序放入批处理请求中。

```http
POST https://graph.microsoft.com/v1.0/$batch
Accept: application/json
Content-Type: application/json
```

```json
{
  "requests": [
    {
      "id": "1",
      "method": "GET",
      "url": "/me/drive/root:/{file}:/content"
    },
    {
      "id": "2",
      "method": "GET",
      "url": "/me/planner/tasks"
    },
    {
      "id": "3",
      "method": "GET",
      "url": "/groups/{id}/events"
    },
    {
      "id": "4",
      "url": "/me",
      "method": "PATCH",
      "body": {
        "city" : "Redmond"
      },
      "headers": {
        "Content-Type": "application/json"
      }
    }
  ]
}
```

对批处理请求的响应可能会按不同的顺序显示。`id` 属性可用于关联各个请求和响应。

```http
200 OK
Content-Type: application/json
```

```json
{
  "responses": [
    {
      "id": "1",
      "status": 302,
      "headers": {
        "location": "https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi"
      }
    },
    {
      "id": "3",
      "status": 401,
      "body": {
        "error": {
          "code": "Forbidden",
          "message": "..."
        }
      }
    },
    {
      "id": "2",
      "status": 200,
      "body": {
        "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.plannerTask)",
        "value": []
      }
    },
    {
      "id": "4",
      "status": 204,
      "body": null
    }
  ]
}
```

## <a name="request-format"></a>请求格式

批处理请求始终使用 `POST` 发送到 `/$batch` 终结点。

JSON 批处理请求正文包含具有一个必需的属性 `requests` 的单个 JSON 对象。`requests` 属性是一组单独请求。对于每个单独请求而言， `id`、`method` 和 `url` 属性是必需的。

`id` 属性主要用作关联单个响应和请求的相关值。这使服务器可以最高效的顺序处理批处理中的请求。

`method` 和 `url` 正是你在任何给定的 HTTP 请求开头看到的属性。该方法是 HTTP 方法，且 URL 是通常会向其发送单独请求的资源 URL。

单独请求还可以视需要包含 `headers` 属性和 `body` 属性。 这两种属性通常都是 JSON 对象，如上一示例所示。 在某些情况下，`body` 可能是经过 base64 URL 编码的值，而不是 JSON 对象（例如，当正文为图像时）。 如果 `body` 包含在该请求中，`headers` 对象必须包含 `Content-Type` 的值。

## <a name="response-format"></a>响应格式

JSON 批处理请求的响应格式与请求格式类似。主要区别如下：

* 主 JSON 对象的中属性被命名为 `responses`，与 `requests` 相反。
* 单独响应可能会按与请求不同的顺序显示。
* 单独响应包含的是 `status` 属性，而不是 `method` 和 `url` 属性。`status` 的值是表示 HTTP 状态代码的数字。

批处理响应中的状态代码通常为 `200` 或 `400`。如果批处理请求本身格式不正确，则状态代码为 `400`。如果批处理请求可分析，则状态代码为 `200`。批处理响应中的 `200` 状态代码并不表示批处理中的单独请求已成功。这就是为什么 `responses` 属性中的每个单独响应都有状态代码。

## <a name="sequencing-requests-with-the-dependson-property"></a>使用 dependsOn 属性对请求进行排序

通过使用 `dependsOn` 属性可按指定顺序执行单独请求。此属性是引用不同的单独请求的 `id` 的字符串数组。出于这个原因，`id` 的值必须唯一。例如，在下面的请求中，客户端指定请求 1 和 3 应该先运行，然后是请求 2，然后是请求 4。

```json
{
  "requests": [
    {
      "id": "1",
      "method": "GET",
      "url": "..."
    },
    {
      "id": "2",
      "dependsOn": [ "1" ],
      "method": "GET",
      "url": "..."
    },
    {
      "id": "3",
      "method": "GET",
      "url": "..."
    },
    {
      "id": "4",
      "dependsOn": [ "2" ],
      "method": "GET",
      "url": "..."
    }
  ]
}
```

如果单独请求失败，任何依赖此请求的请求都会失败，且状态代码为 `424`（依赖项失败）。

## <a name="bypassing-url-length-limitations-with-batching"></a>使用批处理绕过 URL 长度限制

JSON 批处理的其他用例是绕过 URL 长度限制。如果筛选子句太复杂，URL 长度可能会超越浏览器或其他 HTTP 客户端中内置的限制。你可以使用 JSON 批处理作为运行这些请求的解决方法，因为长 URL 只能成为请求有效负载的一部分。

## <a name="known-issues"></a>已知问题

有关与批处理相关的当前限制列表，请参阅[已知问题][batching-known-issues]。

[batching-known-issues]: known-issues.md#json-batching
[odata-4.01-json]: https://www.oasis-open.org/committees/download.php/60365/odata-json-format-v4.01-wd02-2017-03-24.docx


## <a name="see-also"></a>另请参阅

关于JSON批量请求/响应格式的更多信息，请参见 [OData JSON Format 4.01版规范](http://docs.oasis-open.org/odata/odata-json-format/v4.01/odata-json-format-v4.01.html#sec_BatchRequestsandResponses) ，章节 _Batch Requests and Responses_。
