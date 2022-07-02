---
title: 使用 JSON 批处理将多个请求合并为一个 HTTP 调用
description: 通过将多个请求合并到单个 JSON 对象中，使用 JSON 批处理来优化应用程序，从而显著节省应用程序的网络延迟。
author: FaithOmbongi
ms.localizationpriority: high
ms.custom: graphiamtop20
ms.openlocfilehash: 7ba6dace8424158c7d04279de3c53e1734681e00
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2022
ms.locfileid: "66555777"
---
# <a name="combine-multiple-requests-in-one-http-call-using-json-batching"></a>使用 JSON 批处理在一个 HTTP 调用中合并多个请求

通过 JSON 批处理，可通过将多个请求(最多 20 个)合并为一个单一的 JSON 对象来优化应用程序。例如，客户可能希望撰写一个无关数据的视图，例如：

- 存储在 OneDrive 中的图像
- 计划任务列表
- 组日历

将三个单独请求合并到一个单独的批处理请求中可以使应用程序不受重大网络延迟的影响。

Microsoft Graph 实现 `$batch` OData URL 路径段，以支持 JSON 批处理。

> [!VIDEO https://www.youtube-nocookie.com/embed/tzWGOp8zYh8]

## <a name="first-json-batch-request"></a>第一个 JSON 批处理请求

首先，为之前的示例构建 JSON 批处理请求。在这种情况下，单个请求不会以任何方式互相依赖，因此可以按任意顺序放入批处理请求中。

```msgraph-interactive
POST https://graph.microsoft.com/v1.0/$batch
Accept: application/json
Content-Type: application/json

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
    },
    {
      "id": "5",
      "url": "users?$select=id,displayName,userPrincipalName&$filter=city eq null&$count=true",
      "method": "GET",
      "headers": {
        "ConsistencyLevel": "eventual"
      }
    }
  ]
}
```

对批处理请求的响应可能会按不同的顺序显示。**id** 属性可用于关联各个请求和响应。

```http
200 OK
Content-Type: application/json

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
      "id": "5",
      "status": 200,
      "headers": {
        "OData-Version": "4.0",
      },
      "body": {
        "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users(id,displayName,userPrincipalName)",
        "@odata.count": 12,
        "value": [
          {
            "id": "071cc716-8147-4397-a5ba-b2105951cc0b",
            "displayName": "Adele Vance",
            "userPrincipalName": "AdeleV@Contoso.com"
          }
        ]
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

批处理请求始终使用 **POST** 发送到 `/$batch` 终结点。

JSON 批处理请求正文由具有一个必需属性的单个 JSON 对象组成: **请求**。**请求** 属性是单个请求的集合。对于每个单独的请求，可以传递以下属性。


| 属性 | 说明 |
|----------|-------------|
| id       | 必填。用于将单个响应与请求相关联的相关值。此值允许服务器以最高效的顺序处理批处理中的请求。    |
| 方法   | 必需项。 HTTP 方法。    |
| url      | 必需项。 单个请求通常会发送到的相对资源 URL。 因此，尽管绝对 URL 为 `https://graph.microsoft.com/v1.0/users`，但此 URL 为 `/users`。 |
| 标头   | 可选，但在指定 **正文** 时是必填的。 具有标头的键/值对的 JSON 对象。 例如，当需要 **ConsistencyLevel** 标头时，此属性将表示为 `"headers": {"ConsistencyLevel": "eventual"}`。 提供 **正文** 时，必须包含 **Content-Type** 标头。    |
| body   | 可选。 可以是 JSON 对象或 base64 URL 编码的值，例如，当正文是图像时。 当请求中包含 **正文** 时，**标头** 对象必须包含 **Content-Type** 的值。 |

## <a name="response-format"></a>响应格式

JSON 批处理请求的响应格式与请求格式类似。主要区别如下：

* 主 JSON 对象中的属性命名为 **响应** 而不是 **请求**。
* 单独响应可能会按与请求不同的顺序显示。
* 单个响应具有 **状态** 属性，而不是 **方法** 和 **URL**。**状态** 值是表示 HTTP 状态代码的数字。
* 每个响应中的 **headers** 属性表示服务器返回的标头，例如 **Cache-Control** 和 **Content-Type** 标头。

批处理响应中的状态代码通常为 `200` 或 `400`。如果批处理请求本身格式不正确，则状态代码为 `400`。如果批处理请求可分析，则状态代码为 `200`。批处理响应中的 `200` 状态代码并不表示批处理中的单独请求已成功。这就是为什么 **响应** 属性中的每个单独响应都有状态代码。

## <a name="sequencing-requests-with-the-dependson-property"></a>使用 dependsOn 属性对请求进行排序

可以通过使用 **dependsOn** 属性按指定顺序执行单个请求。此属性是引用不同单个请求的 **ID** 的字符串数组。因此，**ID** 值必须是唯一的。例如，在以下请求中，客户端指定应按照请求 1 中运行请求，然后请求 3，然后请求 2，然后请求 4。

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
      "id": "4",
      "dependsOn": [ "2" ],
      "method": "GET",
      "url": "..."
    },
    {
      "id": "3",
      "dependsOn": [ "4" ],
      "method": "GET",
      "url": "..."
    }
  ]
}
```

如果单独请求失败，任何依赖此请求的请求都会失败，且状态代码为 `424`（依赖项失败）。

> [!TIP]
> 批处理应是完全有序的或完全并行的。

## <a name="bypassing-url-length-limitations-with-batching"></a>使用批处理绕过 URL 长度限制

JSON 批处理的其他用例是绕过 URL 长度限制。如果筛选子句太复杂，URL 长度可能会超越浏览器或其他 HTTP 客户端中内置的限制。你可以使用 JSON 批处理作为运行这些请求的解决方法，因为长 URL 只能成为请求有效负载的一部分。

## <a name="batch-size-limitations"></a>批大小限制

JSON 批处理请求目前限制为 20 个单独的请求，此外还有以下限制：

* 根据作为批处理请求一部分的 API，基础服务会施加自己的限制，从而影响使用 Microsoft Graph 访问它们的应用程序。
* 批处理中的请求将根据限制单独进行评估，如果任何请求超过限制，则请求会失败，状态为 `429`。
* 面向 Outlook 资源的批处理（如邮件和日历）只能包含四个针对同一邮箱的请求。 有关详细信息，请参阅 [Outlook 服务限制][throttling-outlook]。

有关详细信息，请参阅 [限制和批处理][throttling-and-batching]。

## <a name="known-issues"></a>已知问题

有关与批处理相关的当前限制列表，请参阅[已知问题][batching-known-issues]。

[batching-known-issues]: known-issues.md#json-batching
[odata-4.01-json]: https://www.oasis-open.org/committees/download.php/60365/odata-json-format-v4.01-wd02-2017-03-24.docx
[throttling-and-batching]: throttling.md#throttling-and-batching
[throttling-outlook]: throttling.md#outlook-service-limits

## <a name="see-also"></a>另请参阅

关于JSON批量请求/响应格式的更多信息，请参见 [OData JSON Format 4.01版规范](http://docs.oasis-open.org/odata/odata-json-format/v4.01/odata-json-format-v4.01.html#sec_BatchRequestsandResponses) ，章节 _Batch Requests and Responses_。
