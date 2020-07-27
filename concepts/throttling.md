---
title: Microsoft Graph 限制指南
description: 限制可调节并发调用服务的数量，以防止资源的过度使用。Microsoft Graph 旨在用于处理大量的请求。如果出现过多请求，限制将有助于保持 Microsoft Graph 的最佳性能和服务的可靠性。
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 8af7a4ce6c303e2ac07e4387ff3dbad38abd735e
ms.sourcegitcommit: 233ac43db0eb5edd46fe944a5515d7dd9abb1298
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2020
ms.locfileid: "45408090"
---
# <a name="microsoft-graph-throttling-guidance"></a><span data-ttu-id="507b4-105">Microsoft Graph 限制指南</span><span class="sxs-lookup"><span data-stu-id="507b4-105">Microsoft Graph throttling guidance</span></span>

<span data-ttu-id="507b4-p102">限制可调节并发调用服务的数量，以防止资源的过度使用。Microsoft Graph 旨在用于处理大量的请求。如果出现过多请求，限制将有助于保持 Microsoft Graph 的最佳性能和服务的可靠性。</span><span class="sxs-lookup"><span data-stu-id="507b4-p102">Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span></span>

<span data-ttu-id="507b4-p103">根据该方案，执行的限制会有所不同。例如，如果你正在执行大量的写入操作，限制的可能性会比仅执行读取时要高。</span><span class="sxs-lookup"><span data-stu-id="507b4-p103">Throttling limits vary based on the scenario. For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span></span>

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a><span data-ttu-id="507b4-111">在限制时，会发生什么情况？</span><span class="sxs-lookup"><span data-stu-id="507b4-111">What happens when throttling occurs?</span></span>
<!-- markdownlint-enable MD026 -->

<span data-ttu-id="507b4-p104">超出限制阈值后，Microsoft Graph 会在一段时间内限制来自该客户端的任何进一步的请求。发生限制时，Microsoft Graph 将返回 HTTP 状态代码 429（请求过多），同时请求失败。在失败的请求的响应标头中返回建议的等待时间。限制行为取决于请求的类型和数量。例如，如果你有大量的请求，则所有请求类型受限。阈值限制根据请求类型而有所不同。因此，你可能会遇到这样一种场景，在场景中，写入被限制，但仍允许读取。</span><span class="sxs-lookup"><span data-stu-id="507b4-p104">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time. When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail. A suggested wait time is returned in the response header of the failed request. Throttling behavior can depend on the type and number of requests. For example, if you have a high volume of requests, all requests types are throttled. Threshold limits vary based on the request type. Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span>

## <a name="common-throttling-scenarios"></a><span data-ttu-id="507b4-119">常见的限制场景</span><span class="sxs-lookup"><span data-stu-id="507b4-119">Common throttling scenarios</span></span>

<span data-ttu-id="507b4-120">客户端受限的最常见原因包括：</span><span class="sxs-lookup"><span data-stu-id="507b4-120">The most common causes of throttling of clients include:</span></span>

- <span data-ttu-id="507b4-121">来自租户中所有应用程序的请求太多。</span><span class="sxs-lookup"><span data-stu-id="507b4-121">A large number of requests across all applications in a tenant.</span></span>
- <span data-ttu-id="507b4-122">来自所有租户中特定应用程序的请求太多。</span><span class="sxs-lookup"><span data-stu-id="507b4-122">A large number of requests from a particular application across all tenants.</span></span>

## <a name="best-practices-to-handle-throttling"></a><span data-ttu-id="507b4-123">处理限制的最佳实践</span><span class="sxs-lookup"><span data-stu-id="507b4-123">Best practices to handle throttling</span></span>

<span data-ttu-id="507b4-124">以下是处理限制的最佳做法：</span><span class="sxs-lookup"><span data-stu-id="507b4-124">The following are best practices for handling throttling:</span></span>

- <span data-ttu-id="507b4-125">减少每个请求的操作数量。</span><span class="sxs-lookup"><span data-stu-id="507b4-125">Reduce the number of operations per request.</span></span>
- <span data-ttu-id="507b4-126">减少调用频率。</span><span class="sxs-lookup"><span data-stu-id="507b4-126">Reduce the frequency of calls.</span></span>
- <span data-ttu-id="507b4-127">不要立即重试，因为所有请求都会计入使用限制。</span><span class="sxs-lookup"><span data-stu-id="507b4-127">Avoid immediate retries, because all requests accrue against your usage limits.</span></span>

<span data-ttu-id="507b4-p105">进行错误处理时，使用 HTTP 错误代码 429 检测限制。失败的响应包括 `Retry-After` 响应标头。使用 `Retry-After` 延迟回退请求是从限制中恢复的最快速的方式，因为 Microsoft Graph 会在客户端受限时继续记录资源使用状况。</span><span class="sxs-lookup"><span data-stu-id="507b4-p105">When you implement error handling, use the HTTP error code 429 to detect throttling. The failed response includes the `Retry-After` response header. Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span></span>

1. <span data-ttu-id="507b4-131">等待 `Retry-After` 标头中指定的秒数。</span><span class="sxs-lookup"><span data-stu-id="507b4-131">Wait the number of seconds specified in the `Retry-After` header.</span></span>
2. <span data-ttu-id="507b4-132">请重试请求。</span><span class="sxs-lookup"><span data-stu-id="507b4-132">Retry the request.</span></span>
3. <span data-ttu-id="507b4-p106">如果请求再次失败，并显示 429 错误代码，则表示你仍然受限。继续使用建议的 `Retry-After` 延迟并重试请求直到成功。</span><span class="sxs-lookup"><span data-stu-id="507b4-p106">If the request fails again with a 429 error code, you are still being throttled. Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span></span>

<span data-ttu-id="507b4-135">下列资源目前提供 `Retry-After` 标头：</span><span class="sxs-lookup"><span data-stu-id="507b4-135">The following resources currently provide a `Retry-After` header:</span></span>

- [<span data-ttu-id="507b4-136">用户</span><span class="sxs-lookup"><span data-stu-id="507b4-136">User</span></span>](/graph/api/resources/user?view=graph-rest-1.0)
- [<span data-ttu-id="507b4-137">照片</span><span class="sxs-lookup"><span data-stu-id="507b4-137">Photo</span></span>](/graph/api/resources/profilephoto?view=graph-rest-1.0)
- [<span data-ttu-id="507b4-138">邮件</span><span class="sxs-lookup"><span data-stu-id="507b4-138">Mail</span></span>](/graph/api/resources/message?view=graph-rest-1.0)
- [<span data-ttu-id="507b4-139">日历（用户和组）</span><span class="sxs-lookup"><span data-stu-id="507b4-139">Calendar (users and groups)</span></span>](/graph/api/resources/event?view=graph-rest-1.0)
- [<span data-ttu-id="507b4-140">联系人</span><span class="sxs-lookup"><span data-stu-id="507b4-140">Contact</span></span>](/graph/api/resources/contact?view=graph-rest-1.0)
- [<span data-ttu-id="507b4-141">附件</span><span class="sxs-lookup"><span data-stu-id="507b4-141">Attachment</span></span>](/graph/api/resources/attachment?view=graph-rest-1.0)
- [<span data-ttu-id="507b4-142">组对话</span><span class="sxs-lookup"><span data-stu-id="507b4-142">Group conversations</span></span>](/graph/api/resources/conversation?view=graph-rest-1.0)
- [<span data-ttu-id="507b4-143">人员和社交活动</span><span class="sxs-lookup"><span data-stu-id="507b4-143">People and social</span></span>](/graph/api/resources/social-overview?view=graph-rest-beta)
- [<span data-ttu-id="507b4-144">Drive (OneDrive)</span><span class="sxs-lookup"><span data-stu-id="507b4-144">Drive (OneDrive)</span></span>](/graph/api/resources/drive?view=graph-rest-1.0)
- [<span data-ttu-id="507b4-145">外部项（Microsoft 搜索）</span><span class="sxs-lookup"><span data-stu-id="507b4-145">External item (Microsoft Search)</span></span>](/graph/api/resources/externalitem?view=graph-rest-beta)
- [<span data-ttu-id="507b4-146">Report</span><span class="sxs-lookup"><span data-stu-id="507b4-146">Report</span></span>](/graph/api/resources/report)
- [<span data-ttu-id="507b4-147">订阅</span><span class="sxs-lookup"><span data-stu-id="507b4-147">Subscription</span></span>](/graph/api/resources/subscription)
- [<span data-ttu-id="507b4-148">威胁评估请求</span><span class="sxs-lookup"><span data-stu-id="507b4-148">Threat assessment request</span></span>](/graph/api/resources/threatassessmentrequest)
- [<span data-ttu-id="507b4-149">邮件评估请求</span><span class="sxs-lookup"><span data-stu-id="507b4-149">Mail assessment request</span></span>](/graph/api/resources/mailassessmentrequest)
- [<span data-ttu-id="507b4-150">电子邮件文件评估请求</span><span class="sxs-lookup"><span data-stu-id="507b4-150">Email file assessment request</span></span>](/graph/api/resources/emailfileassessmentrequest)
- [<span data-ttu-id="507b4-151">文件评估请求</span><span class="sxs-lookup"><span data-stu-id="507b4-151">File assessment request</span></span>](/graph/api/resources/fileassessmentrequest)
- [<span data-ttu-id="507b4-152">URL 评估请求</span><span class="sxs-lookup"><span data-stu-id="507b4-152">URL assessment request</span></span>](/graph/api/resources/urlassessmentrequest)
- [<span data-ttu-id="507b4-153">威胁评估结果</span><span class="sxs-lookup"><span data-stu-id="507b4-153">Threat assessment result</span></span>](/graph/api/resources/threatassessmentresult)
- [<span data-ttu-id="507b4-154">趋势</span><span class="sxs-lookup"><span data-stu-id="507b4-154">Trending</span></span>](/graph/api/resources/insights-trending)
- [<span data-ttu-id="507b4-155">已使用见解</span><span class="sxs-lookup"><span data-stu-id="507b4-155">Used insight</span></span>](/graph/api/resources/insights-used)
- [<span data-ttu-id="507b4-156">共享见解</span><span class="sxs-lookup"><span data-stu-id="507b4-156">Shared insight</span></span>](/graph/api/resources/insights-shared)
- [<span data-ttu-id="507b4-157">用户设置</span><span class="sxs-lookup"><span data-stu-id="507b4-157">User settings</span></span>](/graph/api/resources/usersettings)
- [<span data-ttu-id="507b4-158">邀请</span><span class="sxs-lookup"><span data-stu-id="507b4-158">Invitation</span></span>](/graph/api/resources/invitation)

<span data-ttu-id="507b4-159">有关 Microsoft 云限制的更广泛讨论，请参阅[限制模式](https://docs.microsoft.com/azure/architecture/patterns/throttling)。</span><span class="sxs-lookup"><span data-stu-id="507b4-159">For a broader discussion of throttling in the Microsoft Cloud, see [Throttling pattern](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span></span>

> [!NOTE]
> <span data-ttu-id="507b4-160">如果响应未提供 `Retry-After` 标头，我们建议实施指数退避重试策略。</span><span class="sxs-lookup"><span data-stu-id="507b4-160">If no `Retry-After` header is provided by the response, we recommend implementing an exponential backoff retry policy.</span></span> <span data-ttu-id="507b4-161">构建大型应用程序时，还可以实现[更高级的模式](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency)。</span><span class="sxs-lookup"><span data-stu-id="507b4-161">You can also implement [more advanced patterns](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) when building large-scale applications.</span></span>
>
> <span data-ttu-id="507b4-162">Microsoft Graph SDK 已实施依赖于 `Retry-After` 标头或默认为指数退避重试策略的处理程序。</span><span class="sxs-lookup"><span data-stu-id="507b4-162">Microsoft Graph SDKs already implement handlers that rely on the `Retry-After` header or default to an exponential backoff retry policy.</span></span>

## <a name="best-practices-to-avoid-throttling"></a><span data-ttu-id="507b4-163">避免限制的最佳做法</span><span class="sxs-lookup"><span data-stu-id="507b4-163">Best practices to avoid throttling</span></span>

<span data-ttu-id="507b4-164">如持续轮询资源以检查更新以及定期扫描资源集合以检查新资源或已删除资源之类的编程模式，更有可能导致应用程序受到限制并降低整体性能。</span><span class="sxs-lookup"><span data-stu-id="507b4-164">Programming patterns like continuously polling a resource to check for updates and regularly scanning resource collections to check for new or deleted resources are more likely to lead to applications being throttled and degrade overall performances.</span></span> <span data-ttu-id="507b4-165">如果可用，改为使用[更改跟踪](delta-query-overview.md)并[更改通知](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="507b4-165">You should instead leverage [change tracking](delta-query-overview.md) and [change notifications](webhooks.md) when available.</span></span>

>[!NOTE]
><span data-ttu-id="507b4-166">[大规模发现文件和检测更改的最佳做法](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online)详细介绍最佳做法。</span><span class="sxs-lookup"><span data-stu-id="507b4-166">[Best practices for discovering files and detecting changes at scale](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online) describes best practices in details.</span></span>

## <a name="service-specific-limits"></a><span data-ttu-id="507b4-167">服务特定限制</span><span class="sxs-lookup"><span data-stu-id="507b4-167">Service-specific limits</span></span>

<span data-ttu-id="507b4-168">借助 Microsoft Graph，用户可访问[多个服务](overview-major-services.md)中的数据，如 Outlook 或 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="507b4-168">Microsoft Graph allows you to access data in [multiple services](overview-major-services.md), such as Outlook or Azure Active Directory.</span></span> <span data-ttu-id="507b4-169">这些服务实施自己的限制，这些限制会影响使用 Microsoft Graph 访问它们的应用程序。</span><span class="sxs-lookup"><span data-stu-id="507b4-169">These services impose their own throttling limits that affect applications that use Microsoft Graph to access them.</span></span>

<span data-ttu-id="507b4-170">任何请求均可根据多个限制进行评估，具体取决于限制范围（所有租户中的每个应用、所有应用的每个租户、每个租户的每个应用等）、请求类型（GET、 POST、PATCH等）以及其他因素。</span><span class="sxs-lookup"><span data-stu-id="507b4-170">Any request can be evaluated against multiple limits, depending on the scope of the limit (per app across all tenants, per tenant for all apps, per app per tenant, and so on), the request type (GET, POST, PATCH, and so on), and other factors.</span></span> <span data-ttu-id="507b4-171">即将达到的第一个限制会触发阻止行为。</span><span class="sxs-lookup"><span data-stu-id="507b4-171">The first limit to be reached triggers throttling behavior.</span></span> <span data-ttu-id="507b4-172">除了本节中描述的服务特定限制之外，还适用以下全局限制：</span><span class="sxs-lookup"><span data-stu-id="507b4-172">In addition to the service specific-limits described in the section, the following global limits apply:</span></span>

| <span data-ttu-id="507b4-173">请求类型</span><span class="sxs-lookup"><span data-stu-id="507b4-173">Request type</span></span> | <span data-ttu-id="507b4-174">所有租户中的每个应用</span><span class="sxs-lookup"><span data-stu-id="507b4-174">Per app across all tenants</span></span>  |
| ------------ | ------------------------ |
| <span data-ttu-id="507b4-175">任何</span><span class="sxs-lookup"><span data-stu-id="507b4-175">Any</span></span>          | <span data-ttu-id="507b4-176">每秒 2000 个请求</span><span class="sxs-lookup"><span data-stu-id="507b4-176">2000 requests per second</span></span> |

> [!NOTE]
> <span data-ttu-id="507b4-177">此处所述的具体限制可能会发生更改。</span><span class="sxs-lookup"><span data-stu-id="507b4-177">The specific limits described here are subject to change.</span></span>

> <span data-ttu-id="507b4-178">**备注** 在本节中，*租户*此术语是指指安装应用程序的 Microsoft 365 组织。</span><span class="sxs-lookup"><span data-stu-id="507b4-178">**Note:** In this section, the term *tenant* refers to the Microsoft 365 organization where the application is installed.</span></span> <span data-ttu-id="507b4-179">对于单个租户应用程序，这个租户可以与创建应用程序的租户相同，对于[多租户应用程序](/azure/active-directory/develop/setup-multi-tenant-app)，这个租户可以不同。</span><span class="sxs-lookup"><span data-stu-id="507b4-179">This tenant can be the same as the the one where the application was created, in the case of a single tenant application, or it can be different, in the case of a [multi-tenant application](/azure/active-directory/develop/setup-multi-tenant-app).</span></span>

### <a name="outlook-service-limits"></a><span data-ttu-id="507b4-180">Outlook 服务限制</span><span class="sxs-lookup"><span data-stu-id="507b4-180">Outlook service limits</span></span>

<span data-ttu-id="507b4-181">将评估每个应用 ID 和邮箱组合的 Outlook 服务限制。</span><span class="sxs-lookup"><span data-stu-id="507b4-181">Outlook service limits are evaluated for each app ID and mailbox combination.</span></span> <span data-ttu-id="507b4-182">换言之，上述限制适用于访问特定邮箱（用户或组）的特定应用。</span><span class="sxs-lookup"><span data-stu-id="507b4-182">In other words, the limits described apply to a specific app accessing a specific mailbox (user or group).</span></span> <span data-ttu-id="507b4-183">如果一个邮箱的应用程序超过限制，不会影响访问另一个邮箱的功能。</span><span class="sxs-lookup"><span data-stu-id="507b4-183">If an application exceeds the limit in one mailbox, it does not affect the ability to access another mailbox.</span></span> <span data-ttu-id="507b4-184">下面的限制适用于公共云以及[区域云部署](/graph/deployments)。</span><span class="sxs-lookup"><span data-stu-id="507b4-184">The following limits apply to the public cloud as well as [national cloud deployments](/graph/deployments).</span></span>

| <span data-ttu-id="507b4-185">限制</span><span class="sxs-lookup"><span data-stu-id="507b4-185">Limit</span></span>                                                      | <span data-ttu-id="507b4-186">适用对象</span><span class="sxs-lookup"><span data-stu-id="507b4-186">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="507b4-187">10 分钟内的 10,000 个 API 请求</span><span class="sxs-lookup"><span data-stu-id="507b4-187">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="507b4-188">v1.0 和 beta 终结点</span><span class="sxs-lookup"><span data-stu-id="507b4-188">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="507b4-189">4 个并发请求</span><span class="sxs-lookup"><span data-stu-id="507b4-189">4 concurrent requests</span></span>                                      | <span data-ttu-id="507b4-190">v1.0 和 beta 终结点</span><span class="sxs-lookup"><span data-stu-id="507b4-190">v1.0 and beta endpoints</span></span>   |
| <span data-ttu-id="507b4-191">30 秒内的 15 兆字节 (MB) 上传（PATCH、POST、PUT）</span><span class="sxs-lookup"><span data-stu-id="507b4-191">15 megabytes (MB) upload (PATCH, POST, PUT) in a 30 second period</span></span> | <span data-ttu-id="507b4-192">v1.0 和 beta 终结点</span><span class="sxs-lookup"><span data-stu-id="507b4-192">v1.0 and beta endpoints</span></span>   |

#### <a name="outlook-service-resources"></a><span data-ttu-id="507b4-193">Outlook 服务资源</span><span class="sxs-lookup"><span data-stu-id="507b4-193">Outlook service resources</span></span>

<span data-ttu-id="507b4-194">Outlook 服务提供以下资源。</span><span class="sxs-lookup"><span data-stu-id="507b4-194">The following resources are provided by the Outlook service.</span></span>

##### <a name="calendar-api-resources"></a><span data-ttu-id="507b4-195">日历 API 资源</span><span class="sxs-lookup"><span data-stu-id="507b4-195">Calendar API resources</span></span>

- [<span data-ttu-id="507b4-196">event</span><span class="sxs-lookup"><span data-stu-id="507b4-196">event</span></span>](/graph/api/resources/event)
- [<span data-ttu-id="507b4-197">eventMessage</span><span class="sxs-lookup"><span data-stu-id="507b4-197">eventMessage</span></span>](/graph/api/resources/eventmessage)
- [<span data-ttu-id="507b4-198">calendar</span><span class="sxs-lookup"><span data-stu-id="507b4-198">calendar</span></span>](/graph/api/resources/calendar)
- [<span data-ttu-id="507b4-199">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="507b4-199">calendarGroup</span></span>](/graph/api/resources/calendargroup)
- [<span data-ttu-id="507b4-200">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="507b4-200">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="507b4-201">attachment</span><span class="sxs-lookup"><span data-stu-id="507b4-201">attachment</span></span>](/graph/api/resources/attachment)
- [<span data-ttu-id="507b4-202">place（预览）</span><span class="sxs-lookup"><span data-stu-id="507b4-202">place (preview)</span></span>](/graph/api/resources/place)

##### <a name="mail-api-resources"></a><span data-ttu-id="507b4-203">邮件 API 资源</span><span class="sxs-lookup"><span data-stu-id="507b4-203">Mail API resources</span></span>

- [<span data-ttu-id="507b4-204">message</span><span class="sxs-lookup"><span data-stu-id="507b4-204">message</span></span>](/graph/api/resources/message)
- [<span data-ttu-id="507b4-205">mailFolder</span><span class="sxs-lookup"><span data-stu-id="507b4-205">mailFolder</span></span>](/graph/api/resources/mailfolder)
- [<span data-ttu-id="507b4-206">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="507b4-206">mailSearchFolder</span></span>](/graph/api/resources/mailsearchfolder)
- [<span data-ttu-id="507b4-207">messageRule</span><span class="sxs-lookup"><span data-stu-id="507b4-207">messageRule</span></span>](/graph/api/resources/messagerule)
- [<span data-ttu-id="507b4-208">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="507b4-208">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="507b4-209">attachment</span><span class="sxs-lookup"><span data-stu-id="507b4-209">attachment</span></span>](/graph/api/resources/attachment)

##### <a name="personal-contacts-api-resources"></a><span data-ttu-id="507b4-210">个人联系人 API 资源</span><span class="sxs-lookup"><span data-stu-id="507b4-210">Personal contacts API resources</span></span>

- [<span data-ttu-id="507b4-211">contact</span><span class="sxs-lookup"><span data-stu-id="507b4-211">contact</span></span>](/graph/api/resources/contact)
- [<span data-ttu-id="507b4-212">contactFolder</span><span class="sxs-lookup"><span data-stu-id="507b4-212">contactFolder</span></span>](/graph/api/resources/contactfolder)
- [<span data-ttu-id="507b4-213">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="507b4-213">outlookCategory</span></span>](/graph/api/resources/outlookcategory)

##### <a name="social-and-workplace-intelligence-resources"></a><span data-ttu-id="507b4-214">社交和工作区智能资源</span><span class="sxs-lookup"><span data-stu-id="507b4-214">Social and workplace intelligence resources</span></span>

- [<span data-ttu-id="507b4-215">person</span><span class="sxs-lookup"><span data-stu-id="507b4-215">person</span></span>](/graph/api/resources/person)

##### <a name="to-do-tasks-api-preview-resources"></a><span data-ttu-id="507b4-216">待办任务 API（预览）资源</span><span class="sxs-lookup"><span data-stu-id="507b4-216">To-do tasks API (preview) resources</span></span>

- [<span data-ttu-id="507b4-217">outlookTask</span><span class="sxs-lookup"><span data-stu-id="507b4-217">outlookTask</span></span>](/graph/api/resources/outlooktask)
- [<span data-ttu-id="507b4-218">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="507b4-218">outlookTaskFolder</span></span>](/graph/api/resources/outlooktaskfolder)
- [<span data-ttu-id="507b4-219">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="507b4-219">outlookTaskGroup</span></span>](/graph/api/resources/outlooktaskgroup)
- [<span data-ttu-id="507b4-220">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="507b4-220">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="507b4-221">attachment</span><span class="sxs-lookup"><span data-stu-id="507b4-221">attachment</span></span>](/graph/api/resources/attachment)

### <a name="cloud-communication-service-limits"></a><span data-ttu-id="507b4-222">云通信服务限制</span><span class="sxs-lookup"><span data-stu-id="507b4-222">Cloud communication service limits</span></span>

| <span data-ttu-id="507b4-223">资源</span><span class="sxs-lookup"><span data-stu-id="507b4-223">Resource</span></span>      | <span data-ttu-id="507b4-224">每个租户每个应用限制</span><span class="sxs-lookup"><span data-stu-id="507b4-224">Limits per app per tenant</span></span>    |
| -------------- | ------------ |
| [<span data-ttu-id="507b4-225">通话</span><span class="sxs-lookup"><span data-stu-id="507b4-225">Calls</span></span>](/graph/api/resources/call) | <span data-ttu-id="507b4-226">每月10,000 通通话和 100 通并发通话</span><span class="sxs-lookup"><span data-stu-id="507b4-226">10,000 calls/month and 100 concurrent calls</span></span>   |
| [<span data-ttu-id="507b4-227">会议信息</span><span class="sxs-lookup"><span data-stu-id="507b4-227">Meeting information</span></span>](/graph/api/resources/meetinginfo)   | <span data-ttu-id="507b4-228">每月每位用家会有 2000 则会议</span><span class="sxs-lookup"><span data-stu-id="507b4-228">2000 meetings/user each month</span></span> |
| <span data-ttu-id="507b4-229">[状态](/graph/api/resources/presence)（预览版）</span><span class="sxs-lookup"><span data-stu-id="507b4-229">[Presence](/graph/api/resources/presence) (preview)</span></span>   | <span data-ttu-id="507b4-230">2 rps</span><span class="sxs-lookup"><span data-stu-id="507b4-230">2 rps</span></span> |

### <a name="onenote-service-limits"></a><span data-ttu-id="507b4-231">OneNote 服务限制</span><span class="sxs-lookup"><span data-stu-id="507b4-231">OneNote service limits</span></span>

| <span data-ttu-id="507b4-232">限制类型</span><span class="sxs-lookup"><span data-stu-id="507b4-232">Limit type</span></span> | <span data-ttu-id="507b4-233">每个用户的每个应用程序的限制（委派的上下文）</span><span class="sxs-lookup"><span data-stu-id="507b4-233">Limit per app per user (delegated context)</span></span> | <span data-ttu-id="507b4-234">每个应用程序的限制（仅应用程序上下文）</span><span class="sxs-lookup"><span data-stu-id="507b4-234">Limit per app (app-only context)</span></span> |
| ------------ | ------- | ------- |
| <span data-ttu-id="507b4-235">请求率</span><span class="sxs-lookup"><span data-stu-id="507b4-235">Requests rate</span></span> | <span data-ttu-id="507b4-236">每 1 分钟 120 个请求和每 1 小时 400 个请求</span><span class="sxs-lookup"><span data-stu-id="507b4-236">120 requests per 1 minute and 400 per 1 hour</span></span> | <span data-ttu-id="507b4-237">每 1 分钟 240 个请求和每 1 小时 800 个请求</span><span class="sxs-lookup"><span data-stu-id="507b4-237">240 requests per 1 minute and 800 per 1 hour</span></span> |
| <span data-ttu-id="507b4-238">并发请求</span><span class="sxs-lookup"><span data-stu-id="507b4-238">Concurrent requests</span></span> | <span data-ttu-id="507b4-239">5 个并发请求</span><span class="sxs-lookup"><span data-stu-id="507b4-239">5 concurrent requests</span></span> | <span data-ttu-id="507b4-240">20 个并发请求</span><span class="sxs-lookup"><span data-stu-id="507b4-240">20 concurrent requests</span></span> |

<span data-ttu-id="507b4-241">上述限制适用于下列资源:</span><span class="sxs-lookup"><span data-stu-id="507b4-241">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="507b4-242">onenote, notebook, sectionGroup, onenoteSection, onenotePage, onenoteResource, onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="507b4-242">onenote, notebook, sectionGroup, onenoteSection, onenotePage, onenoteResource, onenoteOperation</span></span>

<span data-ttu-id="507b4-243">可在 [OneNote API 限制及避免方法](https://developer.microsoft.com/zh-CN/office/blogs/onenote-api-throttling-and-how-to-avoid-it/) 中找到有关最佳做法的附加信息。</span><span class="sxs-lookup"><span data-stu-id="507b4-243">You can find additional information about best practices in [OneNote API throttling and how to avoid it](https://developer.microsoft.com/zh-CN/office/blogs/onenote-api-throttling-and-how-to-avoid-it/).</span></span>  

> <span data-ttu-id="507b4-244">**注意：** 上面列出的资源未在 `429 Too Many Requests` 响应上返回 `Retry-After` 标头。</span><span class="sxs-lookup"><span data-stu-id="507b4-244">**Note:** The resources listed above do not return a `Retry-After` header on `429 Too Many Requests` responses.</span></span>

### <a name="project-rome-service-limits"></a><span data-ttu-id="507b4-245">Project Rome 服务限制</span><span class="sxs-lookup"><span data-stu-id="507b4-245">Project Rome service limits</span></span>

| <span data-ttu-id="507b4-246">请求类型</span><span class="sxs-lookup"><span data-stu-id="507b4-246">Request type</span></span> | <span data-ttu-id="507b4-247">所有应用的每个用户的限制</span><span class="sxs-lookup"><span data-stu-id="507b4-247">Limit per user for all apps</span></span> |
| ------------ | --------------------------- |
| <span data-ttu-id="507b4-248">GET</span><span class="sxs-lookup"><span data-stu-id="507b4-248">GET</span></span>          | <span data-ttu-id="507b4-249">每 5 分钟 400 个请求和每天 12000 个请求</span><span class="sxs-lookup"><span data-stu-id="507b4-249">400 requests per 5 minutes and 12000 requests per 1 day</span></span> |
| <span data-ttu-id="507b4-250">POST, PUT, PATCH, DELETE</span><span class="sxs-lookup"><span data-stu-id="507b4-250">POST, PUT, PATCH, DELETE</span></span> | <span data-ttu-id="507b4-251">每 5 分钟 100 个请求和每天 8000 个请求</span><span class="sxs-lookup"><span data-stu-id="507b4-251">100 requests per 5 minutes and 8000 requests per 1 day</span></span> |

<span data-ttu-id="507b4-252">上述限制适用于下列资源:</span><span class="sxs-lookup"><span data-stu-id="507b4-252">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="507b4-253">activityHistoryItem、userActivity</span><span class="sxs-lookup"><span data-stu-id="507b4-253">activityHistoryItem, userActivity</span></span>

### <a name="microsoft-teams-service-limits"></a><span data-ttu-id="507b4-254">Microsoft Teams 服务限制</span><span class="sxs-lookup"><span data-stu-id="507b4-254">Microsoft Teams service limits</span></span>

<span data-ttu-id="507b4-255">限制表示为每秒请求数 (rps)。</span><span class="sxs-lookup"><span data-stu-id="507b4-255">Limits are expressed as requests per second (rps).</span></span>

| <span data-ttu-id="507b4-256">Teams 请求类型</span><span class="sxs-lookup"><span data-stu-id="507b4-256">Teams request type</span></span>                                   | <span data-ttu-id="507b4-257">每个租户每个应用限制</span><span class="sxs-lookup"><span data-stu-id="507b4-257">Limit per app per tenant</span></span>        | <span data-ttu-id="507b4-258">所有租户中的每个应用限制</span><span class="sxs-lookup"><span data-stu-id="507b4-258">Limit per app across all tenants</span></span>      |
|------------------------------------------------------|---------------------------------|------------|
| <span data-ttu-id="507b4-259">Microsoft Teams 的任何图形 API 调用</span><span class="sxs-lookup"><span data-stu-id="507b4-259">Any Graph API calls for Microsoft Teams</span></span>              | <span data-ttu-id="507b4-260">每 10 秒 15000 个请求</span><span class="sxs-lookup"><span data-stu-id="507b4-260">15000 requests every 10 seconds</span></span> | <span data-ttu-id="507b4-261">不适用</span><span class="sxs-lookup"><span data-stu-id="507b4-261">n/a</span></span> |
| <span data-ttu-id="507b4-262">GET team, channel, tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="507b4-262">GET team, channel, tab, installedApps, appCatalogs</span></span>   | <span data-ttu-id="507b4-263">60 rps</span><span class="sxs-lookup"><span data-stu-id="507b4-263">60 rps</span></span>                          | <span data-ttu-id="507b4-264">600 rps</span><span class="sxs-lookup"><span data-stu-id="507b4-264">600 rps</span></span> |
| <span data-ttu-id="507b4-265">POST/PUT channel, tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="507b4-265">POST/PUT channel, tab, installedApps, appCatalogs</span></span>    |  <span data-ttu-id="507b4-266">30 rps</span><span class="sxs-lookup"><span data-stu-id="507b4-266">30 rps</span></span>                         | <span data-ttu-id="507b4-267">300 rps</span><span class="sxs-lookup"><span data-stu-id="507b4-267">300 rps</span></span>  |
| <span data-ttu-id="507b4-268">PATCH team, channel, tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="507b4-268">PATCH team, channel, tab, installedApps, appCatalogs</span></span> |  <span data-ttu-id="507b4-269">30 rps</span><span class="sxs-lookup"><span data-stu-id="507b4-269">30 rps</span></span>                         | <span data-ttu-id="507b4-270">300 rps</span><span class="sxs-lookup"><span data-stu-id="507b4-270">300 rps</span></span>  |
| <span data-ttu-id="507b4-271">DELETE channel, tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="507b4-271">DELETE channel, tab, installedApps, appCatalogs</span></span>      |  <span data-ttu-id="507b4-272">15 rps</span><span class="sxs-lookup"><span data-stu-id="507b4-272">15 rps</span></span>                         | <span data-ttu-id="507b4-273">150 rps</span><span class="sxs-lookup"><span data-stu-id="507b4-273">150 rps</span></span>  |
| <span data-ttu-id="507b4-274">GET /teams/```{team-id}```, joinedTeams</span><span class="sxs-lookup"><span data-stu-id="507b4-274">GET /teams/```{team-id}```, joinedTeams</span></span>              |  <span data-ttu-id="507b4-275">30 rps</span><span class="sxs-lookup"><span data-stu-id="507b4-275">30 rps</span></span>                         | <span data-ttu-id="507b4-276">300 rps</span><span class="sxs-lookup"><span data-stu-id="507b4-276">300 rps</span></span>  |
| <span data-ttu-id="507b4-277">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, clone</span><span class="sxs-lookup"><span data-stu-id="507b4-277">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, clone</span></span> | <span data-ttu-id="507b4-278">6 rps</span><span class="sxs-lookup"><span data-stu-id="507b4-278">6 rps</span></span> | <span data-ttu-id="507b4-279">150 rps</span><span class="sxs-lookup"><span data-stu-id="507b4-279">150 rps</span></span>  | 
| <span data-ttu-id="507b4-280">GET channel message</span><span class="sxs-lookup"><span data-stu-id="507b4-280">GET channel message</span></span>  | <span data-ttu-id="507b4-281">5 rps</span><span class="sxs-lookup"><span data-stu-id="507b4-281">5 rps</span></span> | <span data-ttu-id="507b4-282">100 rps</span><span class="sxs-lookup"><span data-stu-id="507b4-282">100 rps</span></span> |
| <span data-ttu-id="507b4-283">GET 1:1/group chat message</span><span class="sxs-lookup"><span data-stu-id="507b4-283">GET 1:1/group chat message</span></span>  | <span data-ttu-id="507b4-284">3 rps</span><span class="sxs-lookup"><span data-stu-id="507b4-284">3 rps</span></span> | <span data-ttu-id="507b4-285">30 rps</span><span class="sxs-lookup"><span data-stu-id="507b4-285">30 rps</span></span> |
| <span data-ttu-id="507b4-286">POST channel message</span><span class="sxs-lookup"><span data-stu-id="507b4-286">POST channel message</span></span> | <span data-ttu-id="507b4-287">2 rps</span><span class="sxs-lookup"><span data-stu-id="507b4-287">2 rps</span></span> | <span data-ttu-id="507b4-288">20 rps</span><span class="sxs-lookup"><span data-stu-id="507b4-288">20 rps</span></span> |
| <span data-ttu-id="507b4-289">POST 1:1/group chat message</span><span class="sxs-lookup"><span data-stu-id="507b4-289">POST 1:1/group chat message</span></span> | <span data-ttu-id="507b4-290">2 rps</span><span class="sxs-lookup"><span data-stu-id="507b4-290">2 rps</span></span> | <span data-ttu-id="507b4-291">20 rps</span><span class="sxs-lookup"><span data-stu-id="507b4-291">20 rps</span></span> |
| <span data-ttu-id="507b4-292">GET/teams/```{team-id}```/在以下路径下的日程安排和所有 API</span><span class="sxs-lookup"><span data-stu-id="507b4-292">GET /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="507b4-293">60 rps</span><span class="sxs-lookup"><span data-stu-id="507b4-293">60 rps</span></span> | <span data-ttu-id="507b4-294">600 rps</span><span class="sxs-lookup"><span data-stu-id="507b4-294">600 rps</span></span> |
| <span data-ttu-id="507b4-295">POST, PATCH, PUT /teams/```{team-id}```/在以下路径下的日程安排和所有 API</span><span class="sxs-lookup"><span data-stu-id="507b4-295">POST, PATCH, PUT /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="507b4-296">30 rps</span><span class="sxs-lookup"><span data-stu-id="507b4-296">30 rps</span></span> | <span data-ttu-id="507b4-297">300 rps</span><span class="sxs-lookup"><span data-stu-id="507b4-297">300 rps</span></span> |
| <span data-ttu-id="507b4-298">DELETE /teams/```{team-id}```/在以下路径下的日程安排和所有 API</span><span class="sxs-lookup"><span data-stu-id="507b4-298">DELETE /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="507b4-299">15 rps</span><span class="sxs-lookup"><span data-stu-id="507b4-299">15 rps</span></span> | <span data-ttu-id="507b4-300">150 rps</span><span class="sxs-lookup"><span data-stu-id="507b4-300">150 rps</span></span> |

<span data-ttu-id="507b4-301">对于给定团队或频道，每个应用最多可发布 4 个请求。</span><span class="sxs-lookup"><span data-stu-id="507b4-301">A maximum of 4 requests per second per app can be issued on a given team or channel.</span></span>
<span data-ttu-id="507b4-302">每个应用每天最多可以将 3000 条消息发送到给定的频道。</span><span class="sxs-lookup"><span data-stu-id="507b4-302">A maximum of 3000 messages per app per day can be sent to a given channel.</span></span>

<span data-ttu-id="507b4-303">另请参阅 [Microsoft Teams 限制](/graph/api/resources/teams-api-overview#microsoft-teams-limits)和[投票要求](/graph/api/resources/teams-api-overview#polling-requirements)。</span><span class="sxs-lookup"><span data-stu-id="507b4-303">See also [Microsoft Teams limits](/graph/api/resources/teams-api-overview#microsoft-teams-limits) and [polling requirements](/graph/api/resources/teams-api-overview#polling-requirements).</span></span>

### <a name="information-protection"></a><span data-ttu-id="507b4-304">信息保护</span><span class="sxs-lookup"><span data-stu-id="507b4-304">Information protection</span></span>

<span data-ttu-id="507b4-305">以下限制适用于 `/informationProtection` 上的所有请求。</span><span class="sxs-lookup"><span data-stu-id="507b4-305">The following limits apply to any request on `/informationProtection`.</span></span>

| <span data-ttu-id="507b4-306">操作</span><span class="sxs-lookup"><span data-stu-id="507b4-306">Operation</span></span>                 | <span data-ttu-id="507b4-307">每个租户的使用限制</span><span class="sxs-lookup"><span data-stu-id="507b4-307">Limit per tenant</span></span>                                            | <span data-ttu-id="507b4-308">每个资源（电子邮件、URL、文件）的使用限制</span><span class="sxs-lookup"><span data-stu-id="507b4-308">Limit per resource (email, URL, file)</span></span>                |
|---------------------------|-------------------------------------------------------------|------------------------------------------------------|
| <span data-ttu-id="507b4-309">POST</span><span class="sxs-lookup"><span data-stu-id="507b4-309">POST</span></span>                      | <span data-ttu-id="507b4-310">每 15 分钟 150 个请求和每 24 小时 10000 个请求</span><span class="sxs-lookup"><span data-stu-id="507b4-310">150 requests per 15 minutes and 10000 requests per 24 hours</span></span> | <span data-ttu-id="507b4-311">每 15 分钟 1 个请求和每 24 小时 3 个请求</span><span class="sxs-lookup"><span data-stu-id="507b4-311">1 request per 15 minutes and 3 requests per 24 hours</span></span> |

<span data-ttu-id="507b4-312">上述限制适用于下列资源:</span><span class="sxs-lookup"><span data-stu-id="507b4-312">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="507b4-313">threatAssessmentRequest、threatAssessmentResult、mailAssessmentRequest、emailFileAssessmentRequest、fileAssessmentRequest、urlAssessmentRequest。</span><span class="sxs-lookup"><span data-stu-id="507b4-313">threatAssessmentRequest, threatAssessmentResult, mailAssessmentRequest, emailFileAssessmentRequest, fileAssessmentRequest, urlAssessmentRequest.</span></span>

### <a name="identity-protection-and-conditional-access-service-limits"></a><span data-ttu-id="507b4-314">身份保护和条件访问服务限制</span><span class="sxs-lookup"><span data-stu-id="507b4-314">Identity protection and conditional access service limits</span></span>

| <span data-ttu-id="507b4-315">请求类型</span><span class="sxs-lookup"><span data-stu-id="507b4-315">Request type</span></span> | <span data-ttu-id="507b4-316">所有应用的每个租户的使用限制</span><span class="sxs-lookup"><span data-stu-id="507b4-316">Limit per tenant for all apps</span></span> |
| ------------ | ------- |
| <span data-ttu-id="507b4-317">任何</span><span class="sxs-lookup"><span data-stu-id="507b4-317">Any</span></span> | <span data-ttu-id="507b4-318">每秒1个请求</span><span class="sxs-lookup"><span data-stu-id="507b4-318">1 request per second</span></span> |

<span data-ttu-id="507b4-319">上述限制适用于下列资源:</span><span class="sxs-lookup"><span data-stu-id="507b4-319">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="507b4-320">riskDetection, riskyUser, riskyUserHistoryItem, namedLocation, countryNamedLocation, ipNamedLocation, conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="507b4-320">riskDetection, riskyUser, riskyUserHistoryItem, namedLocation, countryNamedLocation, ipNamedLocation, conditionalAccessPolicy.</span></span>

> <span data-ttu-id="507b4-321">**注意：** 上面列出的资源未在 `429 Too Many Requests` 响应上返回 `Retry-After` 标头。</span><span class="sxs-lookup"><span data-stu-id="507b4-321">**Note:** The resources listed above do not return a `Retry-After` header on `429 Too Many Requests` responses.</span></span>

### <a name="insights-service-limits"></a><span data-ttu-id="507b4-322">见解服务限制</span><span class="sxs-lookup"><span data-stu-id="507b4-322">Insights service limits</span></span>

<span data-ttu-id="507b4-323">以下限制适用于 `me/insights`或`users/{id}/insights` 上的所有请求。</span><span class="sxs-lookup"><span data-stu-id="507b4-323">The following limits apply to any request on `me/insights` or `users/{id}/insights`.</span></span>

| <span data-ttu-id="507b4-324">限制</span><span class="sxs-lookup"><span data-stu-id="507b4-324">Limit</span></span>                                                      | <span data-ttu-id="507b4-325">适用对象</span><span class="sxs-lookup"><span data-stu-id="507b4-325">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="507b4-326">10 分钟内的 10,000 个 API 请求</span><span class="sxs-lookup"><span data-stu-id="507b4-326">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="507b4-327">v1.0 和 beta 终结点</span><span class="sxs-lookup"><span data-stu-id="507b4-327">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="507b4-328">4 个并发请求</span><span class="sxs-lookup"><span data-stu-id="507b4-328">4 concurrent requests</span></span>                                      | <span data-ttu-id="507b4-329">v1.0 和 beta 终结点</span><span class="sxs-lookup"><span data-stu-id="507b4-329">v1.0 and beta endpoints</span></span>   |

### <a name="microsoft-graph-reports-service-limits"></a><span data-ttu-id="507b4-330">Microsoft Graph 报告的服务限制</span><span class="sxs-lookup"><span data-stu-id="507b4-330">Microsoft Graph reports service limits</span></span>

<span data-ttu-id="507b4-331">以下限制适用于 `/reports` 上的所有请求。</span><span class="sxs-lookup"><span data-stu-id="507b4-331">The following limits apply to any request on `/reports`.</span></span>

| <span data-ttu-id="507b4-332">操作</span><span class="sxs-lookup"><span data-stu-id="507b4-332">Operation</span></span>                 | <span data-ttu-id="507b4-333">每个租户每个应用限制</span><span class="sxs-lookup"><span data-stu-id="507b4-333">Limit per app per tenant</span></span>     | <span data-ttu-id="507b4-334">所有应用的每个租户的使用限制</span><span class="sxs-lookup"><span data-stu-id="507b4-334">Limit per tenant for all apps</span></span> |
|---------------------------|------------------------------|----------------------------|
| <span data-ttu-id="507b4-335">任何请求（CSV）</span><span class="sxs-lookup"><span data-stu-id="507b4-335">Any request (CSV)</span></span>         | <span data-ttu-id="507b4-336">每10分钟14个请求</span><span class="sxs-lookup"><span data-stu-id="507b4-336">14 requests per 10 minutes</span></span>   | <span data-ttu-id="507b4-337">每10分钟40个请求</span><span class="sxs-lookup"><span data-stu-id="507b4-337">40 requests per 10 minutes</span></span> |
| <span data-ttu-id="507b4-338">任何请求（JSON、beta）</span><span class="sxs-lookup"><span data-stu-id="507b4-338">Any request (JSON, beta)</span></span>  | <span data-ttu-id="507b4-339">每10分钟100个请求</span><span class="sxs-lookup"><span data-stu-id="507b4-339">100 requests per 10 minutes</span></span>  | <span data-ttu-id="507b4-340">不适用</span><span class="sxs-lookup"><span data-stu-id="507b4-340">n/a</span></span>                        |

<span data-ttu-id="507b4-341">上述限制分别适用于每个报表 API。</span><span class="sxs-lookup"><span data-stu-id="507b4-341">The preceding limits apply individually to each report API.</span></span> <span data-ttu-id="507b4-342">例如，在10分钟内分别有对 Microsoft Teams 用户活动报告API的请求及对 Outlook 用户活动报告API的请求，将分别被视为14个请求中的1个请求，而不是14个请求中的2个请求。</span><span class="sxs-lookup"><span data-stu-id="507b4-342">For example a request to Microsoft Teams user activity report API and a request to Outlook user activity report API within 10 minutes will count as 1 request out of 14 for each API, not 2 requests out of 14 for both.</span></span>

### <a name="invitation-manager-service-limits"></a><span data-ttu-id="507b4-343">邀请管理器服务限制</span><span class="sxs-lookup"><span data-stu-id="507b4-343">Invitation manager service limits</span></span>

<span data-ttu-id="507b4-344">以下限制适用于 `/invitations` 上的所有请求。</span><span class="sxs-lookup"><span data-stu-id="507b4-344">The following limits apply to any request on `/invitations`.</span></span>

| <span data-ttu-id="507b4-345">操作</span><span class="sxs-lookup"><span data-stu-id="507b4-345">Operation</span></span>                 | <span data-ttu-id="507b4-346">所有应用的每个租户的使用限制</span><span class="sxs-lookup"><span data-stu-id="507b4-346">Limit per tenant for all apps</span></span> |
|---------------------------|------------------------------|
| <span data-ttu-id="507b4-347">任何操作</span><span class="sxs-lookup"><span data-stu-id="507b4-347">Any operation</span></span>             | <span data-ttu-id="507b4-348">每 5 秒 150 个请求</span><span class="sxs-lookup"><span data-stu-id="507b4-348">150 requests per 5 seconds</span></span>   |

### <a name="security-detections-and-incidents-service-limits"></a><span data-ttu-id="507b4-349">安全检测和事件服务限制</span><span class="sxs-lookup"><span data-stu-id="507b4-349">Security detections and incidents service limits</span></span>

<span data-ttu-id="507b4-350">以下限制适用于 `/security` 上的所有请求。</span><span class="sxs-lookup"><span data-stu-id="507b4-350">The following limits apply to any request on `/security`.</span></span>

| <span data-ttu-id="507b4-351">操作</span><span class="sxs-lookup"><span data-stu-id="507b4-351">Operation</span></span>                  | <span data-ttu-id="507b4-352">每个租户每个应用限制</span><span class="sxs-lookup"><span data-stu-id="507b4-352">Limit per app per tenant</span></span>     |
|----------------------------|------------------------------|
| <span data-ttu-id="507b4-353">`alert`、`securityActions`、`secureScore` 上的任何操作</span><span class="sxs-lookup"><span data-stu-id="507b4-353">Any operation on `alert`, `securityActions`,  `secureScore`</span></span> | <span data-ttu-id="507b4-354">每分钟 150 个请求</span><span class="sxs-lookup"><span data-stu-id="507b4-354">150 requests per minute</span></span>      |
| <span data-ttu-id="507b4-355">`tiIndicator` 上的任何操作</span><span class="sxs-lookup"><span data-stu-id="507b4-355">Any operation on `tiIndicator`</span></span> | <span data-ttu-id="507b4-356">每分钟 1000 个请求</span><span class="sxs-lookup"><span data-stu-id="507b4-356">1000 requests per minute</span></span> |
| <span data-ttu-id="507b4-357">`secureScore` 或 `secureScorecontrolProfile` 上的任何操作</span><span class="sxs-lookup"><span data-stu-id="507b4-357">Any operation on `secureScore` or `secureScorecontrolProfile`</span></span> | <span data-ttu-id="507b4-358">10 分钟内的 10,000 个 API 请求</span><span class="sxs-lookup"><span data-stu-id="507b4-358">10,000 API requests in a 10 minute period</span></span> |
| <span data-ttu-id="507b4-359">`secureScore` 或 `secureScorecontrolProfile` 上的任何操作</span><span class="sxs-lookup"><span data-stu-id="507b4-359">Any operation on `secureScore` or `secureScorecontrolProfile`</span></span> | <span data-ttu-id="507b4-360">4 个并发请求</span><span class="sxs-lookup"><span data-stu-id="507b4-360">4 concurrent requests</span></span> |

### <a name="open-and-schema-extensions-service-limits"></a><span data-ttu-id="507b4-361">开放和架构扩展服务限制</span><span class="sxs-lookup"><span data-stu-id="507b4-361">Open and schema extensions service limits</span></span>

| <span data-ttu-id="507b4-362">请求类型</span><span class="sxs-lookup"><span data-stu-id="507b4-362">Request type</span></span> | <span data-ttu-id="507b4-363">每个租户每个应用限制</span><span class="sxs-lookup"><span data-stu-id="507b4-363">Limit per app per tenant</span></span> |
| ------------ | ------------------------ |
| <span data-ttu-id="507b4-364">任何</span><span class="sxs-lookup"><span data-stu-id="507b4-364">Any</span></span>          | <span data-ttu-id="507b4-365">每 10 秒 455 个请求</span><span class="sxs-lookup"><span data-stu-id="507b4-365">455 requests per 10 seconds</span></span> |

<span data-ttu-id="507b4-366">上述限制适用于以下资源：openTypeExtension、schemaExtension、administrativeUnit、合同、设备、事件、组、消息、组织、帖子和用户。</span><span class="sxs-lookup"><span data-stu-id="507b4-366">The preceding limits apply to the following resources: openTypeExtension, schemaExtension, administrativeUnit, contact, device, event, group, message, organization, post, and user.</span></span>

### <a name="files-and-lists-service-limits"></a><span data-ttu-id="507b4-367">文件和列表服务限制</span><span class="sxs-lookup"><span data-stu-id="507b4-367">Files and lists service limits</span></span>

<span data-ttu-id="507b4-368">OneDrive、OneDrive for Business 和 SharePoint Online 的服务限制不可用。</span><span class="sxs-lookup"><span data-stu-id="507b4-368">Service limits for OneDrive, OneDrive for Business, and SharePoint Online are not available.</span></span> <span data-ttu-id="507b4-369">有关详细信息，请参阅[为什么不能告诉我确切的限制？](/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online#why-cant-you-just-tell-me-the-exact-throttling-limits)。</span><span class="sxs-lookup"><span data-stu-id="507b4-369">For more information, see [why can't you just tell me the exact throttling limits?](/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online#why-cant-you-just-tell-me-the-exact-throttling-limits).</span></span>

<span data-ttu-id="507b4-370">上述信息适用于以下资源：</span><span class="sxs-lookup"><span data-stu-id="507b4-370">The preceding information applies to the following resources:</span></span>  
<span data-ttu-id="507b4-371">baseItem、baseItemVersion、columnDefinition、columnLink、contentType、drive、driveItem、driveItemVersion、fieldValueSet、itemActivity、itemActivityStat、itemAnalytics、list、listItem、listItemVersion、permission、sharedDriveItem、site 和 thumbnailSet。</span><span class="sxs-lookup"><span data-stu-id="507b4-371">baseItem, baseItemVersion, columnDefinition, columnLink, contentType, drive, driveItem, driveItemVersion, fieldValueSet, itemActivity, itemActivityStat, itemAnalytics, list, listItem, listItemVersion, permission, sharedDriveItem, site, and thumbnailSet.</span></span>

### <a name="tasks-and-plans-service-limits"></a><span data-ttu-id="507b4-372">任务和计划服务限制</span><span class="sxs-lookup"><span data-stu-id="507b4-372">Tasks and plans service limits</span></span>

<span data-ttu-id="507b4-373">Planner 的服务限制不可用。</span><span class="sxs-lookup"><span data-stu-id="507b4-373">Service limits for Planner are not available.</span></span>

<span data-ttu-id="507b4-374">上述信息适用于以下资源：</span><span class="sxs-lookup"><span data-stu-id="507b4-374">The preceding information applies to the following resources:</span></span>  
<span data-ttu-id="507b4-375">planner、plannerAssignedToTaskBoardTaskFormat、plannerBucket、plannerBucketTaskBoardTaskFormat、plannerGroup、plannerPlan、plannerPlanDetails、plannerProgressTaskBoardTaskFormat、plannerTask、plannerTaskDetails 和 plannerUser。</span><span class="sxs-lookup"><span data-stu-id="507b4-375">planner, plannerAssignedToTaskBoardTaskFormat, plannerBucket, plannerBucketTaskBoardTaskFormat, plannerGroup, plannerPlan, plannerPlanDetails, plannerProgressTaskBoardTaskFormat, plannerTask, plannerTaskDetails, and plannerUser.</span></span>

### <a name="identity-and-access-data-policy-operation-service-limits"></a><span data-ttu-id="507b4-376">身份和访问数据策略操作服务限制</span><span class="sxs-lookup"><span data-stu-id="507b4-376">Identity and access data policy operation service limits</span></span>

| <span data-ttu-id="507b4-377">请求类型</span><span class="sxs-lookup"><span data-stu-id="507b4-377">Request type</span></span> | <span data-ttu-id="507b4-378">每个租户的使用限制</span><span class="sxs-lookup"><span data-stu-id="507b4-378">Limit per tenant</span></span> |
| ------------ | ---------------- |
| <span data-ttu-id="507b4-379">发布于 `exportPersonalData`</span><span class="sxs-lookup"><span data-stu-id="507b4-379">POST on `exportPersonalData`</span></span> | <span data-ttu-id="507b4-380">每天 1000 个针对任何主题的请求，每个主题每天 100 个请求</span><span class="sxs-lookup"><span data-stu-id="507b4-380">1000 requests per day for any subject and 100 per subject per day</span></span> |
| <span data-ttu-id="507b4-381">任何其他请求</span><span class="sxs-lookup"><span data-stu-id="507b4-381">Any other request</span></span> | <span data-ttu-id="507b4-382">每分钟 10000 个请求</span><span class="sxs-lookup"><span data-stu-id="507b4-382">10000 requests per hour</span></span> |

<span data-ttu-id="507b4-383">上述限制适用于下列资源：dataPolicyOperation。</span><span class="sxs-lookup"><span data-stu-id="507b4-383">The preceding limits apply to the following resources: dataPolicyOperation.</span></span>

> <span data-ttu-id="507b4-384">**注意：** 上面列出的资源未在 `429 Too Many Requests` 响应上返回 `Retry-After` 标头。</span><span class="sxs-lookup"><span data-stu-id="507b4-384">**Note:** The resources listed above do not return a `Retry-After` header on `429 Too Many Requests` responses.</span></span>

<!-- { "blockType": "throttlinggenstart" } -->
### <a name="education-service-limits"></a><span data-ttu-id="507b4-385">教育版服务限制</span><span class="sxs-lookup"><span data-stu-id="507b4-385">Education service limits</span></span>

[!INCLUDE [Education rostering APIS throttling documentation](../includes/throttling-education-rostering-apis.md)]

### <a name="excel-service-limits"></a><span data-ttu-id="507b4-386">Excel 服务限制</span><span class="sxs-lookup"><span data-stu-id="507b4-386">Excel service limits</span></span>

[!INCLUDE [Excel throttling documentation](../includes/throttling-excel.md)]

### <a name="identity-and-access-audit-logs-service-limits"></a><span data-ttu-id="507b4-387">标识和访问审核日志的服务限制</span><span class="sxs-lookup"><span data-stu-id="507b4-387">Identity and access audit logs service limits</span></span>

[!INCLUDE [Identity and access audit logs throttling documentation](../includes/throttling-Identity-and-access-audit-logs.md)]

### <a name="identity-providers-service-limits"></a><span data-ttu-id="507b4-388">身份提供程序的服务限制</span><span class="sxs-lookup"><span data-stu-id="507b4-388">Identity providers service limits</span></span>

[!INCLUDE [CPIM throttling documentation](../includes/throttling-cpim.md)]

### <a name="intune-service-limits"></a><span data-ttu-id="507b4-389">Intune服务限制</span><span class="sxs-lookup"><span data-stu-id="507b4-389">Intune service limits</span></span>

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

### <a name="skype-service-limits"></a><span data-ttu-id="507b4-390">Skype 服务限制</span><span class="sxs-lookup"><span data-stu-id="507b4-390">Skype service limits</span></span>

[!INCLUDE [Skype calling throttling documentation](../includes/throttling-skype-calling.md)]

### <a name="subscription-service-limits"></a><span data-ttu-id="507b4-391">订阅服务</span><span class="sxs-lookup"><span data-stu-id="507b4-391">Subscription service limits</span></span>

[!INCLUDE [Subscription services throttling documentation](../includes/throttling-subscription-services.md)]

<!-- { "blockType": "throttlinggenend" } -->
