---
title: Microsoft Graph 限制指南
description: Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 7678b364855381eaf5a138b42d6172a6cbd233f4
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "44989854"
---
# <a name="microsoft-graph-throttling-guidance"></a><span data-ttu-id="36013-105">Microsoft Graph 限制指南</span><span class="sxs-lookup"><span data-stu-id="36013-105">Microsoft Graph throttling guidance</span></span>

<span data-ttu-id="36013-106">Throttling limits the number of concurrent calls to a service to prevent overuse of resources.</span><span class="sxs-lookup"><span data-stu-id="36013-106">Throttling limits the number of concurrent calls to a service to prevent overuse of resources.</span></span> <span data-ttu-id="36013-107">Microsoft Graph is designed to handle a high volume of requests.</span><span class="sxs-lookup"><span data-stu-id="36013-107">Microsoft Graph is designed to handle a high volume of requests.</span></span> <span data-ttu-id="36013-108">If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span><span class="sxs-lookup"><span data-stu-id="36013-108">If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span></span>

<span data-ttu-id="36013-109">Throttling limits vary based on the scenario.</span><span class="sxs-lookup"><span data-stu-id="36013-109">Throttling limits vary based on the scenario.</span></span> <span data-ttu-id="36013-110">For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span><span class="sxs-lookup"><span data-stu-id="36013-110">For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span></span>

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a><span data-ttu-id="36013-111">在限制时，会发生什么情况？</span><span class="sxs-lookup"><span data-stu-id="36013-111">What happens when throttling occurs?</span></span>
<!-- markdownlint-enable MD026 -->

<span data-ttu-id="36013-112">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time.</span><span class="sxs-lookup"><span data-stu-id="36013-112">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time.</span></span> <span data-ttu-id="36013-113">When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail.</span><span class="sxs-lookup"><span data-stu-id="36013-113">When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail.</span></span> <span data-ttu-id="36013-114">A suggested wait time is returned in the response header of the failed request.</span><span class="sxs-lookup"><span data-stu-id="36013-114">A suggested wait time is returned in the response header of the failed request.</span></span> <span data-ttu-id="36013-115">Throttling behavior can depend on the type and number of requests.</span><span class="sxs-lookup"><span data-stu-id="36013-115">Throttling behavior can depend on the type and number of requests.</span></span> <span data-ttu-id="36013-116">For example, if you have a high volume of requests, all requests types are throttled.</span><span class="sxs-lookup"><span data-stu-id="36013-116">For example, if you have a high volume of requests, all requests types are throttled.</span></span> <span data-ttu-id="36013-117">Threshold limits vary based on the request type.</span><span class="sxs-lookup"><span data-stu-id="36013-117">Threshold limits vary based on the request type.</span></span> <span data-ttu-id="36013-118">Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span><span class="sxs-lookup"><span data-stu-id="36013-118">Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span>

## <a name="common-throttling-scenarios"></a><span data-ttu-id="36013-119">常见的限制场景</span><span class="sxs-lookup"><span data-stu-id="36013-119">Common throttling scenarios</span></span>

<span data-ttu-id="36013-120">客户端受限的最常见原因包括：</span><span class="sxs-lookup"><span data-stu-id="36013-120">The most common causes of throttling of clients include:</span></span>

- <span data-ttu-id="36013-121">来自租户中所有应用程序的请求太多。</span><span class="sxs-lookup"><span data-stu-id="36013-121">A large number of requests across all applications in a tenant.</span></span>
- <span data-ttu-id="36013-122">来自所有租户中特定应用程序的请求太多。</span><span class="sxs-lookup"><span data-stu-id="36013-122">A large number of requests from a particular application across all tenants.</span></span>

## <a name="best-practices-to-handle-throttling"></a><span data-ttu-id="36013-123">处理限制的最佳实践</span><span class="sxs-lookup"><span data-stu-id="36013-123">Best practices to handle throttling</span></span>

<span data-ttu-id="36013-124">以下是处理限制的最佳做法：</span><span class="sxs-lookup"><span data-stu-id="36013-124">The following are best practices for handling throttling:</span></span>

- <span data-ttu-id="36013-125">减少每个请求的操作数量。</span><span class="sxs-lookup"><span data-stu-id="36013-125">Reduce the number of operations per request.</span></span>
- <span data-ttu-id="36013-126">减少调用频率。</span><span class="sxs-lookup"><span data-stu-id="36013-126">Reduce the frequency of calls.</span></span>
- <span data-ttu-id="36013-127">不要立即重试，因为所有请求都会计入使用限制。</span><span class="sxs-lookup"><span data-stu-id="36013-127">Avoid immediate retries, because all requests accrue against your usage limits.</span></span>

<span data-ttu-id="36013-128">When you implement error handling, use the HTTP error code 429 to detect throttling.</span><span class="sxs-lookup"><span data-stu-id="36013-128">When you implement error handling, use the HTTP error code 429 to detect throttling.</span></span> <span data-ttu-id="36013-129">The failed response includes the `Retry-After` response header.</span><span class="sxs-lookup"><span data-stu-id="36013-129">The failed response includes the `Retry-After` response header.</span></span> <span data-ttu-id="36013-130">Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span><span class="sxs-lookup"><span data-stu-id="36013-130">Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span></span>

1. <span data-ttu-id="36013-131">等待 `Retry-After` 标头中指定的秒数。</span><span class="sxs-lookup"><span data-stu-id="36013-131">Wait the number of seconds specified in the `Retry-After` header.</span></span>
2. <span data-ttu-id="36013-132">请重试请求。</span><span class="sxs-lookup"><span data-stu-id="36013-132">Retry the request.</span></span>
3. <span data-ttu-id="36013-133">If the request fails again with a 429 error code, you are still being throttled.</span><span class="sxs-lookup"><span data-stu-id="36013-133">If the request fails again with a 429 error code, you are still being throttled.</span></span> <span data-ttu-id="36013-134">Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span><span class="sxs-lookup"><span data-stu-id="36013-134">Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span></span>

<span data-ttu-id="36013-135">下列资源目前提供 `Retry-After` 标头：</span><span class="sxs-lookup"><span data-stu-id="36013-135">The following resources currently provide a `Retry-After` header:</span></span>

- [<span data-ttu-id="36013-136">用户</span><span class="sxs-lookup"><span data-stu-id="36013-136">User</span></span>](/graph/api/resources/user?view=graph-rest-1.0)
- [<span data-ttu-id="36013-137">照片</span><span class="sxs-lookup"><span data-stu-id="36013-137">Photo</span></span>](/graph/api/resources/profilephoto?view=graph-rest-1.0)
- [<span data-ttu-id="36013-138">邮件</span><span class="sxs-lookup"><span data-stu-id="36013-138">Mail</span></span>](/graph/api/resources/message?view=graph-rest-1.0)
- [<span data-ttu-id="36013-139">日历（用户和组）</span><span class="sxs-lookup"><span data-stu-id="36013-139">Calendar (users and groups)</span></span>](/graph/api/resources/event?view=graph-rest-1.0)
- [<span data-ttu-id="36013-140">联系人</span><span class="sxs-lookup"><span data-stu-id="36013-140">Contact</span></span>](/graph/api/resources/contact?view=graph-rest-1.0)
- [<span data-ttu-id="36013-141">附件</span><span class="sxs-lookup"><span data-stu-id="36013-141">Attachment</span></span>](/graph/api/resources/attachment?view=graph-rest-1.0)
- [<span data-ttu-id="36013-142">组对话</span><span class="sxs-lookup"><span data-stu-id="36013-142">Group conversations</span></span>](/graph/api/resources/conversation?view=graph-rest-1.0)
- [<span data-ttu-id="36013-143">人员和社交活动</span><span class="sxs-lookup"><span data-stu-id="36013-143">People and social</span></span>](/graph/api/resources/social-overview?view=graph-rest-beta)
- [<span data-ttu-id="36013-144">Drive (OneDrive)</span><span class="sxs-lookup"><span data-stu-id="36013-144">Drive (OneDrive)</span></span>](/graph/api/resources/drive?view=graph-rest-1.0)
- [<span data-ttu-id="36013-145">外部项（Microsoft 搜索）</span><span class="sxs-lookup"><span data-stu-id="36013-145">External item (Microsoft Search)</span></span>](/graph/api/resources/externalitem?view=graph-rest-beta)
- [<span data-ttu-id="36013-146">订阅</span><span class="sxs-lookup"><span data-stu-id="36013-146">Subscription</span></span>](/graph/api/resources/subscription)
- [<span data-ttu-id="36013-147">受到</span><span class="sxs-lookup"><span data-stu-id="36013-147">Invitation</span></span>](/graph/api/resources/invitation)

<span data-ttu-id="36013-148">有关 Microsoft 云限制的更广泛讨论，请参阅[限制模式](https://docs.microsoft.com/azure/architecture/patterns/throttling)。</span><span class="sxs-lookup"><span data-stu-id="36013-148">For a broader discussion of throttling on the Microsoft Cloud, see [Throttling Pattern](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span></span>

> [!NOTE]
> <span data-ttu-id="36013-149">如果响应未提供 `Retry-After` 标头，我们建议实施指数退避重试策略。</span><span class="sxs-lookup"><span data-stu-id="36013-149">If no `Retry-After` header is provided by the response, we recommend implementing an exponential backoff retry policy.</span></span> <span data-ttu-id="36013-150">构建大型应用程序时，还可以实现[更高级的模式](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency)。</span><span class="sxs-lookup"><span data-stu-id="36013-150">You can also implement [more advanced patterns](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) when building large-scale applications.</span></span>
>
> <span data-ttu-id="36013-151">Microsoft Graph SDK 已实施依赖于 `Retry-After` 标头或默认为指数退避重试策略的处理程序。</span><span class="sxs-lookup"><span data-stu-id="36013-151">Microsoft Graph SDKs already implement handlers that rely on the `Retry-After` header or default to an exponential backoff retry policy.</span></span>

## <a name="best-practices-to-avoid-throttling"></a><span data-ttu-id="36013-152">避免限制的最佳做法</span><span class="sxs-lookup"><span data-stu-id="36013-152">Best practices to avoid throttling</span></span>

<span data-ttu-id="36013-153">如持续轮询资源以检查更新以及定期扫描资源集合以检查新资源或已删除资源之类的编程模式，更有可能导致应用程序受到限制并降低整体性能。</span><span class="sxs-lookup"><span data-stu-id="36013-153">Programming patterns like continuously polling a resource to check for updates and regularly scanning resource collections to check for new or deleted resources are more likely to lead to applications being throttled and degrade overall performances.</span></span> <span data-ttu-id="36013-154">如果可用，改为使用[更改跟踪](delta-query-overview.md)并[更改通知](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="36013-154">You should instead leverage [change tracking](delta-query-overview.md) and [change notifications](webhooks.md) when available.</span></span>

>[!NOTE]
><span data-ttu-id="36013-155">[大规模发现文件和检测更改的最佳做法](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online)详细介绍最佳做法。</span><span class="sxs-lookup"><span data-stu-id="36013-155">[Best practices for discovering files and detecting changes at scale](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online) describes best practices in details.</span></span>

## <a name="service-specific-limits"></a><span data-ttu-id="36013-156">服务特定限制</span><span class="sxs-lookup"><span data-stu-id="36013-156">Service-specific limits</span></span>

<span data-ttu-id="36013-157">借助 Microsoft Graph，用户可访问[多个服务](overview-major-services.md)中的数据，如 Outlook 或 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="36013-157">Microsoft Graph allows you to access data in [multiple services](overview-major-services.md), such as Outlook or Azure Active Directory.</span></span> <span data-ttu-id="36013-158">这些服务实施自己的限制，这些限制会影响使用 Microsoft Graph 访问它们的应用程序。</span><span class="sxs-lookup"><span data-stu-id="36013-158">These services impose their own throttling limits that affect applications that use Microsoft Graph to access them.</span></span>

> [!NOTE]
> <span data-ttu-id="36013-159">此处所述的具体限制可能会发生更改。</span><span class="sxs-lookup"><span data-stu-id="36013-159">The specific limits described here are subject to change.</span></span>

### <a name="outlook-service-limits"></a><span data-ttu-id="36013-160">Outlook 服务限制</span><span class="sxs-lookup"><span data-stu-id="36013-160">Outlook service limits</span></span>

<span data-ttu-id="36013-161">将评估每个应用 ID 和邮箱组合的 Outlook 服务限制。</span><span class="sxs-lookup"><span data-stu-id="36013-161">Outlook service limits are evaluated for each app ID and mailbox combination.</span></span> <span data-ttu-id="36013-162">换言之，上述限制适用于访问特定邮箱（用户或组）的特定应用。</span><span class="sxs-lookup"><span data-stu-id="36013-162">In other words, the limits described apply to a specific app accessing a specific mailbox (user or group).</span></span> <span data-ttu-id="36013-163">如果一个邮箱的应用程序超过限制，不会影响访问另一个邮箱的功能。</span><span class="sxs-lookup"><span data-stu-id="36013-163">If an application exceeds the limit in one mailbox, it does not affect the ability to access another mailbox.</span></span> <span data-ttu-id="36013-164">以下限制适用于公共云以及[国内云部署](/graph/deployments)。</span><span class="sxs-lookup"><span data-stu-id="36013-164">The following limits apply to the public cloud as well as [national cloud deployments](/graph/deployments).</span></span>

| <span data-ttu-id="36013-165">限制</span><span class="sxs-lookup"><span data-stu-id="36013-165">Limit</span></span>                                                      | <span data-ttu-id="36013-166">适用对象</span><span class="sxs-lookup"><span data-stu-id="36013-166">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="36013-167">10 分钟内的 10,000 个 API 请求</span><span class="sxs-lookup"><span data-stu-id="36013-167">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="36013-168">v1.0 和 beta 终结点</span><span class="sxs-lookup"><span data-stu-id="36013-168">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="36013-169">4 个并发请求</span><span class="sxs-lookup"><span data-stu-id="36013-169">4 concurrent requests</span></span>                                      | <span data-ttu-id="36013-170">v1.0 和 beta 终结点</span><span class="sxs-lookup"><span data-stu-id="36013-170">v1.0 and beta endpoints</span></span>   |
| <span data-ttu-id="36013-171">30 秒内的 15 兆位上传（PATCH、POST、PUT）</span><span class="sxs-lookup"><span data-stu-id="36013-171">15 megabit upload (PATCH, POST, PUT) in a 30 second period</span></span> | <span data-ttu-id="36013-172">v1.0 和 beta 终结点</span><span class="sxs-lookup"><span data-stu-id="36013-172">v1.0 and beta endpoints</span></span>   |

#### <a name="outlook-service-resources"></a><span data-ttu-id="36013-173">Outlook 服务资源</span><span class="sxs-lookup"><span data-stu-id="36013-173">Outlook service resources</span></span>

<span data-ttu-id="36013-174">Outlook 服务提供以下资源。</span><span class="sxs-lookup"><span data-stu-id="36013-174">The following resources are provided by the Outlook service.</span></span>

##### <a name="calendar-api-resources"></a><span data-ttu-id="36013-175">日历 API 资源</span><span class="sxs-lookup"><span data-stu-id="36013-175">Calendar API resources</span></span>

- [<span data-ttu-id="36013-176">event</span><span class="sxs-lookup"><span data-stu-id="36013-176">event</span></span>](/graph/api/resources/event)
- [<span data-ttu-id="36013-177">eventMessage</span><span class="sxs-lookup"><span data-stu-id="36013-177">eventMessage</span></span>](/graph/api/resources/eventmessage)
- [<span data-ttu-id="36013-178">calendar</span><span class="sxs-lookup"><span data-stu-id="36013-178">calendar</span></span>](/graph/api/resources/calendar)
- [<span data-ttu-id="36013-179">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="36013-179">calendarGroup</span></span>](/graph/api/resources/calendargroup)
- [<span data-ttu-id="36013-180">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="36013-180">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="36013-181">attachment</span><span class="sxs-lookup"><span data-stu-id="36013-181">attachment</span></span>](/graph/api/resources/attachment)
- [<span data-ttu-id="36013-182">place（预览）</span><span class="sxs-lookup"><span data-stu-id="36013-182">place (preview)</span></span>](/graph/api/resources/place)

##### <a name="mail-api-resources"></a><span data-ttu-id="36013-183">邮件 API 资源</span><span class="sxs-lookup"><span data-stu-id="36013-183">Mail API resources</span></span>

- [<span data-ttu-id="36013-184">message</span><span class="sxs-lookup"><span data-stu-id="36013-184">message</span></span>](/graph/api/resources/message)
- [<span data-ttu-id="36013-185">mailFolder</span><span class="sxs-lookup"><span data-stu-id="36013-185">mailFolder</span></span>](/graph/api/resources/mailfolder)
- [<span data-ttu-id="36013-186">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="36013-186">mailSearchFolder</span></span>](/graph/api/resources/mailsearchfolder)
- [<span data-ttu-id="36013-187">messageRule</span><span class="sxs-lookup"><span data-stu-id="36013-187">messageRule</span></span>](/graph/api/resources/messagerule)
- [<span data-ttu-id="36013-188">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="36013-188">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="36013-189">attachment</span><span class="sxs-lookup"><span data-stu-id="36013-189">attachment</span></span>](/graph/api/resources/attachment)

##### <a name="personal-contacts-api-resources"></a><span data-ttu-id="36013-190">个人联系人 API 资源</span><span class="sxs-lookup"><span data-stu-id="36013-190">Personal contacts API resources</span></span>

- [<span data-ttu-id="36013-191">contact</span><span class="sxs-lookup"><span data-stu-id="36013-191">contact</span></span>](/graph/api/resources/contact)
- [<span data-ttu-id="36013-192">contactFolder</span><span class="sxs-lookup"><span data-stu-id="36013-192">contactFolder</span></span>](/graph/api/resources/contactfolder)
- [<span data-ttu-id="36013-193">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="36013-193">outlookCategory</span></span>](/graph/api/resources/outlookcategory)

##### <a name="social-and-workplace-intelligence-resources"></a><span data-ttu-id="36013-194">社交和工作区智能资源</span><span class="sxs-lookup"><span data-stu-id="36013-194">Social and workplace intelligence resources</span></span>

- [<span data-ttu-id="36013-195">person</span><span class="sxs-lookup"><span data-stu-id="36013-195">person</span></span>](/graph/api/resources/person)

##### <a name="to-do-tasks-api-preview-resources"></a><span data-ttu-id="36013-196">待办任务 API（预览）资源</span><span class="sxs-lookup"><span data-stu-id="36013-196">To-do tasks API (preview) resources</span></span>

- [<span data-ttu-id="36013-197">outlookTask</span><span class="sxs-lookup"><span data-stu-id="36013-197">outlookTask</span></span>](/graph/api/resources/outlooktask)
- [<span data-ttu-id="36013-198">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="36013-198">outlookTaskFolder</span></span>](/graph/api/resources/outlooktaskfolder)
- [<span data-ttu-id="36013-199">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="36013-199">outlookTaskGroup</span></span>](/graph/api/resources/outlooktaskgroup)
- [<span data-ttu-id="36013-200">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="36013-200">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="36013-201">attachment</span><span class="sxs-lookup"><span data-stu-id="36013-201">attachment</span></span>](/graph/api/resources/attachment)

### <a name="microsoft-teams-service-limits"></a><span data-ttu-id="36013-202">Microsoft Teams 服务限制</span><span class="sxs-lookup"><span data-stu-id="36013-202">Microsoft Teams service limits</span></span>

<span data-ttu-id="36013-203">限制表示为每秒请求数 (rps)。</span><span class="sxs-lookup"><span data-stu-id="36013-203">Limits are expressed as requests per second (rps).</span></span>

| <span data-ttu-id="36013-204">Teams 请求类型</span><span class="sxs-lookup"><span data-stu-id="36013-204">Teams request type</span></span>                                   | <span data-ttu-id="36013-205">每个租户每个应用限制</span><span class="sxs-lookup"><span data-stu-id="36013-205">Limit per app per tenant</span></span>        | <span data-ttu-id="36013-206">所有租户中的每个应用限制</span><span class="sxs-lookup"><span data-stu-id="36013-206">Limit per app across all tenants</span></span>      |
|------------------------------------------------------|---------------------------------|------------|
| <span data-ttu-id="36013-207">Microsoft Teams 的任何图形 API 调用</span><span class="sxs-lookup"><span data-stu-id="36013-207">Any Graph API calls for Microsoft Teams</span></span>              | <span data-ttu-id="36013-208">每 10 秒 15000 个请求</span><span class="sxs-lookup"><span data-stu-id="36013-208">15000 requests every 10 seconds</span></span> | <span data-ttu-id="36013-209">不适用</span><span class="sxs-lookup"><span data-stu-id="36013-209">n/a</span></span> |
| <span data-ttu-id="36013-210">GET team, channel, tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="36013-210">GET team, channel, tab, installedApps, appCatalogs</span></span>   | <span data-ttu-id="36013-211">60 rps</span><span class="sxs-lookup"><span data-stu-id="36013-211">60 rps</span></span>                          | <span data-ttu-id="36013-212">600 rps</span><span class="sxs-lookup"><span data-stu-id="36013-212">600 rps</span></span> |
| <span data-ttu-id="36013-213">POST/PUT channel, tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="36013-213">POST/PUT channel, tab, installedApps, appCatalogs</span></span>    |  <span data-ttu-id="36013-214">30 rps</span><span class="sxs-lookup"><span data-stu-id="36013-214">30 rps</span></span>                         | <span data-ttu-id="36013-215">300 rps</span><span class="sxs-lookup"><span data-stu-id="36013-215">300 rps</span></span>  |
| <span data-ttu-id="36013-216">PATCH team, channel, tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="36013-216">PATCH team, channel, tab, installedApps, appCatalogs</span></span> |  <span data-ttu-id="36013-217">30 rps</span><span class="sxs-lookup"><span data-stu-id="36013-217">30 rps</span></span>                         | <span data-ttu-id="36013-218">300 rps</span><span class="sxs-lookup"><span data-stu-id="36013-218">300 rps</span></span>  |
| <span data-ttu-id="36013-219">DELETE channel, tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="36013-219">DELETE channel, tab, installedApps, appCatalogs</span></span>      |  <span data-ttu-id="36013-220">15 rps</span><span class="sxs-lookup"><span data-stu-id="36013-220">15 rps</span></span>                         | <span data-ttu-id="36013-221">150 rps</span><span class="sxs-lookup"><span data-stu-id="36013-221">150 rps</span></span>  |
| <span data-ttu-id="36013-222">GET /teams/```{team-id}```, joinedTeams</span><span class="sxs-lookup"><span data-stu-id="36013-222">GET /teams/```{team-id}```, joinedTeams</span></span>              |  <span data-ttu-id="36013-223">30 rps</span><span class="sxs-lookup"><span data-stu-id="36013-223">30 rps</span></span>                         | <span data-ttu-id="36013-224">300 rps</span><span class="sxs-lookup"><span data-stu-id="36013-224">300 rps</span></span>  |
| <span data-ttu-id="36013-225">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, clone</span><span class="sxs-lookup"><span data-stu-id="36013-225">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, clone</span></span> | <span data-ttu-id="36013-226">6 rps</span><span class="sxs-lookup"><span data-stu-id="36013-226">6 rps</span></span> | <span data-ttu-id="36013-227">150 rps</span><span class="sxs-lookup"><span data-stu-id="36013-227">150 rps</span></span>  | 
| <span data-ttu-id="36013-228">GET channel message</span><span class="sxs-lookup"><span data-stu-id="36013-228">GET channel message</span></span>  | <span data-ttu-id="36013-229">5 rps</span><span class="sxs-lookup"><span data-stu-id="36013-229">5 rps</span></span> | <span data-ttu-id="36013-230">100 rps</span><span class="sxs-lookup"><span data-stu-id="36013-230">100 rps</span></span> |
| <span data-ttu-id="36013-231">GET 1:1/group chat message</span><span class="sxs-lookup"><span data-stu-id="36013-231">GET 1:1/group chat message</span></span>  | <span data-ttu-id="36013-232">3 rps</span><span class="sxs-lookup"><span data-stu-id="36013-232">3 rps</span></span> | <span data-ttu-id="36013-233">30 rps</span><span class="sxs-lookup"><span data-stu-id="36013-233">30 rps</span></span> |
| <span data-ttu-id="36013-234">POST channel message</span><span class="sxs-lookup"><span data-stu-id="36013-234">POST channel message</span></span> | <span data-ttu-id="36013-235">2 rps</span><span class="sxs-lookup"><span data-stu-id="36013-235">2 rps</span></span> | <span data-ttu-id="36013-236">20 rps</span><span class="sxs-lookup"><span data-stu-id="36013-236">20 rps</span></span> |
| <span data-ttu-id="36013-237">POST 1:1/group chat message</span><span class="sxs-lookup"><span data-stu-id="36013-237">POST 1:1/group chat message</span></span> | <span data-ttu-id="36013-238">2 rps</span><span class="sxs-lookup"><span data-stu-id="36013-238">2 rps</span></span> | <span data-ttu-id="36013-239">20 rps</span><span class="sxs-lookup"><span data-stu-id="36013-239">20 rps</span></span> |

<span data-ttu-id="36013-240">对于给定团队或频道，每个应用最多可发布 4 个请求。</span><span class="sxs-lookup"><span data-stu-id="36013-240">A maximum of 4 requests per second per app can be issued on a given team or channel.</span></span>
<span data-ttu-id="36013-241">每个应用每天最多可以将 3000 条消息发送到给定的频道。</span><span class="sxs-lookup"><span data-stu-id="36013-241">A maximum of 3000 messages per app per day can be sent to a given channel.</span></span>

<span data-ttu-id="36013-242">另请参阅 [Microsoft Teams 限制](/graph/api/resources/teams-api-overview#microsoft-teams-limits)和[投票要求](/graph/api/resources/teams-api-overview#polling-requirements)。</span><span class="sxs-lookup"><span data-stu-id="36013-242">See also [Microsoft Teams limits](/graph/api/resources/teams-api-overview#microsoft-teams-limits) and [polling requirements](/graph/api/resources/teams-api-overview#polling-requirements).</span></span>

### <a name="invitation-manager-service-limits"></a><span data-ttu-id="36013-243">邀请管理器服务限制</span><span class="sxs-lookup"><span data-stu-id="36013-243">Invitation manager service limits</span></span>

<span data-ttu-id="36013-244">以下限制适用于 `/invitations` 上的所有请求。</span><span class="sxs-lookup"><span data-stu-id="36013-244">The following limits apply to any request on `/invitations`.</span></span>

| <span data-ttu-id="36013-245">操作</span><span class="sxs-lookup"><span data-stu-id="36013-245">Operation</span></span>                 | <span data-ttu-id="36013-246">每个租户的限制</span><span class="sxs-lookup"><span data-stu-id="36013-246">Limit per tenant</span></span>             |
|---------------------------|------------------------------|
| <span data-ttu-id="36013-247">任何操作</span><span class="sxs-lookup"><span data-stu-id="36013-247">Any operation</span></span>             | <span data-ttu-id="36013-248">每5秒150个请求</span><span class="sxs-lookup"><span data-stu-id="36013-248">150 requests per 5 seconds</span></span>   |

<!-- { "blockType": "throttlinggenstart" } -->

### <a name="education-service-limits"></a><span data-ttu-id="36013-249">教育服务限制</span><span class="sxs-lookup"><span data-stu-id="36013-249">Education service limits</span></span>

[!INCLUDE [Education rostering APIS throttling documentation](../includes/throttling-education-rostering-apis.md)]

### <a name="excel-service-limits"></a><span data-ttu-id="36013-250">Excel 服务限制</span><span class="sxs-lookup"><span data-stu-id="36013-250">Excel service limits</span></span>

[!INCLUDE [Excel throttling documentation](../includes/throttling-excel.md)]

### <a name="identity-and-access-audit-logs-service-limits"></a><span data-ttu-id="36013-251">标识和访问审核日志服务限制</span><span class="sxs-lookup"><span data-stu-id="36013-251">Identity and access audit logs service limits</span></span>

[!INCLUDE [Identity and access audit logs throttling documentation](../includes/throttling-Identity-and-access-audit-logs.md)]

### <a name="identity-providers-service-limits"></a><span data-ttu-id="36013-252">标识提供程序服务限制</span><span class="sxs-lookup"><span data-stu-id="36013-252">Identity providers service limits</span></span>

[!INCLUDE [CPIM throttling documentation](../includes/throttling-cpim.md)]

### <a name="intune-service-limits"></a><span data-ttu-id="36013-253">Intune 服务限制</span><span class="sxs-lookup"><span data-stu-id="36013-253">Intune service limits</span></span>

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

### <a name="skype-service-limits"></a><span data-ttu-id="36013-254">Skype 服务限制</span><span class="sxs-lookup"><span data-stu-id="36013-254">Skype service limits</span></span>

[!INCLUDE [Skype calling throttling documentation](../includes/throttling-skype-calling.md)]

### <a name="subscription-service-limits"></a><span data-ttu-id="36013-255">订阅服务限制</span><span class="sxs-lookup"><span data-stu-id="36013-255">Subscription service limits</span></span>

[!INCLUDE [Subscription services throttling documentation](../includes/throttling-subscription-services.md)]

<!-- { "blockType": "throttlinggenend" } -->
