---
title: 使用 JSON 批处理将多个请求合并为一个 HTTP 调用
description: JSON 批处理使你能够通过将多个请求合并为一个单一的 JSON 对象优化应用程序。例如，客户可能希望撰写一个无关的数据视图，例如：
author: davidmu1
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 4e1ad5734d0fefe2cdb7634e461ee9f297aae93e
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721570"
---
# <a name="combine-multiple-requests-in-one-http-call-using-json-batching"></a><span data-ttu-id="3d297-104">使用 JSON 批处理在一个 HTTP 调用中合并多个请求</span><span class="sxs-lookup"><span data-stu-id="3d297-104">Combine multiple requests in one HTTP call using JSON batching</span></span>

<span data-ttu-id="3d297-p102">JSON 批处理使你能够通过将多个请求合并为一个单一的 JSON 对象优化应用程序。例如，客户可能希望撰写一个无关的数据视图，例如：</span><span class="sxs-lookup"><span data-stu-id="3d297-p102">JSON batching allows you to optimize your application by combining multiple requests into a single JSON object. For example, a client might want to compose a view of unrelated data such as:</span></span>

1. <span data-ttu-id="3d297-107">存储在 OneDrive 中的图像</span><span class="sxs-lookup"><span data-stu-id="3d297-107">An image stored in OneDrive</span></span>
2. <span data-ttu-id="3d297-108">计划任务列表</span><span class="sxs-lookup"><span data-stu-id="3d297-108">A list of Planner tasks</span></span>
3. <span data-ttu-id="3d297-109">组日历</span><span class="sxs-lookup"><span data-stu-id="3d297-109">The calendar for a group</span></span>

<span data-ttu-id="3d297-110">将三个单独请求合并到一个单独的批处理请求中可以使应用程序不受重大网络延迟的影响。</span><span class="sxs-lookup"><span data-stu-id="3d297-110">Combining these three individual requests into a single batch request can save the application significant network latency.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/tzWGOp8zYh8]

## <a name="first-json-batch-request"></a><span data-ttu-id="3d297-111">第一个 JSON 批处理请求</span><span class="sxs-lookup"><span data-stu-id="3d297-111">First JSON batch request</span></span>

<span data-ttu-id="3d297-p103">首先，为之前的示例构建 JSON 批处理请求。在这种情况下，单个请求不会以任何方式互相依赖，因此可以按任意顺序放入批处理请求中。</span><span class="sxs-lookup"><span data-stu-id="3d297-p103">First you construct the JSON batch request for the previous example. In this scenario, the individual requests are not interdependent in any way and therefore can be placed into the batch request in any order.</span></span>

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

<span data-ttu-id="3d297-p104">对批处理请求的响应可能会按不同的顺序显示。`id` 属性可用于关联各个请求和响应。</span><span class="sxs-lookup"><span data-stu-id="3d297-p104">Responses to the batched requests might appear in a different order. The `id` property can be used to correlate individual requests and responses.</span></span>

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

## <a name="request-format"></a><span data-ttu-id="3d297-116">请求格式</span><span class="sxs-lookup"><span data-stu-id="3d297-116">Request format</span></span>

<span data-ttu-id="3d297-117">批处理请求始终使用 `POST` 发送到 `/$batch` 终结点。</span><span class="sxs-lookup"><span data-stu-id="3d297-117">Batch requests are always sent using `POST` to the `/$batch` endpoint.</span></span>

<span data-ttu-id="3d297-p105">JSON 批处理请求正文包含具有一个必需的属性 `requests` 的单个 JSON 对象。`requests` 属性是一组单独请求。对于每个单独请求而言， `id`、`method` 和 `url` 属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="3d297-p105">A JSON batch request body consists of a single JSON object with one required property: `requests`. The `requests` property is an array of individual requests. For each individual request, the `id`, `method`, and `url` properties are required.</span></span>

<span data-ttu-id="3d297-p106">`id` 属性主要用作关联单个响应和请求的相关值。这使服务器可以最高效的顺序处理批处理中的请求。</span><span class="sxs-lookup"><span data-stu-id="3d297-p106">The `id` property functions primarily as a correlation value to associate individual responses with requests. This allows the server to process requests in the batch in the most efficient order.</span></span>

<span data-ttu-id="3d297-p107">`method` 和 `url` 正是你在任何给定的 HTTP 请求开头看到的属性。该方法是 HTTP 方法，且 URL 是通常会向其发送单独请求的资源 URL。</span><span class="sxs-lookup"><span data-stu-id="3d297-p107">The `method` and `url` properties are exactly what you would see at the start of any given HTTP request. The method is the HTTP method, and the URL is the resource URL the individual request would typically be sent to.</span></span>

<span data-ttu-id="3d297-125">单独请求还可以视需要包含 `headers` 属性和 `body` 属性。</span><span class="sxs-lookup"><span data-stu-id="3d297-125">Individual requests can optionally also contain a `headers` property and a `body` property.</span></span> <span data-ttu-id="3d297-126">这两种属性通常都是 JSON 对象，如上一示例所示。</span><span class="sxs-lookup"><span data-stu-id="3d297-126">Both of these properties are typically JSON objects, as shown in the previous example.</span></span> <span data-ttu-id="3d297-127">在某些情况下，`body` 可能是经过 base64 URL 编码的值，而不是 JSON 对象（例如，当正文为图像时）。</span><span class="sxs-lookup"><span data-stu-id="3d297-127">In some cases, the `body` might be a base64 URL-encoded value rather than a JSON object - for example, when the body is an image.</span></span> <span data-ttu-id="3d297-128">如果 `body` 包含在该请求中，`headers` 对象必须包含 `Content-Type` 的值。</span><span class="sxs-lookup"><span data-stu-id="3d297-128">When a `body` is included with the request, the `headers` object must contain a value for `Content-Type`.</span></span>

## <a name="response-format"></a><span data-ttu-id="3d297-129">响应格式</span><span class="sxs-lookup"><span data-stu-id="3d297-129">Response format</span></span>

<span data-ttu-id="3d297-p109">JSON 批处理请求的响应格式与请求格式类似。主要区别如下：</span><span class="sxs-lookup"><span data-stu-id="3d297-p109">The response format for JSON batch requests is similar to the request format. The following are the key differences:</span></span>

* <span data-ttu-id="3d297-132">主 JSON 对象的中属性被命名为 `responses`，与 `requests` 相反。</span><span class="sxs-lookup"><span data-stu-id="3d297-132">The property in the main JSON object is named `responses` as opposed to `requests`.</span></span>
* <span data-ttu-id="3d297-133">单独响应可能会按与请求不同的顺序显示。</span><span class="sxs-lookup"><span data-stu-id="3d297-133">Individual responses might appear in a different order than the requests.</span></span>
* <span data-ttu-id="3d297-p110">单独响应包含的是 `status` 属性，而不是 `method` 和 `url` 属性。`status` 的值是表示 HTTP 状态代码的数字。</span><span class="sxs-lookup"><span data-stu-id="3d297-p110">Rather than `method` and `url`, individual responses have a `status` property. The value of `status` is a number that represents the HTTP status code.</span></span>

<span data-ttu-id="3d297-p111">批处理响应中的状态代码通常为 `200` 或 `400`。如果批处理请求本身格式不正确，则状态代码为 `400`。如果批处理请求可分析，则状态代码为 `200`。批处理响应中的 `200` 状态代码并不表示批处理中的单独请求已成功。这就是为什么 `responses` 属性中的每个单独响应都有状态代码。</span><span class="sxs-lookup"><span data-stu-id="3d297-p111">The status code on a batch response is typically `200` or `400`. If the batch request itself is malformed, the status code is `400`. If the batch request is parseable, the status code is `200`. A `200` status code on the batch response does not indicate that the individual requests inside the batch succeeded. This is why each individual response in the `responses` property has a status code.</span></span>

## <a name="sequencing-requests-with-the-dependson-property"></a><span data-ttu-id="3d297-141">使用 dependsOn 属性对请求进行排序</span><span class="sxs-lookup"><span data-stu-id="3d297-141">Sequencing requests with the dependsOn property</span></span>

<span data-ttu-id="3d297-p112">通过使用 `dependsOn` 属性可按指定顺序执行单独请求。此属性是引用不同的单独请求的 `id` 的字符串数组。出于这个原因，`id` 的值必须唯一。例如，在下面的请求中，客户端指定请求 1 和 3 应该先运行，然后是请求 2，然后是请求 4。</span><span class="sxs-lookup"><span data-stu-id="3d297-p112">Individual requests can be executed in a specified order by using the `dependsOn` property. This property is an array of strings that reference the `id` of a different individual request. For this reason, the values for `id` must be unique. For example, in the following request, the client is specifying that requests 1 and 3 should be run first, then request 2, then request 4.</span></span>

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

<span data-ttu-id="3d297-146">如果单独请求失败，任何依赖此请求的请求都会失败，且状态代码为 `424`（依赖项失败）。</span><span class="sxs-lookup"><span data-stu-id="3d297-146">If an individual request fails, any request that depends on that request fails with status code `424` (Failed Dependency).</span></span>

## <a name="bypassing-url-length-limitations-with-batching"></a><span data-ttu-id="3d297-147">使用批处理绕过 URL 长度限制</span><span class="sxs-lookup"><span data-stu-id="3d297-147">Bypassing URL length limitations with batching</span></span>

<span data-ttu-id="3d297-p113">JSON 批处理的其他用例是绕过 URL 长度限制。如果筛选子句太复杂，URL 长度可能会超越浏览器或其他 HTTP 客户端中内置的限制。你可以使用 JSON 批处理作为运行这些请求的解决方法，因为长 URL 只能成为请求有效负载的一部分。</span><span class="sxs-lookup"><span data-stu-id="3d297-p113">An additional use case for JSON batching is to bypass URL length limitations. In cases where the filter clause is complex, the URL length might surpass limitations built into browsers or other HTTP clients. You can use JSON batching as a workaround for running these requests because the lengthy URL simply becomes part of the request payload.</span></span>

## <a name="known-issues"></a><span data-ttu-id="3d297-151">已知问题</span><span class="sxs-lookup"><span data-stu-id="3d297-151">Known issues</span></span>

<span data-ttu-id="3d297-152">有关与批处理相关的当前限制列表，请参阅[已知问题][batching-known-issues]。</span><span class="sxs-lookup"><span data-stu-id="3d297-152">For a list of current limitations related to batching, see [known issues][batching-known-issues].</span></span>

[batching-known-issues]: known-issues.md#json-batching
[odata-4.01-json]: https://www.oasis-open.org/committees/download.php/60365/odata-json-format-v4.01-wd02-2017-03-24.docx


## <a name="see-also"></a><span data-ttu-id="3d297-153">另请参阅</span><span class="sxs-lookup"><span data-stu-id="3d297-153">See also</span></span>

<span data-ttu-id="3d297-154">关于JSON批量请求/响应格式的更多信息，请参见 [OData JSON Format 4.01版规范](http://docs.oasis-open.org/odata/odata-json-format/v4.01/odata-json-format-v4.01.html#sec_BatchRequestsandResponses) ，章节 _Batch Requests and Responses_。</span><span class="sxs-lookup"><span data-stu-id="3d297-154">For more information about the JSON batch request/response format, see the [OData JSON Format Version 4.01 specification](http://docs.oasis-open.org/odata/odata-json-format/v4.01/odata-json-format-v4.01.html#sec_BatchRequestsandResponses), section _Batch Requests and Responses_.</span></span>
