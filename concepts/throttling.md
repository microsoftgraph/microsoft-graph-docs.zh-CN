---
title: Microsoft Graph 限制指南
description: 限制可调节并发调用服务的数量，以防止资源的过度使用。Microsoft Graph 旨在用于处理大量的请求。如果出现过多请求，限制将有助于保持 Microsoft Graph 的最佳性能和服务的可靠性。
author: davidmu1
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: f00ef6f5c45736724f145e036a7fa78abdd107df
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811845"
---
# <a name="microsoft-graph-throttling-guidance"></a><span data-ttu-id="945a0-105">Microsoft Graph 限制指南</span><span class="sxs-lookup"><span data-stu-id="945a0-105">Microsoft Graph throttling guidance</span></span>

<span data-ttu-id="945a0-p102">限制可调节并发调用服务的数量，以防止资源的过度使用。Microsoft Graph 旨在用于处理大量的请求。如果出现过多请求，限制将有助于保持 Microsoft Graph 的最佳性能和服务的可靠性。</span><span class="sxs-lookup"><span data-stu-id="945a0-p102">Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span></span>

<span data-ttu-id="945a0-p103">根据该方案，执行的限制会有所不同。例如，如果你正在执行大量的写入操作，限制的可能性会比仅执行读取时要高。</span><span class="sxs-lookup"><span data-stu-id="945a0-p103">Throttling limits vary based on the scenario. For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span></span>

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a><span data-ttu-id="945a0-111">在限制时，会发生什么情况？</span><span class="sxs-lookup"><span data-stu-id="945a0-111">What happens when throttling occurs?</span></span>
<!-- markdownlint-enable MD026 -->

<span data-ttu-id="945a0-p104">超出限制阈值后，Microsoft Graph 会在一段时间内限制来自该客户端的任何进一步的请求。发生限制时，Microsoft Graph 将返回 HTTP 状态代码 429（请求过多），同时请求失败。在失败的请求的响应标头中返回建议的等待时间。限制行为取决于请求的类型和数量。例如，如果你有大量的请求，则所有请求类型受限。阈值限制根据请求类型而有所不同。因此，你可能会遇到这样一种场景，在场景中，写入被限制，但仍允许读取。</span><span class="sxs-lookup"><span data-stu-id="945a0-p104">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time. When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail. A suggested wait time is returned in the response header of the failed request. Throttling behavior can depend on the type and number of requests. For example, if you have a high volume of requests, all requests types are throttled. Threshold limits vary based on the request type. Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span>

## <a name="common-throttling-scenarios"></a><span data-ttu-id="945a0-119">常见的限制场景</span><span class="sxs-lookup"><span data-stu-id="945a0-119">Common throttling scenarios</span></span>

<span data-ttu-id="945a0-120">客户端受限的最常见原因包括：</span><span class="sxs-lookup"><span data-stu-id="945a0-120">The most common causes of throttling of clients include:</span></span>

- <span data-ttu-id="945a0-121">来自租户中所有应用程序的请求太多。</span><span class="sxs-lookup"><span data-stu-id="945a0-121">A large number of requests across all applications in a tenant.</span></span>
- <span data-ttu-id="945a0-122">来自所有租户中特定应用程序的请求太多。</span><span class="sxs-lookup"><span data-stu-id="945a0-122">A large number of requests from a particular application across all tenants.</span></span>

## <a name="sample-response"></a><span data-ttu-id="945a0-123">示例响应</span><span class="sxs-lookup"><span data-stu-id="945a0-123">Sample response</span></span>

<span data-ttu-id="945a0-124">每当超出限制阈值时，Microsoft Graph 都会提供与此类似的响应。</span><span class="sxs-lookup"><span data-stu-id="945a0-124">Whenever the throttling threshold is exceeded, Microsoft Graph responds with a response similar to this one.</span></span>

```http
HTTP/1.1 429 Too Many Requests
Content-Type: application/json
Retry-After: 2.128

{
  "error": {
    "code": "TooManyRequests",
    "innerError": {
      "code": "429",
      "date": "2020-08-18T12:51:51",
      "message": "Please retry after",
      "request-id": "94fb3b52-452a-4535-a601-69e0a90e3aa2",
      "status": "429"
    },
    "message": "Please retry again laster."
  }
}
```

## <a name="best-practices-to-handle-throttling"></a><span data-ttu-id="945a0-125">处理限制的最佳实践</span><span class="sxs-lookup"><span data-stu-id="945a0-125">Best practices to handle throttling</span></span>

<span data-ttu-id="945a0-126">以下是处理限制的最佳做法：</span><span class="sxs-lookup"><span data-stu-id="945a0-126">The following are best practices for handling throttling:</span></span>

- <span data-ttu-id="945a0-127">减少每个请求的操作数量。</span><span class="sxs-lookup"><span data-stu-id="945a0-127">Reduce the number of operations per request.</span></span>
- <span data-ttu-id="945a0-128">减少调用频率。</span><span class="sxs-lookup"><span data-stu-id="945a0-128">Reduce the frequency of calls.</span></span>
- <span data-ttu-id="945a0-129">不要立即重试，因为所有请求都会计入使用限制。</span><span class="sxs-lookup"><span data-stu-id="945a0-129">Avoid immediate retries, because all requests accrue against your usage limits.</span></span>

<span data-ttu-id="945a0-p105">进行错误处理时，使用 HTTP 错误代码 429 检测限制。失败的响应包括 `Retry-After` 响应标头。使用 `Retry-After` 延迟回退请求是从限制中恢复的最快速的方式，因为 Microsoft Graph 会在客户端受限时继续记录资源使用状况。</span><span class="sxs-lookup"><span data-stu-id="945a0-p105">When you implement error handling, use the HTTP error code 429 to detect throttling. The failed response includes the `Retry-After` response header. Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span></span>

1. <span data-ttu-id="945a0-133">等待 `Retry-After` 标头中指定的秒数。</span><span class="sxs-lookup"><span data-stu-id="945a0-133">Wait the number of seconds specified in the `Retry-After` header.</span></span>
2. <span data-ttu-id="945a0-134">请重试请求。</span><span class="sxs-lookup"><span data-stu-id="945a0-134">Retry the request.</span></span>
3. <span data-ttu-id="945a0-p106">如果请求再次失败，并显示 429 错误代码，则表示你仍然受限。继续使用建议的 `Retry-After` 延迟并重试请求直到成功。</span><span class="sxs-lookup"><span data-stu-id="945a0-p106">If the request fails again with a 429 error code, you are still being throttled. Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span></span>

<span data-ttu-id="945a0-137">除非有说明，否则[服务特定限制](#service-specific-limits)部分中所述的所有资源和 API 均提供 `Retry-After` 标头。</span><span class="sxs-lookup"><span data-stu-id="945a0-137">All the resources and APIs described in the [Service-specific limits](#service-specific-limits) section provide a `Retry-After` header except when noted.</span></span>

<span data-ttu-id="945a0-138">有关 Microsoft 云限制的更广泛讨论，请参阅[限制模式](https://docs.microsoft.com/azure/architecture/patterns/throttling)。</span><span class="sxs-lookup"><span data-stu-id="945a0-138">For a broader discussion of throttling in the Microsoft Cloud, see [Throttling pattern](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span></span>

> [!NOTE]
> <span data-ttu-id="945a0-139">如果响应未提供 `Retry-After` 标头，我们建议实施指数退避重试策略。</span><span class="sxs-lookup"><span data-stu-id="945a0-139">If no `Retry-After` header is provided by the response, we recommend implementing an exponential backoff retry policy.</span></span> <span data-ttu-id="945a0-140">构建大型应用程序时，还可以实现[更高级的模式](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency)。</span><span class="sxs-lookup"><span data-stu-id="945a0-140">You can also implement [more advanced patterns](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) when building large-scale applications.</span></span>
>
> <span data-ttu-id="945a0-141">Microsoft Graph SDK 已实施依赖于 `Retry-After` 标头或默认为指数退避重试策略的处理程序。</span><span class="sxs-lookup"><span data-stu-id="945a0-141">Microsoft Graph SDKs already implement handlers that rely on the `Retry-After` header or default to an exponential backoff retry policy.</span></span>

## <a name="best-practices-to-avoid-throttling"></a><span data-ttu-id="945a0-142">避免限制的最佳做法</span><span class="sxs-lookup"><span data-stu-id="945a0-142">Best practices to avoid throttling</span></span>

<span data-ttu-id="945a0-143">如持续轮询资源以检查更新以及定期扫描资源集合以检查新资源或已删除资源之类的编程模式，更有可能导致应用程序受到限制并降低整体性能。</span><span class="sxs-lookup"><span data-stu-id="945a0-143">Programming patterns like continuously polling a resource to check for updates and regularly scanning resource collections to check for new or deleted resources are more likely to lead to applications being throttled and degrade overall performances.</span></span> <span data-ttu-id="945a0-144">如果可用，改为使用[更改跟踪](delta-query-overview.md)并[更改通知](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="945a0-144">You should instead leverage [change tracking](delta-query-overview.md) and [change notifications](webhooks.md) when available.</span></span>

>[!NOTE]
><span data-ttu-id="945a0-145">[大规模发现文件和检测更改的最佳做法](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online)详细介绍最佳做法。</span><span class="sxs-lookup"><span data-stu-id="945a0-145">[Best practices for discovering files and detecting changes at scale](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online) describes best practices in details.</span></span>

## <a name="throttling-and-batching"></a><span data-ttu-id="945a0-146">限制和批处理</span><span class="sxs-lookup"><span data-stu-id="945a0-146">Throttling and batching</span></span>

<span data-ttu-id="945a0-147">[JSON 批处理](./json-batching.md)使你能够通过将多个请求合并为单个 JSON 对象来优化应用程序。</span><span class="sxs-lookup"><span data-stu-id="945a0-147">[JSON batching](./json-batching.md) allows you to optimize your application by combining multiple requests into a single JSON object.</span></span> <span data-ttu-id="945a0-148">批次中的请求将根据限制进行单独评估，如果任何请求超出限制，则它将失败，并出现 `status` `429` 以及类似于上述内容的错误。</span><span class="sxs-lookup"><span data-stu-id="945a0-148">Requests in a batch are evaluated individually against throttling limits and if any request exceeds the limits, it fails with a `status` of `429` and an error similar to the one provided above.</span></span> <span data-ttu-id="945a0-149">批次本身失败，状态代码为 `424`（失败的相关性）。</span><span class="sxs-lookup"><span data-stu-id="945a0-149">The batch itself fails with a status code of `424` (Failed Dependency).</span></span> <span data-ttu-id="945a0-150">多个请求可能会在单个批次中受到限制。</span><span class="sxs-lookup"><span data-stu-id="945a0-150">It is possible for multiple requests to be throttled in a single batch.</span></span> <span data-ttu-id="945a0-151">应使用 JSON 内容的 `retry-after` 响应标头中提供的值，尝试批次中每个失败的请求。</span><span class="sxs-lookup"><span data-stu-id="945a0-151">You should retry each failed request from the batch using the value provided in the `retry-after` response header from the JSON content.</span></span> <span data-ttu-id="945a0-152">你可以在最长 `retry-after` 值之后重试新批次中所有失败的请求。</span><span class="sxs-lookup"><span data-stu-id="945a0-152">You may retry all the failed requests in a new batch after the longest `retry-after` value.</span></span>

<span data-ttu-id="945a0-153">如果在受限制请求未经批处理时，SDK 自动重试这些请求，则不会自动重试属于批次的受限制请求。</span><span class="sxs-lookup"><span data-stu-id="945a0-153">If SDKs retry throttled requests automatically when they are not batched, throttled requests that were part of a batch are not retried automatically.</span></span>

## <a name="service-specific-limits"></a><span data-ttu-id="945a0-154">服务特定限制</span><span class="sxs-lookup"><span data-stu-id="945a0-154">Service-specific limits</span></span>

<span data-ttu-id="945a0-155">借助 Microsoft Graph，用户可访问[多个服务](overview-major-services.md)中的数据，如 Outlook 或 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="945a0-155">Microsoft Graph allows you to access data in [multiple services](overview-major-services.md), such as Outlook or Azure Active Directory.</span></span> <span data-ttu-id="945a0-156">这些服务实施自己的限制，这些限制会影响使用 Microsoft Graph 访问它们的应用程序。</span><span class="sxs-lookup"><span data-stu-id="945a0-156">These services impose their own throttling limits that affect applications that use Microsoft Graph to access them.</span></span>

<span data-ttu-id="945a0-157">任何请求均可根据多个限制进行评估，具体取决于限制范围（所有租户中的每个应用、所有应用的每个租户、每个租户的每个应用等）、请求类型（GET、 POST、PATCH等）以及其他因素。</span><span class="sxs-lookup"><span data-stu-id="945a0-157">Any request can be evaluated against multiple limits, depending on the scope of the limit (per app across all tenants, per tenant for all apps, per app per tenant, and so on), the request type (GET, POST, PATCH, and so on), and other factors.</span></span> <span data-ttu-id="945a0-158">即将达到的第一个限制会触发阻止行为。</span><span class="sxs-lookup"><span data-stu-id="945a0-158">The first limit to be reached triggers throttling behavior.</span></span> <span data-ttu-id="945a0-159">除了本节中描述的服务特定限制之外，还适用以下全局限制：</span><span class="sxs-lookup"><span data-stu-id="945a0-159">In addition to the service specific-limits described in the section, the following global limits apply:</span></span>

| <span data-ttu-id="945a0-160">请求类型</span><span class="sxs-lookup"><span data-stu-id="945a0-160">Request type</span></span> | <span data-ttu-id="945a0-161">所有租户中的每个应用</span><span class="sxs-lookup"><span data-stu-id="945a0-161">Per app across all tenants</span></span>  |
| ------------ | ------------------------ |
| <span data-ttu-id="945a0-162">任何</span><span class="sxs-lookup"><span data-stu-id="945a0-162">Any</span></span>          | <span data-ttu-id="945a0-163">每秒 2000 个请求</span><span class="sxs-lookup"><span data-stu-id="945a0-163">2000 requests per second</span></span> |

> [!NOTE]
> <span data-ttu-id="945a0-164">此处所述的具体限制可能会发生更改。</span><span class="sxs-lookup"><span data-stu-id="945a0-164">The specific limits described here are subject to change.</span></span>

> <span data-ttu-id="945a0-165">**备注** 在本节中，*租户*此术语是指指安装应用程序的 Microsoft 365 组织。</span><span class="sxs-lookup"><span data-stu-id="945a0-165">**Note:** In this section, the term *tenant* refers to the Microsoft 365 organization where the application is installed.</span></span> <span data-ttu-id="945a0-166">对于单个租户应用程序，这个租户可以与创建应用程序的租户相同，对于[多租户应用程序](/azure/active-directory/develop/setup-multi-tenant-app)，这个租户可以不同。</span><span class="sxs-lookup"><span data-stu-id="945a0-166">This tenant can be the same as the the one where the application was created, in the case of a single tenant application, or it can be different, in the case of a [multi-tenant application](/azure/active-directory/develop/setup-multi-tenant-app).</span></span>

### <a name="outlook-service-limits"></a><span data-ttu-id="945a0-167">Outlook 服务限制</span><span class="sxs-lookup"><span data-stu-id="945a0-167">Outlook service limits</span></span>

<span data-ttu-id="945a0-168">将评估每个应用 ID 和邮箱组合的 Outlook 服务限制。</span><span class="sxs-lookup"><span data-stu-id="945a0-168">Outlook service limits are evaluated for each app ID and mailbox combination.</span></span> <span data-ttu-id="945a0-169">换言之，上述限制适用于访问特定邮箱（用户或组）的特定应用。</span><span class="sxs-lookup"><span data-stu-id="945a0-169">In other words, the limits described apply to a specific app accessing a specific mailbox (user or group).</span></span> <span data-ttu-id="945a0-170">如果一个邮箱的应用程序超过限制，不会影响访问另一个邮箱的功能。</span><span class="sxs-lookup"><span data-stu-id="945a0-170">If an application exceeds the limit in one mailbox, it does not affect the ability to access another mailbox.</span></span> <span data-ttu-id="945a0-171">下面的限制适用于公共云以及[区域云部署](/graph/deployments)。</span><span class="sxs-lookup"><span data-stu-id="945a0-171">The following limits apply to the public cloud as well as [national cloud deployments](/graph/deployments).</span></span>

| <span data-ttu-id="945a0-172">限制</span><span class="sxs-lookup"><span data-stu-id="945a0-172">Limit</span></span>                                                      | <span data-ttu-id="945a0-173">适用对象</span><span class="sxs-lookup"><span data-stu-id="945a0-173">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="945a0-174">10 分钟内的 10,000 个 API 请求</span><span class="sxs-lookup"><span data-stu-id="945a0-174">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="945a0-175">v1.0 和 beta 终结点</span><span class="sxs-lookup"><span data-stu-id="945a0-175">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="945a0-176">4 个并发请求</span><span class="sxs-lookup"><span data-stu-id="945a0-176">4 concurrent requests</span></span>                                      | <span data-ttu-id="945a0-177">v1.0 和 beta 终结点</span><span class="sxs-lookup"><span data-stu-id="945a0-177">v1.0 and beta endpoints</span></span>   |
| <span data-ttu-id="945a0-178">30 秒内的 15 兆字节 (MB) 上传（PATCH、POST、PUT）</span><span class="sxs-lookup"><span data-stu-id="945a0-178">15 megabytes (MB) upload (PATCH, POST, PUT) in a 30 second period</span></span> | <span data-ttu-id="945a0-179">v1.0 和 beta 终结点</span><span class="sxs-lookup"><span data-stu-id="945a0-179">v1.0 and beta endpoints</span></span>   |

#### <a name="outlook-service-resources"></a><span data-ttu-id="945a0-180">Outlook 服务资源</span><span class="sxs-lookup"><span data-stu-id="945a0-180">Outlook service resources</span></span>

<span data-ttu-id="945a0-181">Outlook 服务提供以下资源。</span><span class="sxs-lookup"><span data-stu-id="945a0-181">The following resources are provided by the Outlook service.</span></span>

##### <a name="search-api-resources-preview"></a><span data-ttu-id="945a0-182">搜索 API 资源（预览版）</span><span class="sxs-lookup"><span data-stu-id="945a0-182">Search API resources (preview)</span></span>

- [<span data-ttu-id="945a0-183">外部项（Microsoft 搜索）</span><span class="sxs-lookup"><span data-stu-id="945a0-183">External item (Microsoft Search)</span></span>](/graph/api/resources/externalitem?view=graph-rest-beta)

##### <a name="profile-api-resources"></a><span data-ttu-id="945a0-184">配置文件 API 资源</span><span class="sxs-lookup"><span data-stu-id="945a0-184">Profile API resources</span></span>

- [<span data-ttu-id="945a0-185">照片</span><span class="sxs-lookup"><span data-stu-id="945a0-185">Photo</span></span>](/graph/api/resources/profilephoto?view=graph-rest-1.0)

##### <a name="calendar-api-resources"></a><span data-ttu-id="945a0-186">日历 API 资源</span><span class="sxs-lookup"><span data-stu-id="945a0-186">Calendar API resources</span></span>

- [<span data-ttu-id="945a0-187">event</span><span class="sxs-lookup"><span data-stu-id="945a0-187">event</span></span>](/graph/api/resources/event)
- [<span data-ttu-id="945a0-188">eventMessage</span><span class="sxs-lookup"><span data-stu-id="945a0-188">eventMessage</span></span>](/graph/api/resources/eventmessage)
- [<span data-ttu-id="945a0-189">calendar</span><span class="sxs-lookup"><span data-stu-id="945a0-189">calendar</span></span>](/graph/api/resources/calendar)
- [<span data-ttu-id="945a0-190">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="945a0-190">calendarGroup</span></span>](/graph/api/resources/calendargroup)
- [<span data-ttu-id="945a0-191">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="945a0-191">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="945a0-192">attachment</span><span class="sxs-lookup"><span data-stu-id="945a0-192">attachment</span></span>](/graph/api/resources/attachment)
- [<span data-ttu-id="945a0-193">place（预览）</span><span class="sxs-lookup"><span data-stu-id="945a0-193">place (preview)</span></span>](/graph/api/resources/place)

##### <a name="mail-api-resources"></a><span data-ttu-id="945a0-194">邮件 API 资源</span><span class="sxs-lookup"><span data-stu-id="945a0-194">Mail API resources</span></span>

- [<span data-ttu-id="945a0-195">message</span><span class="sxs-lookup"><span data-stu-id="945a0-195">message</span></span>](/graph/api/resources/message)
- [<span data-ttu-id="945a0-196">mailFolder</span><span class="sxs-lookup"><span data-stu-id="945a0-196">mailFolder</span></span>](/graph/api/resources/mailfolder)
- [<span data-ttu-id="945a0-197">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="945a0-197">mailSearchFolder</span></span>](/graph/api/resources/mailsearchfolder)
- [<span data-ttu-id="945a0-198">messageRule</span><span class="sxs-lookup"><span data-stu-id="945a0-198">messageRule</span></span>](/graph/api/resources/messagerule)
- [<span data-ttu-id="945a0-199">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="945a0-199">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="945a0-200">attachment</span><span class="sxs-lookup"><span data-stu-id="945a0-200">attachment</span></span>](/graph/api/resources/attachment)

##### <a name="personal-contacts-api-resources"></a><span data-ttu-id="945a0-201">个人联系人 API 资源</span><span class="sxs-lookup"><span data-stu-id="945a0-201">Personal contacts API resources</span></span>

- [<span data-ttu-id="945a0-202">contact</span><span class="sxs-lookup"><span data-stu-id="945a0-202">contact</span></span>](/graph/api/resources/contact)
- [<span data-ttu-id="945a0-203">contactFolder</span><span class="sxs-lookup"><span data-stu-id="945a0-203">contactFolder</span></span>](/graph/api/resources/contactfolder)
- [<span data-ttu-id="945a0-204">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="945a0-204">outlookCategory</span></span>](/graph/api/resources/outlookcategory)

##### <a name="social-and-workplace-intelligence-resources"></a><span data-ttu-id="945a0-205">社交和工作区智能资源</span><span class="sxs-lookup"><span data-stu-id="945a0-205">Social and workplace intelligence resources</span></span>

- [<span data-ttu-id="945a0-206">person</span><span class="sxs-lookup"><span data-stu-id="945a0-206">person</span></span>](/graph/api/resources/person)

##### <a name="to-do-tasks-api-preview-resources"></a><span data-ttu-id="945a0-207">待办任务 API（预览）资源</span><span class="sxs-lookup"><span data-stu-id="945a0-207">To-do tasks API (preview) resources</span></span>

- [<span data-ttu-id="945a0-208">outlookTask</span><span class="sxs-lookup"><span data-stu-id="945a0-208">outlookTask</span></span>](/graph/api/resources/outlooktask)
- [<span data-ttu-id="945a0-209">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="945a0-209">outlookTaskFolder</span></span>](/graph/api/resources/outlooktaskfolder)
- [<span data-ttu-id="945a0-210">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="945a0-210">outlookTaskGroup</span></span>](/graph/api/resources/outlooktaskgroup)
- [<span data-ttu-id="945a0-211">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="945a0-211">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="945a0-212">attachment</span><span class="sxs-lookup"><span data-stu-id="945a0-212">attachment</span></span>](/graph/api/resources/attachment)

### <a name="cloud-communication-service-limits"></a><span data-ttu-id="945a0-213">云通信服务限制</span><span class="sxs-lookup"><span data-stu-id="945a0-213">Cloud communication service limits</span></span>

| <span data-ttu-id="945a0-214">资源</span><span class="sxs-lookup"><span data-stu-id="945a0-214">Resource</span></span>      | <span data-ttu-id="945a0-215">每个租户每个应用限制</span><span class="sxs-lookup"><span data-stu-id="945a0-215">Limits per app per tenant</span></span>    |
| -------------- | ------------ |
| [<span data-ttu-id="945a0-216">通话</span><span class="sxs-lookup"><span data-stu-id="945a0-216">Calls</span></span>](/graph/api/resources/call) | <span data-ttu-id="945a0-217">每月10,000 通通话和 100 通并发通话</span><span class="sxs-lookup"><span data-stu-id="945a0-217">10,000 calls/month and 100 concurrent calls</span></span>   |
| [<span data-ttu-id="945a0-218">会议信息</span><span class="sxs-lookup"><span data-stu-id="945a0-218">Meeting information</span></span>](/graph/api/resources/meetinginfo)   | <span data-ttu-id="945a0-219">每月每位用家会有 2000 则会议</span><span class="sxs-lookup"><span data-stu-id="945a0-219">2000 meetings/user each month</span></span> |
| <span data-ttu-id="945a0-220">[状态](/graph/api/resources/presence)（预览版）</span><span class="sxs-lookup"><span data-stu-id="945a0-220">[Presence](/graph/api/resources/presence) (preview)</span></span>   | <span data-ttu-id="945a0-221">2 rps</span><span class="sxs-lookup"><span data-stu-id="945a0-221">2 rps</span></span> |

### <a name="onenote-service-limits"></a><span data-ttu-id="945a0-222">OneNote 服务限制</span><span class="sxs-lookup"><span data-stu-id="945a0-222">OneNote service limits</span></span>

| <span data-ttu-id="945a0-223">限制类型</span><span class="sxs-lookup"><span data-stu-id="945a0-223">Limit type</span></span> | <span data-ttu-id="945a0-224">每个用户的每个应用程序的限制（委派的上下文）</span><span class="sxs-lookup"><span data-stu-id="945a0-224">Limit per app per user (delegated context)</span></span> | <span data-ttu-id="945a0-225">每个应用程序的限制（仅应用程序上下文）</span><span class="sxs-lookup"><span data-stu-id="945a0-225">Limit per app (app-only context)</span></span> |
| ------------ | ------- | ------- |
| <span data-ttu-id="945a0-226">请求率</span><span class="sxs-lookup"><span data-stu-id="945a0-226">Requests rate</span></span> | <span data-ttu-id="945a0-227">每 1 分钟 120 个请求和每 1 小时 400 个请求</span><span class="sxs-lookup"><span data-stu-id="945a0-227">120 requests per 1 minute and 400 per 1 hour</span></span> | <span data-ttu-id="945a0-228">每 1 分钟 240 个请求和每 1 小时 800 个请求</span><span class="sxs-lookup"><span data-stu-id="945a0-228">240 requests per 1 minute and 800 per 1 hour</span></span> |
| <span data-ttu-id="945a0-229">并发请求</span><span class="sxs-lookup"><span data-stu-id="945a0-229">Concurrent requests</span></span> | <span data-ttu-id="945a0-230">5 个并发请求</span><span class="sxs-lookup"><span data-stu-id="945a0-230">5 concurrent requests</span></span> | <span data-ttu-id="945a0-231">20 个并发请求</span><span class="sxs-lookup"><span data-stu-id="945a0-231">20 concurrent requests</span></span> |

<span data-ttu-id="945a0-232">上述限制适用于下列资源:</span><span class="sxs-lookup"><span data-stu-id="945a0-232">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="945a0-233">onenote, notebook, sectionGroup, onenoteSection, onenotePage, onenoteResource, onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="945a0-233">onenote, notebook, sectionGroup, onenoteSection, onenotePage, onenoteResource, onenoteOperation</span></span>

<span data-ttu-id="945a0-234">可在 [OneNote API 限制及避免方法](https://developer.microsoft.com/zh-CN/office/blogs/onenote-api-throttling-and-how-to-avoid-it/) 中找到有关最佳做法的附加信息。</span><span class="sxs-lookup"><span data-stu-id="945a0-234">You can find additional information about best practices in [OneNote API throttling and how to avoid it](https://developer.microsoft.com/zh-CN/office/blogs/onenote-api-throttling-and-how-to-avoid-it/).</span></span>  

> <span data-ttu-id="945a0-235">**注意：** 上面列出的资源未在 `429 Too Many Requests` 响应上返回 `Retry-After` 标头。</span><span class="sxs-lookup"><span data-stu-id="945a0-235">**Note:** The resources listed above do not return a `Retry-After` header on `429 Too Many Requests` responses.</span></span>

### <a name="project-rome-service-limits"></a><span data-ttu-id="945a0-236">Project Rome 服务限制</span><span class="sxs-lookup"><span data-stu-id="945a0-236">Project Rome service limits</span></span>

| <span data-ttu-id="945a0-237">请求类型</span><span class="sxs-lookup"><span data-stu-id="945a0-237">Request type</span></span> | <span data-ttu-id="945a0-238">所有应用的每个用户的限制</span><span class="sxs-lookup"><span data-stu-id="945a0-238">Limit per user for all apps</span></span> |
| ------------ | --------------------------- |
| <span data-ttu-id="945a0-239">GET</span><span class="sxs-lookup"><span data-stu-id="945a0-239">GET</span></span>          | <span data-ttu-id="945a0-240">每 5 分钟 400 个请求和每天 12000 个请求</span><span class="sxs-lookup"><span data-stu-id="945a0-240">400 requests per 5 minutes and 12000 requests per 1 day</span></span> |
| <span data-ttu-id="945a0-241">POST, PUT, PATCH, DELETE</span><span class="sxs-lookup"><span data-stu-id="945a0-241">POST, PUT, PATCH, DELETE</span></span> | <span data-ttu-id="945a0-242">每 5 分钟 100 个请求和每天 8000 个请求</span><span class="sxs-lookup"><span data-stu-id="945a0-242">100 requests per 5 minutes and 8000 requests per 1 day</span></span> |

<span data-ttu-id="945a0-243">上述限制适用于下列资源:</span><span class="sxs-lookup"><span data-stu-id="945a0-243">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="945a0-244">activityHistoryItem、userActivity</span><span class="sxs-lookup"><span data-stu-id="945a0-244">activityHistoryItem, userActivity</span></span>

### <a name="microsoft-teams-service-limits"></a><span data-ttu-id="945a0-245">Microsoft Teams 服务限制</span><span class="sxs-lookup"><span data-stu-id="945a0-245">Microsoft Teams service limits</span></span>

<span data-ttu-id="945a0-246">限制表示为每秒请求数 (rps)。</span><span class="sxs-lookup"><span data-stu-id="945a0-246">Limits are expressed as requests per second (rps).</span></span>

| <span data-ttu-id="945a0-247">Teams 请求类型</span><span class="sxs-lookup"><span data-stu-id="945a0-247">Teams request type</span></span>                                   | <span data-ttu-id="945a0-248">每个租户每个应用限制</span><span class="sxs-lookup"><span data-stu-id="945a0-248">Limit per app per tenant</span></span>        | <span data-ttu-id="945a0-249">所有租户中的每个应用限制</span><span class="sxs-lookup"><span data-stu-id="945a0-249">Limit per app across all tenants</span></span>      |
|------------------------------------------------------|---------------------------------|------------|
| <span data-ttu-id="945a0-250">Microsoft Teams 的任何图形 API 调用</span><span class="sxs-lookup"><span data-stu-id="945a0-250">Any Graph API calls for Microsoft Teams</span></span>              | <span data-ttu-id="945a0-251">每 10 秒 15000 个请求</span><span class="sxs-lookup"><span data-stu-id="945a0-251">15000 requests every 10 seconds</span></span> | <span data-ttu-id="945a0-252">不适用</span><span class="sxs-lookup"><span data-stu-id="945a0-252">n/a</span></span> |
| <span data-ttu-id="945a0-253">GET team, channel, tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="945a0-253">GET team, channel, tab, installedApps, appCatalogs</span></span>   | <span data-ttu-id="945a0-254">60 rps</span><span class="sxs-lookup"><span data-stu-id="945a0-254">60 rps</span></span>                          | <span data-ttu-id="945a0-255">600 rps</span><span class="sxs-lookup"><span data-stu-id="945a0-255">600 rps</span></span> |
| <span data-ttu-id="945a0-256">POST/PUT channel, tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="945a0-256">POST/PUT channel, tab, installedApps, appCatalogs</span></span>    |  <span data-ttu-id="945a0-257">30 rps</span><span class="sxs-lookup"><span data-stu-id="945a0-257">30 rps</span></span>                         | <span data-ttu-id="945a0-258">300 rps</span><span class="sxs-lookup"><span data-stu-id="945a0-258">300 rps</span></span>  |
| <span data-ttu-id="945a0-259">PATCH team, channel, tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="945a0-259">PATCH team, channel, tab, installedApps, appCatalogs</span></span> |  <span data-ttu-id="945a0-260">30 rps</span><span class="sxs-lookup"><span data-stu-id="945a0-260">30 rps</span></span>                         | <span data-ttu-id="945a0-261">300 rps</span><span class="sxs-lookup"><span data-stu-id="945a0-261">300 rps</span></span>  |
| <span data-ttu-id="945a0-262">DELETE channel, tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="945a0-262">DELETE channel, tab, installedApps, appCatalogs</span></span>      |  <span data-ttu-id="945a0-263">15 rps</span><span class="sxs-lookup"><span data-stu-id="945a0-263">15 rps</span></span>                         | <span data-ttu-id="945a0-264">150 rps</span><span class="sxs-lookup"><span data-stu-id="945a0-264">150 rps</span></span>  |
| <span data-ttu-id="945a0-265">GET /teams/```{team-id}```, joinedTeams</span><span class="sxs-lookup"><span data-stu-id="945a0-265">GET /teams/```{team-id}```, joinedTeams</span></span>              |  <span data-ttu-id="945a0-266">30 rps</span><span class="sxs-lookup"><span data-stu-id="945a0-266">30 rps</span></span>                         | <span data-ttu-id="945a0-267">300 rps</span><span class="sxs-lookup"><span data-stu-id="945a0-267">300 rps</span></span>  |
| <span data-ttu-id="945a0-268">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, clone</span><span class="sxs-lookup"><span data-stu-id="945a0-268">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, clone</span></span> | <span data-ttu-id="945a0-269">6 rps</span><span class="sxs-lookup"><span data-stu-id="945a0-269">6 rps</span></span> | <span data-ttu-id="945a0-270">150 rps</span><span class="sxs-lookup"><span data-stu-id="945a0-270">150 rps</span></span>  |
| <span data-ttu-id="945a0-271">GET channel message</span><span class="sxs-lookup"><span data-stu-id="945a0-271">GET channel message</span></span>  | <span data-ttu-id="945a0-272">5 rps</span><span class="sxs-lookup"><span data-stu-id="945a0-272">5 rps</span></span> | <span data-ttu-id="945a0-273">100 rps</span><span class="sxs-lookup"><span data-stu-id="945a0-273">100 rps</span></span> |
| <span data-ttu-id="945a0-274">GET 1:1/group chat message</span><span class="sxs-lookup"><span data-stu-id="945a0-274">GET 1:1/group chat message</span></span>  | <span data-ttu-id="945a0-275">3 rps</span><span class="sxs-lookup"><span data-stu-id="945a0-275">3 rps</span></span> | <span data-ttu-id="945a0-276">30 rps</span><span class="sxs-lookup"><span data-stu-id="945a0-276">30 rps</span></span> |
| <span data-ttu-id="945a0-277">POST channel message</span><span class="sxs-lookup"><span data-stu-id="945a0-277">POST channel message</span></span> | <span data-ttu-id="945a0-278">2 rps</span><span class="sxs-lookup"><span data-stu-id="945a0-278">2 rps</span></span> | <span data-ttu-id="945a0-279">20 rps</span><span class="sxs-lookup"><span data-stu-id="945a0-279">20 rps</span></span> |
| <span data-ttu-id="945a0-280">POST 1:1/group chat message</span><span class="sxs-lookup"><span data-stu-id="945a0-280">POST 1:1/group chat message</span></span> | <span data-ttu-id="945a0-281">2 rps</span><span class="sxs-lookup"><span data-stu-id="945a0-281">2 rps</span></span> | <span data-ttu-id="945a0-282">20 rps</span><span class="sxs-lookup"><span data-stu-id="945a0-282">20 rps</span></span> |
| <span data-ttu-id="945a0-283">GET/teams/```{team-id}```/在以下路径下的日程安排和所有 API</span><span class="sxs-lookup"><span data-stu-id="945a0-283">GET /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="945a0-284">60 rps</span><span class="sxs-lookup"><span data-stu-id="945a0-284">60 rps</span></span> | <span data-ttu-id="945a0-285">600 rps</span><span class="sxs-lookup"><span data-stu-id="945a0-285">600 rps</span></span> |
| <span data-ttu-id="945a0-286">POST, PATCH, PUT /teams/```{team-id}```/在以下路径下的日程安排和所有 API</span><span class="sxs-lookup"><span data-stu-id="945a0-286">POST, PATCH, PUT /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="945a0-287">30 rps</span><span class="sxs-lookup"><span data-stu-id="945a0-287">30 rps</span></span> | <span data-ttu-id="945a0-288">300 rps</span><span class="sxs-lookup"><span data-stu-id="945a0-288">300 rps</span></span> |
| <span data-ttu-id="945a0-289">DELETE /teams/```{team-id}```/在以下路径下的日程安排和所有 API</span><span class="sxs-lookup"><span data-stu-id="945a0-289">DELETE /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="945a0-290">15 rps</span><span class="sxs-lookup"><span data-stu-id="945a0-290">15 rps</span></span> | <span data-ttu-id="945a0-291">150 rps</span><span class="sxs-lookup"><span data-stu-id="945a0-291">150 rps</span></span> |

<span data-ttu-id="945a0-292">对于给定团队或频道，每个应用最多可发布 4 个请求。</span><span class="sxs-lookup"><span data-stu-id="945a0-292">A maximum of 4 requests per second per app can be issued on a given team or channel.</span></span>
<span data-ttu-id="945a0-293">每个应用每天最多可以将 3000 条消息发送到给定的频道。</span><span class="sxs-lookup"><span data-stu-id="945a0-293">A maximum of 3000 messages per app per day can be sent to a given channel.</span></span>

<span data-ttu-id="945a0-294">另请参阅 [Microsoft Teams 限制](/graph/api/resources/teams-api-overview#microsoft-teams-limits)和[投票要求](/graph/api/resources/teams-api-overview#polling-requirements)。</span><span class="sxs-lookup"><span data-stu-id="945a0-294">See also [Microsoft Teams limits](/graph/api/resources/teams-api-overview#microsoft-teams-limits) and [polling requirements](/graph/api/resources/teams-api-overview#polling-requirements).</span></span>

<span data-ttu-id="945a0-295">上述限制适用于下列资源:</span><span class="sxs-lookup"><span data-stu-id="945a0-295">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="945a0-296">aadUserConversationMember、appCatalogs、changeTrackedEntity、channel、chatMessage、chatMessageHostedContent、conversationMember、offerShiftRequest、openShift、openShiftChangeRequest、schedule、scheduleChangeRequest、schedulingGroup、shift、shiftPreferences、swapShiftsChangeRequest、team、teamsApp、teamsAppDefinition、teamsAppInstallation、teamsAsyncOperation、teamsTab、teamsTemplate、teamwork、timeOff、timeOffReason、timeOffRequest、userSettings、workforceIntegration。</span><span class="sxs-lookup"><span data-stu-id="945a0-296">aadUserConversationMember, appCatalogs, changeTrackedEntity, channel, chatMessage, chatMessageHostedContent, conversationMember, offerShiftRequest, openShift, openShiftChangeRequest, schedule, scheduleChangeRequest, schedulingGroup, shift, shiftPreferences, swapShiftsChangeRequest, team, teamsApp, teamsAppDefinition, teamsAppInstallation, teamsAsyncOperation, teamsTab, teamsTemplate, teamwork, timeOff, timeOffReason, timeOffRequest, userSettings, workforceIntegration.</span></span>

### <a name="identity-and-access-service-limits"></a><span data-ttu-id="945a0-297">身份和访问服务限制</span><span class="sxs-lookup"><span data-stu-id="945a0-297">Identity and access service limits</span></span>

<span data-ttu-id="945a0-298">这些服务限制适用于以下实体：</span><span class="sxs-lookup"><span data-stu-id="945a0-298">These service limits apply to the following entities:</span></span>

- [<span data-ttu-id="945a0-299">目录对象</span><span class="sxs-lookup"><span data-stu-id="945a0-299">Directory object</span></span>](/graph/api/resources/directoryobject)
- [<span data-ttu-id="945a0-300">扩展属性</span><span class="sxs-lookup"><span data-stu-id="945a0-300">Extension property</span></span>](/graph/api/resources/extensionproperty)
- [<span data-ttu-id="945a0-301">管理单元</span><span class="sxs-lookup"><span data-stu-id="945a0-301">Administrative unit</span></span>](/graph/api/resources/administrativeunit)
- [<span data-ttu-id="945a0-302">应用程序</span><span class="sxs-lookup"><span data-stu-id="945a0-302">Application</span></span>](/graph/api/resources/application)
- [<span data-ttu-id="945a0-303">应用角色分配</span><span class="sxs-lookup"><span data-stu-id="945a0-303">Application role assignment</span></span>](/graph/api/resources/approleassignment)
- [<span data-ttu-id="945a0-304">基于证书的身份配置</span><span class="sxs-lookup"><span data-stu-id="945a0-304">Certificate based auth configuration</span></span>](/graph/api/resources/certificatebasedauthconfiguration)
- [<span data-ttu-id="945a0-305">组织联系人</span><span class="sxs-lookup"><span data-stu-id="945a0-305">Organizational contact</span></span>](/graph/api/resources/orgcontact)
- [<span data-ttu-id="945a0-306">Device</span><span class="sxs-lookup"><span data-stu-id="945a0-306">Device</span></span>](/graph/api/resources/device)
- [<span data-ttu-id="945a0-307">目录对象合作伙伴参考</span><span class="sxs-lookup"><span data-stu-id="945a0-307">Directory object partner reference</span></span>](/graph/api/resources/directoryobjectpartnerreference)
- [<span data-ttu-id="945a0-308">目录角色</span><span class="sxs-lookup"><span data-stu-id="945a0-308">Directory role</span></span>](/graph/api/resources/directoryrole)
- [<span data-ttu-id="945a0-309">目录角色模板</span><span class="sxs-lookup"><span data-stu-id="945a0-309">Directory role template</span></span>](/graph/api/resources/directoryroletemplate)
- [<span data-ttu-id="945a0-310">域</span><span class="sxs-lookup"><span data-stu-id="945a0-310">Domain</span></span>](/graph/api/resources/domain)
- [<span data-ttu-id="945a0-311">域 dns 记录</span><span class="sxs-lookup"><span data-stu-id="945a0-311">Domain dns record</span></span>](/graph/api/resources/domaindnsrecord)
- [<span data-ttu-id="945a0-312">域 dns cname 记录</span><span class="sxs-lookup"><span data-stu-id="945a0-312">Domain dns cname record</span></span>](/graph/api/resources/domaindnscnamerecord)
- [<span data-ttu-id="945a0-313">域 dns mx 记录</span><span class="sxs-lookup"><span data-stu-id="945a0-313">Domain dns mx record</span></span>](/graph/api/resources/domaindnsmxrecord)
- [<span data-ttu-id="945a0-314">域 dns srv 记录</span><span class="sxs-lookup"><span data-stu-id="945a0-314">Domain dns srv record</span></span>](/graph/api/resources/domaindnssrvrecord)
- [<span data-ttu-id="945a0-315">域 dns txt 记录</span><span class="sxs-lookup"><span data-stu-id="945a0-315">Domain dns txt record</span></span>](/graph/api/resources/domaindnstxtrecord)
- [<span data-ttu-id="945a0-316">域 dns 不可用记录</span><span class="sxs-lookup"><span data-stu-id="945a0-316">Domain dns unavailable record</span></span>](/graph/api/resources/domaindnsunavailablerecord)
- [<span data-ttu-id="945a0-317">终结点</span><span class="sxs-lookup"><span data-stu-id="945a0-317">Endpoint</span></span>](/graph/api/resources/endpoint)
- [<span data-ttu-id="945a0-318">扩展属性</span><span class="sxs-lookup"><span data-stu-id="945a0-318">Extension property</span></span>](/graph/api/resources/extensionproperty)
- [<span data-ttu-id="945a0-319">许可证详细信息</span><span class="sxs-lookup"><span data-stu-id="945a0-319">License details</span></span>](/graph/api/resources/licensedetails)
- [<span data-ttu-id="945a0-320">组</span><span class="sxs-lookup"><span data-stu-id="945a0-320">Group</span></span>](/graph/api/resources/group)
- [<span data-ttu-id="945a0-321">基于活动的超时策略</span><span class="sxs-lookup"><span data-stu-id="945a0-321">Activity based timeout policy</span></span>](/graph/api/resources/activitybasedtimeoutpolicy)
- [<span data-ttu-id="945a0-322">声明映射策略</span><span class="sxs-lookup"><span data-stu-id="945a0-322">Claims mapping policy</span></span>](/graph/api/resources/claimsmappingpolicy)
- [<span data-ttu-id="945a0-323">主领域发现策略</span><span class="sxs-lookup"><span data-stu-id="945a0-323">Home realm discovery policy</span></span>](/graph/api/resources/homerealmdiscoverypolicy)
- [<span data-ttu-id="945a0-324">令牌颁发策略</span><span class="sxs-lookup"><span data-stu-id="945a0-324">Token issuance policy</span></span>](/graph/api/resources/tokenissuancepolicy)
- [<span data-ttu-id="945a0-325">令牌生存期策略</span><span class="sxs-lookup"><span data-stu-id="945a0-325">Token lifetime policy</span></span>](/graph/api/resources/tokenlifetimepolicy)
- [<span data-ttu-id="945a0-326">策略基础</span><span class="sxs-lookup"><span data-stu-id="945a0-326">Policy base</span></span>](/graph/api/resources/policybase)
- [<span data-ttu-id="945a0-327">Sts 策略</span><span class="sxs-lookup"><span data-stu-id="945a0-327">Sts policy</span></span>](/graph/api/resources/stspolicy)
- [<span data-ttu-id="945a0-328">合同</span><span class="sxs-lookup"><span data-stu-id="945a0-328">Contract</span></span>](/graph/api/resources/contract)
- [<span data-ttu-id="945a0-329">服务主体</span><span class="sxs-lookup"><span data-stu-id="945a0-329">Service principal</span></span>](/graph/api/resources/serviceprincipal)
- [<span data-ttu-id="945a0-330">订阅的 SKU</span><span class="sxs-lookup"><span data-stu-id="945a0-330">Subscribed sku</span></span>](/graph/api/resources/subscribedsku)
- [<span data-ttu-id="945a0-331">Oauth2 权限授予</span><span class="sxs-lookup"><span data-stu-id="945a0-331">OAuth2 permission grant</span></span>](/graph/api/resources/oauth2permissiongrant)
- [<span data-ttu-id="945a0-332">组织</span><span class="sxs-lookup"><span data-stu-id="945a0-332">Organization</span></span>](/graph/api/resources/organization)
- [<span data-ttu-id="945a0-333">用户</span><span class="sxs-lookup"><span data-stu-id="945a0-333">User</span></span>](/graph/api/resources/user)
- [<span data-ttu-id="945a0-334">组设置</span><span class="sxs-lookup"><span data-stu-id="945a0-334">Group setting</span></span>](/graph/api/resources/groupsetting)
- [<span data-ttu-id="945a0-335">组设置模板</span><span class="sxs-lookup"><span data-stu-id="945a0-335">Group setting template</span></span>](/graph/api/resources/groupsettingtemplate)

#### <a name="pattern"></a><span data-ttu-id="945a0-336">模式</span><span class="sxs-lookup"><span data-stu-id="945a0-336">Pattern</span></span>

<span data-ttu-id="945a0-337">限制基于令牌存储桶算法，后者通过添加各个请求的成本来实现。</span><span class="sxs-lookup"><span data-stu-id="945a0-337">Throttling is based on a token bucket algorithm, which works by adding individual costs of requests.</span></span> <span data-ttu-id="945a0-338">然后将请求成本的总和与预定限制进行比较。</span><span class="sxs-lookup"><span data-stu-id="945a0-338">The sum of request costs is then compared against pre-determined limits.</span></span> <span data-ttu-id="945a0-339">只有超出限制的请求才会被限制。</span><span class="sxs-lookup"><span data-stu-id="945a0-339">Only the requests exceeding the limits will be throttled.</span></span> <span data-ttu-id="945a0-340">如果超出任何限制，则响应将为 `429 Too Many Requests`。</span><span class="sxs-lookup"><span data-stu-id="945a0-340">If any of the limits are exceeded, the response will be `429 Too Many Requests`.</span></span> <span data-ttu-id="945a0-341">即使在服务处于重要负载或基于特定租户的数据量的情况下，也可能会收到 `429 Too Many Requests` 的响应，而不会达到以下限制。</span><span class="sxs-lookup"><span data-stu-id="945a0-341">It is possible to receive `429 Too Many Requests` responses even when the following limits are not reached, in situations when the services are under an important load or based on data volume for a specific tenant.</span></span> <span data-ttu-id="945a0-342">下表列出了现有限制。</span><span class="sxs-lookup"><span data-stu-id="945a0-342">The following table lists existing limits.</span></span>

| <span data-ttu-id="945a0-343">限制类型</span><span class="sxs-lookup"><span data-stu-id="945a0-343">Limit type</span></span> | <span data-ttu-id="945a0-344">资源单元配额</span><span class="sxs-lookup"><span data-stu-id="945a0-344">Resource unit quota</span></span> | <span data-ttu-id="945a0-345">写入配额</span><span class="sxs-lookup"><span data-stu-id="945a0-345">Write quota</span></span> |
| ---------- | ----------- | -------------- |
| <span data-ttu-id="945a0-346">应用 + 租户对</span><span class="sxs-lookup"><span data-stu-id="945a0-346">application+tenant pair</span></span> | <span data-ttu-id="945a0-347">S：3500，M:5000，L:8000 每 10 秒钟</span><span class="sxs-lookup"><span data-stu-id="945a0-347">S: 3500, M:5000, L:8000 per 10 seconds</span></span> | <span data-ttu-id="945a0-348">每 2 分钟 30 秒 3000</span><span class="sxs-lookup"><span data-stu-id="945a0-348">3000 per 2 minutes and 30 seconds</span></span> |
| <span data-ttu-id="945a0-349">应用程序</span><span class="sxs-lookup"><span data-stu-id="945a0-349">application</span></span> | <span data-ttu-id="945a0-350">每 20 秒 150,000</span><span class="sxs-lookup"><span data-stu-id="945a0-350">150,000 per 20 seconds</span></span>  | <span data-ttu-id="945a0-351">每 5 分钟 70,000</span><span class="sxs-lookup"><span data-stu-id="945a0-351">70,000 per 5 minutes</span></span> |
| <span data-ttu-id="945a0-352">租户</span><span class="sxs-lookup"><span data-stu-id="945a0-352">tenant</span></span> | <span data-ttu-id="945a0-353">不适用</span><span class="sxs-lookup"><span data-stu-id="945a0-353">Not Applicable</span></span> | <span data-ttu-id="945a0-354">每 5 分钟 9000</span><span class="sxs-lookup"><span data-stu-id="945a0-354">9000 per 5 minutes</span></span> |

> <span data-ttu-id="945a0-355">**注意**：应用程序 + 租户对限制因租户请求中运行的用户数而异。</span><span class="sxs-lookup"><span data-stu-id="945a0-355">**Note**: The application + tenant pair limit varies based on the number of users in the tenant requests are run against.</span></span> <span data-ttu-id="945a0-356">租户规模定义如下：S - 小于 50 个用户，M - 50 至 500 个用户之间，L - 500 个以上用户。</span><span class="sxs-lookup"><span data-stu-id="945a0-356">The tenant sizes are defined as follows: S - under 50 users, M - between 50 and 500 users, and L - above 500 users.</span></span>

<span data-ttu-id="945a0-357">下表列出了基本请求费用。</span><span class="sxs-lookup"><span data-stu-id="945a0-357">The following table lists base request costs.</span></span> <span data-ttu-id="945a0-358">未列出的任何请求的基础成本为 1。</span><span class="sxs-lookup"><span data-stu-id="945a0-358">Any requests not listed have a base cost of 1.</span></span>

| <span data-ttu-id="945a0-359">操作</span><span class="sxs-lookup"><span data-stu-id="945a0-359">Operation</span></span> | <span data-ttu-id="945a0-360">请求路径</span><span class="sxs-lookup"><span data-stu-id="945a0-360">Request Path</span></span> | <span data-ttu-id="945a0-361">基本资源单位成本</span><span class="sxs-lookup"><span data-stu-id="945a0-361">Base Resource Unit Cost</span></span> | <span data-ttu-id="945a0-362">写入成本</span><span class="sxs-lookup"><span data-stu-id="945a0-362">Write Cost</span></span> |
| --------- | ------------ | ----------------- | ------------------ |
| <span data-ttu-id="945a0-363">GET</span><span class="sxs-lookup"><span data-stu-id="945a0-363">GET</span></span> | `applications` | <span data-ttu-id="945a0-364">2</span><span class="sxs-lookup"><span data-stu-id="945a0-364">2</span></span> | <span data-ttu-id="945a0-365">0</span><span class="sxs-lookup"><span data-stu-id="945a0-365">0</span></span> |
| <span data-ttu-id="945a0-366">GET</span><span class="sxs-lookup"><span data-stu-id="945a0-366">GET</span></span> | `applications/{id}/extensionProperties` | <span data-ttu-id="945a0-367">2</span><span class="sxs-lookup"><span data-stu-id="945a0-367">2</span></span> | <span data-ttu-id="945a0-368">0</span><span class="sxs-lookup"><span data-stu-id="945a0-368">0</span></span> |
| <span data-ttu-id="945a0-369">GET</span><span class="sxs-lookup"><span data-stu-id="945a0-369">GET</span></span> | `contracts` | <span data-ttu-id="945a0-370">3</span><span class="sxs-lookup"><span data-stu-id="945a0-370">3</span></span> | <span data-ttu-id="945a0-371">0</span><span class="sxs-lookup"><span data-stu-id="945a0-371">0</span></span> |
| <span data-ttu-id="945a0-372">POST</span><span class="sxs-lookup"><span data-stu-id="945a0-372">POST</span></span> | `directoryObjects/getByIds` |  <span data-ttu-id="945a0-373">3</span><span class="sxs-lookup"><span data-stu-id="945a0-373">3</span></span> | <span data-ttu-id="945a0-374">0</span><span class="sxs-lookup"><span data-stu-id="945a0-374">0</span></span> |
| <span data-ttu-id="945a0-375">GET</span><span class="sxs-lookup"><span data-stu-id="945a0-375">GET</span></span> | `domains/{id}/domainNameReferences` | <span data-ttu-id="945a0-376">4</span><span class="sxs-lookup"><span data-stu-id="945a0-376">4</span></span> | <span data-ttu-id="945a0-377">0</span><span class="sxs-lookup"><span data-stu-id="945a0-377">0</span></span> |
| <span data-ttu-id="945a0-378">POST</span><span class="sxs-lookup"><span data-stu-id="945a0-378">POST</span></span> | `getObjectsById` | <span data-ttu-id="945a0-379">3</span><span class="sxs-lookup"><span data-stu-id="945a0-379">3</span></span> | <span data-ttu-id="945a0-380">0</span><span class="sxs-lookup"><span data-stu-id="945a0-380">0</span></span> |
| <span data-ttu-id="945a0-381">GET</span><span class="sxs-lookup"><span data-stu-id="945a0-381">GET</span></span> | `groups/{id}/members` | <span data-ttu-id="945a0-382">3</span><span class="sxs-lookup"><span data-stu-id="945a0-382">3</span></span> | <span data-ttu-id="945a0-383">0</span><span class="sxs-lookup"><span data-stu-id="945a0-383">0</span></span> |
| <span data-ttu-id="945a0-384">GET</span><span class="sxs-lookup"><span data-stu-id="945a0-384">GET</span></span> | `groups/{id}/transitiveMembers` | <span data-ttu-id="945a0-385">5</span><span class="sxs-lookup"><span data-stu-id="945a0-385">5</span></span> | <span data-ttu-id="945a0-386">0</span><span class="sxs-lookup"><span data-stu-id="945a0-386">0</span></span> |
| <span data-ttu-id="945a0-387">POST</span><span class="sxs-lookup"><span data-stu-id="945a0-387">POST</span></span> | `isMemberOf` | <span data-ttu-id="945a0-388">4</span><span class="sxs-lookup"><span data-stu-id="945a0-388">4</span></span> | <span data-ttu-id="945a0-389">0</span><span class="sxs-lookup"><span data-stu-id="945a0-389">0</span></span> |
| <span data-ttu-id="945a0-390">POST</span><span class="sxs-lookup"><span data-stu-id="945a0-390">POST</span></span> | `me/checkMemberGroups` | <span data-ttu-id="945a0-391">4</span><span class="sxs-lookup"><span data-stu-id="945a0-391">4</span></span> | <span data-ttu-id="945a0-392">0</span><span class="sxs-lookup"><span data-stu-id="945a0-392">0</span></span> |
| <span data-ttu-id="945a0-393">POST</span><span class="sxs-lookup"><span data-stu-id="945a0-393">POST</span></span> | `me/checkMemberObjects` | <span data-ttu-id="945a0-394">4</span><span class="sxs-lookup"><span data-stu-id="945a0-394">4</span></span> | <span data-ttu-id="945a0-395">0</span><span class="sxs-lookup"><span data-stu-id="945a0-395">0</span></span> |
| <span data-ttu-id="945a0-396">POST</span><span class="sxs-lookup"><span data-stu-id="945a0-396">POST</span></span> | `me/getMemberGroups` | <span data-ttu-id="945a0-397">2</span><span class="sxs-lookup"><span data-stu-id="945a0-397">2</span></span> | <span data-ttu-id="945a0-398">0</span><span class="sxs-lookup"><span data-stu-id="945a0-398">0</span></span> |
| <span data-ttu-id="945a0-399">POST</span><span class="sxs-lookup"><span data-stu-id="945a0-399">POST</span></span> | `me/getMemberObjects` | <span data-ttu-id="945a0-400">2</span><span class="sxs-lookup"><span data-stu-id="945a0-400">2</span></span> | <span data-ttu-id="945a0-401">0</span><span class="sxs-lookup"><span data-stu-id="945a0-401">0</span></span> |
| <span data-ttu-id="945a0-402">GET</span><span class="sxs-lookup"><span data-stu-id="945a0-402">GET</span></span> | `me/licenseDetails` | <span data-ttu-id="945a0-403">2</span><span class="sxs-lookup"><span data-stu-id="945a0-403">2</span></span> | <span data-ttu-id="945a0-404">0</span><span class="sxs-lookup"><span data-stu-id="945a0-404">0</span></span> |
| <span data-ttu-id="945a0-405">GET</span><span class="sxs-lookup"><span data-stu-id="945a0-405">GET</span></span> | `me/memberOf` | <span data-ttu-id="945a0-406">2</span><span class="sxs-lookup"><span data-stu-id="945a0-406">2</span></span> | <span data-ttu-id="945a0-407">0</span><span class="sxs-lookup"><span data-stu-id="945a0-407">0</span></span> |
| <span data-ttu-id="945a0-408">GET</span><span class="sxs-lookup"><span data-stu-id="945a0-408">GET</span></span> | `me/ownedObjects` | <span data-ttu-id="945a0-409">2</span><span class="sxs-lookup"><span data-stu-id="945a0-409">2</span></span> | <span data-ttu-id="945a0-410">0</span><span class="sxs-lookup"><span data-stu-id="945a0-410">0</span></span> |
| <span data-ttu-id="945a0-411">GET</span><span class="sxs-lookup"><span data-stu-id="945a0-411">GET</span></span> | `me/transitiveMemberOf` | <span data-ttu-id="945a0-412">2</span><span class="sxs-lookup"><span data-stu-id="945a0-412">2</span></span> | <span data-ttu-id="945a0-413">0</span><span class="sxs-lookup"><span data-stu-id="945a0-413">0</span></span> |
| <span data-ttu-id="945a0-414">GET</span><span class="sxs-lookup"><span data-stu-id="945a0-414">GET</span></span> | `oauth2PermissionGrants` | <span data-ttu-id="945a0-415">2</span><span class="sxs-lookup"><span data-stu-id="945a0-415">2</span></span> | <span data-ttu-id="945a0-416">0</span><span class="sxs-lookup"><span data-stu-id="945a0-416">0</span></span> |
| <span data-ttu-id="945a0-417">GET</span><span class="sxs-lookup"><span data-stu-id="945a0-417">GET</span></span> | `oauth2PermissionGrants/{id}` | <span data-ttu-id="945a0-418">2</span><span class="sxs-lookup"><span data-stu-id="945a0-418">2</span></span> | <span data-ttu-id="945a0-419">0</span><span class="sxs-lookup"><span data-stu-id="945a0-419">0</span></span> |
| <span data-ttu-id="945a0-420">GET</span><span class="sxs-lookup"><span data-stu-id="945a0-420">GET</span></span> | `servicePrincipals/{id}/appRoleAssignments` | <span data-ttu-id="945a0-421">2</span><span class="sxs-lookup"><span data-stu-id="945a0-421">2</span></span> | <span data-ttu-id="945a0-422">0</span><span class="sxs-lookup"><span data-stu-id="945a0-422">0</span></span> |
| <span data-ttu-id="945a0-423">GET</span><span class="sxs-lookup"><span data-stu-id="945a0-423">GET</span></span> | `subscribedSkus` | <span data-ttu-id="945a0-424">3</span><span class="sxs-lookup"><span data-stu-id="945a0-424">3</span></span> | <span data-ttu-id="945a0-425">0</span><span class="sxs-lookup"><span data-stu-id="945a0-425">0</span></span> |
| <span data-ttu-id="945a0-426">GET</span><span class="sxs-lookup"><span data-stu-id="945a0-426">GET</span></span> | `users` | <span data-ttu-id="945a0-427">2</span><span class="sxs-lookup"><span data-stu-id="945a0-427">2</span></span> | <span data-ttu-id="945a0-428">0</span><span class="sxs-lookup"><span data-stu-id="945a0-428">0</span></span> |
| <span data-ttu-id="945a0-429">GET</span><span class="sxs-lookup"><span data-stu-id="945a0-429">GET</span></span> | <span data-ttu-id="945a0-430">表中未列出的任何身份路径</span><span class="sxs-lookup"><span data-stu-id="945a0-430">Any identity path not listed in the table</span></span> | <span data-ttu-id="945a0-431">1</span><span class="sxs-lookup"><span data-stu-id="945a0-431">1</span></span> | <span data-ttu-id="945a0-432">0</span><span class="sxs-lookup"><span data-stu-id="945a0-432">0</span></span> |
| <span data-ttu-id="945a0-433">POST</span><span class="sxs-lookup"><span data-stu-id="945a0-433">POST</span></span> | <span data-ttu-id="945a0-434">表中未列出的任何身份路径</span><span class="sxs-lookup"><span data-stu-id="945a0-434">Any identity path not listed in the table</span></span> | <span data-ttu-id="945a0-435">1</span><span class="sxs-lookup"><span data-stu-id="945a0-435">1</span></span> | <span data-ttu-id="945a0-436">1</span><span class="sxs-lookup"><span data-stu-id="945a0-436">1</span></span> |
| <span data-ttu-id="945a0-437">PATCH</span><span class="sxs-lookup"><span data-stu-id="945a0-437">PATCH</span></span> | <span data-ttu-id="945a0-438">表中未列出的任何身份路径</span><span class="sxs-lookup"><span data-stu-id="945a0-438">Any identity path not listed in the table</span></span> | <span data-ttu-id="945a0-439">1</span><span class="sxs-lookup"><span data-stu-id="945a0-439">1</span></span> | <span data-ttu-id="945a0-440">1</span><span class="sxs-lookup"><span data-stu-id="945a0-440">1</span></span> |
| <span data-ttu-id="945a0-441">PUT</span><span class="sxs-lookup"><span data-stu-id="945a0-441">PUT</span></span> | <span data-ttu-id="945a0-442">表中未列出的任何身份路径</span><span class="sxs-lookup"><span data-stu-id="945a0-442">Any identity path not listed in the table</span></span> | <span data-ttu-id="945a0-443">1</span><span class="sxs-lookup"><span data-stu-id="945a0-443">1</span></span> | <span data-ttu-id="945a0-444">1</span><span class="sxs-lookup"><span data-stu-id="945a0-444">1</span></span> |
| <span data-ttu-id="945a0-445">DELETE</span><span class="sxs-lookup"><span data-stu-id="945a0-445">DELETE</span></span> | <span data-ttu-id="945a0-446">表中未列出的任何身份路径</span><span class="sxs-lookup"><span data-stu-id="945a0-446">Any identity path not listed in the table</span></span> | <span data-ttu-id="945a0-447">1</span><span class="sxs-lookup"><span data-stu-id="945a0-447">1</span></span> | <span data-ttu-id="945a0-448">1</span><span class="sxs-lookup"><span data-stu-id="945a0-448">1</span></span> |

<span data-ttu-id="945a0-449">影响请求费用的其他因素：</span><span class="sxs-lookup"><span data-stu-id="945a0-449">Other factors that affect a request cost:</span></span>

- <span data-ttu-id="945a0-450">使用 `$select` 可将成本降低 1</span><span class="sxs-lookup"><span data-stu-id="945a0-450">Using `$select` decreases cost by 1</span></span>
- <span data-ttu-id="945a0-451">使用 `$expand` 可将成本增加 1</span><span class="sxs-lookup"><span data-stu-id="945a0-451">Using `$expand` increases cost by 1</span></span>
- <span data-ttu-id="945a0-452">使用值小于 20 的 `$top` 会使成本降低1</span><span class="sxs-lookup"><span data-stu-id="945a0-452">Using `$top` with a value of less than 20 decreases cost by 1</span></span>

> <span data-ttu-id="945a0-453">**注意：** 请求费用不能低于 1。</span><span class="sxs-lookup"><span data-stu-id="945a0-453">**Note:** A request cost can never be lower than 1.</span></span> <span data-ttu-id="945a0-454">适用于从 `me/` 开始的请求路径的任何请求费用也适用于以 `users/{id | userPrincipalName}/`开头的等效请求。</span><span class="sxs-lookup"><span data-stu-id="945a0-454">Any request cost that applies to a request path starting with `me/` also applies to equivalent requests starting with `users/{id | userPrincipalName}/`.</span></span>

#### <a name="additional-headers"></a><span data-ttu-id="945a0-455">附加标题</span><span class="sxs-lookup"><span data-stu-id="945a0-455">Additional headers</span></span>

##### <a name="request-headers"></a><span data-ttu-id="945a0-456">请求标头</span><span class="sxs-lookup"><span data-stu-id="945a0-456">Request headers</span></span>

- <span data-ttu-id="945a0-457">**x-ms-throttle-priority** - 如果标头不存在或设置为任何其他值，则表示正常请求。</span><span class="sxs-lookup"><span data-stu-id="945a0-457">**x-ms-throttle-priority** - If the header doesn't exist or is set to any other value, it indicates a normal request.</span></span> <span data-ttu-id="945a0-458">我们建议将优先级 `high` 用户启动的请求设置优先级。</span><span class="sxs-lookup"><span data-stu-id="945a0-458">We recommend setting priority to `high` only for the requests initiated by the user.</span></span> <span data-ttu-id="945a0-459">此标头的值可以是以下值：</span><span class="sxs-lookup"><span data-stu-id="945a0-459">The values of this header can be the following:</span></span>
  - <span data-ttu-id="945a0-460">低 - 指示请求的优先级较低。</span><span class="sxs-lookup"><span data-stu-id="945a0-460">Low - Indicates the request is low priority.</span></span> <span data-ttu-id="945a0-461">限制此请求不会导致出现用户可见的故障。</span><span class="sxs-lookup"><span data-stu-id="945a0-461">Throttling this request doesn't cause user-visible failures.</span></span>
  - <span data-ttu-id="945a0-462">正常 - 如果未提供任何值，则为默认值。</span><span class="sxs-lookup"><span data-stu-id="945a0-462">Normal - Default if no value is provided.</span></span> <span data-ttu-id="945a0-463">表示请求是默认优先级。</span><span class="sxs-lookup"><span data-stu-id="945a0-463">Indicates that the request is default priority.</span></span>
  - <span data-ttu-id="945a0-464">高 - 表示请求具有高优先级。</span><span class="sxs-lookup"><span data-stu-id="945a0-464">High - Indicates that the request is high priority.</span></span> <span data-ttu-id="945a0-465">限制此请求会导致出现用户可见的故障。</span><span class="sxs-lookup"><span data-stu-id="945a0-465">Throttling this request causes user-visible failures.</span></span>

> <span data-ttu-id="945a0-466">**注意**：如果限制请求，则首先限制低优先级请求，其次限制正常优先级请求，最后限制高优先级请求。</span><span class="sxs-lookup"><span data-stu-id="945a0-466">**Note:** Should requests be throttled, low priority requests will be throttled first, normal priority requests second, and high priority requests last.</span></span> <span data-ttu-id="945a0-467">使用优先级请求标头不会更改限制。</span><span class="sxs-lookup"><span data-stu-id="945a0-467">Using the priority request header does not change the limits.</span></span>

##### <a name="regular-responses-requests"></a><span data-ttu-id="945a0-468">正常响应请求</span><span class="sxs-lookup"><span data-stu-id="945a0-468">Regular responses requests</span></span>

- <span data-ttu-id="945a0-469">**x-ms-resource-unit** - 指示用于此请求的资源单位。</span><span class="sxs-lookup"><span data-stu-id="945a0-469">**x-ms-resource-unit** - Indicates the resource unit used for this request.</span></span> <span data-ttu-id="945a0-470">值为正整数。</span><span class="sxs-lookup"><span data-stu-id="945a0-470">Values are positive integers.</span></span>
- <span data-ttu-id="945a0-471">**x-ms-throttle-limit-percentage** - 仅当应用程序消耗了超过其限制的 0.8 时才返回。</span><span class="sxs-lookup"><span data-stu-id="945a0-471">**x-ms-throttle-limit-percentage** - Returned only when the application consumed more than 0.8 of its limit.</span></span> <span data-ttu-id="945a0-472">该值的范围是 0.8 到 1.8，是使用限制的百分比。</span><span class="sxs-lookup"><span data-stu-id="945a0-472">The value ranges from 0.8 to 1.8 and is a percentage of the use of the limit.</span></span> <span data-ttu-id="945a0-473">调用者可以使用该值设置警报并采取措施。</span><span class="sxs-lookup"><span data-stu-id="945a0-473">The value can be used by the callers to set up an alert and take action.</span></span>

##### <a name="throttled-responses-requests"></a><span data-ttu-id="945a0-474">受限制的响应请求</span><span class="sxs-lookup"><span data-stu-id="945a0-474">Throttled responses requests</span></span>

- <span data-ttu-id="945a0-475">**x-ms-throttle-scope** - eg.</span><span class="sxs-lookup"><span data-stu-id="945a0-475">**x-ms-throttle-scope** - eg.</span></span> <span data-ttu-id="945a0-476">`Tenant_Application/ReadWrite/9a3d526c-b3c1-4479-ba74-197b5c5751ae/0785ef7c-2d7a-4542-b048-95bcab406e0b`（）。</span><span class="sxs-lookup"><span data-stu-id="945a0-476">`Tenant_Application/ReadWrite/9a3d526c-b3c1-4479-ba74-197b5c5751ae/0785ef7c-2d7a-4542-b048-95bcab406e0b`.</span></span> <span data-ttu-id="945a0-477">指示采用下列格式 `<Scope>/<Limit>/<ApplicationId>/<TenantId|UserId|ResourceId>` 的限制范围：</span><span class="sxs-lookup"><span data-stu-id="945a0-477">Indicates the scope of throttling with the following format `<Scope>/<Limit>/<ApplicationId>/<TenantId|UserId|ResourceId>`:</span></span>
  - <span data-ttu-id="945a0-478">范围：（字符串，必填）</span><span class="sxs-lookup"><span data-stu-id="945a0-478">Scope: (string, required)</span></span>
    - <span data-ttu-id="945a0-479">Tenant_Application - 当前应用程序对特定租户的所有请求。</span><span class="sxs-lookup"><span data-stu-id="945a0-479">Tenant_Application - All requests for a particular tenant for the current application.</span></span>
    - <span data-ttu-id="945a0-480">租户 - 当前租户的所有请求，与应用程序无关。</span><span class="sxs-lookup"><span data-stu-id="945a0-480">Tenant - All requests for the current tenant, regardless of the application.</span></span>
    - <span data-ttu-id="945a0-481">应用程序 - 当前应用程序的所有请求。</span><span class="sxs-lookup"><span data-stu-id="945a0-481">Application - All requests for the current application.</span></span>
  - <span data-ttu-id="945a0-482">限制：（字符串、必填）</span><span class="sxs-lookup"><span data-stu-id="945a0-482">Limit: (string, requied)</span></span>
    - <span data-ttu-id="945a0-483">读取：读取范围请求 (GET)</span><span class="sxs-lookup"><span data-stu-id="945a0-483">Read: Read requests for the scope (GET)</span></span>
    - <span data-ttu-id="945a0-484">写入：写入范围请求 (POST、PATCH、PUT、DELETE...)</span><span class="sxs-lookup"><span data-stu-id="945a0-484">Write: Write requests for the scope (POST, PATCH, PUT, DELETE...)</span></span>
    - <span data-ttu-id="945a0-485">ReadWrite：所有范围请求（任何）</span><span class="sxs-lookup"><span data-stu-id="945a0-485">ReadWrite: All Requests for the scope (any)</span></span>
  - <span data-ttu-id="945a0-486">ApplicationId （Guid、必填）</span><span class="sxs-lookup"><span data-stu-id="945a0-486">ApplicationId (Guid, required)</span></span>
  - <span data-ttu-id="945a0-487">TenantId|UserId|ResourceId: (Guid、必填）</span><span class="sxs-lookup"><span data-stu-id="945a0-487">TenantId|UserId|ResourceId: (Guid, required)</span></span>
- <span data-ttu-id="945a0-488">**x-ms-throttle-information** - 指示限制的原因，可以有任何值（字符串）。</span><span class="sxs-lookup"><span data-stu-id="945a0-488">**x-ms-throttle-information** - Indicates the reason for throttling and can have any value (string).</span></span> <span data-ttu-id="945a0-489">提供该值是为了进行诊断和故障排除，其中一些示例包括：</span><span class="sxs-lookup"><span data-stu-id="945a0-489">The value is provided for diagnostics and troubleshooting purposes, some examples include:</span></span>
  - <span data-ttu-id="945a0-490">CPULimitExceeded - 限制因为超过 cpu 应用的限值。</span><span class="sxs-lookup"><span data-stu-id="945a0-490">CPULimitExceeded - Throttling is because the limit for cpu allocation is exceeded.</span></span>
  - <span data-ttu-id="945a0-491">WriteLimitExceeded - 限制因为超过写入限值。</span><span class="sxs-lookup"><span data-stu-id="945a0-491">WriteLimitExceeded - Throttling is because the write limit is exceeded.</span></span>
  - <span data-ttu-id="945a0-492">ResourceUnitLimitExceeded - 限制因为超过已分配资源单位的限值。</span><span class="sxs-lookup"><span data-stu-id="945a0-492">ResourceUnitLimitExceeded - Throttling is because the limit for the allocated resource unit is exceeded.</span></span>

### <a name="information-protection"></a><span data-ttu-id="945a0-493">信息保护</span><span class="sxs-lookup"><span data-stu-id="945a0-493">Information protection</span></span>

<span data-ttu-id="945a0-494">以下限制适用于 `/informationProtection` 上的所有请求。</span><span class="sxs-lookup"><span data-stu-id="945a0-494">The following limits apply to any request on `/informationProtection`.</span></span>

| <span data-ttu-id="945a0-495">操作</span><span class="sxs-lookup"><span data-stu-id="945a0-495">Operation</span></span>                 | <span data-ttu-id="945a0-496">每个租户的使用限制</span><span class="sxs-lookup"><span data-stu-id="945a0-496">Limit per tenant</span></span>                                            | <span data-ttu-id="945a0-497">每个资源（电子邮件、URL、文件）的使用限制</span><span class="sxs-lookup"><span data-stu-id="945a0-497">Limit per resource (email, URL, file)</span></span>                |
|---------------------------|-------------------------------------------------------------|------------------------------------------------------|
| <span data-ttu-id="945a0-498">POST</span><span class="sxs-lookup"><span data-stu-id="945a0-498">POST</span></span>                      | <span data-ttu-id="945a0-499">每 15 分钟 150 个请求和每 24 小时 10000 个请求</span><span class="sxs-lookup"><span data-stu-id="945a0-499">150 requests per 15 minutes and 10000 requests per 24 hours</span></span> | <span data-ttu-id="945a0-500">每 15 分钟 1 个请求和每 24 小时 3 个请求</span><span class="sxs-lookup"><span data-stu-id="945a0-500">1 request per 15 minutes and 3 requests per 24 hours</span></span> |

<span data-ttu-id="945a0-501">上述限制适用于下列资源:</span><span class="sxs-lookup"><span data-stu-id="945a0-501">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="945a0-502">threatAssessmentRequest、threatAssessmentResult、mailAssessmentRequest、emailFileAssessmentRequest、fileAssessmentRequest、urlAssessmentRequest。</span><span class="sxs-lookup"><span data-stu-id="945a0-502">threatAssessmentRequest, threatAssessmentResult, mailAssessmentRequest, emailFileAssessmentRequest, fileAssessmentRequest, urlAssessmentRequest.</span></span>

### <a name="identity-protection-and-conditional-access-service-limits"></a><span data-ttu-id="945a0-503">身份保护和条件访问服务限制</span><span class="sxs-lookup"><span data-stu-id="945a0-503">Identity protection and conditional access service limits</span></span>

| <span data-ttu-id="945a0-504">请求类型</span><span class="sxs-lookup"><span data-stu-id="945a0-504">Request type</span></span> | <span data-ttu-id="945a0-505">所有应用的每个租户的使用限制</span><span class="sxs-lookup"><span data-stu-id="945a0-505">Limit per tenant for all apps</span></span> |
| ------------ | ------- |
| <span data-ttu-id="945a0-506">任何</span><span class="sxs-lookup"><span data-stu-id="945a0-506">Any</span></span> | <span data-ttu-id="945a0-507">每秒1个请求</span><span class="sxs-lookup"><span data-stu-id="945a0-507">1 request per second</span></span> |

<span data-ttu-id="945a0-508">上述限制适用于下列资源:</span><span class="sxs-lookup"><span data-stu-id="945a0-508">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="945a0-509">riskDetection, riskyUser, riskyUserHistoryItem, namedLocation, countryNamedLocation, ipNamedLocation, conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="945a0-509">riskDetection, riskyUser, riskyUserHistoryItem, namedLocation, countryNamedLocation, ipNamedLocation, conditionalAccessPolicy.</span></span>

> <span data-ttu-id="945a0-510">**注意：** 上面列出的资源未在 `429 Too Many Requests` 响应上返回 `Retry-After` 标头。</span><span class="sxs-lookup"><span data-stu-id="945a0-510">**Note:** The resources listed above do not return a `Retry-After` header on `429 Too Many Requests` responses.</span></span>

### <a name="insights-service-limits"></a><span data-ttu-id="945a0-511">见解服务限制</span><span class="sxs-lookup"><span data-stu-id="945a0-511">Insights service limits</span></span>

<span data-ttu-id="945a0-512">以下限制适用于 `me/insights`或`users/{id}/insights` 上的所有请求。</span><span class="sxs-lookup"><span data-stu-id="945a0-512">The following limits apply to any request on `me/insights` or `users/{id}/insights`.</span></span>

| <span data-ttu-id="945a0-513">限制</span><span class="sxs-lookup"><span data-stu-id="945a0-513">Limit</span></span>                                                      | <span data-ttu-id="945a0-514">适用对象</span><span class="sxs-lookup"><span data-stu-id="945a0-514">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="945a0-515">10 分钟内的 10,000 个 API 请求</span><span class="sxs-lookup"><span data-stu-id="945a0-515">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="945a0-516">v1.0 和 beta 终结点</span><span class="sxs-lookup"><span data-stu-id="945a0-516">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="945a0-517">4 个并发请求</span><span class="sxs-lookup"><span data-stu-id="945a0-517">4 concurrent requests</span></span>                                      | <span data-ttu-id="945a0-518">v1.0 和 beta 终结点</span><span class="sxs-lookup"><span data-stu-id="945a0-518">v1.0 and beta endpoints</span></span>   |

<span data-ttu-id="945a0-519">上述限制适用于下列资源:</span><span class="sxs-lookup"><span data-stu-id="945a0-519">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="945a0-520">people、trending、usedinsight、sharedInsight。</span><span class="sxs-lookup"><span data-stu-id="945a0-520">people, trending, usedinsight, sharedInsight.</span></span>

### <a name="microsoft-graph-reports-service-limits"></a><span data-ttu-id="945a0-521">Microsoft Graph 报告的服务限制</span><span class="sxs-lookup"><span data-stu-id="945a0-521">Microsoft Graph reports service limits</span></span>

<span data-ttu-id="945a0-522">以下限制适用于 `/reports` 上的所有请求。</span><span class="sxs-lookup"><span data-stu-id="945a0-522">The following limits apply to any request on `/reports`.</span></span>

| <span data-ttu-id="945a0-523">操作</span><span class="sxs-lookup"><span data-stu-id="945a0-523">Operation</span></span>                 | <span data-ttu-id="945a0-524">每个租户每个应用限制</span><span class="sxs-lookup"><span data-stu-id="945a0-524">Limit per app per tenant</span></span>     | <span data-ttu-id="945a0-525">所有应用的每个租户的使用限制</span><span class="sxs-lookup"><span data-stu-id="945a0-525">Limit per tenant for all apps</span></span> |
|---------------------------|------------------------------|----------------------------|
| <span data-ttu-id="945a0-526">任何请求（CSV）</span><span class="sxs-lookup"><span data-stu-id="945a0-526">Any request (CSV)</span></span>         | <span data-ttu-id="945a0-527">每10分钟14个请求</span><span class="sxs-lookup"><span data-stu-id="945a0-527">14 requests per 10 minutes</span></span>   | <span data-ttu-id="945a0-528">每10分钟40个请求</span><span class="sxs-lookup"><span data-stu-id="945a0-528">40 requests per 10 minutes</span></span> |
| <span data-ttu-id="945a0-529">任何请求（JSON、beta）</span><span class="sxs-lookup"><span data-stu-id="945a0-529">Any request (JSON, beta)</span></span>  | <span data-ttu-id="945a0-530">每10分钟100个请求</span><span class="sxs-lookup"><span data-stu-id="945a0-530">100 requests per 10 minutes</span></span>  | <span data-ttu-id="945a0-531">不适用</span><span class="sxs-lookup"><span data-stu-id="945a0-531">n/a</span></span>                        |

<span data-ttu-id="945a0-532">上述限制分别适用于每个报表 API。</span><span class="sxs-lookup"><span data-stu-id="945a0-532">The preceding limits apply individually to each report API.</span></span> <span data-ttu-id="945a0-533">例如，在 10 分钟内分别有对 Microsoft Teams 用户活动报告 API 的请求及对 Outlook 用户活动报告 API 的请求，将分别被视为 14 个请求中的 1 个请求，而不是 14 个请求中的 2 个请求。</span><span class="sxs-lookup"><span data-stu-id="945a0-533">For example, a request to the Microsoft Teams user activity report API and a request to the Outlook user activity report API within 10 minutes will count as 1 request out of 14 for each API, not 2 requests out of 14 for both.</span></span>

<span data-ttu-id="945a0-534">上述限制适用于**报告**资源。</span><span class="sxs-lookup"><span data-stu-id="945a0-534">The preceding limits apply to the **report** resource.</span></span>  

### <a name="invitation-manager-service-limits"></a><span data-ttu-id="945a0-535">邀请管理器服务限制</span><span class="sxs-lookup"><span data-stu-id="945a0-535">Invitation manager service limits</span></span>

<span data-ttu-id="945a0-536">以下限制适用于 `/invitations` 上的所有请求。</span><span class="sxs-lookup"><span data-stu-id="945a0-536">The following limits apply to any request on `/invitations`.</span></span>

| <span data-ttu-id="945a0-537">操作</span><span class="sxs-lookup"><span data-stu-id="945a0-537">Operation</span></span>                 | <span data-ttu-id="945a0-538">所有应用的每个租户的使用限制</span><span class="sxs-lookup"><span data-stu-id="945a0-538">Limit per tenant for all apps</span></span> |
|---------------------------|------------------------------|
| <span data-ttu-id="945a0-539">任何操作</span><span class="sxs-lookup"><span data-stu-id="945a0-539">Any operation</span></span>             | <span data-ttu-id="945a0-540">每 5 秒 150 个请求</span><span class="sxs-lookup"><span data-stu-id="945a0-540">150 requests per 5 seconds</span></span>   |

### <a name="security-detections-and-incidents-service-limits"></a><span data-ttu-id="945a0-541">安全检测和事件服务限制</span><span class="sxs-lookup"><span data-stu-id="945a0-541">Security detections and incidents service limits</span></span>

<span data-ttu-id="945a0-542">以下限制适用于 `/security` 上的所有请求。</span><span class="sxs-lookup"><span data-stu-id="945a0-542">The following limits apply to any request on `/security`.</span></span>

| <span data-ttu-id="945a0-543">操作</span><span class="sxs-lookup"><span data-stu-id="945a0-543">Operation</span></span>                  | <span data-ttu-id="945a0-544">每个租户每个应用限制</span><span class="sxs-lookup"><span data-stu-id="945a0-544">Limit per app per tenant</span></span>     |
|----------------------------|------------------------------|
| <span data-ttu-id="945a0-545">`alert`、`securityActions`、`secureScore` 上的任何操作</span><span class="sxs-lookup"><span data-stu-id="945a0-545">Any operation on `alert`, `securityActions`,  `secureScore`</span></span> | <span data-ttu-id="945a0-546">每分钟 150 个请求</span><span class="sxs-lookup"><span data-stu-id="945a0-546">150 requests per minute</span></span>      |
| <span data-ttu-id="945a0-547">`tiIndicator` 上的任何操作</span><span class="sxs-lookup"><span data-stu-id="945a0-547">Any operation on `tiIndicator`</span></span> | <span data-ttu-id="945a0-548">每分钟 1000 个请求</span><span class="sxs-lookup"><span data-stu-id="945a0-548">1000 requests per minute</span></span> |
| <span data-ttu-id="945a0-549">`secureScore` 或 `secureScorecontrolProfile` 上的任何操作</span><span class="sxs-lookup"><span data-stu-id="945a0-549">Any operation on `secureScore` or `secureScorecontrolProfile`</span></span> | <span data-ttu-id="945a0-550">10 分钟内的 10,000 个 API 请求</span><span class="sxs-lookup"><span data-stu-id="945a0-550">10,000 API requests in a 10 minute period</span></span> |
| <span data-ttu-id="945a0-551">`secureScore` 或 `secureScorecontrolProfile` 上的任何操作</span><span class="sxs-lookup"><span data-stu-id="945a0-551">Any operation on `secureScore` or `secureScorecontrolProfile`</span></span> | <span data-ttu-id="945a0-552">4 个并发请求</span><span class="sxs-lookup"><span data-stu-id="945a0-552">4 concurrent requests</span></span> |

### <a name="open-and-schema-extensions-service-limits"></a><span data-ttu-id="945a0-553">开放和架构扩展服务限制</span><span class="sxs-lookup"><span data-stu-id="945a0-553">Open and schema extensions service limits</span></span>

| <span data-ttu-id="945a0-554">请求类型</span><span class="sxs-lookup"><span data-stu-id="945a0-554">Request type</span></span> | <span data-ttu-id="945a0-555">每个租户每个应用限制</span><span class="sxs-lookup"><span data-stu-id="945a0-555">Limit per app per tenant</span></span> |
| ------------ | ------------------------ |
| <span data-ttu-id="945a0-556">任何</span><span class="sxs-lookup"><span data-stu-id="945a0-556">Any</span></span>          | <span data-ttu-id="945a0-557">每 10 秒 455 个请求</span><span class="sxs-lookup"><span data-stu-id="945a0-557">455 requests per 10 seconds</span></span> |

<span data-ttu-id="945a0-558">上述限制适用于以下资源：openTypeExtension、schemaExtension、administrativeUnit、合同、设备、事件、组、消息、组织、帖子和用户。</span><span class="sxs-lookup"><span data-stu-id="945a0-558">The preceding limits apply to the following resources: openTypeExtension, schemaExtension, administrativeUnit, contact, device, event, group, message, organization, post, and user.</span></span>

### <a name="files-and-lists-service-limits"></a><span data-ttu-id="945a0-559">文件和列表服务限制</span><span class="sxs-lookup"><span data-stu-id="945a0-559">Files and lists service limits</span></span>

<span data-ttu-id="945a0-560">OneDrive、OneDrive for Business 和 SharePoint Online 的服务限制不可用。</span><span class="sxs-lookup"><span data-stu-id="945a0-560">Service limits for OneDrive, OneDrive for Business, and SharePoint Online are not available.</span></span> <span data-ttu-id="945a0-561">有关详细信息，请参阅[为什么不能告诉我确切的限制？](/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online#why-cant-you-just-tell-me-the-exact-throttling-limits)。</span><span class="sxs-lookup"><span data-stu-id="945a0-561">For more information, see [why can't you just tell me the exact throttling limits?](/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online#why-cant-you-just-tell-me-the-exact-throttling-limits).</span></span>

<span data-ttu-id="945a0-562">上述信息适用于以下资源：</span><span class="sxs-lookup"><span data-stu-id="945a0-562">The preceding information applies to the following resources:</span></span>  
<span data-ttu-id="945a0-563">baseItem、baseItemVersion、columnDefinition、columnLink、contentType、drive、driveItem、driveItemVersion、fieldValueSet、itemActivity、itemActivityStat、itemAnalytics、list、listItem、listItemVersion、permission、sharedDriveItem、site 和 thumbnailSet。</span><span class="sxs-lookup"><span data-stu-id="945a0-563">baseItem, baseItemVersion, columnDefinition, columnLink, contentType, drive, driveItem, driveItemVersion, fieldValueSet, itemActivity, itemActivityStat, itemAnalytics, list, listItem, listItemVersion, permission, sharedDriveItem, site, and thumbnailSet.</span></span>

### <a name="tasks-and-plans-service-limits"></a><span data-ttu-id="945a0-564">任务和计划服务限制</span><span class="sxs-lookup"><span data-stu-id="945a0-564">Tasks and plans service limits</span></span>

<span data-ttu-id="945a0-565">Planner 的服务限制不可用。</span><span class="sxs-lookup"><span data-stu-id="945a0-565">Service limits for Planner are not available.</span></span>

<span data-ttu-id="945a0-566">上述信息适用于以下资源：</span><span class="sxs-lookup"><span data-stu-id="945a0-566">The preceding information applies to the following resources:</span></span>  
<span data-ttu-id="945a0-567">planner、plannerAssignedToTaskBoardTaskFormat、plannerBucket、plannerBucketTaskBoardTaskFormat、plannerGroup、plannerPlan、plannerPlanDetails、plannerProgressTaskBoardTaskFormat、plannerTask、plannerTaskDetails 和 plannerUser。</span><span class="sxs-lookup"><span data-stu-id="945a0-567">planner, plannerAssignedToTaskBoardTaskFormat, plannerBucket, plannerBucketTaskBoardTaskFormat, plannerGroup, plannerPlan, plannerPlanDetails, plannerProgressTaskBoardTaskFormat, plannerTask, plannerTaskDetails, and plannerUser.</span></span>

### <a name="identity-and-access-data-policy-operation-service-limits"></a><span data-ttu-id="945a0-568">身份和访问数据策略操作服务限制</span><span class="sxs-lookup"><span data-stu-id="945a0-568">Identity and access data policy operation service limits</span></span>

| <span data-ttu-id="945a0-569">请求类型</span><span class="sxs-lookup"><span data-stu-id="945a0-569">Request type</span></span> | <span data-ttu-id="945a0-570">每个租户的使用限制</span><span class="sxs-lookup"><span data-stu-id="945a0-570">Limit per tenant</span></span> |
| ------------ | ---------------- |
| <span data-ttu-id="945a0-571">发布于 `exportPersonalData`</span><span class="sxs-lookup"><span data-stu-id="945a0-571">POST on `exportPersonalData`</span></span> | <span data-ttu-id="945a0-572">每天 1000 个针对任何主题的请求，每个主题每天 100 个请求</span><span class="sxs-lookup"><span data-stu-id="945a0-572">1000 requests per day for any subject and 100 per subject per day</span></span> |
| <span data-ttu-id="945a0-573">任何其他请求</span><span class="sxs-lookup"><span data-stu-id="945a0-573">Any other request</span></span> | <span data-ttu-id="945a0-574">每分钟 10000 个请求</span><span class="sxs-lookup"><span data-stu-id="945a0-574">10000 requests per hour</span></span> |

<span data-ttu-id="945a0-575">上述限制适用于下列资源：dataPolicyOperation。</span><span class="sxs-lookup"><span data-stu-id="945a0-575">The preceding limits apply to the following resources: dataPolicyOperation.</span></span>

> <span data-ttu-id="945a0-576">**注意：** 上面列出的资源未在 `429 Too Many Requests` 响应上返回 `Retry-After` 标头。</span><span class="sxs-lookup"><span data-stu-id="945a0-576">**Note:** The resources listed above do not return a `Retry-After` header on `429 Too Many Requests` responses.</span></span>

<!-- { "blockType": "throttlinggenstart" } -->
### <a name="education-service-limits"></a><span data-ttu-id="945a0-577">教育版服务限制</span><span class="sxs-lookup"><span data-stu-id="945a0-577">Education service limits</span></span>

[!INCLUDE [Education rostering APIS throttling documentation](../includes/throttling-education-rostering-apis.md)]

### <a name="excel-service-limits"></a><span data-ttu-id="945a0-578">Excel 服务限制</span><span class="sxs-lookup"><span data-stu-id="945a0-578">Excel service limits</span></span>

[!INCLUDE [Excel throttling documentation](../includes/throttling-excel.md)]

### <a name="identity-and-access-audit-logs-service-limits"></a><span data-ttu-id="945a0-579">标识和访问审核日志的服务限制</span><span class="sxs-lookup"><span data-stu-id="945a0-579">Identity and access audit logs service limits</span></span>

[!INCLUDE [Identity and access audit logs throttling documentation](../includes/throttling-Identity-and-access-audit-logs.md)]

### <a name="identity-providers-service-limits"></a><span data-ttu-id="945a0-580">身份提供程序的服务限制</span><span class="sxs-lookup"><span data-stu-id="945a0-580">Identity providers service limits</span></span>

[!INCLUDE [CPIM throttling documentation](../includes/throttling-cpim.md)]

### <a name="intune-service-limits"></a><span data-ttu-id="945a0-581">Intune服务限制</span><span class="sxs-lookup"><span data-stu-id="945a0-581">Intune service limits</span></span>

[!INCLUDE [Intune applications throttling documentation](../includes/throttling-intune-applications.md)]
[!INCLUDE [Intune books throttling documentation](../includes/throttling-intune-books.md)]
[!INCLUDE [Intune company terms throttling documentation](../includes/throttling-intune-company-terms.md)]
[!INCLUDE [Intune device configuration throttling documentation](../includes/throttling-intune-device-configuration.md)]
[!INCLUDE [Intune device enrollment throttling documentation](../includes/throttling-intune-device-enrollment.md)]
[!INCLUDE [Intune devices throttling documentation](../includes/throttling-intune-devices.md)]
[!INCLUDE [Intune enrollment throttling documentation](../includes/throttling-intune-enrollment.md)]
[!INCLUDE [Intune managed applications throttling documentation](../includes/throttling-intune-managed-applications.md)]
[!INCLUDE [Intune notifications throttling documentation](../includes/throttling-intune-notifications.md)]
[!INCLUDE [Intune rbac throttling documentation](../includes/throttling-intune-rbac.md)]
[!INCLUDE [Intune remote assistance throttling documentation](../includes/throttling-intune-remote-assistance.md)]
[!INCLUDE [Intune reporting throttling documentation](../includes/throttling-intune-reporting.md)]
[!INCLUDE [Intune TEM throttling documentation](../includes/throttling-intune-tem.md)]
[!INCLUDE [Intune troubleshooting throttling documentation](../includes/throttling-intune-troubleshooting.md)]
[!INCLUDE [Intune wip throttling documentation](../includes/throttling-intune-wip.md)]

### <a name="skype-service-limits"></a><span data-ttu-id="945a0-582">Skype 服务限制</span><span class="sxs-lookup"><span data-stu-id="945a0-582">Skype service limits</span></span>

[!INCLUDE [Skype calling throttling documentation](../includes/throttling-skype-calling.md)]

### <a name="subscription-service-limits"></a><span data-ttu-id="945a0-583">订阅服务</span><span class="sxs-lookup"><span data-stu-id="945a0-583">Subscription service limits</span></span>

[!INCLUDE [Subscription services throttling documentation](../includes/throttling-subscription-services.md)]

<!-- { "blockType": "throttlinggenend" } -->
