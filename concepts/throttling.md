---
title: Microsoft Graph 限制指南
description: 限制可调节并发调用服务的数量，以防止资源的过度使用。Microsoft Graph 旨在用于处理大量的请求。如果出现过多请求，限制将有助于保持 Microsoft Graph 的最佳性能和服务的可靠性。
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 96592654fffb3111a398178d807da702c398e0d2
ms.sourcegitcommit: b469176f49aacbd02cd06838cc7c8d36cf5bc768
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2020
ms.locfileid: "45165112"
---
# <a name="microsoft-graph-throttling-guidance"></a><span data-ttu-id="77e6b-105">Microsoft Graph 限制指南</span><span class="sxs-lookup"><span data-stu-id="77e6b-105">Microsoft Graph throttling guidance</span></span>

<span data-ttu-id="77e6b-p102">限制可调节并发调用服务的数量，以防止资源的过度使用。Microsoft Graph 旨在用于处理大量的请求。如果出现过多请求，限制将有助于保持 Microsoft Graph 的最佳性能和服务的可靠性。</span><span class="sxs-lookup"><span data-stu-id="77e6b-p102">Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span></span>

<span data-ttu-id="77e6b-p103">根据该方案，执行的限制会有所不同。例如，如果你正在执行大量的写入操作，限制的可能性会比仅执行读取时要高。</span><span class="sxs-lookup"><span data-stu-id="77e6b-p103">Throttling limits vary based on the scenario. For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span></span>

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a><span data-ttu-id="77e6b-111">在限制时，会发生什么情况？</span><span class="sxs-lookup"><span data-stu-id="77e6b-111">What happens when throttling occurs?</span></span>
<!-- markdownlint-enable MD026 -->

<span data-ttu-id="77e6b-p104">超出限制阈值后，Microsoft Graph 会在一段时间内限制来自该客户端的任何进一步的请求。发生限制时，Microsoft Graph 将返回 HTTP 状态代码 429（请求过多），同时请求失败。在失败的请求的响应标头中返回建议的等待时间。限制行为取决于请求的类型和数量。例如，如果你有大量的请求，则所有请求类型受限。阈值限制根据请求类型而有所不同。因此，你可能会遇到这样一种场景，在场景中，写入被限制，但仍允许读取。</span><span class="sxs-lookup"><span data-stu-id="77e6b-p104">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time. When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail. A suggested wait time is returned in the response header of the failed request. Throttling behavior can depend on the type and number of requests. For example, if you have a high volume of requests, all requests types are throttled. Threshold limits vary based on the request type. Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span>

## <a name="common-throttling-scenarios"></a><span data-ttu-id="77e6b-119">常见的限制场景</span><span class="sxs-lookup"><span data-stu-id="77e6b-119">Common throttling scenarios</span></span>

<span data-ttu-id="77e6b-120">客户端受限的最常见原因包括：</span><span class="sxs-lookup"><span data-stu-id="77e6b-120">The most common causes of throttling of clients include:</span></span>

- <span data-ttu-id="77e6b-121">来自租户中所有应用程序的请求太多。</span><span class="sxs-lookup"><span data-stu-id="77e6b-121">A large number of requests across all applications in a tenant.</span></span>
- <span data-ttu-id="77e6b-122">来自所有租户中特定应用程序的请求太多。</span><span class="sxs-lookup"><span data-stu-id="77e6b-122">A large number of requests from a particular application across all tenants.</span></span>

## <a name="best-practices-to-handle-throttling"></a><span data-ttu-id="77e6b-123">处理限制的最佳实践</span><span class="sxs-lookup"><span data-stu-id="77e6b-123">Best practices to handle throttling</span></span>

<span data-ttu-id="77e6b-124">以下是处理限制的最佳做法：</span><span class="sxs-lookup"><span data-stu-id="77e6b-124">The following are best practices for handling throttling:</span></span>

- <span data-ttu-id="77e6b-125">减少每个请求的操作数量。</span><span class="sxs-lookup"><span data-stu-id="77e6b-125">Reduce the number of operations per request.</span></span>
- <span data-ttu-id="77e6b-126">减少调用频率。</span><span class="sxs-lookup"><span data-stu-id="77e6b-126">Reduce the frequency of calls.</span></span>
- <span data-ttu-id="77e6b-127">不要立即重试，因为所有请求都会计入使用限制。</span><span class="sxs-lookup"><span data-stu-id="77e6b-127">Avoid immediate retries, because all requests accrue against your usage limits.</span></span>

<span data-ttu-id="77e6b-p105">进行错误处理时，使用 HTTP 错误代码 429 检测限制。失败的响应包括 `Retry-After` 响应标头。使用 `Retry-After` 延迟回退请求是从限制中恢复的最快速的方式，因为 Microsoft Graph 会在客户端受限时继续记录资源使用状况。</span><span class="sxs-lookup"><span data-stu-id="77e6b-p105">When you implement error handling, use the HTTP error code 429 to detect throttling. The failed response includes the `Retry-After` response header. Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span></span>

1. <span data-ttu-id="77e6b-131">等待 `Retry-After` 标头中指定的秒数。</span><span class="sxs-lookup"><span data-stu-id="77e6b-131">Wait the number of seconds specified in the `Retry-After` header.</span></span>
2. <span data-ttu-id="77e6b-132">请重试请求。</span><span class="sxs-lookup"><span data-stu-id="77e6b-132">Retry the request.</span></span>
3. <span data-ttu-id="77e6b-p106">如果请求再次失败，并显示 429 错误代码，则表示你仍然受限。继续使用建议的 `Retry-After` 延迟并重试请求直到成功。</span><span class="sxs-lookup"><span data-stu-id="77e6b-p106">If the request fails again with a 429 error code, you are still being throttled. Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span></span>

<span data-ttu-id="77e6b-135">下列资源目前提供 `Retry-After` 标头：</span><span class="sxs-lookup"><span data-stu-id="77e6b-135">The following resources currently provide a `Retry-After` header:</span></span>

- [<span data-ttu-id="77e6b-136">用户</span><span class="sxs-lookup"><span data-stu-id="77e6b-136">User</span></span>](/graph/api/resources/user?view=graph-rest-1.0)
- [<span data-ttu-id="77e6b-137">照片</span><span class="sxs-lookup"><span data-stu-id="77e6b-137">Photo</span></span>](/graph/api/resources/profilephoto?view=graph-rest-1.0)
- [<span data-ttu-id="77e6b-138">邮件</span><span class="sxs-lookup"><span data-stu-id="77e6b-138">Mail</span></span>](/graph/api/resources/message?view=graph-rest-1.0)
- [<span data-ttu-id="77e6b-139">日历（用户和组）</span><span class="sxs-lookup"><span data-stu-id="77e6b-139">Calendar (users and groups)</span></span>](/graph/api/resources/event?view=graph-rest-1.0)
- [<span data-ttu-id="77e6b-140">联系人</span><span class="sxs-lookup"><span data-stu-id="77e6b-140">Contact</span></span>](/graph/api/resources/contact?view=graph-rest-1.0)
- [<span data-ttu-id="77e6b-141">附件</span><span class="sxs-lookup"><span data-stu-id="77e6b-141">Attachment</span></span>](/graph/api/resources/attachment?view=graph-rest-1.0)
- [<span data-ttu-id="77e6b-142">组对话</span><span class="sxs-lookup"><span data-stu-id="77e6b-142">Group conversations</span></span>](/graph/api/resources/conversation?view=graph-rest-1.0)
- [<span data-ttu-id="77e6b-143">人员和社交活动</span><span class="sxs-lookup"><span data-stu-id="77e6b-143">People and social</span></span>](/graph/api/resources/social-overview?view=graph-rest-beta)
- [<span data-ttu-id="77e6b-144">Drive (OneDrive)</span><span class="sxs-lookup"><span data-stu-id="77e6b-144">Drive (OneDrive)</span></span>](/graph/api/resources/drive?view=graph-rest-1.0)
- [<span data-ttu-id="77e6b-145">外部项（Microsoft 搜索）</span><span class="sxs-lookup"><span data-stu-id="77e6b-145">External item (Microsoft Search)</span></span>](/graph/api/resources/externalitem?view=graph-rest-beta)
- [<span data-ttu-id="77e6b-146">Report</span><span class="sxs-lookup"><span data-stu-id="77e6b-146">Report</span></span>](/graph/api/resources/report)
- [<span data-ttu-id="77e6b-147">订阅</span><span class="sxs-lookup"><span data-stu-id="77e6b-147">Subscription</span></span>](/graph/api/resources/subscription)
- [<span data-ttu-id="77e6b-148">威胁评估请求</span><span class="sxs-lookup"><span data-stu-id="77e6b-148">Threat assessment request</span></span>](/graph/api/resources/threatassessmentrequest)
- [<span data-ttu-id="77e6b-149">邮件评估请求</span><span class="sxs-lookup"><span data-stu-id="77e6b-149">Mail assessment request</span></span>](/graph/api/resources/mailassessmentrequest)
- [<span data-ttu-id="77e6b-150">电子邮件文件评估请求</span><span class="sxs-lookup"><span data-stu-id="77e6b-150">Email file assessment request</span></span>](/graph/api/resources/emailfileassessmentrequest)
- [<span data-ttu-id="77e6b-151">文件评估请求</span><span class="sxs-lookup"><span data-stu-id="77e6b-151">File assessment request</span></span>](/graph/api/resources/fileassessmentrequest)
- [<span data-ttu-id="77e6b-152">URL 评估请求</span><span class="sxs-lookup"><span data-stu-id="77e6b-152">URL assessment request</span></span>](/graph/api/resources/urlassessmentrequest)
- [<span data-ttu-id="77e6b-153">威胁评估结果</span><span class="sxs-lookup"><span data-stu-id="77e6b-153">Threat assessment result</span></span>](/graph/api/resources/threatassessmentresult)
- [<span data-ttu-id="77e6b-154">趋势</span><span class="sxs-lookup"><span data-stu-id="77e6b-154">Trending</span></span>](/graph/api/resources/insights-trending)
- [<span data-ttu-id="77e6b-155">已使用见解</span><span class="sxs-lookup"><span data-stu-id="77e6b-155">Used insight</span></span>](/graph/api/resources/insights-used)
- [<span data-ttu-id="77e6b-156">共享见解</span><span class="sxs-lookup"><span data-stu-id="77e6b-156">Shared insight</span></span>](/graph/api/resources/insights-shared)
- [<span data-ttu-id="77e6b-157">用户设置</span><span class="sxs-lookup"><span data-stu-id="77e6b-157">User settings</span></span>](/graph/api/resources/usersettings)
- [<span data-ttu-id="77e6b-158">邀请</span><span class="sxs-lookup"><span data-stu-id="77e6b-158">Invitation</span></span>](/graph/api/resources/invitation)

<span data-ttu-id="77e6b-159">有关 Microsoft 云限制的更广泛讨论，请参阅[限制模式](https://docs.microsoft.com/azure/architecture/patterns/throttling)。</span><span class="sxs-lookup"><span data-stu-id="77e6b-159">For a broader discussion of throttling in the Microsoft Cloud, see [Throttling pattern](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span></span>

> [!NOTE]
> <span data-ttu-id="77e6b-160">如果响应未提供 `Retry-After` 标头，我们建议实施指数退避重试策略。</span><span class="sxs-lookup"><span data-stu-id="77e6b-160">If no `Retry-After` header is provided by the response, we recommend implementing an exponential backoff retry policy.</span></span> <span data-ttu-id="77e6b-161">构建大型应用程序时，还可以实现[更高级的模式](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency)。</span><span class="sxs-lookup"><span data-stu-id="77e6b-161">You can also implement [more advanced patterns](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) when building large-scale applications.</span></span>
>
> <span data-ttu-id="77e6b-162">Microsoft Graph SDK 已实施依赖于 `Retry-After` 标头或默认为指数退避重试策略的处理程序。</span><span class="sxs-lookup"><span data-stu-id="77e6b-162">Microsoft Graph SDKs already implement handlers that rely on the `Retry-After` header or default to an exponential backoff retry policy.</span></span>

## <a name="best-practices-to-avoid-throttling"></a><span data-ttu-id="77e6b-163">避免限制的最佳做法</span><span class="sxs-lookup"><span data-stu-id="77e6b-163">Best practices to avoid throttling</span></span>

<span data-ttu-id="77e6b-164">如持续轮询资源以检查更新以及定期扫描资源集合以检查新资源或已删除资源之类的编程模式，更有可能导致应用程序受到限制并降低整体性能。</span><span class="sxs-lookup"><span data-stu-id="77e6b-164">Programming patterns like continuously polling a resource to check for updates and regularly scanning resource collections to check for new or deleted resources are more likely to lead to applications being throttled and degrade overall performances.</span></span> <span data-ttu-id="77e6b-165">如果可用，改为使用[更改跟踪](delta-query-overview.md)并[更改通知](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="77e6b-165">You should instead leverage [change tracking](delta-query-overview.md) and [change notifications](webhooks.md) when available.</span></span>

>[!NOTE]
><span data-ttu-id="77e6b-166">[大规模发现文件和检测更改的最佳做法](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online)详细介绍最佳做法。</span><span class="sxs-lookup"><span data-stu-id="77e6b-166">[Best practices for discovering files and detecting changes at scale](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online) describes best practices in details.</span></span>

## <a name="service-specific-limits"></a><span data-ttu-id="77e6b-167">服务特定限制</span><span class="sxs-lookup"><span data-stu-id="77e6b-167">Service-specific limits</span></span>

<span data-ttu-id="77e6b-168">借助 Microsoft Graph，用户可访问[多个服务](overview-major-services.md)中的数据，如 Outlook 或 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="77e6b-168">Microsoft Graph allows you to access data in [multiple services](overview-major-services.md), such as Outlook or Azure Active Directory.</span></span> <span data-ttu-id="77e6b-169">这些服务实施自己的限制，这些限制会影响使用 Microsoft Graph 访问它们的应用程序。</span><span class="sxs-lookup"><span data-stu-id="77e6b-169">These services impose their own throttling limits that affect applications that use Microsoft Graph to access them.</span></span>

> [!NOTE]
> <span data-ttu-id="77e6b-170">此处所述的具体限制可能会发生更改。</span><span class="sxs-lookup"><span data-stu-id="77e6b-170">The specific limits described here are subject to change.</span></span>

> <span data-ttu-id="77e6b-171">**备注** 在本节中，*租户*此术语是指指安装应用程序的 Microsoft 365 组织。</span><span class="sxs-lookup"><span data-stu-id="77e6b-171">**Note:** In this section, the term *tenant* refers to the Microsoft 365 organization where the application is installed.</span></span> <span data-ttu-id="77e6b-172">对于单个租户应用程序，这个租户可以与创建应用程序的租户相同，对于[多租户应用程序](/azure/active-directory/develop/setup-multi-tenant-app)，这个租户可以不同。</span><span class="sxs-lookup"><span data-stu-id="77e6b-172">This tenant can be the same as the the one where the application was created, in the case of a single tenant application, or it can be different, in the case of a [multi-tenant application](/azure/active-directory/develop/setup-multi-tenant-app).</span></span>

### <a name="outlook-service-limits"></a><span data-ttu-id="77e6b-173">Outlook 服务限制</span><span class="sxs-lookup"><span data-stu-id="77e6b-173">Outlook service limits</span></span>

<span data-ttu-id="77e6b-174">将评估每个应用 ID 和邮箱组合的 Outlook 服务限制。</span><span class="sxs-lookup"><span data-stu-id="77e6b-174">Outlook service limits are evaluated for each app ID and mailbox combination.</span></span> <span data-ttu-id="77e6b-175">换言之，上述限制适用于访问特定邮箱（用户或组）的特定应用。</span><span class="sxs-lookup"><span data-stu-id="77e6b-175">In other words, the limits described apply to a specific app accessing a specific mailbox (user or group).</span></span> <span data-ttu-id="77e6b-176">如果一个邮箱的应用程序超过限制，不会影响访问另一个邮箱的功能。</span><span class="sxs-lookup"><span data-stu-id="77e6b-176">If an application exceeds the limit in one mailbox, it does not affect the ability to access another mailbox.</span></span> <span data-ttu-id="77e6b-177">下面的限制适用于公共云以及[区域云部署](/graph/deployments)。</span><span class="sxs-lookup"><span data-stu-id="77e6b-177">The following limits apply to the public cloud as well as [national cloud deployments](/graph/deployments).</span></span>

| <span data-ttu-id="77e6b-178">限制</span><span class="sxs-lookup"><span data-stu-id="77e6b-178">Limit</span></span>                                                      | <span data-ttu-id="77e6b-179">适用对象</span><span class="sxs-lookup"><span data-stu-id="77e6b-179">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="77e6b-180">10 分钟内的 10,000 个 API 请求</span><span class="sxs-lookup"><span data-stu-id="77e6b-180">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="77e6b-181">v1.0 和 beta 终结点</span><span class="sxs-lookup"><span data-stu-id="77e6b-181">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="77e6b-182">4 个并发请求</span><span class="sxs-lookup"><span data-stu-id="77e6b-182">4 concurrent requests</span></span>                                      | <span data-ttu-id="77e6b-183">v1.0 和 beta 终结点</span><span class="sxs-lookup"><span data-stu-id="77e6b-183">v1.0 and beta endpoints</span></span>   |
| <span data-ttu-id="77e6b-184">30 秒内的 15 兆字节 (MB) 上传（PATCH、POST、PUT）</span><span class="sxs-lookup"><span data-stu-id="77e6b-184">15 megabytes (MB) upload (PATCH, POST, PUT) in a 30 second period</span></span> | <span data-ttu-id="77e6b-185">v1.0 和 beta 终结点</span><span class="sxs-lookup"><span data-stu-id="77e6b-185">v1.0 and beta endpoints</span></span>   |

#### <a name="outlook-service-resources"></a><span data-ttu-id="77e6b-186">Outlook 服务资源</span><span class="sxs-lookup"><span data-stu-id="77e6b-186">Outlook service resources</span></span>

<span data-ttu-id="77e6b-187">Outlook 服务提供以下资源。</span><span class="sxs-lookup"><span data-stu-id="77e6b-187">The following resources are provided by the Outlook service.</span></span>

##### <a name="calendar-api-resources"></a><span data-ttu-id="77e6b-188">日历 API 资源</span><span class="sxs-lookup"><span data-stu-id="77e6b-188">Calendar API resources</span></span>

- [<span data-ttu-id="77e6b-189">event</span><span class="sxs-lookup"><span data-stu-id="77e6b-189">event</span></span>](/graph/api/resources/event)
- [<span data-ttu-id="77e6b-190">eventMessage</span><span class="sxs-lookup"><span data-stu-id="77e6b-190">eventMessage</span></span>](/graph/api/resources/eventmessage)
- [<span data-ttu-id="77e6b-191">calendar</span><span class="sxs-lookup"><span data-stu-id="77e6b-191">calendar</span></span>](/graph/api/resources/calendar)
- [<span data-ttu-id="77e6b-192">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="77e6b-192">calendarGroup</span></span>](/graph/api/resources/calendargroup)
- [<span data-ttu-id="77e6b-193">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="77e6b-193">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="77e6b-194">attachment</span><span class="sxs-lookup"><span data-stu-id="77e6b-194">attachment</span></span>](/graph/api/resources/attachment)
- [<span data-ttu-id="77e6b-195">place（预览）</span><span class="sxs-lookup"><span data-stu-id="77e6b-195">place (preview)</span></span>](/graph/api/resources/place)

##### <a name="mail-api-resources"></a><span data-ttu-id="77e6b-196">邮件 API 资源</span><span class="sxs-lookup"><span data-stu-id="77e6b-196">Mail API resources</span></span>

- [<span data-ttu-id="77e6b-197">message</span><span class="sxs-lookup"><span data-stu-id="77e6b-197">message</span></span>](/graph/api/resources/message)
- [<span data-ttu-id="77e6b-198">mailFolder</span><span class="sxs-lookup"><span data-stu-id="77e6b-198">mailFolder</span></span>](/graph/api/resources/mailfolder)
- [<span data-ttu-id="77e6b-199">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="77e6b-199">mailSearchFolder</span></span>](/graph/api/resources/mailsearchfolder)
- [<span data-ttu-id="77e6b-200">messageRule</span><span class="sxs-lookup"><span data-stu-id="77e6b-200">messageRule</span></span>](/graph/api/resources/messagerule)
- [<span data-ttu-id="77e6b-201">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="77e6b-201">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="77e6b-202">attachment</span><span class="sxs-lookup"><span data-stu-id="77e6b-202">attachment</span></span>](/graph/api/resources/attachment)

##### <a name="personal-contacts-api-resources"></a><span data-ttu-id="77e6b-203">个人联系人 API 资源</span><span class="sxs-lookup"><span data-stu-id="77e6b-203">Personal contacts API resources</span></span>

- [<span data-ttu-id="77e6b-204">contact</span><span class="sxs-lookup"><span data-stu-id="77e6b-204">contact</span></span>](/graph/api/resources/contact)
- [<span data-ttu-id="77e6b-205">contactFolder</span><span class="sxs-lookup"><span data-stu-id="77e6b-205">contactFolder</span></span>](/graph/api/resources/contactfolder)
- [<span data-ttu-id="77e6b-206">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="77e6b-206">outlookCategory</span></span>](/graph/api/resources/outlookcategory)

##### <a name="social-and-workplace-intelligence-resources"></a><span data-ttu-id="77e6b-207">社交和工作区智能资源</span><span class="sxs-lookup"><span data-stu-id="77e6b-207">Social and workplace intelligence resources</span></span>

- [<span data-ttu-id="77e6b-208">person</span><span class="sxs-lookup"><span data-stu-id="77e6b-208">person</span></span>](/graph/api/resources/person)

##### <a name="to-do-tasks-api-preview-resources"></a><span data-ttu-id="77e6b-209">待办任务 API（预览）资源</span><span class="sxs-lookup"><span data-stu-id="77e6b-209">To-do tasks API (preview) resources</span></span>

- [<span data-ttu-id="77e6b-210">outlookTask</span><span class="sxs-lookup"><span data-stu-id="77e6b-210">outlookTask</span></span>](/graph/api/resources/outlooktask)
- [<span data-ttu-id="77e6b-211">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="77e6b-211">outlookTaskFolder</span></span>](/graph/api/resources/outlooktaskfolder)
- [<span data-ttu-id="77e6b-212">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="77e6b-212">outlookTaskGroup</span></span>](/graph/api/resources/outlooktaskgroup)
- [<span data-ttu-id="77e6b-213">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="77e6b-213">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="77e6b-214">attachment</span><span class="sxs-lookup"><span data-stu-id="77e6b-214">attachment</span></span>](/graph/api/resources/attachment)

### <a name="cloud-communication-service-limits"></a><span data-ttu-id="77e6b-215">云通信服务限制</span><span class="sxs-lookup"><span data-stu-id="77e6b-215">Cloud communication service limits</span></span>

| <span data-ttu-id="77e6b-216">资源</span><span class="sxs-lookup"><span data-stu-id="77e6b-216">Resource</span></span>      | <span data-ttu-id="77e6b-217">每个租户每个应用限制</span><span class="sxs-lookup"><span data-stu-id="77e6b-217">Limits per app per tenant</span></span>    |
| -------------- | ------------ |
| [<span data-ttu-id="77e6b-218">通话</span><span class="sxs-lookup"><span data-stu-id="77e6b-218">Calls</span></span>](/graph/api/resources/call) | <span data-ttu-id="77e6b-219">每月10,000 通通话和 100 通并发通话</span><span class="sxs-lookup"><span data-stu-id="77e6b-219">10,000 calls/month and 100 concurrent calls</span></span>   |
| [<span data-ttu-id="77e6b-220">会议信息</span><span class="sxs-lookup"><span data-stu-id="77e6b-220">Meeting information</span></span>](/graph/api/resources/meetinginfo)   | <span data-ttu-id="77e6b-221">每月每位用家会有 2000 则会议</span><span class="sxs-lookup"><span data-stu-id="77e6b-221">2000 meetings/user each month</span></span> |
| <span data-ttu-id="77e6b-222">[状态](/graph/api/resources/presence)（预览版）</span><span class="sxs-lookup"><span data-stu-id="77e6b-222">[Presence](/graph/api/resources/presence) (preview)</span></span>   | <span data-ttu-id="77e6b-223">2 rps</span><span class="sxs-lookup"><span data-stu-id="77e6b-223">2 rps</span></span> |

### <a name="project-rome-service-limits"></a><span data-ttu-id="77e6b-224">Project Rome 服务限制</span><span class="sxs-lookup"><span data-stu-id="77e6b-224">Project Rome service limits</span></span>

<span data-ttu-id="77e6b-225">| 请求类型 | 所有应用的每个用户限制 | | GET          | 每 5 分钟 400 个请求，每 1 天 12000 个请求 | | POST、PUT、PATCH、DELETE | 每 5 分钟 100 个请求，每 1 天 8000 个请求 |</span><span class="sxs-lookup"><span data-stu-id="77e6b-225">| Request type | Limit per user for all apps | | GET          | 400 requests per 5 minutes and 12000 requests per 1 day | | POST, PUT, PATCH, DELETE | 100 requests per 5 minutes and 8000 requests per 1 day |</span></span>

<span data-ttu-id="77e6b-226">上述限制适用于下列资源:</span><span class="sxs-lookup"><span data-stu-id="77e6b-226">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="77e6b-227">activityHistoryItem、userActivity</span><span class="sxs-lookup"><span data-stu-id="77e6b-227">activityHistoryItem, userActivity</span></span>

### <a name="microsoft-teams-service-limits"></a><span data-ttu-id="77e6b-228">Microsoft Teams 服务限制</span><span class="sxs-lookup"><span data-stu-id="77e6b-228">Microsoft Teams service limits</span></span>

<span data-ttu-id="77e6b-229">限制表示为每秒请求数 (rps)。</span><span class="sxs-lookup"><span data-stu-id="77e6b-229">Limits are expressed as requests per second (rps).</span></span>

| <span data-ttu-id="77e6b-230">Teams 请求类型</span><span class="sxs-lookup"><span data-stu-id="77e6b-230">Teams request type</span></span>                                   | <span data-ttu-id="77e6b-231">每个租户每个应用限制</span><span class="sxs-lookup"><span data-stu-id="77e6b-231">Limit per app per tenant</span></span>        | <span data-ttu-id="77e6b-232">所有租户中的每个应用限制</span><span class="sxs-lookup"><span data-stu-id="77e6b-232">Limit per app across all tenants</span></span>      |
|------------------------------------------------------|---------------------------------|------------|
| <span data-ttu-id="77e6b-233">Microsoft Teams 的任何图形 API 调用</span><span class="sxs-lookup"><span data-stu-id="77e6b-233">Any Graph API calls for Microsoft Teams</span></span>              | <span data-ttu-id="77e6b-234">每 10 秒 15000 个请求</span><span class="sxs-lookup"><span data-stu-id="77e6b-234">15000 requests every 10 seconds</span></span> | <span data-ttu-id="77e6b-235">不适用</span><span class="sxs-lookup"><span data-stu-id="77e6b-235">n/a</span></span> |
| <span data-ttu-id="77e6b-236">GET team, channel, tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="77e6b-236">GET team, channel, tab, installedApps, appCatalogs</span></span>   | <span data-ttu-id="77e6b-237">60 rps</span><span class="sxs-lookup"><span data-stu-id="77e6b-237">60 rps</span></span>                          | <span data-ttu-id="77e6b-238">600 rps</span><span class="sxs-lookup"><span data-stu-id="77e6b-238">600 rps</span></span> |
| <span data-ttu-id="77e6b-239">POST/PUT channel, tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="77e6b-239">POST/PUT channel, tab, installedApps, appCatalogs</span></span>    |  <span data-ttu-id="77e6b-240">30 rps</span><span class="sxs-lookup"><span data-stu-id="77e6b-240">30 rps</span></span>                         | <span data-ttu-id="77e6b-241">300 rps</span><span class="sxs-lookup"><span data-stu-id="77e6b-241">300 rps</span></span>  |
| <span data-ttu-id="77e6b-242">PATCH team, channel, tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="77e6b-242">PATCH team, channel, tab, installedApps, appCatalogs</span></span> |  <span data-ttu-id="77e6b-243">30 rps</span><span class="sxs-lookup"><span data-stu-id="77e6b-243">30 rps</span></span>                         | <span data-ttu-id="77e6b-244">300 rps</span><span class="sxs-lookup"><span data-stu-id="77e6b-244">300 rps</span></span>  |
| <span data-ttu-id="77e6b-245">DELETE channel, tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="77e6b-245">DELETE channel, tab, installedApps, appCatalogs</span></span>      |  <span data-ttu-id="77e6b-246">15 rps</span><span class="sxs-lookup"><span data-stu-id="77e6b-246">15 rps</span></span>                         | <span data-ttu-id="77e6b-247">150 rps</span><span class="sxs-lookup"><span data-stu-id="77e6b-247">150 rps</span></span>  |
| <span data-ttu-id="77e6b-248">GET /teams/```{team-id}```, joinedTeams</span><span class="sxs-lookup"><span data-stu-id="77e6b-248">GET /teams/```{team-id}```, joinedTeams</span></span>              |  <span data-ttu-id="77e6b-249">30 rps</span><span class="sxs-lookup"><span data-stu-id="77e6b-249">30 rps</span></span>                         | <span data-ttu-id="77e6b-250">300 rps</span><span class="sxs-lookup"><span data-stu-id="77e6b-250">300 rps</span></span>  |
| <span data-ttu-id="77e6b-251">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, clone</span><span class="sxs-lookup"><span data-stu-id="77e6b-251">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, clone</span></span> | <span data-ttu-id="77e6b-252">6 rps</span><span class="sxs-lookup"><span data-stu-id="77e6b-252">6 rps</span></span> | <span data-ttu-id="77e6b-253">150 rps</span><span class="sxs-lookup"><span data-stu-id="77e6b-253">150 rps</span></span>  | 
| <span data-ttu-id="77e6b-254">GET channel message</span><span class="sxs-lookup"><span data-stu-id="77e6b-254">GET channel message</span></span>  | <span data-ttu-id="77e6b-255">5 rps</span><span class="sxs-lookup"><span data-stu-id="77e6b-255">5 rps</span></span> | <span data-ttu-id="77e6b-256">100 rps</span><span class="sxs-lookup"><span data-stu-id="77e6b-256">100 rps</span></span> |
| <span data-ttu-id="77e6b-257">GET 1:1/group chat message</span><span class="sxs-lookup"><span data-stu-id="77e6b-257">GET 1:1/group chat message</span></span>  | <span data-ttu-id="77e6b-258">3 rps</span><span class="sxs-lookup"><span data-stu-id="77e6b-258">3 rps</span></span> | <span data-ttu-id="77e6b-259">30 rps</span><span class="sxs-lookup"><span data-stu-id="77e6b-259">30 rps</span></span> |
| <span data-ttu-id="77e6b-260">POST channel message</span><span class="sxs-lookup"><span data-stu-id="77e6b-260">POST channel message</span></span> | <span data-ttu-id="77e6b-261">2 rps</span><span class="sxs-lookup"><span data-stu-id="77e6b-261">2 rps</span></span> | <span data-ttu-id="77e6b-262">20 rps</span><span class="sxs-lookup"><span data-stu-id="77e6b-262">20 rps</span></span> |
| <span data-ttu-id="77e6b-263">POST 1:1/group chat message</span><span class="sxs-lookup"><span data-stu-id="77e6b-263">POST 1:1/group chat message</span></span> | <span data-ttu-id="77e6b-264">2 rps</span><span class="sxs-lookup"><span data-stu-id="77e6b-264">2 rps</span></span> | <span data-ttu-id="77e6b-265">20 rps</span><span class="sxs-lookup"><span data-stu-id="77e6b-265">20 rps</span></span> |
| <span data-ttu-id="77e6b-266">GET/teams/```{team-id}```/在以下路径下的日程安排和所有 API</span><span class="sxs-lookup"><span data-stu-id="77e6b-266">GET /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="77e6b-267">60 rps</span><span class="sxs-lookup"><span data-stu-id="77e6b-267">60 rps</span></span> | <span data-ttu-id="77e6b-268">600 rps</span><span class="sxs-lookup"><span data-stu-id="77e6b-268">600 rps</span></span> |
| <span data-ttu-id="77e6b-269">POST, PATCH, PUT /teams/```{team-id}```/在以下路径下的日程安排和所有 API</span><span class="sxs-lookup"><span data-stu-id="77e6b-269">POST, PATCH, PUT /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="77e6b-270">30 rps</span><span class="sxs-lookup"><span data-stu-id="77e6b-270">30 rps</span></span> | <span data-ttu-id="77e6b-271">300 rps</span><span class="sxs-lookup"><span data-stu-id="77e6b-271">300 rps</span></span> |
| <span data-ttu-id="77e6b-272">DELETE /teams/```{team-id}```/在以下路径下的日程安排和所有 API</span><span class="sxs-lookup"><span data-stu-id="77e6b-272">DELETE /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="77e6b-273">15 rps</span><span class="sxs-lookup"><span data-stu-id="77e6b-273">15 rps</span></span> | <span data-ttu-id="77e6b-274">150 rps</span><span class="sxs-lookup"><span data-stu-id="77e6b-274">150 rps</span></span> |

<span data-ttu-id="77e6b-275">对于给定团队或频道，每个应用最多可发布 4 个请求。</span><span class="sxs-lookup"><span data-stu-id="77e6b-275">A maximum of 4 requests per second per app can be issued on a given team or channel.</span></span>
<span data-ttu-id="77e6b-276">每个应用每天最多可以将 3000 条消息发送到给定的频道。</span><span class="sxs-lookup"><span data-stu-id="77e6b-276">A maximum of 3000 messages per app per day can be sent to a given channel.</span></span>

<span data-ttu-id="77e6b-277">另请参阅 [Microsoft Teams 限制](/graph/api/resources/teams-api-overview#microsoft-teams-limits)和[投票要求](/graph/api/resources/teams-api-overview#polling-requirements)。</span><span class="sxs-lookup"><span data-stu-id="77e6b-277">See also [Microsoft Teams limits](/graph/api/resources/teams-api-overview#microsoft-teams-limits) and [polling requirements](/graph/api/resources/teams-api-overview#polling-requirements).</span></span>

### <a name="information-protection"></a><span data-ttu-id="77e6b-278">信息保护</span><span class="sxs-lookup"><span data-stu-id="77e6b-278">Information protection</span></span>

<span data-ttu-id="77e6b-279">以下限制适用于 `/informationProtection` 上的所有请求。</span><span class="sxs-lookup"><span data-stu-id="77e6b-279">The following limits apply to any request on `/informationProtection`.</span></span>

| <span data-ttu-id="77e6b-280">操作</span><span class="sxs-lookup"><span data-stu-id="77e6b-280">Operation</span></span>                 | <span data-ttu-id="77e6b-281">每个租户的使用限制</span><span class="sxs-lookup"><span data-stu-id="77e6b-281">Limit per tenant</span></span>                                            | <span data-ttu-id="77e6b-282">每个资源（电子邮件、URL、文件）的使用限制</span><span class="sxs-lookup"><span data-stu-id="77e6b-282">Limit per resource (email, URL, file)</span></span>                |
|---------------------------|-------------------------------------------------------------|------------------------------------------------------|
| <span data-ttu-id="77e6b-283">POST</span><span class="sxs-lookup"><span data-stu-id="77e6b-283">POST</span></span>                      | <span data-ttu-id="77e6b-284">每 15 分钟 150 个请求和每 24 小时 10000 个请求</span><span class="sxs-lookup"><span data-stu-id="77e6b-284">150 requests per 15 minutes and 10000 requests per 24 hours</span></span> | <span data-ttu-id="77e6b-285">每 15 分钟 1 个请求和每 24 小时 3 个请求</span><span class="sxs-lookup"><span data-stu-id="77e6b-285">1 request per 15 minutes and 3 requests per 24 hours</span></span> |

<span data-ttu-id="77e6b-286">上述限制适用于下列资源:</span><span class="sxs-lookup"><span data-stu-id="77e6b-286">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="77e6b-287">threatAssessmentRequest、threatAssessmentResult、mailAssessmentRequest、emailFileAssessmentRequest、fileAssessmentRequest、urlAssessmentRequest。</span><span class="sxs-lookup"><span data-stu-id="77e6b-287">threatAssessmentRequest, threatAssessmentResult, mailAssessmentRequest, emailFileAssessmentRequest, fileAssessmentRequest, urlAssessmentRequest.</span></span>

### <a name="identity-protection-and-conditional-access-service-limits"></a><span data-ttu-id="77e6b-288">身份保护和条件访问服务限制</span><span class="sxs-lookup"><span data-stu-id="77e6b-288">Identity protection and conditional access service limits</span></span>

| <span data-ttu-id="77e6b-289">请求类型</span><span class="sxs-lookup"><span data-stu-id="77e6b-289">Request type</span></span> | <span data-ttu-id="77e6b-290">每个租户的使用限制</span><span class="sxs-lookup"><span data-stu-id="77e6b-290">Limit per tenant</span></span> |
| ------------ | ------- |
| <span data-ttu-id="77e6b-291">任何</span><span class="sxs-lookup"><span data-stu-id="77e6b-291">Any</span></span> | <span data-ttu-id="77e6b-292">每秒1个请求</span><span class="sxs-lookup"><span data-stu-id="77e6b-292">1 request per second</span></span> |

<span data-ttu-id="77e6b-293">上述限制适用于下列资源:</span><span class="sxs-lookup"><span data-stu-id="77e6b-293">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="77e6b-294">riskDetection, riskyUser, riskyUserHistoryItem, namedLocation, countryNamedLocation, ipNamedLocation, conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="77e6b-294">riskDetection, riskyUser, riskyUserHistoryItem, namedLocation, countryNamedLocation, ipNamedLocation, conditionalAccessPolicy.</span></span>

> <span data-ttu-id="77e6b-295">**备注:** 目前上面列出的资源没有返回`Retry-After`页眉`429 Too Many Requests`上答复。</span><span class="sxs-lookup"><span data-stu-id="77e6b-295">**Note:** at the moment the resources listed above do not return a `Retry-After` header on `429 Too Many Requests` responses.</span></span>

### <a name="insights-service-limits"></a><span data-ttu-id="77e6b-296">见解服务限制</span><span class="sxs-lookup"><span data-stu-id="77e6b-296">Insights service limits</span></span>

<span data-ttu-id="77e6b-297">以下限制适用于 `me/insights`或`users/{id}/insights` 上的所有请求。</span><span class="sxs-lookup"><span data-stu-id="77e6b-297">The following limits apply to any request on `me/insights` or `users/{id}/insights`.</span></span>

| <span data-ttu-id="77e6b-298">限制</span><span class="sxs-lookup"><span data-stu-id="77e6b-298">Limit</span></span>                                                      | <span data-ttu-id="77e6b-299">适用对象</span><span class="sxs-lookup"><span data-stu-id="77e6b-299">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="77e6b-300">10 分钟内的 10,000 个 API 请求</span><span class="sxs-lookup"><span data-stu-id="77e6b-300">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="77e6b-301">v1.0 和 beta 终结点</span><span class="sxs-lookup"><span data-stu-id="77e6b-301">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="77e6b-302">4 个并发请求</span><span class="sxs-lookup"><span data-stu-id="77e6b-302">4 concurrent requests</span></span>                                      | <span data-ttu-id="77e6b-303">v1.0 和 beta 终结点</span><span class="sxs-lookup"><span data-stu-id="77e6b-303">v1.0 and beta endpoints</span></span>   |

### <a name="microsoft-graph-reports-service-limits"></a><span data-ttu-id="77e6b-304">Microsoft Graph 报告的服务限制</span><span class="sxs-lookup"><span data-stu-id="77e6b-304">Microsoft Graph reports service limits</span></span>

<span data-ttu-id="77e6b-305">以下限制适用于 `/reports` 上的所有请求。</span><span class="sxs-lookup"><span data-stu-id="77e6b-305">The following limits apply to any request on `/reports`.</span></span>

| <span data-ttu-id="77e6b-306">操作</span><span class="sxs-lookup"><span data-stu-id="77e6b-306">Operation</span></span>                 | <span data-ttu-id="77e6b-307">每个租户每个应用限制</span><span class="sxs-lookup"><span data-stu-id="77e6b-307">Limit per app per tenant</span></span>     | <span data-ttu-id="77e6b-308">每个租户的使用限制</span><span class="sxs-lookup"><span data-stu-id="77e6b-308">Limit per tenant</span></span>           |
|---------------------------|------------------------------|----------------------------|
| <span data-ttu-id="77e6b-309">任何请求（CSV）</span><span class="sxs-lookup"><span data-stu-id="77e6b-309">Any request (CSV)</span></span>         | <span data-ttu-id="77e6b-310">每10分钟14个请求</span><span class="sxs-lookup"><span data-stu-id="77e6b-310">14 requests per 10 minutes</span></span>   | <span data-ttu-id="77e6b-311">每10分钟40个请求</span><span class="sxs-lookup"><span data-stu-id="77e6b-311">40 requests per 10 minutes</span></span> |
| <span data-ttu-id="77e6b-312">任何请求（JSON、beta）</span><span class="sxs-lookup"><span data-stu-id="77e6b-312">Any request (JSON, beta)</span></span>  | <span data-ttu-id="77e6b-313">每10分钟100个请求</span><span class="sxs-lookup"><span data-stu-id="77e6b-313">100 requests per 10 minutes</span></span>  | <span data-ttu-id="77e6b-314">不适用</span><span class="sxs-lookup"><span data-stu-id="77e6b-314">n/a</span></span>                        |

<span data-ttu-id="77e6b-315">上述限制分别适用于每个报表 API。</span><span class="sxs-lookup"><span data-stu-id="77e6b-315">The preceding limits apply individually to each report API.</span></span> <span data-ttu-id="77e6b-316">例如，在10分钟内分别有对 Microsoft Teams 用户活动报告API的请求及对 Outlook 用户活动报告API的请求，将分别被视为14个请求中的1个请求，而不是14个请求中的2个请求。</span><span class="sxs-lookup"><span data-stu-id="77e6b-316">For example a request to Microsoft Teams user activity report API and a request to Outlook user activity report API within 10 minutes will count as 1 request out of 14 for each API, not 2 requests out of 14 for both.</span></span>

### <a name="invitation-manager-service-limits"></a><span data-ttu-id="77e6b-317">邀请管理器服务限制</span><span class="sxs-lookup"><span data-stu-id="77e6b-317">Invitation manager service limits</span></span>

<span data-ttu-id="77e6b-318">以下限制适用于 `/invitations` 上的所有请求。</span><span class="sxs-lookup"><span data-stu-id="77e6b-318">The following limits apply to any request on `/invitations`.</span></span>

| <span data-ttu-id="77e6b-319">操作</span><span class="sxs-lookup"><span data-stu-id="77e6b-319">Operation</span></span>                 | <span data-ttu-id="77e6b-320">每个租户的使用限制</span><span class="sxs-lookup"><span data-stu-id="77e6b-320">Limit per tenant</span></span>             |
|---------------------------|------------------------------|
| <span data-ttu-id="77e6b-321">任何操作</span><span class="sxs-lookup"><span data-stu-id="77e6b-321">Any operation</span></span>             | <span data-ttu-id="77e6b-322">每 5 秒 150 个请求</span><span class="sxs-lookup"><span data-stu-id="77e6b-322">150 requests per 5 seconds</span></span>   |

### <a name="open-and-schema-extensions-service-limits"></a><span data-ttu-id="77e6b-323">开放和架构扩展服务限制</span><span class="sxs-lookup"><span data-stu-id="77e6b-323">Open and schema extensions service limits</span></span>

| <span data-ttu-id="77e6b-324">请求类型</span><span class="sxs-lookup"><span data-stu-id="77e6b-324">Request type</span></span> | <span data-ttu-id="77e6b-325">每个租户每个应用限制</span><span class="sxs-lookup"><span data-stu-id="77e6b-325">Limit per app per tenant</span></span> |
| ------------ | ------------------------ |
| <span data-ttu-id="77e6b-326">任何</span><span class="sxs-lookup"><span data-stu-id="77e6b-326">Any</span></span>          | <span data-ttu-id="77e6b-327">每 10 秒 455 个请求</span><span class="sxs-lookup"><span data-stu-id="77e6b-327">455 requests per 10 seconds</span></span> |

<span data-ttu-id="77e6b-328">上述限制适用于以下资源：openTypeExtension、schemaExtension、administrativeUnit、合同、设备、事件、组、消息、组织、帖子和用户。</span><span class="sxs-lookup"><span data-stu-id="77e6b-328">The preceding limits apply to the following resources: openTypeExtension, schemaExtension, administrativeUnit, contact, device, event, group, message, organization, post, and user.</span></span>

<!-- { "blockType": "throttlinggenstart" } -->
### <a name="education-service-limits"></a><span data-ttu-id="77e6b-329">教育版服务限制</span><span class="sxs-lookup"><span data-stu-id="77e6b-329">Education service limits</span></span>

[!INCLUDE [Education rostering APIS throttling documentation](../includes/throttling-education-rostering-apis.md)]

### <a name="excel-service-limits"></a><span data-ttu-id="77e6b-330">Excel 服务限制</span><span class="sxs-lookup"><span data-stu-id="77e6b-330">Excel service limits</span></span>

[!INCLUDE [Excel throttling documentation](../includes/throttling-excel.md)]

### <a name="identity-and-access-audit-logs-service-limits"></a><span data-ttu-id="77e6b-331">标识和访问审核日志的服务限制</span><span class="sxs-lookup"><span data-stu-id="77e6b-331">Identity and access audit logs service limits</span></span>

[!INCLUDE [Identity and access audit logs throttling documentation](../includes/throttling-Identity-and-access-audit-logs.md)]

### <a name="identity-providers-service-limits"></a><span data-ttu-id="77e6b-332">身份提供程序的服务限制</span><span class="sxs-lookup"><span data-stu-id="77e6b-332">Identity providers service limits</span></span>

[!INCLUDE [CPIM throttling documentation](../includes/throttling-cpim.md)]

### <a name="intune-service-limits"></a><span data-ttu-id="77e6b-333">Intune服务限制</span><span class="sxs-lookup"><span data-stu-id="77e6b-333">Intune service limits</span></span>

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

### <a name="skype-service-limits"></a><span data-ttu-id="77e6b-334">Skype 服务限制</span><span class="sxs-lookup"><span data-stu-id="77e6b-334">Skype service limits</span></span>

[!INCLUDE [Skype calling throttling documentation](../includes/throttling-skype-calling.md)]

### <a name="subscription-service-limits"></a><span data-ttu-id="77e6b-335">订阅服务</span><span class="sxs-lookup"><span data-stu-id="77e6b-335">Subscription service limits</span></span>

[!INCLUDE [Subscription services throttling documentation](../includes/throttling-subscription-services.md)]

<!-- { "blockType": "throttlinggenend" } -->
