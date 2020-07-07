---
title: Microsoft Graph 限制指南
description: Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 5561e8a28440f05adcd074b6cd7d4d61edbb2852
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050783"
---
# <a name="microsoft-graph-throttling-guidance"></a><span data-ttu-id="4ef04-105">Microsoft Graph 限制指南</span><span class="sxs-lookup"><span data-stu-id="4ef04-105">Microsoft Graph throttling guidance</span></span>

<span data-ttu-id="4ef04-106">Throttling limits the number of concurrent calls to a service to prevent overuse of resources.</span><span class="sxs-lookup"><span data-stu-id="4ef04-106">Throttling limits the number of concurrent calls to a service to prevent overuse of resources.</span></span> <span data-ttu-id="4ef04-107">Microsoft Graph is designed to handle a high volume of requests.</span><span class="sxs-lookup"><span data-stu-id="4ef04-107">Microsoft Graph is designed to handle a high volume of requests.</span></span> <span data-ttu-id="4ef04-108">If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span><span class="sxs-lookup"><span data-stu-id="4ef04-108">If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span></span>

<span data-ttu-id="4ef04-109">Throttling limits vary based on the scenario.</span><span class="sxs-lookup"><span data-stu-id="4ef04-109">Throttling limits vary based on the scenario.</span></span> <span data-ttu-id="4ef04-110">For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span><span class="sxs-lookup"><span data-stu-id="4ef04-110">For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span></span>

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a><span data-ttu-id="4ef04-111">在限制时，会发生什么情况？</span><span class="sxs-lookup"><span data-stu-id="4ef04-111">What happens when throttling occurs?</span></span>
<!-- markdownlint-enable MD026 -->

<span data-ttu-id="4ef04-112">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time.</span><span class="sxs-lookup"><span data-stu-id="4ef04-112">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time.</span></span> <span data-ttu-id="4ef04-113">When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail.</span><span class="sxs-lookup"><span data-stu-id="4ef04-113">When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail.</span></span> <span data-ttu-id="4ef04-114">A suggested wait time is returned in the response header of the failed request.</span><span class="sxs-lookup"><span data-stu-id="4ef04-114">A suggested wait time is returned in the response header of the failed request.</span></span> <span data-ttu-id="4ef04-115">Throttling behavior can depend on the type and number of requests.</span><span class="sxs-lookup"><span data-stu-id="4ef04-115">Throttling behavior can depend on the type and number of requests.</span></span> <span data-ttu-id="4ef04-116">For example, if you have a high volume of requests, all requests types are throttled.</span><span class="sxs-lookup"><span data-stu-id="4ef04-116">For example, if you have a high volume of requests, all requests types are throttled.</span></span> <span data-ttu-id="4ef04-117">Threshold limits vary based on the request type.</span><span class="sxs-lookup"><span data-stu-id="4ef04-117">Threshold limits vary based on the request type.</span></span> <span data-ttu-id="4ef04-118">Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span><span class="sxs-lookup"><span data-stu-id="4ef04-118">Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span>

## <a name="common-throttling-scenarios"></a><span data-ttu-id="4ef04-119">常见的限制场景</span><span class="sxs-lookup"><span data-stu-id="4ef04-119">Common throttling scenarios</span></span>

<span data-ttu-id="4ef04-120">客户端受限的最常见原因包括：</span><span class="sxs-lookup"><span data-stu-id="4ef04-120">The most common causes of throttling of clients include:</span></span>

- <span data-ttu-id="4ef04-121">来自租户中所有应用程序的请求太多。</span><span class="sxs-lookup"><span data-stu-id="4ef04-121">A large number of requests across all applications in a tenant.</span></span>
- <span data-ttu-id="4ef04-122">来自所有租户中特定应用程序的请求太多。</span><span class="sxs-lookup"><span data-stu-id="4ef04-122">A large number of requests from a particular application across all tenants.</span></span>

## <a name="best-practices-to-handle-throttling"></a><span data-ttu-id="4ef04-123">处理限制的最佳实践</span><span class="sxs-lookup"><span data-stu-id="4ef04-123">Best practices to handle throttling</span></span>

<span data-ttu-id="4ef04-124">以下是处理限制的最佳做法：</span><span class="sxs-lookup"><span data-stu-id="4ef04-124">The following are best practices for handling throttling:</span></span>

- <span data-ttu-id="4ef04-125">减少每个请求的操作数量。</span><span class="sxs-lookup"><span data-stu-id="4ef04-125">Reduce the number of operations per request.</span></span>
- <span data-ttu-id="4ef04-126">减少调用频率。</span><span class="sxs-lookup"><span data-stu-id="4ef04-126">Reduce the frequency of calls.</span></span>
- <span data-ttu-id="4ef04-127">不要立即重试，因为所有请求都会计入使用限制。</span><span class="sxs-lookup"><span data-stu-id="4ef04-127">Avoid immediate retries, because all requests accrue against your usage limits.</span></span>

<span data-ttu-id="4ef04-128">When you implement error handling, use the HTTP error code 429 to detect throttling.</span><span class="sxs-lookup"><span data-stu-id="4ef04-128">When you implement error handling, use the HTTP error code 429 to detect throttling.</span></span> <span data-ttu-id="4ef04-129">The failed response includes the `Retry-After` response header.</span><span class="sxs-lookup"><span data-stu-id="4ef04-129">The failed response includes the `Retry-After` response header.</span></span> <span data-ttu-id="4ef04-130">Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span><span class="sxs-lookup"><span data-stu-id="4ef04-130">Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span></span>

1. <span data-ttu-id="4ef04-131">等待 `Retry-After` 标头中指定的秒数。</span><span class="sxs-lookup"><span data-stu-id="4ef04-131">Wait the number of seconds specified in the `Retry-After` header.</span></span>
2. <span data-ttu-id="4ef04-132">请重试请求。</span><span class="sxs-lookup"><span data-stu-id="4ef04-132">Retry the request.</span></span>
3. <span data-ttu-id="4ef04-133">If the request fails again with a 429 error code, you are still being throttled.</span><span class="sxs-lookup"><span data-stu-id="4ef04-133">If the request fails again with a 429 error code, you are still being throttled.</span></span> <span data-ttu-id="4ef04-134">Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span><span class="sxs-lookup"><span data-stu-id="4ef04-134">Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span></span>

<span data-ttu-id="4ef04-135">下列资源目前提供 `Retry-After` 标头：</span><span class="sxs-lookup"><span data-stu-id="4ef04-135">The following resources currently provide a `Retry-After` header:</span></span>

- [<span data-ttu-id="4ef04-136">用户</span><span class="sxs-lookup"><span data-stu-id="4ef04-136">User</span></span>](/graph/api/resources/user?view=graph-rest-1.0)
- [<span data-ttu-id="4ef04-137">照片</span><span class="sxs-lookup"><span data-stu-id="4ef04-137">Photo</span></span>](/graph/api/resources/profilephoto?view=graph-rest-1.0)
- [<span data-ttu-id="4ef04-138">邮件</span><span class="sxs-lookup"><span data-stu-id="4ef04-138">Mail</span></span>](/graph/api/resources/message?view=graph-rest-1.0)
- [<span data-ttu-id="4ef04-139">日历（用户和组）</span><span class="sxs-lookup"><span data-stu-id="4ef04-139">Calendar (users and groups)</span></span>](/graph/api/resources/event?view=graph-rest-1.0)
- [<span data-ttu-id="4ef04-140">联系人</span><span class="sxs-lookup"><span data-stu-id="4ef04-140">Contact</span></span>](/graph/api/resources/contact?view=graph-rest-1.0)
- [<span data-ttu-id="4ef04-141">附件</span><span class="sxs-lookup"><span data-stu-id="4ef04-141">Attachment</span></span>](/graph/api/resources/attachment?view=graph-rest-1.0)
- [<span data-ttu-id="4ef04-142">组对话</span><span class="sxs-lookup"><span data-stu-id="4ef04-142">Group conversations</span></span>](/graph/api/resources/conversation?view=graph-rest-1.0)
- [<span data-ttu-id="4ef04-143">人员和社交活动</span><span class="sxs-lookup"><span data-stu-id="4ef04-143">People and social</span></span>](/graph/api/resources/social-overview?view=graph-rest-beta)
- [<span data-ttu-id="4ef04-144">Drive (OneDrive)</span><span class="sxs-lookup"><span data-stu-id="4ef04-144">Drive (OneDrive)</span></span>](/graph/api/resources/drive?view=graph-rest-1.0)
- [<span data-ttu-id="4ef04-145">外部项（Microsoft 搜索）</span><span class="sxs-lookup"><span data-stu-id="4ef04-145">External item (Microsoft Search)</span></span>](/graph/api/resources/externalitem?view=graph-rest-beta)
- [<span data-ttu-id="4ef04-146">Report</span><span class="sxs-lookup"><span data-stu-id="4ef04-146">Report</span></span>](/graph/api/resources/report)
- [<span data-ttu-id="4ef04-147">订阅</span><span class="sxs-lookup"><span data-stu-id="4ef04-147">Subscription</span></span>](/graph/api/resources/subscription)
- [<span data-ttu-id="4ef04-148">趋势</span><span class="sxs-lookup"><span data-stu-id="4ef04-148">Trending</span></span>](/graph/api/resources/insights-trending)
- [<span data-ttu-id="4ef04-149">使用的洞察力</span><span class="sxs-lookup"><span data-stu-id="4ef04-149">Used insight</span></span>](/graph/api/resources/insights-used)
- [<span data-ttu-id="4ef04-150">共享洞察力</span><span class="sxs-lookup"><span data-stu-id="4ef04-150">Shared insight</span></span>](/graph/api/resources/insights-shared)
- [<span data-ttu-id="4ef04-151">用户设置</span><span class="sxs-lookup"><span data-stu-id="4ef04-151">User settings</span></span>](/graph/api/resources/usersettings)
- [<span data-ttu-id="4ef04-152">受到</span><span class="sxs-lookup"><span data-stu-id="4ef04-152">Invitation</span></span>](/graph/api/resources/invitation)

<span data-ttu-id="4ef04-153">有关 Microsoft 云限制的更广泛讨论，请参阅[限制模式](https://docs.microsoft.com/azure/architecture/patterns/throttling)。</span><span class="sxs-lookup"><span data-stu-id="4ef04-153">For a broader discussion of throttling on the Microsoft Cloud, see [Throttling Pattern](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span></span>

> [!NOTE]
> <span data-ttu-id="4ef04-154">如果响应未提供 `Retry-After` 标头，我们建议实施指数退避重试策略。</span><span class="sxs-lookup"><span data-stu-id="4ef04-154">If no `Retry-After` header is provided by the response, we recommend implementing an exponential backoff retry policy.</span></span> <span data-ttu-id="4ef04-155">构建大型应用程序时，还可以实现[更高级的模式](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency)。</span><span class="sxs-lookup"><span data-stu-id="4ef04-155">You can also implement [more advanced patterns](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) when building large-scale applications.</span></span>
>
> <span data-ttu-id="4ef04-156">Microsoft Graph SDK 已实施依赖于 `Retry-After` 标头或默认为指数退避重试策略的处理程序。</span><span class="sxs-lookup"><span data-stu-id="4ef04-156">Microsoft Graph SDKs already implement handlers that rely on the `Retry-After` header or default to an exponential backoff retry policy.</span></span>

## <a name="best-practices-to-avoid-throttling"></a><span data-ttu-id="4ef04-157">避免限制的最佳做法</span><span class="sxs-lookup"><span data-stu-id="4ef04-157">Best practices to avoid throttling</span></span>

<span data-ttu-id="4ef04-158">如持续轮询资源以检查更新以及定期扫描资源集合以检查新资源或已删除资源之类的编程模式，更有可能导致应用程序受到限制并降低整体性能。</span><span class="sxs-lookup"><span data-stu-id="4ef04-158">Programming patterns like continuously polling a resource to check for updates and regularly scanning resource collections to check for new or deleted resources are more likely to lead to applications being throttled and degrade overall performances.</span></span> <span data-ttu-id="4ef04-159">如果可用，改为使用[更改跟踪](delta-query-overview.md)并[更改通知](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="4ef04-159">You should instead leverage [change tracking](delta-query-overview.md) and [change notifications](webhooks.md) when available.</span></span>

>[!NOTE]
><span data-ttu-id="4ef04-160">[大规模发现文件和检测更改的最佳做法](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online)详细介绍最佳做法。</span><span class="sxs-lookup"><span data-stu-id="4ef04-160">[Best practices for discovering files and detecting changes at scale](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online) describes best practices in details.</span></span>

## <a name="service-specific-limits"></a><span data-ttu-id="4ef04-161">服务特定限制</span><span class="sxs-lookup"><span data-stu-id="4ef04-161">Service-specific limits</span></span>

<span data-ttu-id="4ef04-162">借助 Microsoft Graph，用户可访问[多个服务](overview-major-services.md)中的数据，如 Outlook 或 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="4ef04-162">Microsoft Graph allows you to access data in [multiple services](overview-major-services.md), such as Outlook or Azure Active Directory.</span></span> <span data-ttu-id="4ef04-163">这些服务实施自己的限制，这些限制会影响使用 Microsoft Graph 访问它们的应用程序。</span><span class="sxs-lookup"><span data-stu-id="4ef04-163">These services impose their own throttling limits that affect applications that use Microsoft Graph to access them.</span></span>

> [!NOTE]
> <span data-ttu-id="4ef04-164">此处所述的具体限制可能会发生更改。</span><span class="sxs-lookup"><span data-stu-id="4ef04-164">The specific limits described here are subject to change.</span></span>

> <span data-ttu-id="4ef04-165">**注意：** 在本节中，术语 "*租户*" 是指安装了应用程序的 Microsoft 365 组织。</span><span class="sxs-lookup"><span data-stu-id="4ef04-165">**Note:** In this section, the term *tenant* refers to the Microsoft 365 organization where the application is installed.</span></span> <span data-ttu-id="4ef04-166">此租户可以与创建应用程序的位置相同，在单个租户应用程序中也可以是不同的，如果是[多租户应用程序](/azure/active-directory/develop/setup-multi-tenant-app)，则也可以是不同的。</span><span class="sxs-lookup"><span data-stu-id="4ef04-166">This tenant can be the same as the the one where the application was created, in the case of a single tenant application, or it can be different, in the case of a [multi-tenant application](/azure/active-directory/develop/setup-multi-tenant-app).</span></span>

### <a name="outlook-service-limits"></a><span data-ttu-id="4ef04-167">Outlook 服务限制</span><span class="sxs-lookup"><span data-stu-id="4ef04-167">Outlook service limits</span></span>

<span data-ttu-id="4ef04-168">将评估每个应用 ID 和邮箱组合的 Outlook 服务限制。</span><span class="sxs-lookup"><span data-stu-id="4ef04-168">Outlook service limits are evaluated for each app ID and mailbox combination.</span></span> <span data-ttu-id="4ef04-169">换言之，上述限制适用于访问特定邮箱（用户或组）的特定应用。</span><span class="sxs-lookup"><span data-stu-id="4ef04-169">In other words, the limits described apply to a specific app accessing a specific mailbox (user or group).</span></span> <span data-ttu-id="4ef04-170">如果一个邮箱的应用程序超过限制，不会影响访问另一个邮箱的功能。</span><span class="sxs-lookup"><span data-stu-id="4ef04-170">If an application exceeds the limit in one mailbox, it does not affect the ability to access another mailbox.</span></span> <span data-ttu-id="4ef04-171">以下限制适用于公共云以及[国内云部署](/graph/deployments)。</span><span class="sxs-lookup"><span data-stu-id="4ef04-171">The following limits apply to the public cloud as well as [national cloud deployments](/graph/deployments).</span></span>

| <span data-ttu-id="4ef04-172">限制</span><span class="sxs-lookup"><span data-stu-id="4ef04-172">Limit</span></span>                                                      | <span data-ttu-id="4ef04-173">适用对象</span><span class="sxs-lookup"><span data-stu-id="4ef04-173">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="4ef04-174">10 分钟内的 10,000 个 API 请求</span><span class="sxs-lookup"><span data-stu-id="4ef04-174">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="4ef04-175">v1.0 和 beta 终结点</span><span class="sxs-lookup"><span data-stu-id="4ef04-175">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="4ef04-176">4 个并发请求</span><span class="sxs-lookup"><span data-stu-id="4ef04-176">4 concurrent requests</span></span>                                      | <span data-ttu-id="4ef04-177">v1.0 和 beta 终结点</span><span class="sxs-lookup"><span data-stu-id="4ef04-177">v1.0 and beta endpoints</span></span>   |
| <span data-ttu-id="4ef04-178">在30秒内，将15兆字节（MB）上传（PATCH、POST、PUT）</span><span class="sxs-lookup"><span data-stu-id="4ef04-178">15 megabytes (MB) upload (PATCH, POST, PUT) in a 30 second period</span></span> | <span data-ttu-id="4ef04-179">v1.0 和 beta 终结点</span><span class="sxs-lookup"><span data-stu-id="4ef04-179">v1.0 and beta endpoints</span></span>   |

#### <a name="outlook-service-resources"></a><span data-ttu-id="4ef04-180">Outlook 服务资源</span><span class="sxs-lookup"><span data-stu-id="4ef04-180">Outlook service resources</span></span>

<span data-ttu-id="4ef04-181">Outlook 服务提供以下资源。</span><span class="sxs-lookup"><span data-stu-id="4ef04-181">The following resources are provided by the Outlook service.</span></span>

##### <a name="calendar-api-resources"></a><span data-ttu-id="4ef04-182">日历 API 资源</span><span class="sxs-lookup"><span data-stu-id="4ef04-182">Calendar API resources</span></span>

- [<span data-ttu-id="4ef04-183">event</span><span class="sxs-lookup"><span data-stu-id="4ef04-183">event</span></span>](/graph/api/resources/event)
- [<span data-ttu-id="4ef04-184">eventMessage</span><span class="sxs-lookup"><span data-stu-id="4ef04-184">eventMessage</span></span>](/graph/api/resources/eventmessage)
- [<span data-ttu-id="4ef04-185">calendar</span><span class="sxs-lookup"><span data-stu-id="4ef04-185">calendar</span></span>](/graph/api/resources/calendar)
- [<span data-ttu-id="4ef04-186">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="4ef04-186">calendarGroup</span></span>](/graph/api/resources/calendargroup)
- [<span data-ttu-id="4ef04-187">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="4ef04-187">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="4ef04-188">attachment</span><span class="sxs-lookup"><span data-stu-id="4ef04-188">attachment</span></span>](/graph/api/resources/attachment)
- [<span data-ttu-id="4ef04-189">place（预览）</span><span class="sxs-lookup"><span data-stu-id="4ef04-189">place (preview)</span></span>](/graph/api/resources/place)

##### <a name="mail-api-resources"></a><span data-ttu-id="4ef04-190">邮件 API 资源</span><span class="sxs-lookup"><span data-stu-id="4ef04-190">Mail API resources</span></span>

- [<span data-ttu-id="4ef04-191">message</span><span class="sxs-lookup"><span data-stu-id="4ef04-191">message</span></span>](/graph/api/resources/message)
- [<span data-ttu-id="4ef04-192">mailFolder</span><span class="sxs-lookup"><span data-stu-id="4ef04-192">mailFolder</span></span>](/graph/api/resources/mailfolder)
- [<span data-ttu-id="4ef04-193">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="4ef04-193">mailSearchFolder</span></span>](/graph/api/resources/mailsearchfolder)
- [<span data-ttu-id="4ef04-194">messageRule</span><span class="sxs-lookup"><span data-stu-id="4ef04-194">messageRule</span></span>](/graph/api/resources/messagerule)
- [<span data-ttu-id="4ef04-195">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="4ef04-195">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="4ef04-196">attachment</span><span class="sxs-lookup"><span data-stu-id="4ef04-196">attachment</span></span>](/graph/api/resources/attachment)

##### <a name="personal-contacts-api-resources"></a><span data-ttu-id="4ef04-197">个人联系人 API 资源</span><span class="sxs-lookup"><span data-stu-id="4ef04-197">Personal contacts API resources</span></span>

- [<span data-ttu-id="4ef04-198">contact</span><span class="sxs-lookup"><span data-stu-id="4ef04-198">contact</span></span>](/graph/api/resources/contact)
- [<span data-ttu-id="4ef04-199">contactFolder</span><span class="sxs-lookup"><span data-stu-id="4ef04-199">contactFolder</span></span>](/graph/api/resources/contactfolder)
- [<span data-ttu-id="4ef04-200">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="4ef04-200">outlookCategory</span></span>](/graph/api/resources/outlookcategory)

##### <a name="social-and-workplace-intelligence-resources"></a><span data-ttu-id="4ef04-201">社交和工作区智能资源</span><span class="sxs-lookup"><span data-stu-id="4ef04-201">Social and workplace intelligence resources</span></span>

- [<span data-ttu-id="4ef04-202">person</span><span class="sxs-lookup"><span data-stu-id="4ef04-202">person</span></span>](/graph/api/resources/person)

##### <a name="to-do-tasks-api-preview-resources"></a><span data-ttu-id="4ef04-203">待办任务 API（预览）资源</span><span class="sxs-lookup"><span data-stu-id="4ef04-203">To-do tasks API (preview) resources</span></span>

- [<span data-ttu-id="4ef04-204">outlookTask</span><span class="sxs-lookup"><span data-stu-id="4ef04-204">outlookTask</span></span>](/graph/api/resources/outlooktask)
- [<span data-ttu-id="4ef04-205">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="4ef04-205">outlookTaskFolder</span></span>](/graph/api/resources/outlooktaskfolder)
- [<span data-ttu-id="4ef04-206">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="4ef04-206">outlookTaskGroup</span></span>](/graph/api/resources/outlooktaskgroup)
- [<span data-ttu-id="4ef04-207">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="4ef04-207">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="4ef04-208">attachment</span><span class="sxs-lookup"><span data-stu-id="4ef04-208">attachment</span></span>](/graph/api/resources/attachment)

### <a name="cloud-communication-service-limits"></a><span data-ttu-id="4ef04-209">云通信服务限制</span><span class="sxs-lookup"><span data-stu-id="4ef04-209">Cloud communication service limits</span></span>

| <span data-ttu-id="4ef04-210">资源</span><span class="sxs-lookup"><span data-stu-id="4ef04-210">Resource</span></span>      | <span data-ttu-id="4ef04-211">每个租户每个应用程序的限制</span><span class="sxs-lookup"><span data-stu-id="4ef04-211">Limits per app per tenant</span></span>    |
| -------------- | ------------ |
| [<span data-ttu-id="4ef04-212">呼叫</span><span class="sxs-lookup"><span data-stu-id="4ef04-212">Calls</span></span>](/graph/api/resources/call) | <span data-ttu-id="4ef04-213">10000呼叫/月和100并发呼叫</span><span class="sxs-lookup"><span data-stu-id="4ef04-213">10,000 calls/month and 100 concurrent calls</span></span>   |
| [<span data-ttu-id="4ef04-214">会议信息</span><span class="sxs-lookup"><span data-stu-id="4ef04-214">Meeting information</span></span>](/graph/api/resources/meetinginfo)   | <span data-ttu-id="4ef04-215">每月2000会议/用户</span><span class="sxs-lookup"><span data-stu-id="4ef04-215">2000 meetings/user each month</span></span> |
| <span data-ttu-id="4ef04-216">[状态](/graph/api/resources/presence)（预览）</span><span class="sxs-lookup"><span data-stu-id="4ef04-216">[Presence](/graph/api/resources/presence) (preview)</span></span>   | <span data-ttu-id="4ef04-217">2 rps</span><span class="sxs-lookup"><span data-stu-id="4ef04-217">2 rps</span></span> |

### <a name="microsoft-teams-service-limits"></a><span data-ttu-id="4ef04-218">Microsoft Teams 服务限制</span><span class="sxs-lookup"><span data-stu-id="4ef04-218">Microsoft Teams service limits</span></span>

<span data-ttu-id="4ef04-219">限制表示为每秒请求数 (rps)。</span><span class="sxs-lookup"><span data-stu-id="4ef04-219">Limits are expressed as requests per second (rps).</span></span>

| <span data-ttu-id="4ef04-220">Teams 请求类型</span><span class="sxs-lookup"><span data-stu-id="4ef04-220">Teams request type</span></span>                                   | <span data-ttu-id="4ef04-221">每个租户每个应用限制</span><span class="sxs-lookup"><span data-stu-id="4ef04-221">Limit per app per tenant</span></span>        | <span data-ttu-id="4ef04-222">所有租户中的每个应用限制</span><span class="sxs-lookup"><span data-stu-id="4ef04-222">Limit per app across all tenants</span></span>      |
|------------------------------------------------------|---------------------------------|------------|
| <span data-ttu-id="4ef04-223">Microsoft Teams 的任何图形 API 调用</span><span class="sxs-lookup"><span data-stu-id="4ef04-223">Any Graph API calls for Microsoft Teams</span></span>              | <span data-ttu-id="4ef04-224">每 10 秒 15000 个请求</span><span class="sxs-lookup"><span data-stu-id="4ef04-224">15000 requests every 10 seconds</span></span> | <span data-ttu-id="4ef04-225">不适用</span><span class="sxs-lookup"><span data-stu-id="4ef04-225">n/a</span></span> |
| <span data-ttu-id="4ef04-226">GET team, channel, tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="4ef04-226">GET team, channel, tab, installedApps, appCatalogs</span></span>   | <span data-ttu-id="4ef04-227">60 rps</span><span class="sxs-lookup"><span data-stu-id="4ef04-227">60 rps</span></span>                          | <span data-ttu-id="4ef04-228">600 rps</span><span class="sxs-lookup"><span data-stu-id="4ef04-228">600 rps</span></span> |
| <span data-ttu-id="4ef04-229">POST/PUT channel, tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="4ef04-229">POST/PUT channel, tab, installedApps, appCatalogs</span></span>    |  <span data-ttu-id="4ef04-230">30 rps</span><span class="sxs-lookup"><span data-stu-id="4ef04-230">30 rps</span></span>                         | <span data-ttu-id="4ef04-231">300 rps</span><span class="sxs-lookup"><span data-stu-id="4ef04-231">300 rps</span></span>  |
| <span data-ttu-id="4ef04-232">PATCH team, channel, tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="4ef04-232">PATCH team, channel, tab, installedApps, appCatalogs</span></span> |  <span data-ttu-id="4ef04-233">30 rps</span><span class="sxs-lookup"><span data-stu-id="4ef04-233">30 rps</span></span>                         | <span data-ttu-id="4ef04-234">300 rps</span><span class="sxs-lookup"><span data-stu-id="4ef04-234">300 rps</span></span>  |
| <span data-ttu-id="4ef04-235">DELETE channel, tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="4ef04-235">DELETE channel, tab, installedApps, appCatalogs</span></span>      |  <span data-ttu-id="4ef04-236">15 rps</span><span class="sxs-lookup"><span data-stu-id="4ef04-236">15 rps</span></span>                         | <span data-ttu-id="4ef04-237">150 rps</span><span class="sxs-lookup"><span data-stu-id="4ef04-237">150 rps</span></span>  |
| <span data-ttu-id="4ef04-238">GET /teams/```{team-id}```, joinedTeams</span><span class="sxs-lookup"><span data-stu-id="4ef04-238">GET /teams/```{team-id}```, joinedTeams</span></span>              |  <span data-ttu-id="4ef04-239">30 rps</span><span class="sxs-lookup"><span data-stu-id="4ef04-239">30 rps</span></span>                         | <span data-ttu-id="4ef04-240">300 rps</span><span class="sxs-lookup"><span data-stu-id="4ef04-240">300 rps</span></span>  |
| <span data-ttu-id="4ef04-241">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, clone</span><span class="sxs-lookup"><span data-stu-id="4ef04-241">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, clone</span></span> | <span data-ttu-id="4ef04-242">6 rps</span><span class="sxs-lookup"><span data-stu-id="4ef04-242">6 rps</span></span> | <span data-ttu-id="4ef04-243">150 rps</span><span class="sxs-lookup"><span data-stu-id="4ef04-243">150 rps</span></span>  | 
| <span data-ttu-id="4ef04-244">GET channel message</span><span class="sxs-lookup"><span data-stu-id="4ef04-244">GET channel message</span></span>  | <span data-ttu-id="4ef04-245">5 rps</span><span class="sxs-lookup"><span data-stu-id="4ef04-245">5 rps</span></span> | <span data-ttu-id="4ef04-246">100 rps</span><span class="sxs-lookup"><span data-stu-id="4ef04-246">100 rps</span></span> |
| <span data-ttu-id="4ef04-247">GET 1:1/group chat message</span><span class="sxs-lookup"><span data-stu-id="4ef04-247">GET 1:1/group chat message</span></span>  | <span data-ttu-id="4ef04-248">3 rps</span><span class="sxs-lookup"><span data-stu-id="4ef04-248">3 rps</span></span> | <span data-ttu-id="4ef04-249">30 rps</span><span class="sxs-lookup"><span data-stu-id="4ef04-249">30 rps</span></span> |
| <span data-ttu-id="4ef04-250">POST channel message</span><span class="sxs-lookup"><span data-stu-id="4ef04-250">POST channel message</span></span> | <span data-ttu-id="4ef04-251">2 rps</span><span class="sxs-lookup"><span data-stu-id="4ef04-251">2 rps</span></span> | <span data-ttu-id="4ef04-252">20 rps</span><span class="sxs-lookup"><span data-stu-id="4ef04-252">20 rps</span></span> |
| <span data-ttu-id="4ef04-253">POST 1:1/group chat message</span><span class="sxs-lookup"><span data-stu-id="4ef04-253">POST 1:1/group chat message</span></span> | <span data-ttu-id="4ef04-254">2 rps</span><span class="sxs-lookup"><span data-stu-id="4ef04-254">2 rps</span></span> | <span data-ttu-id="4ef04-255">20 rps</span><span class="sxs-lookup"><span data-stu-id="4ef04-255">20 rps</span></span> |
| <span data-ttu-id="4ef04-256">获取 ```{team-id}``` 此路径下的/teams//schedule 和所有 api</span><span class="sxs-lookup"><span data-stu-id="4ef04-256">GET /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="4ef04-257">60 rps</span><span class="sxs-lookup"><span data-stu-id="4ef04-257">60 rps</span></span> | <span data-ttu-id="4ef04-258">600 rps</span><span class="sxs-lookup"><span data-stu-id="4ef04-258">600 rps</span></span> |
| <span data-ttu-id="4ef04-259">POST、PATCH、PUT/teams/ ```{team-id}``` /schedule 和此路径下的所有 api</span><span class="sxs-lookup"><span data-stu-id="4ef04-259">POST, PATCH, PUT /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="4ef04-260">30 rps</span><span class="sxs-lookup"><span data-stu-id="4ef04-260">30 rps</span></span> | <span data-ttu-id="4ef04-261">300 rps</span><span class="sxs-lookup"><span data-stu-id="4ef04-261">300 rps</span></span> |
| <span data-ttu-id="4ef04-262">删除 ```{team-id}``` 此路径下的/teams//schedule 和所有 api</span><span class="sxs-lookup"><span data-stu-id="4ef04-262">DELETE /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="4ef04-263">15 rps</span><span class="sxs-lookup"><span data-stu-id="4ef04-263">15 rps</span></span> | <span data-ttu-id="4ef04-264">150 rps</span><span class="sxs-lookup"><span data-stu-id="4ef04-264">150 rps</span></span> |

<span data-ttu-id="4ef04-265">对于给定团队或频道，每个应用最多可发布 4 个请求。</span><span class="sxs-lookup"><span data-stu-id="4ef04-265">A maximum of 4 requests per second per app can be issued on a given team or channel.</span></span>
<span data-ttu-id="4ef04-266">每个应用每天最多可以将 3000 条消息发送到给定的频道。</span><span class="sxs-lookup"><span data-stu-id="4ef04-266">A maximum of 3000 messages per app per day can be sent to a given channel.</span></span>

<span data-ttu-id="4ef04-267">另请参阅 [Microsoft Teams 限制](/graph/api/resources/teams-api-overview#microsoft-teams-limits)和[投票要求](/graph/api/resources/teams-api-overview#polling-requirements)。</span><span class="sxs-lookup"><span data-stu-id="4ef04-267">See also [Microsoft Teams limits](/graph/api/resources/teams-api-overview#microsoft-teams-limits) and [polling requirements](/graph/api/resources/teams-api-overview#polling-requirements).</span></span>

### <a name="insights-service-limits"></a><span data-ttu-id="4ef04-268">Insights 服务限制</span><span class="sxs-lookup"><span data-stu-id="4ef04-268">Insights service limits</span></span>

<span data-ttu-id="4ef04-269">以下限制适用于或上的任何 `me/insights` 请求 `users/{id}/insights` 。</span><span class="sxs-lookup"><span data-stu-id="4ef04-269">The following limits apply to any request on `me/insights` or `users/{id}/insights`.</span></span>

| <span data-ttu-id="4ef04-270">限制</span><span class="sxs-lookup"><span data-stu-id="4ef04-270">Limit</span></span>                                                      | <span data-ttu-id="4ef04-271">适用对象</span><span class="sxs-lookup"><span data-stu-id="4ef04-271">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="4ef04-272">10 分钟内的 10,000 个 API 请求</span><span class="sxs-lookup"><span data-stu-id="4ef04-272">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="4ef04-273">v1.0 和 beta 终结点</span><span class="sxs-lookup"><span data-stu-id="4ef04-273">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="4ef04-274">4 个并发请求</span><span class="sxs-lookup"><span data-stu-id="4ef04-274">4 concurrent requests</span></span>                                      | <span data-ttu-id="4ef04-275">v1.0 和 beta 终结点</span><span class="sxs-lookup"><span data-stu-id="4ef04-275">v1.0 and beta endpoints</span></span>   |

### <a name="microsoft-graph-reports-service-limits"></a><span data-ttu-id="4ef04-276">Microsoft Graph 报告服务限制</span><span class="sxs-lookup"><span data-stu-id="4ef04-276">Microsoft Graph reports service limits</span></span>

<span data-ttu-id="4ef04-277">以下限制适用于 `/reports` 上的所有请求。</span><span class="sxs-lookup"><span data-stu-id="4ef04-277">The following limits apply to any request on `/reports`.</span></span>

| <span data-ttu-id="4ef04-278">操作</span><span class="sxs-lookup"><span data-stu-id="4ef04-278">Operation</span></span>                 | <span data-ttu-id="4ef04-279">每个租户每个应用限制</span><span class="sxs-lookup"><span data-stu-id="4ef04-279">Limit per app per tenant</span></span>     | <span data-ttu-id="4ef04-280">每个租户的限制</span><span class="sxs-lookup"><span data-stu-id="4ef04-280">Limit per tenant</span></span>           |
|---------------------------|------------------------------|----------------------------|
| <span data-ttu-id="4ef04-281">任何请求（CSV）</span><span class="sxs-lookup"><span data-stu-id="4ef04-281">Any request (CSV)</span></span>         | <span data-ttu-id="4ef04-282">每10分钟14个请求</span><span class="sxs-lookup"><span data-stu-id="4ef04-282">14 requests per 10 minutes</span></span>   | <span data-ttu-id="4ef04-283">每10分钟40个请求</span><span class="sxs-lookup"><span data-stu-id="4ef04-283">40 requests per 10 minutes</span></span> |
| <span data-ttu-id="4ef04-284">任何请求（JSON、beta）</span><span class="sxs-lookup"><span data-stu-id="4ef04-284">Any request (JSON, beta)</span></span>  | <span data-ttu-id="4ef04-285">每10分钟100个请求</span><span class="sxs-lookup"><span data-stu-id="4ef04-285">100 requests per 10 minutes</span></span>  | <span data-ttu-id="4ef04-286">不适用</span><span class="sxs-lookup"><span data-stu-id="4ef04-286">n/a</span></span>                        |

<span data-ttu-id="4ef04-287">上述限制将分别应用于每个报告 API。</span><span class="sxs-lookup"><span data-stu-id="4ef04-287">The preceding limits apply individually to each report API.</span></span> <span data-ttu-id="4ef04-288">例如，对 Microsoft 团队用户活动报告 API 的请求和在10分钟内对 Outlook 用户活动报告 API 的请求计数为每个 API 1 个请求（每个 API 一个14个），而不是两个请求都是14个。</span><span class="sxs-lookup"><span data-stu-id="4ef04-288">For example a request to Microsoft Teams user activity report API and a request to Outlook user activity report API within 10 minutes will count as 1 request out of 14 for each API, not 2 requests out of 14 for both.</span></span>

### <a name="invitation-manager-service-limits"></a><span data-ttu-id="4ef04-289">邀请管理器服务限制</span><span class="sxs-lookup"><span data-stu-id="4ef04-289">Invitation manager service limits</span></span>

<span data-ttu-id="4ef04-290">以下限制适用于 `/invitations` 上的所有请求。</span><span class="sxs-lookup"><span data-stu-id="4ef04-290">The following limits apply to any request on `/invitations`.</span></span>

| <span data-ttu-id="4ef04-291">操作</span><span class="sxs-lookup"><span data-stu-id="4ef04-291">Operation</span></span>                 | <span data-ttu-id="4ef04-292">每个租户的限制</span><span class="sxs-lookup"><span data-stu-id="4ef04-292">Limit per tenant</span></span>             |
|---------------------------|------------------------------|
| <span data-ttu-id="4ef04-293">任何操作</span><span class="sxs-lookup"><span data-stu-id="4ef04-293">Any operation</span></span>             | <span data-ttu-id="4ef04-294">每5秒150个请求</span><span class="sxs-lookup"><span data-stu-id="4ef04-294">150 requests per 5 seconds</span></span>   |

<!-- { "blockType": "throttlinggenstart" } -->

### <a name="education-service-limits"></a><span data-ttu-id="4ef04-295">教育服务限制</span><span class="sxs-lookup"><span data-stu-id="4ef04-295">Education service limits</span></span>

[!INCLUDE [Education rostering APIS throttling documentation](../includes/throttling-education-rostering-apis.md)]

### <a name="excel-service-limits"></a><span data-ttu-id="4ef04-296">Excel 服务限制</span><span class="sxs-lookup"><span data-stu-id="4ef04-296">Excel service limits</span></span>

[!INCLUDE [Excel throttling documentation](../includes/throttling-excel.md)]

### <a name="identity-and-access-audit-logs-service-limits"></a><span data-ttu-id="4ef04-297">标识和访问审核日志服务限制</span><span class="sxs-lookup"><span data-stu-id="4ef04-297">Identity and access audit logs service limits</span></span>

[!INCLUDE [Identity and access audit logs throttling documentation](../includes/throttling-Identity-and-access-audit-logs.md)]

### <a name="identity-providers-service-limits"></a><span data-ttu-id="4ef04-298">标识提供程序服务限制</span><span class="sxs-lookup"><span data-stu-id="4ef04-298">Identity providers service limits</span></span>

[!INCLUDE [CPIM throttling documentation](../includes/throttling-cpim.md)]

### <a name="intune-service-limits"></a><span data-ttu-id="4ef04-299">Intune 服务限制</span><span class="sxs-lookup"><span data-stu-id="4ef04-299">Intune service limits</span></span>

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

### <a name="skype-service-limits"></a><span data-ttu-id="4ef04-300">Skype 服务限制</span><span class="sxs-lookup"><span data-stu-id="4ef04-300">Skype service limits</span></span>

[!INCLUDE [Skype calling throttling documentation](../includes/throttling-skype-calling.md)]

### <a name="subscription-service-limits"></a><span data-ttu-id="4ef04-301">订阅服务限制</span><span class="sxs-lookup"><span data-stu-id="4ef04-301">Subscription service limits</span></span>

[!INCLUDE [Subscription services throttling documentation](../includes/throttling-subscription-services.md)]

<!-- { "blockType": "throttlinggenend" } -->
