---
title: Microsoft Graph 限制指南
description: Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: f2acb34994f0877a051d31e276feb22b2d47179c
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44682038"
---
# <a name="microsoft-graph-throttling-guidance"></a><span data-ttu-id="0904d-105">Microsoft Graph 限制指南</span><span class="sxs-lookup"><span data-stu-id="0904d-105">Microsoft Graph throttling guidance</span></span>

<span data-ttu-id="0904d-106">Throttling limits the number of concurrent calls to a service to prevent overuse of resources.</span><span class="sxs-lookup"><span data-stu-id="0904d-106">Throttling limits the number of concurrent calls to a service to prevent overuse of resources.</span></span> <span data-ttu-id="0904d-107">Microsoft Graph is designed to handle a high volume of requests.</span><span class="sxs-lookup"><span data-stu-id="0904d-107">Microsoft Graph is designed to handle a high volume of requests.</span></span> <span data-ttu-id="0904d-108">If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span><span class="sxs-lookup"><span data-stu-id="0904d-108">If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span></span>

<span data-ttu-id="0904d-109">Throttling limits vary based on the scenario.</span><span class="sxs-lookup"><span data-stu-id="0904d-109">Throttling limits vary based on the scenario.</span></span> <span data-ttu-id="0904d-110">For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span><span class="sxs-lookup"><span data-stu-id="0904d-110">For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span></span>

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a><span data-ttu-id="0904d-111">在限制时，会发生什么情况？</span><span class="sxs-lookup"><span data-stu-id="0904d-111">What happens when throttling occurs?</span></span>
<!-- markdownlint-enable MD026 -->

<span data-ttu-id="0904d-112">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time.</span><span class="sxs-lookup"><span data-stu-id="0904d-112">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time.</span></span> <span data-ttu-id="0904d-113">When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail.</span><span class="sxs-lookup"><span data-stu-id="0904d-113">When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail.</span></span> <span data-ttu-id="0904d-114">A suggested wait time is returned in the response header of the failed request.</span><span class="sxs-lookup"><span data-stu-id="0904d-114">A suggested wait time is returned in the response header of the failed request.</span></span> <span data-ttu-id="0904d-115">Throttling behavior can depend on the type and number of requests.</span><span class="sxs-lookup"><span data-stu-id="0904d-115">Throttling behavior can depend on the type and number of requests.</span></span> <span data-ttu-id="0904d-116">For example, if you have a high volume of requests, all requests types are throttled.</span><span class="sxs-lookup"><span data-stu-id="0904d-116">For example, if you have a high volume of requests, all requests types are throttled.</span></span> <span data-ttu-id="0904d-117">Threshold limits vary based on the request type.</span><span class="sxs-lookup"><span data-stu-id="0904d-117">Threshold limits vary based on the request type.</span></span> <span data-ttu-id="0904d-118">Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span><span class="sxs-lookup"><span data-stu-id="0904d-118">Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span>

## <a name="common-throttling-scenarios"></a><span data-ttu-id="0904d-119">常见的限制场景</span><span class="sxs-lookup"><span data-stu-id="0904d-119">Common throttling scenarios</span></span>

<span data-ttu-id="0904d-120">客户端受限的最常见原因包括：</span><span class="sxs-lookup"><span data-stu-id="0904d-120">The most common causes of throttling of clients include:</span></span>

- <span data-ttu-id="0904d-121">来自租户中所有应用程序的请求太多。</span><span class="sxs-lookup"><span data-stu-id="0904d-121">A large number of requests across all applications in a tenant.</span></span>
- <span data-ttu-id="0904d-122">来自所有租户中特定应用程序的请求太多。</span><span class="sxs-lookup"><span data-stu-id="0904d-122">A large number of requests from a particular application across all tenants.</span></span>

## <a name="best-practices-to-handle-throttling"></a><span data-ttu-id="0904d-123">处理限制的最佳实践</span><span class="sxs-lookup"><span data-stu-id="0904d-123">Best practices to handle throttling</span></span>

<span data-ttu-id="0904d-124">以下是处理限制的最佳做法：</span><span class="sxs-lookup"><span data-stu-id="0904d-124">The following are best practices for handling throttling:</span></span>

- <span data-ttu-id="0904d-125">减少每个请求的操作数量。</span><span class="sxs-lookup"><span data-stu-id="0904d-125">Reduce the number of operations per request.</span></span>
- <span data-ttu-id="0904d-126">减少调用频率。</span><span class="sxs-lookup"><span data-stu-id="0904d-126">Reduce the frequency of calls.</span></span>
- <span data-ttu-id="0904d-127">不要立即重试，因为所有请求都会计入使用限制。</span><span class="sxs-lookup"><span data-stu-id="0904d-127">Avoid immediate retries, because all requests accrue against your usage limits.</span></span>

<span data-ttu-id="0904d-128">When you implement error handling, use the HTTP error code 429 to detect throttling.</span><span class="sxs-lookup"><span data-stu-id="0904d-128">When you implement error handling, use the HTTP error code 429 to detect throttling.</span></span> <span data-ttu-id="0904d-129">The failed response includes the `Retry-After` response header.</span><span class="sxs-lookup"><span data-stu-id="0904d-129">The failed response includes the `Retry-After` response header.</span></span> <span data-ttu-id="0904d-130">Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span><span class="sxs-lookup"><span data-stu-id="0904d-130">Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span></span>

1. <span data-ttu-id="0904d-131">等待 `Retry-After` 标头中指定的秒数。</span><span class="sxs-lookup"><span data-stu-id="0904d-131">Wait the number of seconds specified in the `Retry-After` header.</span></span>
2. <span data-ttu-id="0904d-132">请重试请求。</span><span class="sxs-lookup"><span data-stu-id="0904d-132">Retry the request.</span></span>
3. <span data-ttu-id="0904d-133">If the request fails again with a 429 error code, you are still being throttled.</span><span class="sxs-lookup"><span data-stu-id="0904d-133">If the request fails again with a 429 error code, you are still being throttled.</span></span> <span data-ttu-id="0904d-134">Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span><span class="sxs-lookup"><span data-stu-id="0904d-134">Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span></span>

<span data-ttu-id="0904d-135">下列资源目前提供 `Retry-After` 标头：</span><span class="sxs-lookup"><span data-stu-id="0904d-135">The following resources currently provide a `Retry-After` header:</span></span>

- [<span data-ttu-id="0904d-136">用户</span><span class="sxs-lookup"><span data-stu-id="0904d-136">User</span></span>](/graph/api/resources/user?view=graph-rest-1.0)
- [<span data-ttu-id="0904d-137">照片</span><span class="sxs-lookup"><span data-stu-id="0904d-137">Photo</span></span>](/graph/api/resources/profilephoto?view=graph-rest-1.0)
- [<span data-ttu-id="0904d-138">邮件</span><span class="sxs-lookup"><span data-stu-id="0904d-138">Mail</span></span>](/graph/api/resources/message?view=graph-rest-1.0)
- [<span data-ttu-id="0904d-139">日历（用户和组）</span><span class="sxs-lookup"><span data-stu-id="0904d-139">Calendar (users and groups)</span></span>](/graph/api/resources/event?view=graph-rest-1.0)
- [<span data-ttu-id="0904d-140">联系人</span><span class="sxs-lookup"><span data-stu-id="0904d-140">Contact</span></span>](/graph/api/resources/contact?view=graph-rest-1.0)
- [<span data-ttu-id="0904d-141">附件</span><span class="sxs-lookup"><span data-stu-id="0904d-141">Attachment</span></span>](/graph/api/resources/attachment?view=graph-rest-1.0)
- [<span data-ttu-id="0904d-142">组对话</span><span class="sxs-lookup"><span data-stu-id="0904d-142">Group conversations</span></span>](/graph/api/resources/conversation?view=graph-rest-1.0)
- [<span data-ttu-id="0904d-143">人员和社交活动</span><span class="sxs-lookup"><span data-stu-id="0904d-143">People and social</span></span>](/graph/api/resources/social-overview?view=graph-rest-beta)
- [<span data-ttu-id="0904d-144">Drive (OneDrive)</span><span class="sxs-lookup"><span data-stu-id="0904d-144">Drive (OneDrive)</span></span>](/graph/api/resources/drive?view=graph-rest-1.0)
- [<span data-ttu-id="0904d-145">外部项（Microsoft 搜索）</span><span class="sxs-lookup"><span data-stu-id="0904d-145">External item (Microsoft Search)</span></span>](/graph/api/resources/externalitem?view=graph-rest-beta)
- [<span data-ttu-id="0904d-146">订阅</span><span class="sxs-lookup"><span data-stu-id="0904d-146">Subscription</span></span>](/graph/api/resources/subscription)

<span data-ttu-id="0904d-147">有关 Microsoft 云限制的更广泛讨论，请参阅[限制模式](https://docs.microsoft.com/azure/architecture/patterns/throttling)。</span><span class="sxs-lookup"><span data-stu-id="0904d-147">For a broader discussion of throttling on the Microsoft Cloud, see [Throttling Pattern](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span></span>

> [!NOTE]
> <span data-ttu-id="0904d-148">如果响应未提供 `Retry-After` 标头，我们建议实施指数退避重试策略。</span><span class="sxs-lookup"><span data-stu-id="0904d-148">If no `Retry-After` header is provided by the response, we recommend implementing an exponential backoff retry policy.</span></span> <span data-ttu-id="0904d-149">构建大型应用程序时，还可以实现[更高级的模式](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency)。</span><span class="sxs-lookup"><span data-stu-id="0904d-149">You can also implement [more advanced patterns](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) when building large-scale applications.</span></span>
>
> <span data-ttu-id="0904d-150">Microsoft Graph SDK 已实施依赖于 `Retry-After` 标头或默认为指数退避重试策略的处理程序。</span><span class="sxs-lookup"><span data-stu-id="0904d-150">Microsoft Graph SDKs already implement handlers that rely on the `Retry-After` header or default to an exponential backoff retry policy.</span></span>

## <a name="best-practices-to-avoid-throttling"></a><span data-ttu-id="0904d-151">避免限制的最佳做法</span><span class="sxs-lookup"><span data-stu-id="0904d-151">Best practices to avoid throttling</span></span>

<span data-ttu-id="0904d-152">如持续轮询资源以检查更新以及定期扫描资源集合以检查新资源或已删除资源之类的编程模式，更有可能导致应用程序受到限制并降低整体性能。</span><span class="sxs-lookup"><span data-stu-id="0904d-152">Programming patterns like continuously polling a resource to check for updates and regularly scanning resource collections to check for new or deleted resources are more likely to lead to applications being throttled and degrade overall performances.</span></span> <span data-ttu-id="0904d-153">如果可用，改为使用[更改跟踪](delta-query-overview.md)并[更改通知](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="0904d-153">You should instead leverage [change tracking](delta-query-overview.md) and [change notifications](webhooks.md) when available.</span></span>

>[!NOTE]
><span data-ttu-id="0904d-154">[大规模发现文件和检测更改的最佳做法](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online)详细介绍最佳做法。</span><span class="sxs-lookup"><span data-stu-id="0904d-154">[Best practices for discovering files and detecting changes at scale](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online) describes best practices in details.</span></span>

## <a name="service-specific-limits"></a><span data-ttu-id="0904d-155">服务特定限制</span><span class="sxs-lookup"><span data-stu-id="0904d-155">Service-specific limits</span></span>

<span data-ttu-id="0904d-156">借助 Microsoft Graph，用户可访问[多个服务](overview-major-services.md)中的数据，如 Outlook 或 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="0904d-156">Microsoft Graph allows you to access data in [multiple services](overview-major-services.md), such as Outlook or Azure Active Directory.</span></span> <span data-ttu-id="0904d-157">这些服务实施自己的限制，这些限制会影响使用 Microsoft Graph 访问它们的应用程序。</span><span class="sxs-lookup"><span data-stu-id="0904d-157">These services impose their own throttling limits that affect applications that use Microsoft Graph to access them.</span></span>

> [!NOTE]
> <span data-ttu-id="0904d-158">此处所述的具体限制可能会发生更改。</span><span class="sxs-lookup"><span data-stu-id="0904d-158">The specific limits described here are subject to change.</span></span>

### <a name="outlook-service-limits"></a><span data-ttu-id="0904d-159">Outlook 服务限制</span><span class="sxs-lookup"><span data-stu-id="0904d-159">Outlook service limits</span></span>

<span data-ttu-id="0904d-160">将评估每个应用 ID 和邮箱组合的 Outlook 服务限制。</span><span class="sxs-lookup"><span data-stu-id="0904d-160">Outlook service limits are evaluated for each app ID and mailbox combination.</span></span> <span data-ttu-id="0904d-161">换言之，上述限制适用于访问特定邮箱（用户或组）的特定应用。</span><span class="sxs-lookup"><span data-stu-id="0904d-161">In other words, the limits described apply to a specific app accessing a specific mailbox (user or group).</span></span> <span data-ttu-id="0904d-162">如果一个邮箱的应用程序超过限制，不会影响访问另一个邮箱的功能。</span><span class="sxs-lookup"><span data-stu-id="0904d-162">If an application exceeds the limit in one mailbox, it does not affect the ability to access another mailbox.</span></span>

| <span data-ttu-id="0904d-163">限制</span><span class="sxs-lookup"><span data-stu-id="0904d-163">Limit</span></span>                                                      | <span data-ttu-id="0904d-164">适用对象</span><span class="sxs-lookup"><span data-stu-id="0904d-164">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="0904d-165">10 分钟内的 10,000 个 API 请求</span><span class="sxs-lookup"><span data-stu-id="0904d-165">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="0904d-166">v1.0 和 beta 终结点</span><span class="sxs-lookup"><span data-stu-id="0904d-166">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="0904d-167">4 个并发请求</span><span class="sxs-lookup"><span data-stu-id="0904d-167">4 concurrent requests</span></span>                                      | <span data-ttu-id="0904d-168">Beta 终结点</span><span class="sxs-lookup"><span data-stu-id="0904d-168">Beta endpoint</span></span>   |
| <span data-ttu-id="0904d-169">30 秒内的 15 兆位上传（PATCH、POST、PUT）</span><span class="sxs-lookup"><span data-stu-id="0904d-169">15 megabit upload (PATCH, POST, PUT) in a 30 second period</span></span> | <span data-ttu-id="0904d-170">Beta 终结点</span><span class="sxs-lookup"><span data-stu-id="0904d-170">Beta endpoint</span></span>   |

#### <a name="outlook-service-resources"></a><span data-ttu-id="0904d-171">Outlook 服务资源</span><span class="sxs-lookup"><span data-stu-id="0904d-171">Outlook service resources</span></span>

<span data-ttu-id="0904d-172">Outlook 服务提供以下资源。</span><span class="sxs-lookup"><span data-stu-id="0904d-172">The following resources are provided by the Outlook service.</span></span>

##### <a name="calendar-api-resources"></a><span data-ttu-id="0904d-173">日历 API 资源</span><span class="sxs-lookup"><span data-stu-id="0904d-173">Calendar API resources</span></span>

- [<span data-ttu-id="0904d-174">event</span><span class="sxs-lookup"><span data-stu-id="0904d-174">event</span></span>](/graph/api/resources/event)
- [<span data-ttu-id="0904d-175">eventMessage</span><span class="sxs-lookup"><span data-stu-id="0904d-175">eventMessage</span></span>](/graph/api/resources/eventmessage)
- [<span data-ttu-id="0904d-176">calendar</span><span class="sxs-lookup"><span data-stu-id="0904d-176">calendar</span></span>](/graph/api/resources/calendar)
- [<span data-ttu-id="0904d-177">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="0904d-177">calendarGroup</span></span>](/graph/api/resources/calendargroup)
- [<span data-ttu-id="0904d-178">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="0904d-178">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="0904d-179">attachment</span><span class="sxs-lookup"><span data-stu-id="0904d-179">attachment</span></span>](/graph/api/resources/attachment)
- [<span data-ttu-id="0904d-180">place（预览）</span><span class="sxs-lookup"><span data-stu-id="0904d-180">place (preview)</span></span>](/graph/api/resources/place)

##### <a name="mail-api-resources"></a><span data-ttu-id="0904d-181">邮件 API 资源</span><span class="sxs-lookup"><span data-stu-id="0904d-181">Mail API resources</span></span>

- [<span data-ttu-id="0904d-182">message</span><span class="sxs-lookup"><span data-stu-id="0904d-182">message</span></span>](/graph/api/resources/message)
- [<span data-ttu-id="0904d-183">mailFolder</span><span class="sxs-lookup"><span data-stu-id="0904d-183">mailFolder</span></span>](/graph/api/resources/mailfolder)
- [<span data-ttu-id="0904d-184">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="0904d-184">mailSearchFolder</span></span>](/graph/api/resources/mailsearchfolder)
- [<span data-ttu-id="0904d-185">messageRule</span><span class="sxs-lookup"><span data-stu-id="0904d-185">messageRule</span></span>](/graph/api/resources/messagerule)
- [<span data-ttu-id="0904d-186">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="0904d-186">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="0904d-187">attachment</span><span class="sxs-lookup"><span data-stu-id="0904d-187">attachment</span></span>](/graph/api/resources/attachment)

##### <a name="personal-contacts-api-resources"></a><span data-ttu-id="0904d-188">个人联系人 API 资源</span><span class="sxs-lookup"><span data-stu-id="0904d-188">Personal contacts API resources</span></span>

- [<span data-ttu-id="0904d-189">contact</span><span class="sxs-lookup"><span data-stu-id="0904d-189">contact</span></span>](/graph/api/resources/contact)
- [<span data-ttu-id="0904d-190">contactFolder</span><span class="sxs-lookup"><span data-stu-id="0904d-190">contactFolder</span></span>](/graph/api/resources/contactfolder)
- [<span data-ttu-id="0904d-191">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="0904d-191">outlookCategory</span></span>](/graph/api/resources/outlookcategory)

##### <a name="social-and-workplace-intelligence-resources"></a><span data-ttu-id="0904d-192">社交和工作区智能资源</span><span class="sxs-lookup"><span data-stu-id="0904d-192">Social and workplace intelligence resources</span></span>

- [<span data-ttu-id="0904d-193">person</span><span class="sxs-lookup"><span data-stu-id="0904d-193">person</span></span>](/graph/api/resources/person)

##### <a name="to-do-tasks-api-preview-resources"></a><span data-ttu-id="0904d-194">待办任务 API（预览）资源</span><span class="sxs-lookup"><span data-stu-id="0904d-194">To-do tasks API (preview) resources</span></span>

- [<span data-ttu-id="0904d-195">outlookTask</span><span class="sxs-lookup"><span data-stu-id="0904d-195">outlookTask</span></span>](/graph/api/resources/outlooktask)
- [<span data-ttu-id="0904d-196">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="0904d-196">outlookTaskFolder</span></span>](/graph/api/resources/outlooktaskfolder)
- [<span data-ttu-id="0904d-197">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="0904d-197">outlookTaskGroup</span></span>](/graph/api/resources/outlooktaskgroup)
- [<span data-ttu-id="0904d-198">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="0904d-198">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="0904d-199">attachment</span><span class="sxs-lookup"><span data-stu-id="0904d-199">attachment</span></span>](/graph/api/resources/attachment)

### <a name="microsoft-teams-service-limits"></a><span data-ttu-id="0904d-200">Microsoft Teams 服务限制</span><span class="sxs-lookup"><span data-stu-id="0904d-200">Microsoft Teams service limits</span></span>

<span data-ttu-id="0904d-201">限制表示为每秒请求数 (rps)。</span><span class="sxs-lookup"><span data-stu-id="0904d-201">Limits are expressed as requests per second (rps).</span></span>

| <span data-ttu-id="0904d-202">Teams 请求类型</span><span class="sxs-lookup"><span data-stu-id="0904d-202">Teams request type</span></span>                                   | <span data-ttu-id="0904d-203">每个租户每个应用限制</span><span class="sxs-lookup"><span data-stu-id="0904d-203">Limit per app per tenant</span></span>        | <span data-ttu-id="0904d-204">所有租户中的每个应用限制</span><span class="sxs-lookup"><span data-stu-id="0904d-204">Limit per app across all tenants</span></span>      |
|------------------------------------------------------|---------------------------------|------------|
| <span data-ttu-id="0904d-205">Microsoft Teams 的任何图形 API 调用</span><span class="sxs-lookup"><span data-stu-id="0904d-205">Any Graph API calls for Microsoft Teams</span></span>              | <span data-ttu-id="0904d-206">每 10 秒 15000 个请求</span><span class="sxs-lookup"><span data-stu-id="0904d-206">15000 requests every 10 seconds</span></span> | <span data-ttu-id="0904d-207">不适用</span><span class="sxs-lookup"><span data-stu-id="0904d-207">n/a</span></span> |
| <span data-ttu-id="0904d-208">GET team, channel, tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="0904d-208">GET team, channel, tab, installedApps, appCatalogs</span></span>   | <span data-ttu-id="0904d-209">60 rps</span><span class="sxs-lookup"><span data-stu-id="0904d-209">60 rps</span></span>                          | <span data-ttu-id="0904d-210">600 rps</span><span class="sxs-lookup"><span data-stu-id="0904d-210">600 rps</span></span> |
| <span data-ttu-id="0904d-211">POST/PUT channel, tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="0904d-211">POST/PUT channel, tab, installedApps, appCatalogs</span></span>    |  <span data-ttu-id="0904d-212">30 rps</span><span class="sxs-lookup"><span data-stu-id="0904d-212">30 rps</span></span>                         | <span data-ttu-id="0904d-213">300 rps</span><span class="sxs-lookup"><span data-stu-id="0904d-213">300 rps</span></span>  |
| <span data-ttu-id="0904d-214">PATCH team, channel, tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="0904d-214">PATCH team, channel, tab, installedApps, appCatalogs</span></span> |  <span data-ttu-id="0904d-215">30 rps</span><span class="sxs-lookup"><span data-stu-id="0904d-215">30 rps</span></span>                         | <span data-ttu-id="0904d-216">300 rps</span><span class="sxs-lookup"><span data-stu-id="0904d-216">300 rps</span></span>  |
| <span data-ttu-id="0904d-217">DELETE channel, tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="0904d-217">DELETE channel, tab, installedApps, appCatalogs</span></span>      |  <span data-ttu-id="0904d-218">15 rps</span><span class="sxs-lookup"><span data-stu-id="0904d-218">15 rps</span></span>                         | <span data-ttu-id="0904d-219">150 rps</span><span class="sxs-lookup"><span data-stu-id="0904d-219">150 rps</span></span>  |
| <span data-ttu-id="0904d-220">GET /teams/```{team-id}```, joinedTeams</span><span class="sxs-lookup"><span data-stu-id="0904d-220">GET /teams/```{team-id}```, joinedTeams</span></span>              |  <span data-ttu-id="0904d-221">30 rps</span><span class="sxs-lookup"><span data-stu-id="0904d-221">30 rps</span></span>                         | <span data-ttu-id="0904d-222">300 rps</span><span class="sxs-lookup"><span data-stu-id="0904d-222">300 rps</span></span>  |
| <span data-ttu-id="0904d-223">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, clone</span><span class="sxs-lookup"><span data-stu-id="0904d-223">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, clone</span></span> | <span data-ttu-id="0904d-224">6 rps</span><span class="sxs-lookup"><span data-stu-id="0904d-224">6 rps</span></span> | <span data-ttu-id="0904d-225">150 rps</span><span class="sxs-lookup"><span data-stu-id="0904d-225">150 rps</span></span>  | 
| <span data-ttu-id="0904d-226">GET channel message</span><span class="sxs-lookup"><span data-stu-id="0904d-226">GET channel message</span></span>  | <span data-ttu-id="0904d-227">5 rps</span><span class="sxs-lookup"><span data-stu-id="0904d-227">5 rps</span></span> | <span data-ttu-id="0904d-228">100 rps</span><span class="sxs-lookup"><span data-stu-id="0904d-228">100 rps</span></span> |
| <span data-ttu-id="0904d-229">GET 1:1/group chat message</span><span class="sxs-lookup"><span data-stu-id="0904d-229">GET 1:1/group chat message</span></span>  | <span data-ttu-id="0904d-230">3 rps</span><span class="sxs-lookup"><span data-stu-id="0904d-230">3 rps</span></span> | <span data-ttu-id="0904d-231">30 rps</span><span class="sxs-lookup"><span data-stu-id="0904d-231">30 rps</span></span> |
| <span data-ttu-id="0904d-232">POST channel message</span><span class="sxs-lookup"><span data-stu-id="0904d-232">POST channel message</span></span> | <span data-ttu-id="0904d-233">2 rps</span><span class="sxs-lookup"><span data-stu-id="0904d-233">2 rps</span></span> | <span data-ttu-id="0904d-234">20 rps</span><span class="sxs-lookup"><span data-stu-id="0904d-234">20 rps</span></span> |
| <span data-ttu-id="0904d-235">POST 1:1/group chat message</span><span class="sxs-lookup"><span data-stu-id="0904d-235">POST 1:1/group chat message</span></span> | <span data-ttu-id="0904d-236">2 rps</span><span class="sxs-lookup"><span data-stu-id="0904d-236">2 rps</span></span> | <span data-ttu-id="0904d-237">20 rps</span><span class="sxs-lookup"><span data-stu-id="0904d-237">20 rps</span></span> |

<span data-ttu-id="0904d-238">对于给定团队或频道，每个应用最多可发布 4 个请求。</span><span class="sxs-lookup"><span data-stu-id="0904d-238">A maximum of 4 requests per second per app can be issued on a given team or channel.</span></span>
<span data-ttu-id="0904d-239">每个应用每天最多可以将 3000 条消息发送到给定的频道。</span><span class="sxs-lookup"><span data-stu-id="0904d-239">A maximum of 3000 messages per app per day can be sent to a given channel.</span></span>

<span data-ttu-id="0904d-240">另请参阅 [Microsoft Teams 限制](/graph/api/resources/teams-api-overview#microsoft-teams-limits)和[投票要求](/graph/api/resources/teams-api-overview#polling-requirements)。</span><span class="sxs-lookup"><span data-stu-id="0904d-240">See also [Microsoft Teams limits](/graph/api/resources/teams-api-overview#microsoft-teams-limits) and [polling requirements](/graph/api/resources/teams-api-overview#polling-requirements).</span></span>

### <a name="microsoft-graph-change-notifications-subscription-operations"></a><span data-ttu-id="0904d-241">Microsoft Graph 更改通知订阅操作</span><span class="sxs-lookup"><span data-stu-id="0904d-241">Microsoft Graph change notifications subscription operations</span></span>

<span data-ttu-id="0904d-242">以下限制适用于 `/subscriptions` 上的所有请求。</span><span class="sxs-lookup"><span data-stu-id="0904d-242">The following limits apply to any request on `/subscriptions`.</span></span>

| <span data-ttu-id="0904d-243">操作</span><span class="sxs-lookup"><span data-stu-id="0904d-243">Operation</span></span>                 | <span data-ttu-id="0904d-244">每个租户每个应用限制</span><span class="sxs-lookup"><span data-stu-id="0904d-244">Limit per app per tenant</span></span>     | <span data-ttu-id="0904d-245">所有租户中的每个应用限制</span><span class="sxs-lookup"><span data-stu-id="0904d-245">Limit per app accross all tenants</span></span> |
|---------------------------|------------------------------|-----------------------------------|
| <span data-ttu-id="0904d-246">POST, PUT, DELETE, PATCH</span><span class="sxs-lookup"><span data-stu-id="0904d-246">POST, PUT, DELETE, PATCH</span></span>  | <span data-ttu-id="0904d-247">每 20 秒 1000 个请求</span><span class="sxs-lookup"><span data-stu-id="0904d-247">1000 requests per 20 seconds</span></span> | <span data-ttu-id="0904d-248">每 20 秒 2000 个请求</span><span class="sxs-lookup"><span data-stu-id="0904d-248">2000 requests per 20 seconds</span></span>      |
| <span data-ttu-id="0904d-249">所有其他 HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="0904d-249">All other HTTP methods</span></span>    | <span data-ttu-id="0904d-250">每 20 秒 5000 个请求</span><span class="sxs-lookup"><span data-stu-id="0904d-250">5000 requests per 20 seconds</span></span> | <span data-ttu-id="0904d-251">每 20 秒 10000 个请求</span><span class="sxs-lookup"><span data-stu-id="0904d-251">10000 requests per 20 seconds</span></span>     |
