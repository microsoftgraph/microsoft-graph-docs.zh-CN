---
title: Microsoft Graph 限制指南
description: 限制可调节并发调用服务的数量，以防止资源的过度使用。Microsoft Graph 旨在用于处理大量的请求。如果出现过多请求，限制将有助于保持 Microsoft Graph 的最佳性能和服务的可靠性。
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: d33ac4612f4fe3934c53235360626dac1393ab21
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44215785"
---
# <a name="microsoft-graph-throttling-guidance"></a><span data-ttu-id="a22e5-105">Microsoft Graph 限制指南</span><span class="sxs-lookup"><span data-stu-id="a22e5-105">Microsoft Graph throttling guidance</span></span>

<span data-ttu-id="a22e5-p102">限制可调节并发调用服务的数量，以防止资源的过度使用。Microsoft Graph 旨在用于处理大量的请求。如果出现过多请求，限制将有助于保持 Microsoft Graph 的最佳性能和服务的可靠性。</span><span class="sxs-lookup"><span data-stu-id="a22e5-p102">Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span></span>

<span data-ttu-id="a22e5-p103">根据该方案，执行的限制会有所不同。例如，如果你正在执行大量的写入操作，限制的可能性会比仅执行读取时要高。</span><span class="sxs-lookup"><span data-stu-id="a22e5-p103">Throttling limits vary based on the scenario. For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span></span>

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a><span data-ttu-id="a22e5-111">在限制时，会发生什么情况？</span><span class="sxs-lookup"><span data-stu-id="a22e5-111">What happens when throttling occurs?</span></span>
<!-- markdownlint-enable MD026 -->

<span data-ttu-id="a22e5-p104">超出限制阈值后，Microsoft Graph 会在一段时间内限制来自该客户端的任何进一步的请求。发生限制时，Microsoft Graph 将返回 HTTP 状态代码 429（请求过多），同时请求失败。在失败的请求的响应标头中返回建议的等待时间。限制行为取决于请求的类型和数量。例如，如果你有大量的请求，则所有请求类型受限。阈值限制根据请求类型而有所不同。因此，你可能会遇到这样一种场景，在场景中，写入被限制，但仍允许读取。</span><span class="sxs-lookup"><span data-stu-id="a22e5-p104">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time. When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail. A suggested wait time is returned in the response header of the failed request. Throttling behavior can depend on the type and number of requests. For example, if you have a high volume of requests, all requests types are throttled. Threshold limits vary based on the request type. Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span>

## <a name="common-throttling-scenarios"></a><span data-ttu-id="a22e5-119">常见的限制场景</span><span class="sxs-lookup"><span data-stu-id="a22e5-119">Common throttling scenarios</span></span>

<span data-ttu-id="a22e5-120">客户端受限的最常见原因包括：</span><span class="sxs-lookup"><span data-stu-id="a22e5-120">The most common causes of throttling of clients include:</span></span>

- <span data-ttu-id="a22e5-121">来自租户中所有应用程序的请求太多。</span><span class="sxs-lookup"><span data-stu-id="a22e5-121">A large number of requests across all applications in a tenant.</span></span>
- <span data-ttu-id="a22e5-122">来自所有租户中特定应用程序的请求太多。</span><span class="sxs-lookup"><span data-stu-id="a22e5-122">A large number of requests from a particular application across all tenants.</span></span>

## <a name="best-practices-to-handle-throttling"></a><span data-ttu-id="a22e5-123">处理限制的最佳实践</span><span class="sxs-lookup"><span data-stu-id="a22e5-123">Best practices to handle throttling</span></span>

<span data-ttu-id="a22e5-124">以下是处理限制的最佳做法：</span><span class="sxs-lookup"><span data-stu-id="a22e5-124">The following are best practices for handling throttling:</span></span>

- <span data-ttu-id="a22e5-125">减少每个请求的操作数量。</span><span class="sxs-lookup"><span data-stu-id="a22e5-125">Reduce the number of operations per request.</span></span>
- <span data-ttu-id="a22e5-126">减少调用频率。</span><span class="sxs-lookup"><span data-stu-id="a22e5-126">Reduce the frequency of calls.</span></span>
- <span data-ttu-id="a22e5-127">不要立即重试，因为所有请求都会计入使用限制。</span><span class="sxs-lookup"><span data-stu-id="a22e5-127">Avoid immediate retries, because all requests accrue against your usage limits.</span></span>

<span data-ttu-id="a22e5-p105">进行错误处理时，使用 HTTP 错误代码 429 检测限制。失败的响应包括 `Retry-After` 响应标头。使用 `Retry-After` 延迟回退请求是从限制中恢复的最快速的方式，因为 Microsoft Graph 会在客户端受限时继续记录资源使用状况。</span><span class="sxs-lookup"><span data-stu-id="a22e5-p105">When you implement error handling, use the HTTP error code 429 to detect throttling. The failed response includes the `Retry-After` response header. Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span></span>

1. <span data-ttu-id="a22e5-131">等待 `Retry-After` 标头中指定的秒数。</span><span class="sxs-lookup"><span data-stu-id="a22e5-131">Wait the number of seconds specified in the `Retry-After` header.</span></span>
2. <span data-ttu-id="a22e5-132">请重试请求。</span><span class="sxs-lookup"><span data-stu-id="a22e5-132">Retry the request.</span></span>
3. <span data-ttu-id="a22e5-p106">如果请求再次失败，并显示 429 错误代码，则表示你仍然受限。继续使用建议的 `Retry-After` 延迟并重试请求直到成功。</span><span class="sxs-lookup"><span data-stu-id="a22e5-p106">If the request fails again with a 429 error code, you are still being throttled. Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span></span>

<span data-ttu-id="a22e5-135">下列资源目前提供 `Retry-After` 标头：</span><span class="sxs-lookup"><span data-stu-id="a22e5-135">The following resources currently provide a `Retry-After` header:</span></span>

- [<span data-ttu-id="a22e5-136">用户</span><span class="sxs-lookup"><span data-stu-id="a22e5-136">User</span></span>](/graph/api/resources/user?view=graph-rest-1.0)
- [<span data-ttu-id="a22e5-137">照片</span><span class="sxs-lookup"><span data-stu-id="a22e5-137">Photo</span></span>](/graph/api/resources/profilephoto?view=graph-rest-1.0)
- [<span data-ttu-id="a22e5-138">邮件</span><span class="sxs-lookup"><span data-stu-id="a22e5-138">Mail</span></span>](/graph/api/resources/message?view=graph-rest-1.0)
- [<span data-ttu-id="a22e5-139">日历（用户和组）</span><span class="sxs-lookup"><span data-stu-id="a22e5-139">Calendar (users and groups)</span></span>](/graph/api/resources/event?view=graph-rest-1.0)
- [<span data-ttu-id="a22e5-140">联系人</span><span class="sxs-lookup"><span data-stu-id="a22e5-140">Contact</span></span>](/graph/api/resources/contact?view=graph-rest-1.0)
- [<span data-ttu-id="a22e5-141">附件</span><span class="sxs-lookup"><span data-stu-id="a22e5-141">Attachment</span></span>](/graph/api/resources/attachment?view=graph-rest-1.0)
- [<span data-ttu-id="a22e5-142">组对话</span><span class="sxs-lookup"><span data-stu-id="a22e5-142">Group conversations</span></span>](/graph/api/resources/conversation?view=graph-rest-1.0)
- [<span data-ttu-id="a22e5-143">人员和社交活动</span><span class="sxs-lookup"><span data-stu-id="a22e5-143">People and social</span></span>](/graph/api/resources/social-overview?view=graph-rest-beta)
- [<span data-ttu-id="a22e5-144">Drive (OneDrive)</span><span class="sxs-lookup"><span data-stu-id="a22e5-144">Drive (OneDrive)</span></span>](/graph/api/resources/drive?view=graph-rest-1.0)
- [<span data-ttu-id="a22e5-145">外部项（Microsoft 搜索）</span><span class="sxs-lookup"><span data-stu-id="a22e5-145">External item (Microsoft Search)</span></span>](/graph/api/resources/externalitem?view=graph-rest-beta)

<span data-ttu-id="a22e5-146">有关 Microsoft 云限制的更广泛讨论，请参阅[限制模式](https://docs.microsoft.com/azure/architecture/patterns/throttling)。</span><span class="sxs-lookup"><span data-stu-id="a22e5-146">For a broader discussion of throttling on the Microsoft Cloud, see [Throttling Pattern](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span></span>

> [!NOTE]
> <span data-ttu-id="a22e5-147">如果响应未提供 `Retry-After` 标头，我们建议实施指数退避重试策略。</span><span class="sxs-lookup"><span data-stu-id="a22e5-147">If no `Retry-After` header is provided by the response, we recommend implementing an exponential backoff retry policy.</span></span> <span data-ttu-id="a22e5-148">构建大型应用程序时，还可以实现[更高级的模式](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency)。</span><span class="sxs-lookup"><span data-stu-id="a22e5-148">You can also implement [more advanced patterns](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) when building large-scale applications.</span></span>
>
> <span data-ttu-id="a22e5-149">Microsoft Graph SDK 已实施依赖于 `Retry-After` 标头或默认为指数退避重试策略的处理程序。</span><span class="sxs-lookup"><span data-stu-id="a22e5-149">Microsoft Graph SDKs already implement handlers that rely on the `Retry-After` header or default to an exponential backoff retry policy.</span></span>

## <a name="best-practices-to-avoid-throttling"></a><span data-ttu-id="a22e5-150">避免限制的最佳做法</span><span class="sxs-lookup"><span data-stu-id="a22e5-150">Best practices to avoid throttling</span></span>

<span data-ttu-id="a22e5-151">如持续轮询资源以检查更新以及定期扫描资源集合以检查新资源或已删除资源之类的编程模式，更有可能导致应用程序受到限制并降低整体性能。</span><span class="sxs-lookup"><span data-stu-id="a22e5-151">Programming patterns like continuously polling a resource to check for updates and regularly scanning resource collections to check for new or deleted resources are more likely to lead to applications being throttled and degrade overall performances.</span></span> <span data-ttu-id="a22e5-152">如果可用，改为使用[更改跟踪](delta-query-overview.md)并[更改通知](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="a22e5-152">You should instead leverage [change tracking](delta-query-overview.md) and [change notifications](webhooks.md) when available.</span></span>

>[!NOTE]
><span data-ttu-id="a22e5-153">[大规模发现文件和检测更改的最佳做法](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online)详细介绍最佳做法。</span><span class="sxs-lookup"><span data-stu-id="a22e5-153">[Best practices for discovering files and detecting changes at scale](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online) describes best practices in details.</span></span>

## <a name="service-specific-limits"></a><span data-ttu-id="a22e5-154">服务特定限制</span><span class="sxs-lookup"><span data-stu-id="a22e5-154">Service-specific limits</span></span>

<span data-ttu-id="a22e5-155">借助 Microsoft Graph，用户可访问[多个服务](overview-major-services.md)中的数据，如 Outlook 或 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="a22e5-155">Microsoft Graph allows you to access data in [multiple services](overview-major-services.md), such as Outlook or Azure Active Directory.</span></span> <span data-ttu-id="a22e5-156">这些服务实施自己的限制，这些限制会影响使用 Microsoft Graph 访问它们的应用程序。</span><span class="sxs-lookup"><span data-stu-id="a22e5-156">These services impose their own throttling limits that affect applications that use Microsoft Graph to access them.</span></span>

> [!NOTE]
> <span data-ttu-id="a22e5-157">此处所述的具体限制可能会发生更改。</span><span class="sxs-lookup"><span data-stu-id="a22e5-157">The specific limits described here are subject to change.</span></span>

### <a name="outlook-service-limits"></a><span data-ttu-id="a22e5-158">Outlook 服务限制</span><span class="sxs-lookup"><span data-stu-id="a22e5-158">Outlook service limits</span></span>

<span data-ttu-id="a22e5-159">将评估每个应用 ID 和邮箱组合的 Outlook 服务限制。</span><span class="sxs-lookup"><span data-stu-id="a22e5-159">Outlook service limits are evaluated for each app ID and mailbox combination.</span></span> <span data-ttu-id="a22e5-160">换言之，上述限制适用于访问特定邮箱（用户或组）的特定应用。</span><span class="sxs-lookup"><span data-stu-id="a22e5-160">In other words, the limits described apply to a specific app accessing a specific mailbox (user or group).</span></span> <span data-ttu-id="a22e5-161">如果一个邮箱的应用程序超过限制，不会影响访问另一个邮箱的功能。</span><span class="sxs-lookup"><span data-stu-id="a22e5-161">If an application exceeds the limit in one mailbox, it does not affect the ability to access another mailbox.</span></span>

| <span data-ttu-id="a22e5-162">限制</span><span class="sxs-lookup"><span data-stu-id="a22e5-162">Limit</span></span>                                                      | <span data-ttu-id="a22e5-163">适用对象</span><span class="sxs-lookup"><span data-stu-id="a22e5-163">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="a22e5-164">10 分钟内的 10,000 个 API 请求</span><span class="sxs-lookup"><span data-stu-id="a22e5-164">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="a22e5-165">v1.0 和 beta 终结点</span><span class="sxs-lookup"><span data-stu-id="a22e5-165">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="a22e5-166">4 个并发请求</span><span class="sxs-lookup"><span data-stu-id="a22e5-166">4 concurrent requests</span></span>                                      | <span data-ttu-id="a22e5-167">Beta 终结点</span><span class="sxs-lookup"><span data-stu-id="a22e5-167">Beta endpoint</span></span>   |
| <span data-ttu-id="a22e5-168">30 秒内的 15 兆位上传（PATCH、POST、PUT）</span><span class="sxs-lookup"><span data-stu-id="a22e5-168">15 megabit upload (PATCH, POST, PUT) in a 30 second period</span></span> | <span data-ttu-id="a22e5-169">Beta 终结点</span><span class="sxs-lookup"><span data-stu-id="a22e5-169">Beta endpoint</span></span>   |

#### <a name="outlook-service-resources"></a><span data-ttu-id="a22e5-170">Outlook 服务资源</span><span class="sxs-lookup"><span data-stu-id="a22e5-170">Outlook service resources</span></span>

<span data-ttu-id="a22e5-171">Outlook 服务提供以下资源。</span><span class="sxs-lookup"><span data-stu-id="a22e5-171">The following resources are provided by the Outlook service.</span></span>

##### <a name="calendar-api-resources"></a><span data-ttu-id="a22e5-172">日历 API 资源</span><span class="sxs-lookup"><span data-stu-id="a22e5-172">Calendar API resources</span></span>

- [<span data-ttu-id="a22e5-173">event</span><span class="sxs-lookup"><span data-stu-id="a22e5-173">event</span></span>](/graph/api/resources/event)
- [<span data-ttu-id="a22e5-174">eventMessage</span><span class="sxs-lookup"><span data-stu-id="a22e5-174">eventMessage</span></span>](/graph/api/resources/eventmessage)
- [<span data-ttu-id="a22e5-175">calendar</span><span class="sxs-lookup"><span data-stu-id="a22e5-175">calendar</span></span>](/graph/api/resources/calendar)
- [<span data-ttu-id="a22e5-176">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="a22e5-176">calendarGroup</span></span>](/graph/api/resources/calendargroup)
- [<span data-ttu-id="a22e5-177">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="a22e5-177">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="a22e5-178">attachment</span><span class="sxs-lookup"><span data-stu-id="a22e5-178">attachment</span></span>](/graph/api/resources/attachment)
- [<span data-ttu-id="a22e5-179">place（预览）</span><span class="sxs-lookup"><span data-stu-id="a22e5-179">place (preview)</span></span>](/graph/api/resources/place)

##### <a name="mail-api-resources"></a><span data-ttu-id="a22e5-180">邮件 API 资源</span><span class="sxs-lookup"><span data-stu-id="a22e5-180">Mail API resources</span></span>

- [<span data-ttu-id="a22e5-181">message</span><span class="sxs-lookup"><span data-stu-id="a22e5-181">message</span></span>](/graph/api/resources/message)
- [<span data-ttu-id="a22e5-182">mailFolder</span><span class="sxs-lookup"><span data-stu-id="a22e5-182">mailFolder</span></span>](/graph/api/resources/mailfolder)
- [<span data-ttu-id="a22e5-183">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="a22e5-183">mailSearchFolder</span></span>](/graph/api/resources/mailsearchfolder)
- [<span data-ttu-id="a22e5-184">messageRule</span><span class="sxs-lookup"><span data-stu-id="a22e5-184">messageRule</span></span>](/graph/api/resources/messagerule)
- [<span data-ttu-id="a22e5-185">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="a22e5-185">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="a22e5-186">attachment</span><span class="sxs-lookup"><span data-stu-id="a22e5-186">attachment</span></span>](/graph/api/resources/attachment)

##### <a name="personal-contacts-api-resources"></a><span data-ttu-id="a22e5-187">个人联系人 API 资源</span><span class="sxs-lookup"><span data-stu-id="a22e5-187">Personal contacts API resources</span></span>

- [<span data-ttu-id="a22e5-188">contact</span><span class="sxs-lookup"><span data-stu-id="a22e5-188">contact</span></span>](/graph/api/resources/contact)
- [<span data-ttu-id="a22e5-189">contactFolder</span><span class="sxs-lookup"><span data-stu-id="a22e5-189">contactFolder</span></span>](/graph/api/resources/contactfolder)
- [<span data-ttu-id="a22e5-190">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="a22e5-190">outlookCategory</span></span>](/graph/api/resources/outlookcategory)

##### <a name="social-and-workplace-intelligence-resources"></a><span data-ttu-id="a22e5-191">社交和工作区智能资源</span><span class="sxs-lookup"><span data-stu-id="a22e5-191">Social and workplace intelligence resources</span></span>

- [<span data-ttu-id="a22e5-192">person</span><span class="sxs-lookup"><span data-stu-id="a22e5-192">person</span></span>](/graph/api/resources/person)

##### <a name="to-do-tasks-api-preview-resources"></a><span data-ttu-id="a22e5-193">待办任务 API（预览）资源</span><span class="sxs-lookup"><span data-stu-id="a22e5-193">To-do tasks API (preview) resources</span></span>

- [<span data-ttu-id="a22e5-194">outlookTask</span><span class="sxs-lookup"><span data-stu-id="a22e5-194">outlookTask</span></span>](/graph/api/resources/outlooktask)
- [<span data-ttu-id="a22e5-195">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="a22e5-195">outlookTaskFolder</span></span>](/graph/api/resources/outlooktaskfolder)
- [<span data-ttu-id="a22e5-196">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="a22e5-196">outlookTaskGroup</span></span>](/graph/api/resources/outlooktaskgroup)
- [<span data-ttu-id="a22e5-197">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="a22e5-197">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="a22e5-198">attachment</span><span class="sxs-lookup"><span data-stu-id="a22e5-198">attachment</span></span>](/graph/api/resources/attachment)

### <a name="microsoft-teams-service-limits"></a><span data-ttu-id="a22e5-199">Microsoft Teams 服务限制</span><span class="sxs-lookup"><span data-stu-id="a22e5-199">Microsoft Teams service limits</span></span>

<span data-ttu-id="a22e5-200">限制表示为每秒请求数 (rps)。</span><span class="sxs-lookup"><span data-stu-id="a22e5-200">Limits are expressed as requests per second (rps).</span></span>

| <span data-ttu-id="a22e5-201">Teams 请求类型</span><span class="sxs-lookup"><span data-stu-id="a22e5-201">Teams request type</span></span>                                   | <span data-ttu-id="a22e5-202">每个租户每个应用限制</span><span class="sxs-lookup"><span data-stu-id="a22e5-202">Limit per app per tenant</span></span>        | <span data-ttu-id="a22e5-203">所有租户中的每个应用限制</span><span class="sxs-lookup"><span data-stu-id="a22e5-203">Limit per app across all tenants</span></span>      |
|------------------------------------------------------|---------------------------------|------------|
| <span data-ttu-id="a22e5-204">Microsoft Teams 的任何图形 API 调用</span><span class="sxs-lookup"><span data-stu-id="a22e5-204">Any Graph API calls for Microsoft Teams</span></span>              | <span data-ttu-id="a22e5-205">每 10 秒 15000 个请求</span><span class="sxs-lookup"><span data-stu-id="a22e5-205">15000 requests every 10 seconds</span></span> | <span data-ttu-id="a22e5-206">不适用</span><span class="sxs-lookup"><span data-stu-id="a22e5-206">n/a</span></span> |
| <span data-ttu-id="a22e5-207">GET team, channel, tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="a22e5-207">GET team, channel, tab, installedApps, appCatalogs</span></span>   | <span data-ttu-id="a22e5-208">60 rps</span><span class="sxs-lookup"><span data-stu-id="a22e5-208">60 rps</span></span>                          | <span data-ttu-id="a22e5-209">600 rps</span><span class="sxs-lookup"><span data-stu-id="a22e5-209">600 rps</span></span> |
| <span data-ttu-id="a22e5-210">POST/PUT channel, tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="a22e5-210">POST/PUT channel, tab, installedApps, appCatalogs</span></span>    |  <span data-ttu-id="a22e5-211">30 rps</span><span class="sxs-lookup"><span data-stu-id="a22e5-211">30 rps</span></span>                         | <span data-ttu-id="a22e5-212">300 rps</span><span class="sxs-lookup"><span data-stu-id="a22e5-212">300 rps</span></span>  |
| <span data-ttu-id="a22e5-213">PATCH team, channel, tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="a22e5-213">PATCH team, channel, tab, installedApps, appCatalogs</span></span> |  <span data-ttu-id="a22e5-214">30 rps</span><span class="sxs-lookup"><span data-stu-id="a22e5-214">30 rps</span></span>                         | <span data-ttu-id="a22e5-215">300 rps</span><span class="sxs-lookup"><span data-stu-id="a22e5-215">300 rps</span></span>  |
| <span data-ttu-id="a22e5-216">DELETE channel, tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="a22e5-216">DELETE channel, tab, installedApps, appCatalogs</span></span>      |  <span data-ttu-id="a22e5-217">15 rps</span><span class="sxs-lookup"><span data-stu-id="a22e5-217">15 rps</span></span>                         | <span data-ttu-id="a22e5-218">150 rps</span><span class="sxs-lookup"><span data-stu-id="a22e5-218">150 rps</span></span>  |
| <span data-ttu-id="a22e5-219">GET /teams/```{team-id}```, joinedTeams</span><span class="sxs-lookup"><span data-stu-id="a22e5-219">GET /teams/```{team-id}```, joinedTeams</span></span>              |  <span data-ttu-id="a22e5-220">30 rps</span><span class="sxs-lookup"><span data-stu-id="a22e5-220">30 rps</span></span>                         | <span data-ttu-id="a22e5-221">300 rps</span><span class="sxs-lookup"><span data-stu-id="a22e5-221">300 rps</span></span>  |
| <span data-ttu-id="a22e5-222">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, clone</span><span class="sxs-lookup"><span data-stu-id="a22e5-222">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, clone</span></span> | <span data-ttu-id="a22e5-223">6 rps</span><span class="sxs-lookup"><span data-stu-id="a22e5-223">6 rps</span></span> | <span data-ttu-id="a22e5-224">150 rps</span><span class="sxs-lookup"><span data-stu-id="a22e5-224">150 rps</span></span>  | 
| <span data-ttu-id="a22e5-225">GET channel message</span><span class="sxs-lookup"><span data-stu-id="a22e5-225">GET channel message</span></span>  | <span data-ttu-id="a22e5-226">5 rps</span><span class="sxs-lookup"><span data-stu-id="a22e5-226">5 rps</span></span> | <span data-ttu-id="a22e5-227">100 rps</span><span class="sxs-lookup"><span data-stu-id="a22e5-227">100 rps</span></span> |
| <span data-ttu-id="a22e5-228">GET 1:1/group chat message</span><span class="sxs-lookup"><span data-stu-id="a22e5-228">GET 1:1/group chat message</span></span>  | <span data-ttu-id="a22e5-229">3 rps</span><span class="sxs-lookup"><span data-stu-id="a22e5-229">3 rps</span></span> | <span data-ttu-id="a22e5-230">30 rps</span><span class="sxs-lookup"><span data-stu-id="a22e5-230">30 rps</span></span> |
| <span data-ttu-id="a22e5-231">POST channel message</span><span class="sxs-lookup"><span data-stu-id="a22e5-231">POST channel message</span></span> | <span data-ttu-id="a22e5-232">2 rps</span><span class="sxs-lookup"><span data-stu-id="a22e5-232">2 rps</span></span> | <span data-ttu-id="a22e5-233">20 rps</span><span class="sxs-lookup"><span data-stu-id="a22e5-233">20 rps</span></span> |
| <span data-ttu-id="a22e5-234">POST 1:1/group chat message</span><span class="sxs-lookup"><span data-stu-id="a22e5-234">POST 1:1/group chat message</span></span> | <span data-ttu-id="a22e5-235">2 rps</span><span class="sxs-lookup"><span data-stu-id="a22e5-235">2 rps</span></span> | <span data-ttu-id="a22e5-236">20 rps</span><span class="sxs-lookup"><span data-stu-id="a22e5-236">20 rps</span></span> |

<span data-ttu-id="a22e5-237">对于给定团队或频道，每个应用最多可发布 4 个请求。</span><span class="sxs-lookup"><span data-stu-id="a22e5-237">A maximum of 4 requests per second per app can be issued on a given team or channel.</span></span>
<span data-ttu-id="a22e5-238">每个应用每天最多可以将 3000 条消息发送到给定的频道。</span><span class="sxs-lookup"><span data-stu-id="a22e5-238">A maximum of 3000 messages per app per day can be sent to a given channel.</span></span>

<span data-ttu-id="a22e5-239">另请参阅 [Microsoft Teams 限制](/graph/api/resources/teams-api-overview#microsoft-teams-limits)和[投票要求](/graph/api/resources/teams-api-overview#polling-requirements)。</span><span class="sxs-lookup"><span data-stu-id="a22e5-239">See also [Microsoft Teams limits](/graph/api/resources/teams-api-overview#microsoft-teams-limits) and [polling requirements](/graph/api/resources/teams-api-overview#polling-requirements).</span></span>

### <a name="microsoft-graph-change-notifications-subscription-operations"></a><span data-ttu-id="a22e5-240">Microsoft Graph 更改通知订阅操作</span><span class="sxs-lookup"><span data-stu-id="a22e5-240">Microsoft Graph change notifications subscription operations</span></span>

<span data-ttu-id="a22e5-241">以下限制适用于 `/subscriptions` 上的所有请求。</span><span class="sxs-lookup"><span data-stu-id="a22e5-241">The following limits apply to any request on `/subscriptions`.</span></span>

| <span data-ttu-id="a22e5-242">操作</span><span class="sxs-lookup"><span data-stu-id="a22e5-242">Operation</span></span>                 | <span data-ttu-id="a22e5-243">每个租户每个应用限制</span><span class="sxs-lookup"><span data-stu-id="a22e5-243">Limit per app per tenant</span></span>     | <span data-ttu-id="a22e5-244">所有租户中的每个应用限制</span><span class="sxs-lookup"><span data-stu-id="a22e5-244">Limit per app accross all tenants</span></span> |
|---------------------------|------------------------------|-----------------------------------|
| <span data-ttu-id="a22e5-245">POST, PUT, DELETE, PATCH</span><span class="sxs-lookup"><span data-stu-id="a22e5-245">POST, PUT, DELETE, PATCH</span></span>  | <span data-ttu-id="a22e5-246">每 20 秒 1000 个请求</span><span class="sxs-lookup"><span data-stu-id="a22e5-246">1000 requests per 20 seconds</span></span> | <span data-ttu-id="a22e5-247">每 20 秒 2000 个请求</span><span class="sxs-lookup"><span data-stu-id="a22e5-247">2000 requests per 20 seconds</span></span>      |
| <span data-ttu-id="a22e5-248">所有其他 HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="a22e5-248">All other HTTP methods</span></span>    | <span data-ttu-id="a22e5-249">每 20 秒 5000 个请求</span><span class="sxs-lookup"><span data-stu-id="a22e5-249">5000 requests per 20 seconds</span></span> | <span data-ttu-id="a22e5-250">每 20 秒 10000 个请求</span><span class="sxs-lookup"><span data-stu-id="a22e5-250">10000 requests per 20 seconds</span></span>     |
