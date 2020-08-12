---
title: Microsoft Graph 限制指南
description: 限制可调节并发调用服务的数量，以防止资源的过度使用。Microsoft Graph 旨在用于处理大量的请求。如果出现过多请求，限制将有助于保持 Microsoft Graph 的最佳性能和服务的可靠性。
author: davidmu1
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: a38c6c77daa5a9a6adab469681b4f7b0c4291e32
ms.sourcegitcommit: bbff139eea483faaa2d1dd08af39314f35ef48ce
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/08/2020
ms.locfileid: "46598012"
---
# <a name="microsoft-graph-throttling-guidance"></a><span data-ttu-id="c8e97-105">Microsoft Graph 限制指南</span><span class="sxs-lookup"><span data-stu-id="c8e97-105">Microsoft Graph throttling guidance</span></span>

<span data-ttu-id="c8e97-p102">限制可调节并发调用服务的数量，以防止资源的过度使用。Microsoft Graph 旨在用于处理大量的请求。如果出现过多请求，限制将有助于保持 Microsoft Graph 的最佳性能和服务的可靠性。</span><span class="sxs-lookup"><span data-stu-id="c8e97-p102">Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span></span>

<span data-ttu-id="c8e97-p103">根据该方案，执行的限制会有所不同。例如，如果你正在执行大量的写入操作，限制的可能性会比仅执行读取时要高。</span><span class="sxs-lookup"><span data-stu-id="c8e97-p103">Throttling limits vary based on the scenario. For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span></span>

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a><span data-ttu-id="c8e97-111">在限制时，会发生什么情况？</span><span class="sxs-lookup"><span data-stu-id="c8e97-111">What happens when throttling occurs?</span></span>
<!-- markdownlint-enable MD026 -->

<span data-ttu-id="c8e97-p104">超出限制阈值后，Microsoft Graph 会在一段时间内限制来自该客户端的任何进一步的请求。发生限制时，Microsoft Graph 将返回 HTTP 状态代码 429（请求过多），同时请求失败。在失败的请求的响应标头中返回建议的等待时间。限制行为取决于请求的类型和数量。例如，如果你有大量的请求，则所有请求类型受限。阈值限制根据请求类型而有所不同。因此，你可能会遇到这样一种场景，在场景中，写入被限制，但仍允许读取。</span><span class="sxs-lookup"><span data-stu-id="c8e97-p104">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time. When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail. A suggested wait time is returned in the response header of the failed request. Throttling behavior can depend on the type and number of requests. For example, if you have a high volume of requests, all requests types are throttled. Threshold limits vary based on the request type. Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span>

## <a name="common-throttling-scenarios"></a><span data-ttu-id="c8e97-119">常见的限制场景</span><span class="sxs-lookup"><span data-stu-id="c8e97-119">Common throttling scenarios</span></span>

<span data-ttu-id="c8e97-120">客户端受限的最常见原因包括：</span><span class="sxs-lookup"><span data-stu-id="c8e97-120">The most common causes of throttling of clients include:</span></span>

- <span data-ttu-id="c8e97-121">来自租户中所有应用程序的请求太多。</span><span class="sxs-lookup"><span data-stu-id="c8e97-121">A large number of requests across all applications in a tenant.</span></span>
- <span data-ttu-id="c8e97-122">来自所有租户中特定应用程序的请求太多。</span><span class="sxs-lookup"><span data-stu-id="c8e97-122">A large number of requests from a particular application across all tenants.</span></span>

## <a name="best-practices-to-handle-throttling"></a><span data-ttu-id="c8e97-123">处理限制的最佳实践</span><span class="sxs-lookup"><span data-stu-id="c8e97-123">Best practices to handle throttling</span></span>

<span data-ttu-id="c8e97-124">以下是处理限制的最佳做法：</span><span class="sxs-lookup"><span data-stu-id="c8e97-124">The following are best practices for handling throttling:</span></span>

- <span data-ttu-id="c8e97-125">减少每个请求的操作数量。</span><span class="sxs-lookup"><span data-stu-id="c8e97-125">Reduce the number of operations per request.</span></span>
- <span data-ttu-id="c8e97-126">减少调用频率。</span><span class="sxs-lookup"><span data-stu-id="c8e97-126">Reduce the frequency of calls.</span></span>
- <span data-ttu-id="c8e97-127">不要立即重试，因为所有请求都会计入使用限制。</span><span class="sxs-lookup"><span data-stu-id="c8e97-127">Avoid immediate retries, because all requests accrue against your usage limits.</span></span>

<span data-ttu-id="c8e97-p105">进行错误处理时，使用 HTTP 错误代码 429 检测限制。失败的响应包括 `Retry-After` 响应标头。使用 `Retry-After` 延迟回退请求是从限制中恢复的最快速的方式，因为 Microsoft Graph 会在客户端受限时继续记录资源使用状况。</span><span class="sxs-lookup"><span data-stu-id="c8e97-p105">When you implement error handling, use the HTTP error code 429 to detect throttling. The failed response includes the `Retry-After` response header. Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span></span>

1. <span data-ttu-id="c8e97-131">等待 `Retry-After` 标头中指定的秒数。</span><span class="sxs-lookup"><span data-stu-id="c8e97-131">Wait the number of seconds specified in the `Retry-After` header.</span></span>
2. <span data-ttu-id="c8e97-132">请重试请求。</span><span class="sxs-lookup"><span data-stu-id="c8e97-132">Retry the request.</span></span>
3. <span data-ttu-id="c8e97-p106">如果请求再次失败，并显示 429 错误代码，则表示你仍然受限。继续使用建议的 `Retry-After` 延迟并重试请求直到成功。</span><span class="sxs-lookup"><span data-stu-id="c8e97-p106">If the request fails again with a 429 error code, you are still being throttled. Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span></span>

<span data-ttu-id="c8e97-135">除非有说明，否则[服务特定限制](#service-specific-limits)部分中所述的所有资源和 API 均提供 `Retry-After` 标头。</span><span class="sxs-lookup"><span data-stu-id="c8e97-135">All the resources and APIs described in the [Service-specific limits](#service-specific-limits) section provide a `Retry-After` header except when noted.</span></span>

<span data-ttu-id="c8e97-136">有关 Microsoft 云限制的更广泛讨论，请参阅[限制模式](https://docs.microsoft.com/azure/architecture/patterns/throttling)。</span><span class="sxs-lookup"><span data-stu-id="c8e97-136">For a broader discussion of throttling in the Microsoft Cloud, see [Throttling pattern](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span></span>

> [!NOTE]
> <span data-ttu-id="c8e97-137">如果响应未提供 `Retry-After` 标头，我们建议实施指数退避重试策略。</span><span class="sxs-lookup"><span data-stu-id="c8e97-137">If no `Retry-After` header is provided by the response, we recommend implementing an exponential backoff retry policy.</span></span> <span data-ttu-id="c8e97-138">构建大型应用程序时，还可以实现[更高级的模式](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency)。</span><span class="sxs-lookup"><span data-stu-id="c8e97-138">You can also implement [more advanced patterns](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) when building large-scale applications.</span></span>
>
> <span data-ttu-id="c8e97-139">Microsoft Graph SDK 已实施依赖于 `Retry-After` 标头或默认为指数退避重试策略的处理程序。</span><span class="sxs-lookup"><span data-stu-id="c8e97-139">Microsoft Graph SDKs already implement handlers that rely on the `Retry-After` header or default to an exponential backoff retry policy.</span></span>

## <a name="best-practices-to-avoid-throttling"></a><span data-ttu-id="c8e97-140">避免限制的最佳做法</span><span class="sxs-lookup"><span data-stu-id="c8e97-140">Best practices to avoid throttling</span></span>

<span data-ttu-id="c8e97-141">如持续轮询资源以检查更新以及定期扫描资源集合以检查新资源或已删除资源之类的编程模式，更有可能导致应用程序受到限制并降低整体性能。</span><span class="sxs-lookup"><span data-stu-id="c8e97-141">Programming patterns like continuously polling a resource to check for updates and regularly scanning resource collections to check for new or deleted resources are more likely to lead to applications being throttled and degrade overall performances.</span></span> <span data-ttu-id="c8e97-142">如果可用，改为使用[更改跟踪](delta-query-overview.md)并[更改通知](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="c8e97-142">You should instead leverage [change tracking](delta-query-overview.md) and [change notifications](webhooks.md) when available.</span></span>

>[!NOTE]
><span data-ttu-id="c8e97-143">[大规模发现文件和检测更改的最佳做法](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online)详细介绍最佳做法。</span><span class="sxs-lookup"><span data-stu-id="c8e97-143">[Best practices for discovering files and detecting changes at scale](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online) describes best practices in details.</span></span>

## <a name="service-specific-limits"></a><span data-ttu-id="c8e97-144">服务特定限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-144">Service-specific limits</span></span>

<span data-ttu-id="c8e97-145">借助 Microsoft Graph，用户可访问[多个服务](overview-major-services.md)中的数据，如 Outlook 或 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="c8e97-145">Microsoft Graph allows you to access data in [multiple services](overview-major-services.md), such as Outlook or Azure Active Directory.</span></span> <span data-ttu-id="c8e97-146">这些服务实施自己的限制，这些限制会影响使用 Microsoft Graph 访问它们的应用程序。</span><span class="sxs-lookup"><span data-stu-id="c8e97-146">These services impose their own throttling limits that affect applications that use Microsoft Graph to access them.</span></span>

<span data-ttu-id="c8e97-147">任何请求均可根据多个限制进行评估，具体取决于限制范围（所有租户中的每个应用、所有应用的每个租户、每个租户的每个应用等）、请求类型（GET、 POST、PATCH等）以及其他因素。</span><span class="sxs-lookup"><span data-stu-id="c8e97-147">Any request can be evaluated against multiple limits, depending on the scope of the limit (per app across all tenants, per tenant for all apps, per app per tenant, and so on), the request type (GET, POST, PATCH, and so on), and other factors.</span></span> <span data-ttu-id="c8e97-148">即将达到的第一个限制会触发阻止行为。</span><span class="sxs-lookup"><span data-stu-id="c8e97-148">The first limit to be reached triggers throttling behavior.</span></span> <span data-ttu-id="c8e97-149">除了本节中描述的服务特定限制之外，还适用以下全局限制：</span><span class="sxs-lookup"><span data-stu-id="c8e97-149">In addition to the service specific-limits described in the section, the following global limits apply:</span></span>

| <span data-ttu-id="c8e97-150">请求类型</span><span class="sxs-lookup"><span data-stu-id="c8e97-150">Request type</span></span> | <span data-ttu-id="c8e97-151">所有租户中的每个应用</span><span class="sxs-lookup"><span data-stu-id="c8e97-151">Per app across all tenants</span></span>  |
| ------------ | ------------------------ |
| <span data-ttu-id="c8e97-152">任何</span><span class="sxs-lookup"><span data-stu-id="c8e97-152">Any</span></span>          | <span data-ttu-id="c8e97-153">每秒 2000 个请求</span><span class="sxs-lookup"><span data-stu-id="c8e97-153">2000 requests per second</span></span> |

> [!NOTE]
> <span data-ttu-id="c8e97-154">此处所述的具体限制可能会发生更改。</span><span class="sxs-lookup"><span data-stu-id="c8e97-154">The specific limits described here are subject to change.</span></span>

> <span data-ttu-id="c8e97-155">**备注** 在本节中，*租户*此术语是指指安装应用程序的 Microsoft 365 组织。</span><span class="sxs-lookup"><span data-stu-id="c8e97-155">**Note:** In this section, the term *tenant* refers to the Microsoft 365 organization where the application is installed.</span></span> <span data-ttu-id="c8e97-156">对于单个租户应用程序，这个租户可以与创建应用程序的租户相同，对于[多租户应用程序](/azure/active-directory/develop/setup-multi-tenant-app)，这个租户可以不同。</span><span class="sxs-lookup"><span data-stu-id="c8e97-156">This tenant can be the same as the the one where the application was created, in the case of a single tenant application, or it can be different, in the case of a [multi-tenant application](/azure/active-directory/develop/setup-multi-tenant-app).</span></span>

### <a name="outlook-service-limits"></a><span data-ttu-id="c8e97-157">Outlook 服务限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-157">Outlook service limits</span></span>

<span data-ttu-id="c8e97-158">将评估每个应用 ID 和邮箱组合的 Outlook 服务限制。</span><span class="sxs-lookup"><span data-stu-id="c8e97-158">Outlook service limits are evaluated for each app ID and mailbox combination.</span></span> <span data-ttu-id="c8e97-159">换言之，上述限制适用于访问特定邮箱（用户或组）的特定应用。</span><span class="sxs-lookup"><span data-stu-id="c8e97-159">In other words, the limits described apply to a specific app accessing a specific mailbox (user or group).</span></span> <span data-ttu-id="c8e97-160">如果一个邮箱的应用程序超过限制，不会影响访问另一个邮箱的功能。</span><span class="sxs-lookup"><span data-stu-id="c8e97-160">If an application exceeds the limit in one mailbox, it does not affect the ability to access another mailbox.</span></span> <span data-ttu-id="c8e97-161">下面的限制适用于公共云以及[区域云部署](/graph/deployments)。</span><span class="sxs-lookup"><span data-stu-id="c8e97-161">The following limits apply to the public cloud as well as [national cloud deployments](/graph/deployments).</span></span>

| <span data-ttu-id="c8e97-162">限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-162">Limit</span></span>                                                      | <span data-ttu-id="c8e97-163">适用对象</span><span class="sxs-lookup"><span data-stu-id="c8e97-163">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="c8e97-164">10 分钟内的 10,000 个 API 请求</span><span class="sxs-lookup"><span data-stu-id="c8e97-164">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="c8e97-165">v1.0 和 beta 终结点</span><span class="sxs-lookup"><span data-stu-id="c8e97-165">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="c8e97-166">4 个并发请求</span><span class="sxs-lookup"><span data-stu-id="c8e97-166">4 concurrent requests</span></span>                                      | <span data-ttu-id="c8e97-167">v1.0 和 beta 终结点</span><span class="sxs-lookup"><span data-stu-id="c8e97-167">v1.0 and beta endpoints</span></span>   |
| <span data-ttu-id="c8e97-168">30 秒内的 15 兆字节 (MB) 上传（PATCH、POST、PUT）</span><span class="sxs-lookup"><span data-stu-id="c8e97-168">15 megabytes (MB) upload (PATCH, POST, PUT) in a 30 second period</span></span> | <span data-ttu-id="c8e97-169">v1.0 和 beta 终结点</span><span class="sxs-lookup"><span data-stu-id="c8e97-169">v1.0 and beta endpoints</span></span>   |

#### <a name="outlook-service-resources"></a><span data-ttu-id="c8e97-170">Outlook 服务资源</span><span class="sxs-lookup"><span data-stu-id="c8e97-170">Outlook service resources</span></span>

<span data-ttu-id="c8e97-171">Outlook 服务提供以下资源。</span><span class="sxs-lookup"><span data-stu-id="c8e97-171">The following resources are provided by the Outlook service.</span></span>

##### <a name="search-api-resources-preview"></a><span data-ttu-id="c8e97-172">搜索 API 资源（预览版）</span><span class="sxs-lookup"><span data-stu-id="c8e97-172">Search API resources (preview)</span></span>

- [<span data-ttu-id="c8e97-173">外部项（Microsoft 搜索）</span><span class="sxs-lookup"><span data-stu-id="c8e97-173">External item (Microsoft Search)</span></span>](/graph/api/resources/externalitem?view=graph-rest-beta)

##### <a name="profile-api-resources"></a><span data-ttu-id="c8e97-174">配置文件 API 资源</span><span class="sxs-lookup"><span data-stu-id="c8e97-174">Profile API resources</span></span>

- [<span data-ttu-id="c8e97-175">照片</span><span class="sxs-lookup"><span data-stu-id="c8e97-175">Photo</span></span>](/graph/api/resources/profilephoto?view=graph-rest-1.0)

##### <a name="calendar-api-resources"></a><span data-ttu-id="c8e97-176">日历 API 资源</span><span class="sxs-lookup"><span data-stu-id="c8e97-176">Calendar API resources</span></span>

- [<span data-ttu-id="c8e97-177">event</span><span class="sxs-lookup"><span data-stu-id="c8e97-177">event</span></span>](/graph/api/resources/event)
- [<span data-ttu-id="c8e97-178">eventMessage</span><span class="sxs-lookup"><span data-stu-id="c8e97-178">eventMessage</span></span>](/graph/api/resources/eventmessage)
- [<span data-ttu-id="c8e97-179">calendar</span><span class="sxs-lookup"><span data-stu-id="c8e97-179">calendar</span></span>](/graph/api/resources/calendar)
- [<span data-ttu-id="c8e97-180">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="c8e97-180">calendarGroup</span></span>](/graph/api/resources/calendargroup)
- [<span data-ttu-id="c8e97-181">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="c8e97-181">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="c8e97-182">attachment</span><span class="sxs-lookup"><span data-stu-id="c8e97-182">attachment</span></span>](/graph/api/resources/attachment)
- [<span data-ttu-id="c8e97-183">place（预览）</span><span class="sxs-lookup"><span data-stu-id="c8e97-183">place (preview)</span></span>](/graph/api/resources/place)

##### <a name="mail-api-resources"></a><span data-ttu-id="c8e97-184">邮件 API 资源</span><span class="sxs-lookup"><span data-stu-id="c8e97-184">Mail API resources</span></span>

- [<span data-ttu-id="c8e97-185">message</span><span class="sxs-lookup"><span data-stu-id="c8e97-185">message</span></span>](/graph/api/resources/message)
- [<span data-ttu-id="c8e97-186">mailFolder</span><span class="sxs-lookup"><span data-stu-id="c8e97-186">mailFolder</span></span>](/graph/api/resources/mailfolder)
- [<span data-ttu-id="c8e97-187">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="c8e97-187">mailSearchFolder</span></span>](/graph/api/resources/mailsearchfolder)
- [<span data-ttu-id="c8e97-188">messageRule</span><span class="sxs-lookup"><span data-stu-id="c8e97-188">messageRule</span></span>](/graph/api/resources/messagerule)
- [<span data-ttu-id="c8e97-189">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="c8e97-189">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="c8e97-190">attachment</span><span class="sxs-lookup"><span data-stu-id="c8e97-190">attachment</span></span>](/graph/api/resources/attachment)

##### <a name="personal-contacts-api-resources"></a><span data-ttu-id="c8e97-191">个人联系人 API 资源</span><span class="sxs-lookup"><span data-stu-id="c8e97-191">Personal contacts API resources</span></span>

- [<span data-ttu-id="c8e97-192">contact</span><span class="sxs-lookup"><span data-stu-id="c8e97-192">contact</span></span>](/graph/api/resources/contact)
- [<span data-ttu-id="c8e97-193">contactFolder</span><span class="sxs-lookup"><span data-stu-id="c8e97-193">contactFolder</span></span>](/graph/api/resources/contactfolder)
- [<span data-ttu-id="c8e97-194">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="c8e97-194">outlookCategory</span></span>](/graph/api/resources/outlookcategory)

##### <a name="social-and-workplace-intelligence-resources"></a><span data-ttu-id="c8e97-195">社交和工作区智能资源</span><span class="sxs-lookup"><span data-stu-id="c8e97-195">Social and workplace intelligence resources</span></span>

- [<span data-ttu-id="c8e97-196">person</span><span class="sxs-lookup"><span data-stu-id="c8e97-196">person</span></span>](/graph/api/resources/person)

##### <a name="to-do-tasks-api-preview-resources"></a><span data-ttu-id="c8e97-197">待办任务 API（预览）资源</span><span class="sxs-lookup"><span data-stu-id="c8e97-197">To-do tasks API (preview) resources</span></span>

- [<span data-ttu-id="c8e97-198">outlookTask</span><span class="sxs-lookup"><span data-stu-id="c8e97-198">outlookTask</span></span>](/graph/api/resources/outlooktask)
- [<span data-ttu-id="c8e97-199">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="c8e97-199">outlookTaskFolder</span></span>](/graph/api/resources/outlooktaskfolder)
- [<span data-ttu-id="c8e97-200">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="c8e97-200">outlookTaskGroup</span></span>](/graph/api/resources/outlooktaskgroup)
- [<span data-ttu-id="c8e97-201">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="c8e97-201">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="c8e97-202">attachment</span><span class="sxs-lookup"><span data-stu-id="c8e97-202">attachment</span></span>](/graph/api/resources/attachment)

### <a name="cloud-communication-service-limits"></a><span data-ttu-id="c8e97-203">云通信服务限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-203">Cloud communication service limits</span></span>

| <span data-ttu-id="c8e97-204">资源</span><span class="sxs-lookup"><span data-stu-id="c8e97-204">Resource</span></span>      | <span data-ttu-id="c8e97-205">每个租户每个应用限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-205">Limits per app per tenant</span></span>    |
| -------------- | ------------ |
| [<span data-ttu-id="c8e97-206">通话</span><span class="sxs-lookup"><span data-stu-id="c8e97-206">Calls</span></span>](/graph/api/resources/call) | <span data-ttu-id="c8e97-207">每月10,000 通通话和 100 通并发通话</span><span class="sxs-lookup"><span data-stu-id="c8e97-207">10,000 calls/month and 100 concurrent calls</span></span>   |
| [<span data-ttu-id="c8e97-208">会议信息</span><span class="sxs-lookup"><span data-stu-id="c8e97-208">Meeting information</span></span>](/graph/api/resources/meetinginfo)   | <span data-ttu-id="c8e97-209">每月每位用家会有 2000 则会议</span><span class="sxs-lookup"><span data-stu-id="c8e97-209">2000 meetings/user each month</span></span> |
| <span data-ttu-id="c8e97-210">[状态](/graph/api/resources/presence)（预览版）</span><span class="sxs-lookup"><span data-stu-id="c8e97-210">[Presence](/graph/api/resources/presence) (preview)</span></span>   | <span data-ttu-id="c8e97-211">2 rps</span><span class="sxs-lookup"><span data-stu-id="c8e97-211">2 rps</span></span> |

### <a name="onenote-service-limits"></a><span data-ttu-id="c8e97-212">OneNote 服务限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-212">OneNote service limits</span></span>

| <span data-ttu-id="c8e97-213">限制类型</span><span class="sxs-lookup"><span data-stu-id="c8e97-213">Limit type</span></span> | <span data-ttu-id="c8e97-214">每个用户的每个应用程序的限制（委派的上下文）</span><span class="sxs-lookup"><span data-stu-id="c8e97-214">Limit per app per user (delegated context)</span></span> | <span data-ttu-id="c8e97-215">每个应用程序的限制（仅应用程序上下文）</span><span class="sxs-lookup"><span data-stu-id="c8e97-215">Limit per app (app-only context)</span></span> |
| ------------ | ------- | ------- |
| <span data-ttu-id="c8e97-216">请求率</span><span class="sxs-lookup"><span data-stu-id="c8e97-216">Requests rate</span></span> | <span data-ttu-id="c8e97-217">每 1 分钟 120 个请求和每 1 小时 400 个请求</span><span class="sxs-lookup"><span data-stu-id="c8e97-217">120 requests per 1 minute and 400 per 1 hour</span></span> | <span data-ttu-id="c8e97-218">每 1 分钟 240 个请求和每 1 小时 800 个请求</span><span class="sxs-lookup"><span data-stu-id="c8e97-218">240 requests per 1 minute and 800 per 1 hour</span></span> |
| <span data-ttu-id="c8e97-219">并发请求</span><span class="sxs-lookup"><span data-stu-id="c8e97-219">Concurrent requests</span></span> | <span data-ttu-id="c8e97-220">5 个并发请求</span><span class="sxs-lookup"><span data-stu-id="c8e97-220">5 concurrent requests</span></span> | <span data-ttu-id="c8e97-221">20 个并发请求</span><span class="sxs-lookup"><span data-stu-id="c8e97-221">20 concurrent requests</span></span> |

<span data-ttu-id="c8e97-222">上述限制适用于下列资源:</span><span class="sxs-lookup"><span data-stu-id="c8e97-222">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="c8e97-223">onenote, notebook, sectionGroup, onenoteSection, onenotePage, onenoteResource, onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="c8e97-223">onenote, notebook, sectionGroup, onenoteSection, onenotePage, onenoteResource, onenoteOperation</span></span>

<span data-ttu-id="c8e97-224">可在 [OneNote API 限制及避免方法](https://developer.microsoft.com/zh-CN/office/blogs/onenote-api-throttling-and-how-to-avoid-it/) 中找到有关最佳做法的附加信息。</span><span class="sxs-lookup"><span data-stu-id="c8e97-224">You can find additional information about best practices in [OneNote API throttling and how to avoid it](https://developer.microsoft.com/zh-CN/office/blogs/onenote-api-throttling-and-how-to-avoid-it/).</span></span>  

> <span data-ttu-id="c8e97-225">**注意：** 上面列出的资源未在 `429 Too Many Requests` 响应上返回 `Retry-After` 标头。</span><span class="sxs-lookup"><span data-stu-id="c8e97-225">**Note:** The resources listed above do not return a `Retry-After` header on `429 Too Many Requests` responses.</span></span>

### <a name="project-rome-service-limits"></a><span data-ttu-id="c8e97-226">Project Rome 服务限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-226">Project Rome service limits</span></span>

| <span data-ttu-id="c8e97-227">请求类型</span><span class="sxs-lookup"><span data-stu-id="c8e97-227">Request type</span></span> | <span data-ttu-id="c8e97-228">所有应用的每个用户的限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-228">Limit per user for all apps</span></span> |
| ------------ | --------------------------- |
| <span data-ttu-id="c8e97-229">GET</span><span class="sxs-lookup"><span data-stu-id="c8e97-229">GET</span></span>          | <span data-ttu-id="c8e97-230">每 5 分钟 400 个请求和每天 12000 个请求</span><span class="sxs-lookup"><span data-stu-id="c8e97-230">400 requests per 5 minutes and 12000 requests per 1 day</span></span> |
| <span data-ttu-id="c8e97-231">POST, PUT, PATCH, DELETE</span><span class="sxs-lookup"><span data-stu-id="c8e97-231">POST, PUT, PATCH, DELETE</span></span> | <span data-ttu-id="c8e97-232">每 5 分钟 100 个请求和每天 8000 个请求</span><span class="sxs-lookup"><span data-stu-id="c8e97-232">100 requests per 5 minutes and 8000 requests per 1 day</span></span> |

<span data-ttu-id="c8e97-233">上述限制适用于下列资源:</span><span class="sxs-lookup"><span data-stu-id="c8e97-233">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="c8e97-234">activityHistoryItem、userActivity</span><span class="sxs-lookup"><span data-stu-id="c8e97-234">activityHistoryItem, userActivity</span></span>

### <a name="microsoft-teams-service-limits"></a><span data-ttu-id="c8e97-235">Microsoft Teams 服务限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-235">Microsoft Teams service limits</span></span>

<span data-ttu-id="c8e97-236">限制表示为每秒请求数 (rps)。</span><span class="sxs-lookup"><span data-stu-id="c8e97-236">Limits are expressed as requests per second (rps).</span></span>

| <span data-ttu-id="c8e97-237">Teams 请求类型</span><span class="sxs-lookup"><span data-stu-id="c8e97-237">Teams request type</span></span>                                   | <span data-ttu-id="c8e97-238">每个租户每个应用限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-238">Limit per app per tenant</span></span>        | <span data-ttu-id="c8e97-239">所有租户中的每个应用限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-239">Limit per app across all tenants</span></span>      |
|------------------------------------------------------|---------------------------------|------------|
| <span data-ttu-id="c8e97-240">Microsoft Teams 的任何图形 API 调用</span><span class="sxs-lookup"><span data-stu-id="c8e97-240">Any Graph API calls for Microsoft Teams</span></span>              | <span data-ttu-id="c8e97-241">每 10 秒 15000 个请求</span><span class="sxs-lookup"><span data-stu-id="c8e97-241">15000 requests every 10 seconds</span></span> | <span data-ttu-id="c8e97-242">不适用</span><span class="sxs-lookup"><span data-stu-id="c8e97-242">n/a</span></span> |
| <span data-ttu-id="c8e97-243">GET team, channel, tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="c8e97-243">GET team, channel, tab, installedApps, appCatalogs</span></span>   | <span data-ttu-id="c8e97-244">60 rps</span><span class="sxs-lookup"><span data-stu-id="c8e97-244">60 rps</span></span>                          | <span data-ttu-id="c8e97-245">600 rps</span><span class="sxs-lookup"><span data-stu-id="c8e97-245">600 rps</span></span> |
| <span data-ttu-id="c8e97-246">POST/PUT channel, tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="c8e97-246">POST/PUT channel, tab, installedApps, appCatalogs</span></span>    |  <span data-ttu-id="c8e97-247">30 rps</span><span class="sxs-lookup"><span data-stu-id="c8e97-247">30 rps</span></span>                         | <span data-ttu-id="c8e97-248">300 rps</span><span class="sxs-lookup"><span data-stu-id="c8e97-248">300 rps</span></span>  |
| <span data-ttu-id="c8e97-249">PATCH team, channel, tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="c8e97-249">PATCH team, channel, tab, installedApps, appCatalogs</span></span> |  <span data-ttu-id="c8e97-250">30 rps</span><span class="sxs-lookup"><span data-stu-id="c8e97-250">30 rps</span></span>                         | <span data-ttu-id="c8e97-251">300 rps</span><span class="sxs-lookup"><span data-stu-id="c8e97-251">300 rps</span></span>  |
| <span data-ttu-id="c8e97-252">DELETE channel, tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="c8e97-252">DELETE channel, tab, installedApps, appCatalogs</span></span>      |  <span data-ttu-id="c8e97-253">15 rps</span><span class="sxs-lookup"><span data-stu-id="c8e97-253">15 rps</span></span>                         | <span data-ttu-id="c8e97-254">150 rps</span><span class="sxs-lookup"><span data-stu-id="c8e97-254">150 rps</span></span>  |
| <span data-ttu-id="c8e97-255">GET /teams/```{team-id}```, joinedTeams</span><span class="sxs-lookup"><span data-stu-id="c8e97-255">GET /teams/```{team-id}```, joinedTeams</span></span>              |  <span data-ttu-id="c8e97-256">30 rps</span><span class="sxs-lookup"><span data-stu-id="c8e97-256">30 rps</span></span>                         | <span data-ttu-id="c8e97-257">300 rps</span><span class="sxs-lookup"><span data-stu-id="c8e97-257">300 rps</span></span>  |
| <span data-ttu-id="c8e97-258">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, clone</span><span class="sxs-lookup"><span data-stu-id="c8e97-258">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, clone</span></span> | <span data-ttu-id="c8e97-259">6 rps</span><span class="sxs-lookup"><span data-stu-id="c8e97-259">6 rps</span></span> | <span data-ttu-id="c8e97-260">150 rps</span><span class="sxs-lookup"><span data-stu-id="c8e97-260">150 rps</span></span>  |
| <span data-ttu-id="c8e97-261">GET channel message</span><span class="sxs-lookup"><span data-stu-id="c8e97-261">GET channel message</span></span>  | <span data-ttu-id="c8e97-262">5 rps</span><span class="sxs-lookup"><span data-stu-id="c8e97-262">5 rps</span></span> | <span data-ttu-id="c8e97-263">100 rps</span><span class="sxs-lookup"><span data-stu-id="c8e97-263">100 rps</span></span> |
| <span data-ttu-id="c8e97-264">GET 1:1/group chat message</span><span class="sxs-lookup"><span data-stu-id="c8e97-264">GET 1:1/group chat message</span></span>  | <span data-ttu-id="c8e97-265">3 rps</span><span class="sxs-lookup"><span data-stu-id="c8e97-265">3 rps</span></span> | <span data-ttu-id="c8e97-266">30 rps</span><span class="sxs-lookup"><span data-stu-id="c8e97-266">30 rps</span></span> |
| <span data-ttu-id="c8e97-267">POST channel message</span><span class="sxs-lookup"><span data-stu-id="c8e97-267">POST channel message</span></span> | <span data-ttu-id="c8e97-268">2 rps</span><span class="sxs-lookup"><span data-stu-id="c8e97-268">2 rps</span></span> | <span data-ttu-id="c8e97-269">20 rps</span><span class="sxs-lookup"><span data-stu-id="c8e97-269">20 rps</span></span> |
| <span data-ttu-id="c8e97-270">POST 1:1/group chat message</span><span class="sxs-lookup"><span data-stu-id="c8e97-270">POST 1:1/group chat message</span></span> | <span data-ttu-id="c8e97-271">2 rps</span><span class="sxs-lookup"><span data-stu-id="c8e97-271">2 rps</span></span> | <span data-ttu-id="c8e97-272">20 rps</span><span class="sxs-lookup"><span data-stu-id="c8e97-272">20 rps</span></span> |
| <span data-ttu-id="c8e97-273">GET/teams/```{team-id}```/在以下路径下的日程安排和所有 API</span><span class="sxs-lookup"><span data-stu-id="c8e97-273">GET /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="c8e97-274">60 rps</span><span class="sxs-lookup"><span data-stu-id="c8e97-274">60 rps</span></span> | <span data-ttu-id="c8e97-275">600 rps</span><span class="sxs-lookup"><span data-stu-id="c8e97-275">600 rps</span></span> |
| <span data-ttu-id="c8e97-276">POST, PATCH, PUT /teams/```{team-id}```/在以下路径下的日程安排和所有 API</span><span class="sxs-lookup"><span data-stu-id="c8e97-276">POST, PATCH, PUT /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="c8e97-277">30 rps</span><span class="sxs-lookup"><span data-stu-id="c8e97-277">30 rps</span></span> | <span data-ttu-id="c8e97-278">300 rps</span><span class="sxs-lookup"><span data-stu-id="c8e97-278">300 rps</span></span> |
| <span data-ttu-id="c8e97-279">DELETE /teams/```{team-id}```/在以下路径下的日程安排和所有 API</span><span class="sxs-lookup"><span data-stu-id="c8e97-279">DELETE /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="c8e97-280">15 rps</span><span class="sxs-lookup"><span data-stu-id="c8e97-280">15 rps</span></span> | <span data-ttu-id="c8e97-281">150 rps</span><span class="sxs-lookup"><span data-stu-id="c8e97-281">150 rps</span></span> |

<span data-ttu-id="c8e97-282">对于给定团队或频道，每个应用最多可发布 4 个请求。</span><span class="sxs-lookup"><span data-stu-id="c8e97-282">A maximum of 4 requests per second per app can be issued on a given team or channel.</span></span>
<span data-ttu-id="c8e97-283">每个应用每天最多可以将 3000 条消息发送到给定的频道。</span><span class="sxs-lookup"><span data-stu-id="c8e97-283">A maximum of 3000 messages per app per day can be sent to a given channel.</span></span>

<span data-ttu-id="c8e97-284">另请参阅 [Microsoft Teams 限制](/graph/api/resources/teams-api-overview#microsoft-teams-limits)和[投票要求](/graph/api/resources/teams-api-overview#polling-requirements)。</span><span class="sxs-lookup"><span data-stu-id="c8e97-284">See also [Microsoft Teams limits](/graph/api/resources/teams-api-overview#microsoft-teams-limits) and [polling requirements](/graph/api/resources/teams-api-overview#polling-requirements).</span></span>

<span data-ttu-id="c8e97-285">上述限制适用于下列资源:</span><span class="sxs-lookup"><span data-stu-id="c8e97-285">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="c8e97-286">aadUserConversationMember、appCatalogs、changeTrackedEntity、channel、chatMessage、chatMessageHostedContent、conversationMember、offerShiftRequest、openShift、openShiftChangeRequest、schedule、scheduleChangeRequest、schedulingGroup、shift、shiftPreferences、swapShiftsChangeRequest、team、teamsApp、teamsAppDefinition、teamsAppInstallation、teamsAsyncOperation、teamsTab、teamsTemplate、teamwork、timeOff、timeOffReason、timeOffRequest、userSettings、workforceIntegration。</span><span class="sxs-lookup"><span data-stu-id="c8e97-286">aadUserConversationMember, appCatalogs, changeTrackedEntity, channel, chatMessage, chatMessageHostedContent, conversationMember, offerShiftRequest, openShift, openShiftChangeRequest, schedule, scheduleChangeRequest, schedulingGroup, shift, shiftPreferences, swapShiftsChangeRequest, team, teamsApp, teamsAppDefinition, teamsAppInstallation, teamsAsyncOperation, teamsTab, teamsTemplate, teamwork, timeOff, timeOffReason, timeOffRequest, userSettings, workforceIntegration.</span></span>

### <a name="identity-and-access-service-limits"></a><span data-ttu-id="c8e97-287">身份和访问服务限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-287">Identity and access service limits</span></span>

<span data-ttu-id="c8e97-288">这些服务限制适用于以下实体：</span><span class="sxs-lookup"><span data-stu-id="c8e97-288">These service limits apply to the following entities:</span></span>

- [<span data-ttu-id="c8e97-289">目录对象</span><span class="sxs-lookup"><span data-stu-id="c8e97-289">Directory object</span></span>](/graph/api/resources/directoryobject)
- [<span data-ttu-id="c8e97-290">扩展属性</span><span class="sxs-lookup"><span data-stu-id="c8e97-290">Extension property</span></span>](/graph/api/resources/extensionproperty)
- [<span data-ttu-id="c8e97-291">管理单元</span><span class="sxs-lookup"><span data-stu-id="c8e97-291">Administrative unit</span></span>](/graph/api/resources/administrativeunit)
- [<span data-ttu-id="c8e97-292">应用程序</span><span class="sxs-lookup"><span data-stu-id="c8e97-292">Application</span></span>](/graph/api/resources/application)
- [<span data-ttu-id="c8e97-293">应用角色分配</span><span class="sxs-lookup"><span data-stu-id="c8e97-293">Application role assignment</span></span>](/graph/api/resources/approleassignment)
- [<span data-ttu-id="c8e97-294">基于证书的身份配置</span><span class="sxs-lookup"><span data-stu-id="c8e97-294">Certificate based auth configuration</span></span>](/graph/api/resources/certificatebasedauthconfiguration)
- [<span data-ttu-id="c8e97-295">组织联系人</span><span class="sxs-lookup"><span data-stu-id="c8e97-295">Organizational contact</span></span>](/graph/api/resources/orgcontact)
- [<span data-ttu-id="c8e97-296">Device</span><span class="sxs-lookup"><span data-stu-id="c8e97-296">Device</span></span>](/graph/api/resources/device)
- [<span data-ttu-id="c8e97-297">目录对象合作伙伴参考</span><span class="sxs-lookup"><span data-stu-id="c8e97-297">Directory object partner reference</span></span>](/graph/api/resources/directoryobjectpartnerreference)
- [<span data-ttu-id="c8e97-298">目录角色</span><span class="sxs-lookup"><span data-stu-id="c8e97-298">Directory role</span></span>](/graph/api/resources/directoryrole)
- [<span data-ttu-id="c8e97-299">目录角色模板</span><span class="sxs-lookup"><span data-stu-id="c8e97-299">Directory role template</span></span>](/graph/api/resources/directoryroletemplate)
- [<span data-ttu-id="c8e97-300">域</span><span class="sxs-lookup"><span data-stu-id="c8e97-300">Domain</span></span>](/graph/api/resources/domain)
- [<span data-ttu-id="c8e97-301">域 dns 记录</span><span class="sxs-lookup"><span data-stu-id="c8e97-301">Domain dns record</span></span>](/graph/api/resources/domaindnsrecord)
- [<span data-ttu-id="c8e97-302">域 dns cname 记录</span><span class="sxs-lookup"><span data-stu-id="c8e97-302">Domain dns cname record</span></span>](/graph/api/resources/domaindnscnamerecord)
- [<span data-ttu-id="c8e97-303">域 dns mx 记录</span><span class="sxs-lookup"><span data-stu-id="c8e97-303">Domain dns mx record</span></span>](/graph/api/resources/domaindnsmxrecord)
- [<span data-ttu-id="c8e97-304">域 dns srv 记录</span><span class="sxs-lookup"><span data-stu-id="c8e97-304">Domain dns srv record</span></span>](/graph/api/resources/domaindnssrvrecord)
- [<span data-ttu-id="c8e97-305">域 dns txt 记录</span><span class="sxs-lookup"><span data-stu-id="c8e97-305">Domain dns txt record</span></span>](/graph/api/resources/domaindnstxtrecord)
- [<span data-ttu-id="c8e97-306">域 dns 不可用记录</span><span class="sxs-lookup"><span data-stu-id="c8e97-306">Domain dns unavailable record</span></span>](/graph/api/resources/domaindnsunavailablerecord)
- [<span data-ttu-id="c8e97-307">终结点</span><span class="sxs-lookup"><span data-stu-id="c8e97-307">Endpoint</span></span>](/graph/api/resources/endpoint)
- [<span data-ttu-id="c8e97-308">扩展属性</span><span class="sxs-lookup"><span data-stu-id="c8e97-308">Extension property</span></span>](/graph/api/resources/extensionproperty)
- [<span data-ttu-id="c8e97-309">许可证详细信息</span><span class="sxs-lookup"><span data-stu-id="c8e97-309">License details</span></span>](/graph/api/resources/licensedetails)
- [<span data-ttu-id="c8e97-310">组</span><span class="sxs-lookup"><span data-stu-id="c8e97-310">Group</span></span>](/graph/api/resources/group)
- [<span data-ttu-id="c8e97-311">基于活动的超时策略</span><span class="sxs-lookup"><span data-stu-id="c8e97-311">Activity based timeout policy</span></span>](/graph/api/resources/activitybasedtimeoutpolicy)
- [<span data-ttu-id="c8e97-312">声明映射策略</span><span class="sxs-lookup"><span data-stu-id="c8e97-312">Claims mapping policy</span></span>](/graph/api/resources/claimsmappingpolicy)
- [<span data-ttu-id="c8e97-313">主领域发现策略</span><span class="sxs-lookup"><span data-stu-id="c8e97-313">Home realm discovery policy</span></span>](/graph/api/resources/homerealmdiscoverypolicy)
- [<span data-ttu-id="c8e97-314">令牌颁发策略</span><span class="sxs-lookup"><span data-stu-id="c8e97-314">Token issuance policy</span></span>](/graph/api/resources/tokenissuancepolicy)
- [<span data-ttu-id="c8e97-315">令牌生存期策略</span><span class="sxs-lookup"><span data-stu-id="c8e97-315">Token lifetime policy</span></span>](/graph/api/resources/tokenlifetimepolicy)
- [<span data-ttu-id="c8e97-316">策略基础</span><span class="sxs-lookup"><span data-stu-id="c8e97-316">Policy base</span></span>](/graph/api/resources/policybase)
- [<span data-ttu-id="c8e97-317">Sts 策略</span><span class="sxs-lookup"><span data-stu-id="c8e97-317">Sts policy</span></span>](/graph/api/resources/stspolicy)
- [<span data-ttu-id="c8e97-318">合同</span><span class="sxs-lookup"><span data-stu-id="c8e97-318">Contract</span></span>](/graph/api/resources/contract)
- [<span data-ttu-id="c8e97-319">服务主体</span><span class="sxs-lookup"><span data-stu-id="c8e97-319">Service principal</span></span>](/graph/api/resources/serviceprincipal)
- [<span data-ttu-id="c8e97-320">订阅的 SKU</span><span class="sxs-lookup"><span data-stu-id="c8e97-320">Subscribed sku</span></span>](/graph/api/resources/subscribedsku)
- [<span data-ttu-id="c8e97-321">Oauth2 权限授予</span><span class="sxs-lookup"><span data-stu-id="c8e97-321">OAuth2 permission grant</span></span>](/graph/api/resources/oauth2permissiongrant)
- [<span data-ttu-id="c8e97-322">组织</span><span class="sxs-lookup"><span data-stu-id="c8e97-322">Organization</span></span>](/graph/api/resources/organization)
- [<span data-ttu-id="c8e97-323">用户</span><span class="sxs-lookup"><span data-stu-id="c8e97-323">User</span></span>](/graph/api/resources/user)
- [<span data-ttu-id="c8e97-324">组设置</span><span class="sxs-lookup"><span data-stu-id="c8e97-324">Group setting</span></span>](/graph/api/resources/groupsetting)
- [<span data-ttu-id="c8e97-325">组设置模板</span><span class="sxs-lookup"><span data-stu-id="c8e97-325">Group setting template</span></span>](/graph/api/resources/groupsettingtemplate)

#### <a name="pattern"></a><span data-ttu-id="c8e97-326">模式</span><span class="sxs-lookup"><span data-stu-id="c8e97-326">Pattern</span></span>

<span data-ttu-id="c8e97-327">限制基于令牌存储桶算法，后者通过添加各个请求的成本来实现。</span><span class="sxs-lookup"><span data-stu-id="c8e97-327">Throttling is based on a token bucket algorithm, which works by adding individual costs of requests.</span></span> <span data-ttu-id="c8e97-328">然后将请求成本的总和与预定限制进行比较。</span><span class="sxs-lookup"><span data-stu-id="c8e97-328">The sum of request costs is then compared against pre-determined limits.</span></span> <span data-ttu-id="c8e97-329">只有超出限制的请求才会被限制。</span><span class="sxs-lookup"><span data-stu-id="c8e97-329">Only the requests exceeding the limits will be throttled.</span></span> <span data-ttu-id="c8e97-330">如果超出任何限制，则响应将为 `429 Too Many Requests`。</span><span class="sxs-lookup"><span data-stu-id="c8e97-330">If any of the limits are exceeded, the response will be `429 Too Many Requests`.</span></span> <span data-ttu-id="c8e97-331">即使在服务处于重要负载或基于特定租户的数据量的情况下，也可能会收到 `429 Too Many Requests` 的响应，而不会达到以下限制。</span><span class="sxs-lookup"><span data-stu-id="c8e97-331">It is possible to receive `429 Too Many Requests` responses even when the following limits are not reached, in situations when the services are under an important load or based on data volume for a specific tenant.</span></span> <span data-ttu-id="c8e97-332">下表列出了现有限制。</span><span class="sxs-lookup"><span data-stu-id="c8e97-332">The following table lists existing limits.</span></span>

| <span data-ttu-id="c8e97-333">限制类型</span><span class="sxs-lookup"><span data-stu-id="c8e97-333">Limit type</span></span> | <span data-ttu-id="c8e97-334">资源单元配额</span><span class="sxs-lookup"><span data-stu-id="c8e97-334">Resource unit quota</span></span> | <span data-ttu-id="c8e97-335">写入配额</span><span class="sxs-lookup"><span data-stu-id="c8e97-335">Write quota</span></span> |
| ---------- | ----------- | -------------- |
| <span data-ttu-id="c8e97-336">应用 + 租户对</span><span class="sxs-lookup"><span data-stu-id="c8e97-336">application+tenant pair</span></span> | <span data-ttu-id="c8e97-337">S：3500，M:5000，L:8000 每 10 秒钟</span><span class="sxs-lookup"><span data-stu-id="c8e97-337">S: 3500, M:5000, L:8000 per 10 seconds</span></span> | <span data-ttu-id="c8e97-338">每 2 分钟 30 秒 3000</span><span class="sxs-lookup"><span data-stu-id="c8e97-338">3000 per 2 minutes and 30 seconds</span></span> |
| <span data-ttu-id="c8e97-339">应用程序</span><span class="sxs-lookup"><span data-stu-id="c8e97-339">application</span></span> | <span data-ttu-id="c8e97-340">每 20 秒 150,000</span><span class="sxs-lookup"><span data-stu-id="c8e97-340">150,000 per 20 seconds</span></span>  | <span data-ttu-id="c8e97-341">每 5 分钟 70,000</span><span class="sxs-lookup"><span data-stu-id="c8e97-341">70,000 per 5 minutes</span></span> |
| <span data-ttu-id="c8e97-342">租户</span><span class="sxs-lookup"><span data-stu-id="c8e97-342">tenant</span></span> | <span data-ttu-id="c8e97-343">不适用</span><span class="sxs-lookup"><span data-stu-id="c8e97-343">Not Applicable</span></span> | <span data-ttu-id="c8e97-344">每 5 分钟 9000</span><span class="sxs-lookup"><span data-stu-id="c8e97-344">9000 per 5 minutes</span></span> |

> <span data-ttu-id="c8e97-345">**注意**：应用程序 + 租户对限制因租户请求中运行的用户数而异。</span><span class="sxs-lookup"><span data-stu-id="c8e97-345">**Note**: The application + tenant pair limit varies based on the number of users in the tenant requests are run against.</span></span> <span data-ttu-id="c8e97-346">租户规模定义如下：S - 小于 50 个用户，M - 50 至 500 个用户之间，L - 500 个以上用户。</span><span class="sxs-lookup"><span data-stu-id="c8e97-346">The tenant sizes are defined as follows: S - under 50 users, M - between 50 and 500 users, and L - above 500 users.</span></span>

<span data-ttu-id="c8e97-347">下表列出了基本请求费用。</span><span class="sxs-lookup"><span data-stu-id="c8e97-347">The following table lists base request costs.</span></span> <span data-ttu-id="c8e97-348">未列出的任何请求的基础成本为 1。</span><span class="sxs-lookup"><span data-stu-id="c8e97-348">Any requests not listed have a base cost of 1.</span></span>

| <span data-ttu-id="c8e97-349">操作</span><span class="sxs-lookup"><span data-stu-id="c8e97-349">Operation</span></span> | <span data-ttu-id="c8e97-350">请求路径</span><span class="sxs-lookup"><span data-stu-id="c8e97-350">Request Path</span></span> | <span data-ttu-id="c8e97-351">基本资源单位成本</span><span class="sxs-lookup"><span data-stu-id="c8e97-351">Base Resource Unit Cost</span></span> | <span data-ttu-id="c8e97-352">写入成本</span><span class="sxs-lookup"><span data-stu-id="c8e97-352">Write Cost</span></span> |
| --------- | ------------ | ----------------- | ------------------ |
| <span data-ttu-id="c8e97-353">GET</span><span class="sxs-lookup"><span data-stu-id="c8e97-353">GET</span></span> | `applications` | <span data-ttu-id="c8e97-354">2</span><span class="sxs-lookup"><span data-stu-id="c8e97-354">2</span></span> | <span data-ttu-id="c8e97-355">0</span><span class="sxs-lookup"><span data-stu-id="c8e97-355">0</span></span> |
| <span data-ttu-id="c8e97-356">GET</span><span class="sxs-lookup"><span data-stu-id="c8e97-356">GET</span></span> | `applications/{id}/extensionProperties` | <span data-ttu-id="c8e97-357">2</span><span class="sxs-lookup"><span data-stu-id="c8e97-357">2</span></span> | <span data-ttu-id="c8e97-358">0</span><span class="sxs-lookup"><span data-stu-id="c8e97-358">0</span></span> |
| <span data-ttu-id="c8e97-359">GET</span><span class="sxs-lookup"><span data-stu-id="c8e97-359">GET</span></span> | `contracts` | <span data-ttu-id="c8e97-360">3</span><span class="sxs-lookup"><span data-stu-id="c8e97-360">3</span></span> | <span data-ttu-id="c8e97-361">0</span><span class="sxs-lookup"><span data-stu-id="c8e97-361">0</span></span> |
| <span data-ttu-id="c8e97-362">POST</span><span class="sxs-lookup"><span data-stu-id="c8e97-362">POST</span></span> | `directoryObjects/getByIds` |  <span data-ttu-id="c8e97-363">3</span><span class="sxs-lookup"><span data-stu-id="c8e97-363">3</span></span> | <span data-ttu-id="c8e97-364">0</span><span class="sxs-lookup"><span data-stu-id="c8e97-364">0</span></span> |
| <span data-ttu-id="c8e97-365">GET</span><span class="sxs-lookup"><span data-stu-id="c8e97-365">GET</span></span> | `domains/{id}/domainNameReferences` | <span data-ttu-id="c8e97-366">4</span><span class="sxs-lookup"><span data-stu-id="c8e97-366">4</span></span> | <span data-ttu-id="c8e97-367">0</span><span class="sxs-lookup"><span data-stu-id="c8e97-367">0</span></span> |
| <span data-ttu-id="c8e97-368">POST</span><span class="sxs-lookup"><span data-stu-id="c8e97-368">POST</span></span> | `getObjectsById` | <span data-ttu-id="c8e97-369">3</span><span class="sxs-lookup"><span data-stu-id="c8e97-369">3</span></span> | <span data-ttu-id="c8e97-370">0</span><span class="sxs-lookup"><span data-stu-id="c8e97-370">0</span></span> |
| <span data-ttu-id="c8e97-371">GET</span><span class="sxs-lookup"><span data-stu-id="c8e97-371">GET</span></span> | `groups/{id}/members` | <span data-ttu-id="c8e97-372">3</span><span class="sxs-lookup"><span data-stu-id="c8e97-372">3</span></span> | <span data-ttu-id="c8e97-373">0</span><span class="sxs-lookup"><span data-stu-id="c8e97-373">0</span></span> |
| <span data-ttu-id="c8e97-374">GET</span><span class="sxs-lookup"><span data-stu-id="c8e97-374">GET</span></span> | `groups/{id}/transitiveMembers` | <span data-ttu-id="c8e97-375">5</span><span class="sxs-lookup"><span data-stu-id="c8e97-375">5</span></span> | <span data-ttu-id="c8e97-376">0</span><span class="sxs-lookup"><span data-stu-id="c8e97-376">0</span></span> |
| <span data-ttu-id="c8e97-377">POST</span><span class="sxs-lookup"><span data-stu-id="c8e97-377">POST</span></span> | `isMemberOf` | <span data-ttu-id="c8e97-378">4</span><span class="sxs-lookup"><span data-stu-id="c8e97-378">4</span></span> | <span data-ttu-id="c8e97-379">0</span><span class="sxs-lookup"><span data-stu-id="c8e97-379">0</span></span> |
| <span data-ttu-id="c8e97-380">POST</span><span class="sxs-lookup"><span data-stu-id="c8e97-380">POST</span></span> | `me/checkMemberGroups` | <span data-ttu-id="c8e97-381">4</span><span class="sxs-lookup"><span data-stu-id="c8e97-381">4</span></span> | <span data-ttu-id="c8e97-382">0</span><span class="sxs-lookup"><span data-stu-id="c8e97-382">0</span></span> |
| <span data-ttu-id="c8e97-383">POST</span><span class="sxs-lookup"><span data-stu-id="c8e97-383">POST</span></span> | `me/checkMemberObjects` | <span data-ttu-id="c8e97-384">4</span><span class="sxs-lookup"><span data-stu-id="c8e97-384">4</span></span> | <span data-ttu-id="c8e97-385">0</span><span class="sxs-lookup"><span data-stu-id="c8e97-385">0</span></span> |
| <span data-ttu-id="c8e97-386">POST</span><span class="sxs-lookup"><span data-stu-id="c8e97-386">POST</span></span> | `me/getMemberGroups` | <span data-ttu-id="c8e97-387">2</span><span class="sxs-lookup"><span data-stu-id="c8e97-387">2</span></span> | <span data-ttu-id="c8e97-388">0</span><span class="sxs-lookup"><span data-stu-id="c8e97-388">0</span></span> |
| <span data-ttu-id="c8e97-389">POST</span><span class="sxs-lookup"><span data-stu-id="c8e97-389">POST</span></span> | `me/getMemberObjects` | <span data-ttu-id="c8e97-390">2</span><span class="sxs-lookup"><span data-stu-id="c8e97-390">2</span></span> | <span data-ttu-id="c8e97-391">0</span><span class="sxs-lookup"><span data-stu-id="c8e97-391">0</span></span> |
| <span data-ttu-id="c8e97-392">GET</span><span class="sxs-lookup"><span data-stu-id="c8e97-392">GET</span></span> | `me/licenseDetails` | <span data-ttu-id="c8e97-393">2</span><span class="sxs-lookup"><span data-stu-id="c8e97-393">2</span></span> | <span data-ttu-id="c8e97-394">0</span><span class="sxs-lookup"><span data-stu-id="c8e97-394">0</span></span> |
| <span data-ttu-id="c8e97-395">GET</span><span class="sxs-lookup"><span data-stu-id="c8e97-395">GET</span></span> | `me/memberOf` | <span data-ttu-id="c8e97-396">2</span><span class="sxs-lookup"><span data-stu-id="c8e97-396">2</span></span> | <span data-ttu-id="c8e97-397">0</span><span class="sxs-lookup"><span data-stu-id="c8e97-397">0</span></span> |
| <span data-ttu-id="c8e97-398">GET</span><span class="sxs-lookup"><span data-stu-id="c8e97-398">GET</span></span> | `me/ownedObjects` | <span data-ttu-id="c8e97-399">2</span><span class="sxs-lookup"><span data-stu-id="c8e97-399">2</span></span> | <span data-ttu-id="c8e97-400">0</span><span class="sxs-lookup"><span data-stu-id="c8e97-400">0</span></span> |
| <span data-ttu-id="c8e97-401">GET</span><span class="sxs-lookup"><span data-stu-id="c8e97-401">GET</span></span> | `me/transitiveMemberOf` | <span data-ttu-id="c8e97-402">2</span><span class="sxs-lookup"><span data-stu-id="c8e97-402">2</span></span> | <span data-ttu-id="c8e97-403">0</span><span class="sxs-lookup"><span data-stu-id="c8e97-403">0</span></span> |
| <span data-ttu-id="c8e97-404">GET</span><span class="sxs-lookup"><span data-stu-id="c8e97-404">GET</span></span> | `oauth2PermissionGrants` | <span data-ttu-id="c8e97-405">2</span><span class="sxs-lookup"><span data-stu-id="c8e97-405">2</span></span> | <span data-ttu-id="c8e97-406">0</span><span class="sxs-lookup"><span data-stu-id="c8e97-406">0</span></span> |
| <span data-ttu-id="c8e97-407">GET</span><span class="sxs-lookup"><span data-stu-id="c8e97-407">GET</span></span> | `oauth2PermissionGrants/{id}` | <span data-ttu-id="c8e97-408">2</span><span class="sxs-lookup"><span data-stu-id="c8e97-408">2</span></span> | <span data-ttu-id="c8e97-409">0</span><span class="sxs-lookup"><span data-stu-id="c8e97-409">0</span></span> |
| <span data-ttu-id="c8e97-410">GET</span><span class="sxs-lookup"><span data-stu-id="c8e97-410">GET</span></span> | `servicePrincipals/{id}/appRoleAssignments` | <span data-ttu-id="c8e97-411">2</span><span class="sxs-lookup"><span data-stu-id="c8e97-411">2</span></span> | <span data-ttu-id="c8e97-412">0</span><span class="sxs-lookup"><span data-stu-id="c8e97-412">0</span></span> |
| <span data-ttu-id="c8e97-413">GET</span><span class="sxs-lookup"><span data-stu-id="c8e97-413">GET</span></span> | `subscribedSkus` | <span data-ttu-id="c8e97-414">3</span><span class="sxs-lookup"><span data-stu-id="c8e97-414">3</span></span> | <span data-ttu-id="c8e97-415">0</span><span class="sxs-lookup"><span data-stu-id="c8e97-415">0</span></span> |
| <span data-ttu-id="c8e97-416">GET</span><span class="sxs-lookup"><span data-stu-id="c8e97-416">GET</span></span> | `users` | <span data-ttu-id="c8e97-417">2</span><span class="sxs-lookup"><span data-stu-id="c8e97-417">2</span></span> | <span data-ttu-id="c8e97-418">0</span><span class="sxs-lookup"><span data-stu-id="c8e97-418">0</span></span> |
| <span data-ttu-id="c8e97-419">GET</span><span class="sxs-lookup"><span data-stu-id="c8e97-419">GET</span></span> | <span data-ttu-id="c8e97-420">表中未列出的任何身份路径</span><span class="sxs-lookup"><span data-stu-id="c8e97-420">Any identity path not listed in the table</span></span> | <span data-ttu-id="c8e97-421">1</span><span class="sxs-lookup"><span data-stu-id="c8e97-421">1</span></span> | <span data-ttu-id="c8e97-422">0</span><span class="sxs-lookup"><span data-stu-id="c8e97-422">0</span></span> |
| <span data-ttu-id="c8e97-423">POST</span><span class="sxs-lookup"><span data-stu-id="c8e97-423">POST</span></span> | <span data-ttu-id="c8e97-424">表中未列出的任何身份路径</span><span class="sxs-lookup"><span data-stu-id="c8e97-424">Any identity path not listed in the table</span></span> | <span data-ttu-id="c8e97-425">1</span><span class="sxs-lookup"><span data-stu-id="c8e97-425">1</span></span> | <span data-ttu-id="c8e97-426">1</span><span class="sxs-lookup"><span data-stu-id="c8e97-426">1</span></span> |
| <span data-ttu-id="c8e97-427">PATCH</span><span class="sxs-lookup"><span data-stu-id="c8e97-427">PATCH</span></span> | <span data-ttu-id="c8e97-428">表中未列出的任何身份路径</span><span class="sxs-lookup"><span data-stu-id="c8e97-428">Any identity path not listed in the table</span></span> | <span data-ttu-id="c8e97-429">1</span><span class="sxs-lookup"><span data-stu-id="c8e97-429">1</span></span> | <span data-ttu-id="c8e97-430">1</span><span class="sxs-lookup"><span data-stu-id="c8e97-430">1</span></span> |
| <span data-ttu-id="c8e97-431">PUT</span><span class="sxs-lookup"><span data-stu-id="c8e97-431">PUT</span></span> | <span data-ttu-id="c8e97-432">表中未列出的任何身份路径</span><span class="sxs-lookup"><span data-stu-id="c8e97-432">Any identity path not listed in the table</span></span> | <span data-ttu-id="c8e97-433">1</span><span class="sxs-lookup"><span data-stu-id="c8e97-433">1</span></span> | <span data-ttu-id="c8e97-434">1</span><span class="sxs-lookup"><span data-stu-id="c8e97-434">1</span></span> |
| <span data-ttu-id="c8e97-435">DELETE</span><span class="sxs-lookup"><span data-stu-id="c8e97-435">DELETE</span></span> | <span data-ttu-id="c8e97-436">表中未列出的任何身份路径</span><span class="sxs-lookup"><span data-stu-id="c8e97-436">Any identity path not listed in the table</span></span> | <span data-ttu-id="c8e97-437">1</span><span class="sxs-lookup"><span data-stu-id="c8e97-437">1</span></span> | <span data-ttu-id="c8e97-438">1</span><span class="sxs-lookup"><span data-stu-id="c8e97-438">1</span></span> |

<span data-ttu-id="c8e97-439">影响请求费用的其他因素：</span><span class="sxs-lookup"><span data-stu-id="c8e97-439">Other factors that affect a request cost:</span></span>

- <span data-ttu-id="c8e97-440">使用 `$select` 可将成本降低 1</span><span class="sxs-lookup"><span data-stu-id="c8e97-440">Using `$select` decreases cost by 1</span></span>
- <span data-ttu-id="c8e97-441">使用 `$expand` 可将成本增加 1</span><span class="sxs-lookup"><span data-stu-id="c8e97-441">Using `$expand` increases cost by 1</span></span>
- <span data-ttu-id="c8e97-442">使用值小于 20 的 `$top` 会使成本降低1</span><span class="sxs-lookup"><span data-stu-id="c8e97-442">Using `$top` with a value of less than 20 decreases cost by 1</span></span>

> <span data-ttu-id="c8e97-443">**注意：** 请求费用不能低于 1。</span><span class="sxs-lookup"><span data-stu-id="c8e97-443">**Note:** A request cost can never be lower than 1.</span></span> <span data-ttu-id="c8e97-444">适用于从 `me/` 开始的请求路径的任何请求费用也适用于以 `users/{id | userPrincipalName}/`开头的等效请求。</span><span class="sxs-lookup"><span data-stu-id="c8e97-444">Any request cost that applies to a request path starting with `me/` also applies to equivalent requests starting with `users/{id | userPrincipalName}/`.</span></span>

#### <a name="additional-headers"></a><span data-ttu-id="c8e97-445">附加标题</span><span class="sxs-lookup"><span data-stu-id="c8e97-445">Additional headers</span></span>

##### <a name="request-headers"></a><span data-ttu-id="c8e97-446">请求标头</span><span class="sxs-lookup"><span data-stu-id="c8e97-446">Request headers</span></span>

- <span data-ttu-id="c8e97-447">**x-ms-throttle-priority** - 如果标头不存在或设置为任何其他值，则表示正常请求。</span><span class="sxs-lookup"><span data-stu-id="c8e97-447">**x-ms-throttle-priority** - If the header doesn't exist or is set to any other value, it indicates a normal request.</span></span> <span data-ttu-id="c8e97-448">我们建议将优先级 `high` 用户启动的请求设置优先级。</span><span class="sxs-lookup"><span data-stu-id="c8e97-448">We recommend setting priority to `high` only for the requests initiated by the user.</span></span> <span data-ttu-id="c8e97-449">此标头的值可以是以下值：</span><span class="sxs-lookup"><span data-stu-id="c8e97-449">The values of this header can be the following:</span></span>
  - <span data-ttu-id="c8e97-450">低 - 指示请求的优先级较低。</span><span class="sxs-lookup"><span data-stu-id="c8e97-450">Low - Indicates the request is low priority.</span></span> <span data-ttu-id="c8e97-451">限制此请求不会导致出现用户可见的故障。</span><span class="sxs-lookup"><span data-stu-id="c8e97-451">Throttling this request doesn't cause user-visible failures.</span></span>
  - <span data-ttu-id="c8e97-452">正常 - 如果未提供任何值，则为默认值。</span><span class="sxs-lookup"><span data-stu-id="c8e97-452">Normal - Default if no value is provided.</span></span> <span data-ttu-id="c8e97-453">表示请求是默认优先级。</span><span class="sxs-lookup"><span data-stu-id="c8e97-453">Indicates that the request is default priority.</span></span>
  - <span data-ttu-id="c8e97-454">高 - 表示请求具有高优先级。</span><span class="sxs-lookup"><span data-stu-id="c8e97-454">High - Indicates that the request is high priority.</span></span> <span data-ttu-id="c8e97-455">限制此请求会导致出现用户可见的故障。</span><span class="sxs-lookup"><span data-stu-id="c8e97-455">Throttling this request causes user-visible failures.</span></span>

> <span data-ttu-id="c8e97-456">**注意**：如果限制请求，则首先限制低优先级请求，其次限制正常优先级请求，最后限制高优先级请求。</span><span class="sxs-lookup"><span data-stu-id="c8e97-456">**Note:** Should requests be throttled, low priority requests will be throttled first, normal priority requests second, and high priority requests last.</span></span> <span data-ttu-id="c8e97-457">使用优先级请求标头不会更改限制。</span><span class="sxs-lookup"><span data-stu-id="c8e97-457">Using the priority request header does not change the limits.</span></span>

##### <a name="regular-responses-requests"></a><span data-ttu-id="c8e97-458">正常响应请求</span><span class="sxs-lookup"><span data-stu-id="c8e97-458">Regular responses requests</span></span>

- <span data-ttu-id="c8e97-459">**x-ms-resource-unit** - 指示用于此请求的资源单位。</span><span class="sxs-lookup"><span data-stu-id="c8e97-459">**x-ms-resource-unit** - Indicates the resource unit used for this request.</span></span> <span data-ttu-id="c8e97-460">值为正整数。</span><span class="sxs-lookup"><span data-stu-id="c8e97-460">Values are positive integers.</span></span>
- <span data-ttu-id="c8e97-461">**x-ms-throttle-limit-percentage** - 仅当应用程序消耗了超过其限制的 0.8 时才返回。</span><span class="sxs-lookup"><span data-stu-id="c8e97-461">**x-ms-throttle-limit-percentage** - Returned only when the application consumed more than 0.8 of its limit.</span></span> <span data-ttu-id="c8e97-462">该值的范围是 0.8 到 1.8，是使用限制的百分比。</span><span class="sxs-lookup"><span data-stu-id="c8e97-462">The value ranges from 0.8 to 1.8 and is a percentage of the use of the limit.</span></span> <span data-ttu-id="c8e97-463">调用者可以使用该值设置警报并采取措施。</span><span class="sxs-lookup"><span data-stu-id="c8e97-463">The value can be used by the callers to set up an alert and take action.</span></span>

##### <a name="throttled-responses-requests"></a><span data-ttu-id="c8e97-464">受限制的响应请求</span><span class="sxs-lookup"><span data-stu-id="c8e97-464">Throttled responses requests</span></span>

- <span data-ttu-id="c8e97-465">**x-ms-throttle-scope** - eg.</span><span class="sxs-lookup"><span data-stu-id="c8e97-465">**x-ms-throttle-scope** - eg.</span></span> <span data-ttu-id="c8e97-466">`Tenant_Application/ReadWrite/9a3d526c-b3c1-4479-ba74-197b5c5751ae/0785ef7c-2d7a-4542-b048-95bcab406e0b`（）。</span><span class="sxs-lookup"><span data-stu-id="c8e97-466">`Tenant_Application/ReadWrite/9a3d526c-b3c1-4479-ba74-197b5c5751ae/0785ef7c-2d7a-4542-b048-95bcab406e0b`.</span></span> <span data-ttu-id="c8e97-467">指示采用下列格式 `<Scope>/<Limit>/<ApplicationId>/<TenantId|UserId|ResourceId>` 的限制范围：</span><span class="sxs-lookup"><span data-stu-id="c8e97-467">Indicates the scope of throttling with the following format `<Scope>/<Limit>/<ApplicationId>/<TenantId|UserId|ResourceId>`:</span></span>
  - <span data-ttu-id="c8e97-468">范围：（字符串，必填）</span><span class="sxs-lookup"><span data-stu-id="c8e97-468">Scope: (string, required)</span></span>
    - <span data-ttu-id="c8e97-469">Tenant_Application - 当前应用程序对特定租户的所有请求。</span><span class="sxs-lookup"><span data-stu-id="c8e97-469">Tenant_Application - All requests for a particular tenant for the current application.</span></span>
    - <span data-ttu-id="c8e97-470">租户 - 当前租户的所有请求，与应用程序无关。</span><span class="sxs-lookup"><span data-stu-id="c8e97-470">Tenant - All requests for the current tenant, regardless of the application.</span></span>
    - <span data-ttu-id="c8e97-471">应用程序 - 当前应用程序的所有请求。</span><span class="sxs-lookup"><span data-stu-id="c8e97-471">Application - All requests for the current application.</span></span>
  - <span data-ttu-id="c8e97-472">限制：（字符串、必填）</span><span class="sxs-lookup"><span data-stu-id="c8e97-472">Limit: (string, requied)</span></span>
    - <span data-ttu-id="c8e97-473">读取：读取范围请求 (GET)</span><span class="sxs-lookup"><span data-stu-id="c8e97-473">Read: Read requests for the scope (GET)</span></span>
    - <span data-ttu-id="c8e97-474">写入：写入范围请求 (POST、PATCH、PUT、DELETE...)</span><span class="sxs-lookup"><span data-stu-id="c8e97-474">Write: Write requests for the scope (POST, PATCH, PUT, DELETE...)</span></span>
    - <span data-ttu-id="c8e97-475">ReadWrite：所有范围请求（任何）</span><span class="sxs-lookup"><span data-stu-id="c8e97-475">ReadWrite: All Requests for the scope (any)</span></span>
  - <span data-ttu-id="c8e97-476">ApplicationId （Guid、必填）</span><span class="sxs-lookup"><span data-stu-id="c8e97-476">ApplicationId (Guid, required)</span></span>
  - <span data-ttu-id="c8e97-477">TenantId|UserId|ResourceId: (Guid、必填）</span><span class="sxs-lookup"><span data-stu-id="c8e97-477">TenantId|UserId|ResourceId: (Guid, required)</span></span>
- <span data-ttu-id="c8e97-478">**x-ms-throttle-information** - 指示限制的原因，可以有任何值（字符串）。</span><span class="sxs-lookup"><span data-stu-id="c8e97-478">**x-ms-throttle-information** - Indicates the reason for throttling and can have any value (string).</span></span> <span data-ttu-id="c8e97-479">提供该值是为了进行诊断和故障排除，其中一些示例包括：</span><span class="sxs-lookup"><span data-stu-id="c8e97-479">The value is provided for diagnostics and troubleshooting purposes, some examples include:</span></span>
  - <span data-ttu-id="c8e97-480">CPULimitExceeded - 限制因为超过 cpu 应用的限值。</span><span class="sxs-lookup"><span data-stu-id="c8e97-480">CPULimitExceeded - Throttling is because the limit for cpu allocation is exceeded.</span></span>
  - <span data-ttu-id="c8e97-481">WriteLimitExceeded - 限制因为超过写入限值。</span><span class="sxs-lookup"><span data-stu-id="c8e97-481">WriteLimitExceeded - Throttling is because the write limit is exceeded.</span></span>
  - <span data-ttu-id="c8e97-482">ResourceUnitLimitExceeded - 限制因为超过已分配资源单位的限值。</span><span class="sxs-lookup"><span data-stu-id="c8e97-482">ResourceUnitLimitExceeded - Throttling is because the limit for the allocated resource unit is exceeded.</span></span>

### <a name="information-protection"></a><span data-ttu-id="c8e97-483">信息保护</span><span class="sxs-lookup"><span data-stu-id="c8e97-483">Information protection</span></span>

<span data-ttu-id="c8e97-484">以下限制适用于 `/informationProtection` 上的所有请求。</span><span class="sxs-lookup"><span data-stu-id="c8e97-484">The following limits apply to any request on `/informationProtection`.</span></span>

| <span data-ttu-id="c8e97-485">操作</span><span class="sxs-lookup"><span data-stu-id="c8e97-485">Operation</span></span>                 | <span data-ttu-id="c8e97-486">每个租户的使用限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-486">Limit per tenant</span></span>                                            | <span data-ttu-id="c8e97-487">每个资源（电子邮件、URL、文件）的使用限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-487">Limit per resource (email, URL, file)</span></span>                |
|---------------------------|-------------------------------------------------------------|------------------------------------------------------|
| <span data-ttu-id="c8e97-488">POST</span><span class="sxs-lookup"><span data-stu-id="c8e97-488">POST</span></span>                      | <span data-ttu-id="c8e97-489">每 15 分钟 150 个请求和每 24 小时 10000 个请求</span><span class="sxs-lookup"><span data-stu-id="c8e97-489">150 requests per 15 minutes and 10000 requests per 24 hours</span></span> | <span data-ttu-id="c8e97-490">每 15 分钟 1 个请求和每 24 小时 3 个请求</span><span class="sxs-lookup"><span data-stu-id="c8e97-490">1 request per 15 minutes and 3 requests per 24 hours</span></span> |

<span data-ttu-id="c8e97-491">上述限制适用于下列资源:</span><span class="sxs-lookup"><span data-stu-id="c8e97-491">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="c8e97-492">threatAssessmentRequest、threatAssessmentResult、mailAssessmentRequest、emailFileAssessmentRequest、fileAssessmentRequest、urlAssessmentRequest。</span><span class="sxs-lookup"><span data-stu-id="c8e97-492">threatAssessmentRequest, threatAssessmentResult, mailAssessmentRequest, emailFileAssessmentRequest, fileAssessmentRequest, urlAssessmentRequest.</span></span>

### <a name="identity-protection-and-conditional-access-service-limits"></a><span data-ttu-id="c8e97-493">身份保护和条件访问服务限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-493">Identity protection and conditional access service limits</span></span>

| <span data-ttu-id="c8e97-494">请求类型</span><span class="sxs-lookup"><span data-stu-id="c8e97-494">Request type</span></span> | <span data-ttu-id="c8e97-495">所有应用的每个租户的使用限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-495">Limit per tenant for all apps</span></span> |
| ------------ | ------- |
| <span data-ttu-id="c8e97-496">任何</span><span class="sxs-lookup"><span data-stu-id="c8e97-496">Any</span></span> | <span data-ttu-id="c8e97-497">每秒1个请求</span><span class="sxs-lookup"><span data-stu-id="c8e97-497">1 request per second</span></span> |

<span data-ttu-id="c8e97-498">上述限制适用于下列资源:</span><span class="sxs-lookup"><span data-stu-id="c8e97-498">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="c8e97-499">riskDetection, riskyUser, riskyUserHistoryItem, namedLocation, countryNamedLocation, ipNamedLocation, conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="c8e97-499">riskDetection, riskyUser, riskyUserHistoryItem, namedLocation, countryNamedLocation, ipNamedLocation, conditionalAccessPolicy.</span></span>

> <span data-ttu-id="c8e97-500">**注意：** 上面列出的资源未在 `429 Too Many Requests` 响应上返回 `Retry-After` 标头。</span><span class="sxs-lookup"><span data-stu-id="c8e97-500">**Note:** The resources listed above do not return a `Retry-After` header on `429 Too Many Requests` responses.</span></span>

### <a name="insights-service-limits"></a><span data-ttu-id="c8e97-501">见解服务限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-501">Insights service limits</span></span>

<span data-ttu-id="c8e97-502">以下限制适用于 `me/insights`或`users/{id}/insights` 上的所有请求。</span><span class="sxs-lookup"><span data-stu-id="c8e97-502">The following limits apply to any request on `me/insights` or `users/{id}/insights`.</span></span>

| <span data-ttu-id="c8e97-503">限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-503">Limit</span></span>                                                      | <span data-ttu-id="c8e97-504">适用对象</span><span class="sxs-lookup"><span data-stu-id="c8e97-504">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="c8e97-505">10 分钟内的 10,000 个 API 请求</span><span class="sxs-lookup"><span data-stu-id="c8e97-505">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="c8e97-506">v1.0 和 beta 终结点</span><span class="sxs-lookup"><span data-stu-id="c8e97-506">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="c8e97-507">4 个并发请求</span><span class="sxs-lookup"><span data-stu-id="c8e97-507">4 concurrent requests</span></span>                                      | <span data-ttu-id="c8e97-508">v1.0 和 beta 终结点</span><span class="sxs-lookup"><span data-stu-id="c8e97-508">v1.0 and beta endpoints</span></span>   |

<span data-ttu-id="c8e97-509">上述限制适用于下列资源:</span><span class="sxs-lookup"><span data-stu-id="c8e97-509">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="c8e97-510">people、trending、usedinsight、sharedInsight。</span><span class="sxs-lookup"><span data-stu-id="c8e97-510">people, trending, usedinsight, sharedInsight.</span></span>

### <a name="microsoft-graph-reports-service-limits"></a><span data-ttu-id="c8e97-511">Microsoft Graph 报告的服务限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-511">Microsoft Graph reports service limits</span></span>

<span data-ttu-id="c8e97-512">以下限制适用于 `/reports` 上的所有请求。</span><span class="sxs-lookup"><span data-stu-id="c8e97-512">The following limits apply to any request on `/reports`.</span></span>

| <span data-ttu-id="c8e97-513">操作</span><span class="sxs-lookup"><span data-stu-id="c8e97-513">Operation</span></span>                 | <span data-ttu-id="c8e97-514">每个租户每个应用限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-514">Limit per app per tenant</span></span>     | <span data-ttu-id="c8e97-515">所有应用的每个租户的使用限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-515">Limit per tenant for all apps</span></span> |
|---------------------------|------------------------------|----------------------------|
| <span data-ttu-id="c8e97-516">任何请求（CSV）</span><span class="sxs-lookup"><span data-stu-id="c8e97-516">Any request (CSV)</span></span>         | <span data-ttu-id="c8e97-517">每10分钟14个请求</span><span class="sxs-lookup"><span data-stu-id="c8e97-517">14 requests per 10 minutes</span></span>   | <span data-ttu-id="c8e97-518">每10分钟40个请求</span><span class="sxs-lookup"><span data-stu-id="c8e97-518">40 requests per 10 minutes</span></span> |
| <span data-ttu-id="c8e97-519">任何请求（JSON、beta）</span><span class="sxs-lookup"><span data-stu-id="c8e97-519">Any request (JSON, beta)</span></span>  | <span data-ttu-id="c8e97-520">每10分钟100个请求</span><span class="sxs-lookup"><span data-stu-id="c8e97-520">100 requests per 10 minutes</span></span>  | <span data-ttu-id="c8e97-521">不适用</span><span class="sxs-lookup"><span data-stu-id="c8e97-521">n/a</span></span>                        |

<span data-ttu-id="c8e97-522">上述限制分别适用于每个报表 API。</span><span class="sxs-lookup"><span data-stu-id="c8e97-522">The preceding limits apply individually to each report API.</span></span> <span data-ttu-id="c8e97-523">例如，在 10 分钟内分别有对 Microsoft Teams 用户活动报告 API 的请求及对 Outlook 用户活动报告 API 的请求，将分别被视为 14 个请求中的 1 个请求，而不是 14 个请求中的 2 个请求。</span><span class="sxs-lookup"><span data-stu-id="c8e97-523">For example, a request to the Microsoft Teams user activity report API and a request to the Outlook user activity report API within 10 minutes will count as 1 request out of 14 for each API, not 2 requests out of 14 for both.</span></span>

<span data-ttu-id="c8e97-524">上述限制适用于**报告**资源。</span><span class="sxs-lookup"><span data-stu-id="c8e97-524">The preceding limits apply to the **report** resource.</span></span>  

### <a name="invitation-manager-service-limits"></a><span data-ttu-id="c8e97-525">邀请管理器服务限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-525">Invitation manager service limits</span></span>

<span data-ttu-id="c8e97-526">以下限制适用于 `/invitations` 上的所有请求。</span><span class="sxs-lookup"><span data-stu-id="c8e97-526">The following limits apply to any request on `/invitations`.</span></span>

| <span data-ttu-id="c8e97-527">操作</span><span class="sxs-lookup"><span data-stu-id="c8e97-527">Operation</span></span>                 | <span data-ttu-id="c8e97-528">所有应用的每个租户的使用限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-528">Limit per tenant for all apps</span></span> |
|---------------------------|------------------------------|
| <span data-ttu-id="c8e97-529">任何操作</span><span class="sxs-lookup"><span data-stu-id="c8e97-529">Any operation</span></span>             | <span data-ttu-id="c8e97-530">每 5 秒 150 个请求</span><span class="sxs-lookup"><span data-stu-id="c8e97-530">150 requests per 5 seconds</span></span>   |

### <a name="security-detections-and-incidents-service-limits"></a><span data-ttu-id="c8e97-531">安全检测和事件服务限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-531">Security detections and incidents service limits</span></span>

<span data-ttu-id="c8e97-532">以下限制适用于 `/security` 上的所有请求。</span><span class="sxs-lookup"><span data-stu-id="c8e97-532">The following limits apply to any request on `/security`.</span></span>

| <span data-ttu-id="c8e97-533">操作</span><span class="sxs-lookup"><span data-stu-id="c8e97-533">Operation</span></span>                  | <span data-ttu-id="c8e97-534">每个租户每个应用限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-534">Limit per app per tenant</span></span>     |
|----------------------------|------------------------------|
| <span data-ttu-id="c8e97-535">`alert`、`securityActions`、`secureScore` 上的任何操作</span><span class="sxs-lookup"><span data-stu-id="c8e97-535">Any operation on `alert`, `securityActions`,  `secureScore`</span></span> | <span data-ttu-id="c8e97-536">每分钟 150 个请求</span><span class="sxs-lookup"><span data-stu-id="c8e97-536">150 requests per minute</span></span>      |
| <span data-ttu-id="c8e97-537">`tiIndicator` 上的任何操作</span><span class="sxs-lookup"><span data-stu-id="c8e97-537">Any operation on `tiIndicator`</span></span> | <span data-ttu-id="c8e97-538">每分钟 1000 个请求</span><span class="sxs-lookup"><span data-stu-id="c8e97-538">1000 requests per minute</span></span> |
| <span data-ttu-id="c8e97-539">`secureScore` 或 `secureScorecontrolProfile` 上的任何操作</span><span class="sxs-lookup"><span data-stu-id="c8e97-539">Any operation on `secureScore` or `secureScorecontrolProfile`</span></span> | <span data-ttu-id="c8e97-540">10 分钟内的 10,000 个 API 请求</span><span class="sxs-lookup"><span data-stu-id="c8e97-540">10,000 API requests in a 10 minute period</span></span> |
| <span data-ttu-id="c8e97-541">`secureScore` 或 `secureScorecontrolProfile` 上的任何操作</span><span class="sxs-lookup"><span data-stu-id="c8e97-541">Any operation on `secureScore` or `secureScorecontrolProfile`</span></span> | <span data-ttu-id="c8e97-542">4 个并发请求</span><span class="sxs-lookup"><span data-stu-id="c8e97-542">4 concurrent requests</span></span> |

### <a name="open-and-schema-extensions-service-limits"></a><span data-ttu-id="c8e97-543">开放和架构扩展服务限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-543">Open and schema extensions service limits</span></span>

| <span data-ttu-id="c8e97-544">请求类型</span><span class="sxs-lookup"><span data-stu-id="c8e97-544">Request type</span></span> | <span data-ttu-id="c8e97-545">每个租户每个应用限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-545">Limit per app per tenant</span></span> |
| ------------ | ------------------------ |
| <span data-ttu-id="c8e97-546">任何</span><span class="sxs-lookup"><span data-stu-id="c8e97-546">Any</span></span>          | <span data-ttu-id="c8e97-547">每 10 秒 455 个请求</span><span class="sxs-lookup"><span data-stu-id="c8e97-547">455 requests per 10 seconds</span></span> |

<span data-ttu-id="c8e97-548">上述限制适用于以下资源：openTypeExtension、schemaExtension、administrativeUnit、合同、设备、事件、组、消息、组织、帖子和用户。</span><span class="sxs-lookup"><span data-stu-id="c8e97-548">The preceding limits apply to the following resources: openTypeExtension, schemaExtension, administrativeUnit, contact, device, event, group, message, organization, post, and user.</span></span>

### <a name="files-and-lists-service-limits"></a><span data-ttu-id="c8e97-549">文件和列表服务限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-549">Files and lists service limits</span></span>

<span data-ttu-id="c8e97-550">OneDrive、OneDrive for Business 和 SharePoint Online 的服务限制不可用。</span><span class="sxs-lookup"><span data-stu-id="c8e97-550">Service limits for OneDrive, OneDrive for Business, and SharePoint Online are not available.</span></span> <span data-ttu-id="c8e97-551">有关详细信息，请参阅[为什么不能告诉我确切的限制？](/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online#why-cant-you-just-tell-me-the-exact-throttling-limits)。</span><span class="sxs-lookup"><span data-stu-id="c8e97-551">For more information, see [why can't you just tell me the exact throttling limits?](/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online#why-cant-you-just-tell-me-the-exact-throttling-limits).</span></span>

<span data-ttu-id="c8e97-552">上述信息适用于以下资源：</span><span class="sxs-lookup"><span data-stu-id="c8e97-552">The preceding information applies to the following resources:</span></span>  
<span data-ttu-id="c8e97-553">baseItem、baseItemVersion、columnDefinition、columnLink、contentType、drive、driveItem、driveItemVersion、fieldValueSet、itemActivity、itemActivityStat、itemAnalytics、list、listItem、listItemVersion、permission、sharedDriveItem、site 和 thumbnailSet。</span><span class="sxs-lookup"><span data-stu-id="c8e97-553">baseItem, baseItemVersion, columnDefinition, columnLink, contentType, drive, driveItem, driveItemVersion, fieldValueSet, itemActivity, itemActivityStat, itemAnalytics, list, listItem, listItemVersion, permission, sharedDriveItem, site, and thumbnailSet.</span></span>

### <a name="tasks-and-plans-service-limits"></a><span data-ttu-id="c8e97-554">任务和计划服务限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-554">Tasks and plans service limits</span></span>

<span data-ttu-id="c8e97-555">Planner 的服务限制不可用。</span><span class="sxs-lookup"><span data-stu-id="c8e97-555">Service limits for Planner are not available.</span></span>

<span data-ttu-id="c8e97-556">上述信息适用于以下资源：</span><span class="sxs-lookup"><span data-stu-id="c8e97-556">The preceding information applies to the following resources:</span></span>  
<span data-ttu-id="c8e97-557">planner、plannerAssignedToTaskBoardTaskFormat、plannerBucket、plannerBucketTaskBoardTaskFormat、plannerGroup、plannerPlan、plannerPlanDetails、plannerProgressTaskBoardTaskFormat、plannerTask、plannerTaskDetails 和 plannerUser。</span><span class="sxs-lookup"><span data-stu-id="c8e97-557">planner, plannerAssignedToTaskBoardTaskFormat, plannerBucket, plannerBucketTaskBoardTaskFormat, plannerGroup, plannerPlan, plannerPlanDetails, plannerProgressTaskBoardTaskFormat, plannerTask, plannerTaskDetails, and plannerUser.</span></span>

### <a name="identity-and-access-data-policy-operation-service-limits"></a><span data-ttu-id="c8e97-558">身份和访问数据策略操作服务限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-558">Identity and access data policy operation service limits</span></span>

| <span data-ttu-id="c8e97-559">请求类型</span><span class="sxs-lookup"><span data-stu-id="c8e97-559">Request type</span></span> | <span data-ttu-id="c8e97-560">每个租户的使用限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-560">Limit per tenant</span></span> |
| ------------ | ---------------- |
| <span data-ttu-id="c8e97-561">发布于 `exportPersonalData`</span><span class="sxs-lookup"><span data-stu-id="c8e97-561">POST on `exportPersonalData`</span></span> | <span data-ttu-id="c8e97-562">每天 1000 个针对任何主题的请求，每个主题每天 100 个请求</span><span class="sxs-lookup"><span data-stu-id="c8e97-562">1000 requests per day for any subject and 100 per subject per day</span></span> |
| <span data-ttu-id="c8e97-563">任何其他请求</span><span class="sxs-lookup"><span data-stu-id="c8e97-563">Any other request</span></span> | <span data-ttu-id="c8e97-564">每分钟 10000 个请求</span><span class="sxs-lookup"><span data-stu-id="c8e97-564">10000 requests per hour</span></span> |

<span data-ttu-id="c8e97-565">上述限制适用于下列资源：dataPolicyOperation。</span><span class="sxs-lookup"><span data-stu-id="c8e97-565">The preceding limits apply to the following resources: dataPolicyOperation.</span></span>

> <span data-ttu-id="c8e97-566">**注意：** 上面列出的资源未在 `429 Too Many Requests` 响应上返回 `Retry-After` 标头。</span><span class="sxs-lookup"><span data-stu-id="c8e97-566">**Note:** The resources listed above do not return a `Retry-After` header on `429 Too Many Requests` responses.</span></span>

<!-- { "blockType": "throttlinggenstart" } -->
### <a name="education-service-limits"></a><span data-ttu-id="c8e97-567">教育版服务限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-567">Education service limits</span></span>

[!INCLUDE [Education rostering APIS throttling documentation](../includes/throttling-education-rostering-apis.md)]

### <a name="excel-service-limits"></a><span data-ttu-id="c8e97-568">Excel 服务限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-568">Excel service limits</span></span>

[!INCLUDE [Excel throttling documentation](../includes/throttling-excel.md)]

### <a name="identity-and-access-audit-logs-service-limits"></a><span data-ttu-id="c8e97-569">标识和访问审核日志的服务限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-569">Identity and access audit logs service limits</span></span>

[!INCLUDE [Identity and access audit logs throttling documentation](../includes/throttling-Identity-and-access-audit-logs.md)]

### <a name="identity-providers-service-limits"></a><span data-ttu-id="c8e97-570">身份提供程序的服务限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-570">Identity providers service limits</span></span>

[!INCLUDE [CPIM throttling documentation](../includes/throttling-cpim.md)]

### <a name="intune-service-limits"></a><span data-ttu-id="c8e97-571">Intune服务限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-571">Intune service limits</span></span>

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

### <a name="skype-service-limits"></a><span data-ttu-id="c8e97-572">Skype 服务限制</span><span class="sxs-lookup"><span data-stu-id="c8e97-572">Skype service limits</span></span>

[!INCLUDE [Skype calling throttling documentation](../includes/throttling-skype-calling.md)]

### <a name="subscription-service-limits"></a><span data-ttu-id="c8e97-573">订阅服务</span><span class="sxs-lookup"><span data-stu-id="c8e97-573">Subscription service limits</span></span>

[!INCLUDE [Subscription services throttling documentation](../includes/throttling-subscription-services.md)]

<!-- { "blockType": "throttlinggenend" } -->
