---
title: Microsoft Graph 限制指南
description: Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 12ae7bf122d23c6460dcbc253b1fe743768e49ba
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123713"
---
# <a name="microsoft-graph-throttling-guidance"></a><span data-ttu-id="f244d-105">Microsoft Graph 限制指南</span><span class="sxs-lookup"><span data-stu-id="f244d-105">Microsoft Graph throttling guidance</span></span>

<span data-ttu-id="f244d-106">Throttling limits the number of concurrent calls to a service to prevent overuse of resources.</span><span class="sxs-lookup"><span data-stu-id="f244d-106">Throttling limits the number of concurrent calls to a service to prevent overuse of resources.</span></span> <span data-ttu-id="f244d-107">Microsoft Graph is designed to handle a high volume of requests.</span><span class="sxs-lookup"><span data-stu-id="f244d-107">Microsoft Graph is designed to handle a high volume of requests.</span></span> <span data-ttu-id="f244d-108">If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span><span class="sxs-lookup"><span data-stu-id="f244d-108">If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span></span>

<span data-ttu-id="f244d-109">Throttling limits vary based on the scenario.</span><span class="sxs-lookup"><span data-stu-id="f244d-109">Throttling limits vary based on the scenario.</span></span> <span data-ttu-id="f244d-110">For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span><span class="sxs-lookup"><span data-stu-id="f244d-110">For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span></span>

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a><span data-ttu-id="f244d-111">在限制时，会发生什么情况？</span><span class="sxs-lookup"><span data-stu-id="f244d-111">What happens when throttling occurs?</span></span>
<!-- markdownlint-enable MD026 -->

<span data-ttu-id="f244d-112">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time.</span><span class="sxs-lookup"><span data-stu-id="f244d-112">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time.</span></span> <span data-ttu-id="f244d-113">When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail.</span><span class="sxs-lookup"><span data-stu-id="f244d-113">When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail.</span></span> <span data-ttu-id="f244d-114">A suggested wait time is returned in the response header of the failed request.</span><span class="sxs-lookup"><span data-stu-id="f244d-114">A suggested wait time is returned in the response header of the failed request.</span></span> <span data-ttu-id="f244d-115">Throttling behavior can depend on the type and number of requests.</span><span class="sxs-lookup"><span data-stu-id="f244d-115">Throttling behavior can depend on the type and number of requests.</span></span> <span data-ttu-id="f244d-116">For example, if you have a high volume of requests, all requests types are throttled.</span><span class="sxs-lookup"><span data-stu-id="f244d-116">For example, if you have a high volume of requests, all requests types are throttled.</span></span> <span data-ttu-id="f244d-117">Threshold limits vary based on the request type.</span><span class="sxs-lookup"><span data-stu-id="f244d-117">Threshold limits vary based on the request type.</span></span> <span data-ttu-id="f244d-118">Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span><span class="sxs-lookup"><span data-stu-id="f244d-118">Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span>

## <a name="common-throttling-scenarios"></a><span data-ttu-id="f244d-119">常见的限制场景</span><span class="sxs-lookup"><span data-stu-id="f244d-119">Common throttling scenarios</span></span>

<span data-ttu-id="f244d-120">客户端受限的最常见原因包括：</span><span class="sxs-lookup"><span data-stu-id="f244d-120">The most common causes of throttling of clients include:</span></span>

- <span data-ttu-id="f244d-121">来自租户中所有应用程序的请求太多。</span><span class="sxs-lookup"><span data-stu-id="f244d-121">A large number of requests across all applications in a tenant.</span></span>
- <span data-ttu-id="f244d-122">来自所有租户中特定应用程序的请求太多。</span><span class="sxs-lookup"><span data-stu-id="f244d-122">A large number of requests from a particular application across all tenants.</span></span>

## <a name="best-practices-to-handle-throttling"></a><span data-ttu-id="f244d-123">处理限制的最佳实践</span><span class="sxs-lookup"><span data-stu-id="f244d-123">Best practices to handle throttling</span></span>

<span data-ttu-id="f244d-124">以下是处理限制的最佳做法：</span><span class="sxs-lookup"><span data-stu-id="f244d-124">The following are best practices for handling throttling:</span></span>

- <span data-ttu-id="f244d-125">减少每个请求的操作数量。</span><span class="sxs-lookup"><span data-stu-id="f244d-125">Reduce the number of operations per request.</span></span>
- <span data-ttu-id="f244d-126">减少调用频率。</span><span class="sxs-lookup"><span data-stu-id="f244d-126">Reduce the frequency of calls.</span></span>
- <span data-ttu-id="f244d-127">不要立即重试，因为所有请求都会计入使用限制。</span><span class="sxs-lookup"><span data-stu-id="f244d-127">Avoid immediate retries, because all requests accrue against your usage limits.</span></span>

<span data-ttu-id="f244d-128">When you implement error handling, use the HTTP error code 429 to detect throttling.</span><span class="sxs-lookup"><span data-stu-id="f244d-128">When you implement error handling, use the HTTP error code 429 to detect throttling.</span></span> <span data-ttu-id="f244d-129">The failed response includes the `Retry-After` response header.</span><span class="sxs-lookup"><span data-stu-id="f244d-129">The failed response includes the `Retry-After` response header.</span></span> <span data-ttu-id="f244d-130">Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span><span class="sxs-lookup"><span data-stu-id="f244d-130">Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span></span>

1. <span data-ttu-id="f244d-131">等待 `Retry-After` 标头中指定的秒数。</span><span class="sxs-lookup"><span data-stu-id="f244d-131">Wait the number of seconds specified in the `Retry-After` header.</span></span>
2. <span data-ttu-id="f244d-132">请重试请求。</span><span class="sxs-lookup"><span data-stu-id="f244d-132">Retry the request.</span></span>
3. <span data-ttu-id="f244d-133">If the request fails again with a 429 error code, you are still being throttled.</span><span class="sxs-lookup"><span data-stu-id="f244d-133">If the request fails again with a 429 error code, you are still being throttled.</span></span> <span data-ttu-id="f244d-134">Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span><span class="sxs-lookup"><span data-stu-id="f244d-134">Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span></span>

<span data-ttu-id="f244d-135">下列资源目前提供 `Retry-After` 标头：</span><span class="sxs-lookup"><span data-stu-id="f244d-135">The following resources currently provide a `Retry-After` header:</span></span>

- [<span data-ttu-id="f244d-136">用户</span><span class="sxs-lookup"><span data-stu-id="f244d-136">User</span></span>](/graph/api/resources/user?view=graph-rest-1.0)
- [<span data-ttu-id="f244d-137">照片</span><span class="sxs-lookup"><span data-stu-id="f244d-137">Photo</span></span>](/graph/api/resources/profilephoto?view=graph-rest-1.0)
- [<span data-ttu-id="f244d-138">邮件</span><span class="sxs-lookup"><span data-stu-id="f244d-138">Mail</span></span>](/graph/api/resources/message?view=graph-rest-1.0)
- [<span data-ttu-id="f244d-139">日历（用户和组）</span><span class="sxs-lookup"><span data-stu-id="f244d-139">Calendar (users and groups)</span></span>](/graph/api/resources/event?view=graph-rest-1.0)
- [<span data-ttu-id="f244d-140">联系人</span><span class="sxs-lookup"><span data-stu-id="f244d-140">Contact</span></span>](/graph/api/resources/contact?view=graph-rest-1.0)
- [<span data-ttu-id="f244d-141">附件</span><span class="sxs-lookup"><span data-stu-id="f244d-141">Attachment</span></span>](/graph/api/resources/attachment?view=graph-rest-1.0)
- [<span data-ttu-id="f244d-142">组对话</span><span class="sxs-lookup"><span data-stu-id="f244d-142">Group conversations</span></span>](/graph/api/resources/conversation?view=graph-rest-1.0)
- [<span data-ttu-id="f244d-143">人员和社交活动</span><span class="sxs-lookup"><span data-stu-id="f244d-143">People and social</span></span>](/graph/api/resources/social-overview?view=graph-rest-beta)
- [<span data-ttu-id="f244d-144">Drive (OneDrive)</span><span class="sxs-lookup"><span data-stu-id="f244d-144">Drive (OneDrive)</span></span>](/graph/api/resources/drive?view=graph-rest-1.0)
- [<span data-ttu-id="f244d-145">外部项（Microsoft 搜索）</span><span class="sxs-lookup"><span data-stu-id="f244d-145">External item (Microsoft Search)</span></span>](/graph/api/resources/externalitem?view=graph-rest-beta)
- [<span data-ttu-id="f244d-146">Report</span><span class="sxs-lookup"><span data-stu-id="f244d-146">Report</span></span>](/graph/api/resources/report)
- [<span data-ttu-id="f244d-147">订阅</span><span class="sxs-lookup"><span data-stu-id="f244d-147">Subscription</span></span>](/graph/api/resources/subscription)
- [<span data-ttu-id="f244d-148">趋势</span><span class="sxs-lookup"><span data-stu-id="f244d-148">Trending</span></span>](/graph/api/resources/insights-trending)
- [<span data-ttu-id="f244d-149">已使用见解</span><span class="sxs-lookup"><span data-stu-id="f244d-149">Used insight</span></span>](/graph/api/resources/insights-used)
- [<span data-ttu-id="f244d-150">共享见解</span><span class="sxs-lookup"><span data-stu-id="f244d-150">Shared insight</span></span>](/graph/api/resources/insights-shared)
- [<span data-ttu-id="f244d-151">用户设置</span><span class="sxs-lookup"><span data-stu-id="f244d-151">User settings</span></span>](/graph/api/resources/usersettings)
- [<span data-ttu-id="f244d-152">邀请</span><span class="sxs-lookup"><span data-stu-id="f244d-152">Invitation</span></span>](/graph/api/resources/invitation)

<span data-ttu-id="f244d-153">有关 Microsoft 云限制的更广泛讨论，请参阅[限制模式](https://docs.microsoft.com/azure/architecture/patterns/throttling)。</span><span class="sxs-lookup"><span data-stu-id="f244d-153">For a broader discussion of throttling on the Microsoft Cloud, see [Throttling Pattern](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span></span>

> [!NOTE]
> <span data-ttu-id="f244d-154">如果响应未提供 `Retry-After` 标头，我们建议实施指数退避重试策略。</span><span class="sxs-lookup"><span data-stu-id="f244d-154">If no `Retry-After` header is provided by the response, we recommend implementing an exponential backoff retry policy.</span></span> <span data-ttu-id="f244d-155">构建大型应用程序时，还可以实现[更高级的模式](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency)。</span><span class="sxs-lookup"><span data-stu-id="f244d-155">You can also implement [more advanced patterns](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) when building large-scale applications.</span></span>
>
> <span data-ttu-id="f244d-156">Microsoft Graph SDK 已实施依赖于 `Retry-After` 标头或默认为指数退避重试策略的处理程序。</span><span class="sxs-lookup"><span data-stu-id="f244d-156">Microsoft Graph SDKs already implement handlers that rely on the `Retry-After` header or default to an exponential backoff retry policy.</span></span>

## <a name="best-practices-to-avoid-throttling"></a><span data-ttu-id="f244d-157">避免限制的最佳做法</span><span class="sxs-lookup"><span data-stu-id="f244d-157">Best practices to avoid throttling</span></span>

<span data-ttu-id="f244d-158">如持续轮询资源以检查更新以及定期扫描资源集合以检查新资源或已删除资源之类的编程模式，更有可能导致应用程序受到限制并降低整体性能。</span><span class="sxs-lookup"><span data-stu-id="f244d-158">Programming patterns like continuously polling a resource to check for updates and regularly scanning resource collections to check for new or deleted resources are more likely to lead to applications being throttled and degrade overall performances.</span></span> <span data-ttu-id="f244d-159">如果可用，改为使用[更改跟踪](delta-query-overview.md)并[更改通知](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="f244d-159">You should instead leverage [change tracking](delta-query-overview.md) and [change notifications](webhooks.md) when available.</span></span>

>[!NOTE]
><span data-ttu-id="f244d-160">[大规模发现文件和检测更改的最佳做法](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online)详细介绍最佳做法。</span><span class="sxs-lookup"><span data-stu-id="f244d-160">[Best practices for discovering files and detecting changes at scale](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online) describes best practices in details.</span></span>

## <a name="service-specific-limits"></a><span data-ttu-id="f244d-161">服务特定限制</span><span class="sxs-lookup"><span data-stu-id="f244d-161">Service-specific limits</span></span>

<span data-ttu-id="f244d-162">借助 Microsoft Graph，用户可访问[多个服务](overview-major-services.md)中的数据，如 Outlook 或 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="f244d-162">Microsoft Graph allows you to access data in [multiple services](overview-major-services.md), such as Outlook or Azure Active Directory.</span></span> <span data-ttu-id="f244d-163">这些服务实施自己的限制，这些限制会影响使用 Microsoft Graph 访问它们的应用程序。</span><span class="sxs-lookup"><span data-stu-id="f244d-163">These services impose their own throttling limits that affect applications that use Microsoft Graph to access them.</span></span>

> [!NOTE]
> <span data-ttu-id="f244d-164">此处所述的具体限制可能会发生更改。</span><span class="sxs-lookup"><span data-stu-id="f244d-164">The specific limits described here are subject to change.</span></span>

> <span data-ttu-id="f244d-165">**备注** 在本节中，*租户*此术语是指指安装应用程序的 Microsoft 365 组织。</span><span class="sxs-lookup"><span data-stu-id="f244d-165">**Note:** In this section, the term *tenant* refers to the Microsoft 365 organization where the application is installed.</span></span> <span data-ttu-id="f244d-166">对于单个租户应用程序，这个租户可以与创建应用程序的租户相同，对于[多租户应用程序](/azure/active-directory/develop/setup-multi-tenant-app)，这个租户可以不同。</span><span class="sxs-lookup"><span data-stu-id="f244d-166">This tenant can be the same as the the one where the application was created, in the case of a single tenant application, or it can be different, in the case of a [multi-tenant application](/azure/active-directory/develop/setup-multi-tenant-app).</span></span>

### <a name="outlook-service-limits"></a><span data-ttu-id="f244d-167">Outlook 服务限制</span><span class="sxs-lookup"><span data-stu-id="f244d-167">Outlook service limits</span></span>

<span data-ttu-id="f244d-168">将评估每个应用 ID 和邮箱组合的 Outlook 服务限制。</span><span class="sxs-lookup"><span data-stu-id="f244d-168">Outlook service limits are evaluated for each app ID and mailbox combination.</span></span> <span data-ttu-id="f244d-169">换言之，上述限制适用于访问特定邮箱（用户或组）的特定应用。</span><span class="sxs-lookup"><span data-stu-id="f244d-169">In other words, the limits described apply to a specific app accessing a specific mailbox (user or group).</span></span> <span data-ttu-id="f244d-170">如果一个邮箱的应用程序超过限制，不会影响访问另一个邮箱的功能。</span><span class="sxs-lookup"><span data-stu-id="f244d-170">If an application exceeds the limit in one mailbox, it does not affect the ability to access another mailbox.</span></span> <span data-ttu-id="f244d-171">下面的限制适用于公共云以及[区域云部署](/graph/deployments)。</span><span class="sxs-lookup"><span data-stu-id="f244d-171">The following limits apply to the public cloud as well as [national cloud deployments](/graph/deployments).</span></span>

| <span data-ttu-id="f244d-172">限制</span><span class="sxs-lookup"><span data-stu-id="f244d-172">Limit</span></span>                                                      | <span data-ttu-id="f244d-173">适用对象</span><span class="sxs-lookup"><span data-stu-id="f244d-173">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="f244d-174">10 分钟内的 10,000 个 API 请求</span><span class="sxs-lookup"><span data-stu-id="f244d-174">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="f244d-175">v1.0 和 beta 终结点</span><span class="sxs-lookup"><span data-stu-id="f244d-175">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="f244d-176">4 个并发请求</span><span class="sxs-lookup"><span data-stu-id="f244d-176">4 concurrent requests</span></span>                                      | <span data-ttu-id="f244d-177">v1.0 和 beta 终结点</span><span class="sxs-lookup"><span data-stu-id="f244d-177">v1.0 and beta endpoints</span></span>   |
| <span data-ttu-id="f244d-178">30 秒内的 15 兆字节 (MB) 上传（PATCH、POST、PUT）</span><span class="sxs-lookup"><span data-stu-id="f244d-178">15 megabytes (MB) upload (PATCH, POST, PUT) in a 30 second period</span></span> | <span data-ttu-id="f244d-179">v1.0 和 beta 终结点</span><span class="sxs-lookup"><span data-stu-id="f244d-179">v1.0 and beta endpoints</span></span>   |

#### <a name="outlook-service-resources"></a><span data-ttu-id="f244d-180">Outlook 服务资源</span><span class="sxs-lookup"><span data-stu-id="f244d-180">Outlook service resources</span></span>

<span data-ttu-id="f244d-181">Outlook 服务提供以下资源。</span><span class="sxs-lookup"><span data-stu-id="f244d-181">The following resources are provided by the Outlook service.</span></span>

##### <a name="calendar-api-resources"></a><span data-ttu-id="f244d-182">日历 API 资源</span><span class="sxs-lookup"><span data-stu-id="f244d-182">Calendar API resources</span></span>

- [<span data-ttu-id="f244d-183">event</span><span class="sxs-lookup"><span data-stu-id="f244d-183">event</span></span>](/graph/api/resources/event)
- [<span data-ttu-id="f244d-184">eventMessage</span><span class="sxs-lookup"><span data-stu-id="f244d-184">eventMessage</span></span>](/graph/api/resources/eventmessage)
- [<span data-ttu-id="f244d-185">calendar</span><span class="sxs-lookup"><span data-stu-id="f244d-185">calendar</span></span>](/graph/api/resources/calendar)
- [<span data-ttu-id="f244d-186">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="f244d-186">calendarGroup</span></span>](/graph/api/resources/calendargroup)
- [<span data-ttu-id="f244d-187">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="f244d-187">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="f244d-188">attachment</span><span class="sxs-lookup"><span data-stu-id="f244d-188">attachment</span></span>](/graph/api/resources/attachment)
- [<span data-ttu-id="f244d-189">place（预览）</span><span class="sxs-lookup"><span data-stu-id="f244d-189">place (preview)</span></span>](/graph/api/resources/place)

##### <a name="mail-api-resources"></a><span data-ttu-id="f244d-190">邮件 API 资源</span><span class="sxs-lookup"><span data-stu-id="f244d-190">Mail API resources</span></span>

- [<span data-ttu-id="f244d-191">message</span><span class="sxs-lookup"><span data-stu-id="f244d-191">message</span></span>](/graph/api/resources/message)
- [<span data-ttu-id="f244d-192">mailFolder</span><span class="sxs-lookup"><span data-stu-id="f244d-192">mailFolder</span></span>](/graph/api/resources/mailfolder)
- [<span data-ttu-id="f244d-193">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="f244d-193">mailSearchFolder</span></span>](/graph/api/resources/mailsearchfolder)
- [<span data-ttu-id="f244d-194">messageRule</span><span class="sxs-lookup"><span data-stu-id="f244d-194">messageRule</span></span>](/graph/api/resources/messagerule)
- [<span data-ttu-id="f244d-195">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="f244d-195">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="f244d-196">attachment</span><span class="sxs-lookup"><span data-stu-id="f244d-196">attachment</span></span>](/graph/api/resources/attachment)

##### <a name="personal-contacts-api-resources"></a><span data-ttu-id="f244d-197">个人联系人 API 资源</span><span class="sxs-lookup"><span data-stu-id="f244d-197">Personal contacts API resources</span></span>

- [<span data-ttu-id="f244d-198">contact</span><span class="sxs-lookup"><span data-stu-id="f244d-198">contact</span></span>](/graph/api/resources/contact)
- [<span data-ttu-id="f244d-199">contactFolder</span><span class="sxs-lookup"><span data-stu-id="f244d-199">contactFolder</span></span>](/graph/api/resources/contactfolder)
- [<span data-ttu-id="f244d-200">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="f244d-200">outlookCategory</span></span>](/graph/api/resources/outlookcategory)

##### <a name="social-and-workplace-intelligence-resources"></a><span data-ttu-id="f244d-201">社交和工作区智能资源</span><span class="sxs-lookup"><span data-stu-id="f244d-201">Social and workplace intelligence resources</span></span>

- [<span data-ttu-id="f244d-202">person</span><span class="sxs-lookup"><span data-stu-id="f244d-202">person</span></span>](/graph/api/resources/person)

##### <a name="to-do-tasks-api-preview-resources"></a><span data-ttu-id="f244d-203">待办任务 API（预览）资源</span><span class="sxs-lookup"><span data-stu-id="f244d-203">To-do tasks API (preview) resources</span></span>

- [<span data-ttu-id="f244d-204">outlookTask</span><span class="sxs-lookup"><span data-stu-id="f244d-204">outlookTask</span></span>](/graph/api/resources/outlooktask)
- [<span data-ttu-id="f244d-205">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="f244d-205">outlookTaskFolder</span></span>](/graph/api/resources/outlooktaskfolder)
- [<span data-ttu-id="f244d-206">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="f244d-206">outlookTaskGroup</span></span>](/graph/api/resources/outlooktaskgroup)
- [<span data-ttu-id="f244d-207">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="f244d-207">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="f244d-208">attachment</span><span class="sxs-lookup"><span data-stu-id="f244d-208">attachment</span></span>](/graph/api/resources/attachment)

### <a name="cloud-communication-service-limits"></a><span data-ttu-id="f244d-209">云通信服务限制</span><span class="sxs-lookup"><span data-stu-id="f244d-209">Cloud communication service limits</span></span>

| <span data-ttu-id="f244d-210">资源</span><span class="sxs-lookup"><span data-stu-id="f244d-210">Resource</span></span>      | <span data-ttu-id="f244d-211">每个租户每个应用限制</span><span class="sxs-lookup"><span data-stu-id="f244d-211">Limits per app per tenant</span></span>    |
| -------------- | ------------ |
| [<span data-ttu-id="f244d-212">通话</span><span class="sxs-lookup"><span data-stu-id="f244d-212">Calls</span></span>](/graph/api/resources/call) | <span data-ttu-id="f244d-213">每月10,000 通通话和 100 通并发通话</span><span class="sxs-lookup"><span data-stu-id="f244d-213">10,000 calls/month and 100 concurrent calls</span></span>   |
| [<span data-ttu-id="f244d-214">会议信息</span><span class="sxs-lookup"><span data-stu-id="f244d-214">Meeting information</span></span>](/graph/api/resources/meetinginfo)   | <span data-ttu-id="f244d-215">每月每位用家会有 2000 则会议</span><span class="sxs-lookup"><span data-stu-id="f244d-215">2000 meetings/user each month</span></span> |
| <span data-ttu-id="f244d-216">[状态](/graph/api/resources/presence)（预览版）</span><span class="sxs-lookup"><span data-stu-id="f244d-216">[Presence](/graph/api/resources/presence) (preview)</span></span>   | <span data-ttu-id="f244d-217">2 rps</span><span class="sxs-lookup"><span data-stu-id="f244d-217">2 rps</span></span> |

### <a name="microsoft-teams-service-limits"></a><span data-ttu-id="f244d-218">Microsoft Teams 服务限制</span><span class="sxs-lookup"><span data-stu-id="f244d-218">Microsoft Teams service limits</span></span>

<span data-ttu-id="f244d-219">限制表示为每秒请求数 (rps)。</span><span class="sxs-lookup"><span data-stu-id="f244d-219">Limits are expressed as requests per second (rps).</span></span>

| <span data-ttu-id="f244d-220">Teams 请求类型</span><span class="sxs-lookup"><span data-stu-id="f244d-220">Teams request type</span></span>                                   | <span data-ttu-id="f244d-221">每个租户每个应用限制</span><span class="sxs-lookup"><span data-stu-id="f244d-221">Limit per app per tenant</span></span>        | <span data-ttu-id="f244d-222">所有租户中的每个应用限制</span><span class="sxs-lookup"><span data-stu-id="f244d-222">Limit per app across all tenants</span></span>      |
|------------------------------------------------------|---------------------------------|------------|
| <span data-ttu-id="f244d-223">Microsoft Teams 的任何图形 API 调用</span><span class="sxs-lookup"><span data-stu-id="f244d-223">Any Graph API calls for Microsoft Teams</span></span>              | <span data-ttu-id="f244d-224">每 10 秒 15000 个请求</span><span class="sxs-lookup"><span data-stu-id="f244d-224">15000 requests every 10 seconds</span></span> | <span data-ttu-id="f244d-225">不适用</span><span class="sxs-lookup"><span data-stu-id="f244d-225">n/a</span></span> |
| <span data-ttu-id="f244d-226">GET team, channel, tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="f244d-226">GET team, channel, tab, installedApps, appCatalogs</span></span>   | <span data-ttu-id="f244d-227">60 rps</span><span class="sxs-lookup"><span data-stu-id="f244d-227">60 rps</span></span>                          | <span data-ttu-id="f244d-228">600 rps</span><span class="sxs-lookup"><span data-stu-id="f244d-228">600 rps</span></span> |
| <span data-ttu-id="f244d-229">POST/PUT channel, tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="f244d-229">POST/PUT channel, tab, installedApps, appCatalogs</span></span>    |  <span data-ttu-id="f244d-230">30 rps</span><span class="sxs-lookup"><span data-stu-id="f244d-230">30 rps</span></span>                         | <span data-ttu-id="f244d-231">300 rps</span><span class="sxs-lookup"><span data-stu-id="f244d-231">300 rps</span></span>  |
| <span data-ttu-id="f244d-232">PATCH team, channel, tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="f244d-232">PATCH team, channel, tab, installedApps, appCatalogs</span></span> |  <span data-ttu-id="f244d-233">30 rps</span><span class="sxs-lookup"><span data-stu-id="f244d-233">30 rps</span></span>                         | <span data-ttu-id="f244d-234">300 rps</span><span class="sxs-lookup"><span data-stu-id="f244d-234">300 rps</span></span>  |
| <span data-ttu-id="f244d-235">DELETE channel, tab, installedApps, appCatalogs</span><span class="sxs-lookup"><span data-stu-id="f244d-235">DELETE channel, tab, installedApps, appCatalogs</span></span>      |  <span data-ttu-id="f244d-236">15 rps</span><span class="sxs-lookup"><span data-stu-id="f244d-236">15 rps</span></span>                         | <span data-ttu-id="f244d-237">150 rps</span><span class="sxs-lookup"><span data-stu-id="f244d-237">150 rps</span></span>  |
| <span data-ttu-id="f244d-238">GET /teams/```{team-id}```, joinedTeams</span><span class="sxs-lookup"><span data-stu-id="f244d-238">GET /teams/```{team-id}```, joinedTeams</span></span>              |  <span data-ttu-id="f244d-239">30 rps</span><span class="sxs-lookup"><span data-stu-id="f244d-239">30 rps</span></span>                         | <span data-ttu-id="f244d-240">300 rps</span><span class="sxs-lookup"><span data-stu-id="f244d-240">300 rps</span></span>  |
| <span data-ttu-id="f244d-241">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, clone</span><span class="sxs-lookup"><span data-stu-id="f244d-241">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, clone</span></span> | <span data-ttu-id="f244d-242">6 rps</span><span class="sxs-lookup"><span data-stu-id="f244d-242">6 rps</span></span> | <span data-ttu-id="f244d-243">150 rps</span><span class="sxs-lookup"><span data-stu-id="f244d-243">150 rps</span></span>  | 
| <span data-ttu-id="f244d-244">GET channel message</span><span class="sxs-lookup"><span data-stu-id="f244d-244">GET channel message</span></span>  | <span data-ttu-id="f244d-245">5 rps</span><span class="sxs-lookup"><span data-stu-id="f244d-245">5 rps</span></span> | <span data-ttu-id="f244d-246">100 rps</span><span class="sxs-lookup"><span data-stu-id="f244d-246">100 rps</span></span> |
| <span data-ttu-id="f244d-247">GET 1:1/group chat message</span><span class="sxs-lookup"><span data-stu-id="f244d-247">GET 1:1/group chat message</span></span>  | <span data-ttu-id="f244d-248">3 rps</span><span class="sxs-lookup"><span data-stu-id="f244d-248">3 rps</span></span> | <span data-ttu-id="f244d-249">30 rps</span><span class="sxs-lookup"><span data-stu-id="f244d-249">30 rps</span></span> |
| <span data-ttu-id="f244d-250">POST channel message</span><span class="sxs-lookup"><span data-stu-id="f244d-250">POST channel message</span></span> | <span data-ttu-id="f244d-251">2 rps</span><span class="sxs-lookup"><span data-stu-id="f244d-251">2 rps</span></span> | <span data-ttu-id="f244d-252">20 rps</span><span class="sxs-lookup"><span data-stu-id="f244d-252">20 rps</span></span> |
| <span data-ttu-id="f244d-253">POST 1:1/group chat message</span><span class="sxs-lookup"><span data-stu-id="f244d-253">POST 1:1/group chat message</span></span> | <span data-ttu-id="f244d-254">2 rps</span><span class="sxs-lookup"><span data-stu-id="f244d-254">2 rps</span></span> | <span data-ttu-id="f244d-255">20 rps</span><span class="sxs-lookup"><span data-stu-id="f244d-255">20 rps</span></span> |
| <span data-ttu-id="f244d-256">GET/teams/```{team-id}```/在以下路径下的日程安排和所有 API</span><span class="sxs-lookup"><span data-stu-id="f244d-256">GET /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="f244d-257">60 rps</span><span class="sxs-lookup"><span data-stu-id="f244d-257">60 rps</span></span> | <span data-ttu-id="f244d-258">600 rps</span><span class="sxs-lookup"><span data-stu-id="f244d-258">600 rps</span></span> |
| <span data-ttu-id="f244d-259">POST, PATCH, PUT /teams/```{team-id}```/在以下路径下的日程安排和所有 API</span><span class="sxs-lookup"><span data-stu-id="f244d-259">POST, PATCH, PUT /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="f244d-260">30 rps</span><span class="sxs-lookup"><span data-stu-id="f244d-260">30 rps</span></span> | <span data-ttu-id="f244d-261">300 rps</span><span class="sxs-lookup"><span data-stu-id="f244d-261">300 rps</span></span> |
| <span data-ttu-id="f244d-262">DELETE /teams/```{team-id}```/在以下路径下的日程安排和所有 API</span><span class="sxs-lookup"><span data-stu-id="f244d-262">DELETE /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="f244d-263">15 rps</span><span class="sxs-lookup"><span data-stu-id="f244d-263">15 rps</span></span> | <span data-ttu-id="f244d-264">150 rps</span><span class="sxs-lookup"><span data-stu-id="f244d-264">150 rps</span></span> |

<span data-ttu-id="f244d-265">对于给定团队或频道，每个应用最多可发布 4 个请求。</span><span class="sxs-lookup"><span data-stu-id="f244d-265">A maximum of 4 requests per second per app can be issued on a given team or channel.</span></span>
<span data-ttu-id="f244d-266">每个应用每天最多可以将 3000 条消息发送到给定的频道。</span><span class="sxs-lookup"><span data-stu-id="f244d-266">A maximum of 3000 messages per app per day can be sent to a given channel.</span></span>

<span data-ttu-id="f244d-267">另请参阅 [Microsoft Teams 限制](/graph/api/resources/teams-api-overview#microsoft-teams-limits)和[投票要求](/graph/api/resources/teams-api-overview#polling-requirements)。</span><span class="sxs-lookup"><span data-stu-id="f244d-267">See also [Microsoft Teams limits](/graph/api/resources/teams-api-overview#microsoft-teams-limits) and [polling requirements](/graph/api/resources/teams-api-overview#polling-requirements).</span></span>

### <a name="identity-protection-and-conditional-access-service-limits"></a><span data-ttu-id="f244d-268">身份保护和条件访问服务限制</span><span class="sxs-lookup"><span data-stu-id="f244d-268">Identity protection and conditional access service limits</span></span>

| <span data-ttu-id="f244d-269">请求类型</span><span class="sxs-lookup"><span data-stu-id="f244d-269">Request type</span></span> | <span data-ttu-id="f244d-270">每个租户的使用限制</span><span class="sxs-lookup"><span data-stu-id="f244d-270">Limit per tenant</span></span> |
| ------------ | ------- |
| <span data-ttu-id="f244d-271">任何</span><span class="sxs-lookup"><span data-stu-id="f244d-271">Any</span></span> | <span data-ttu-id="f244d-272">每秒1个请求</span><span class="sxs-lookup"><span data-stu-id="f244d-272">1 request per second</span></span> |

<span data-ttu-id="f244d-273">上述限制适用于下列资源:</span><span class="sxs-lookup"><span data-stu-id="f244d-273">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="f244d-274">riskDetection, riskyUser, riskyUserHistoryItem, namedLocation, countryNamedLocation, ipNamedLocation, conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="f244d-274">riskDetection, riskyUser, riskyUserHistoryItem, namedLocation, countryNamedLocation, ipNamedLocation, conditionalAccessPolicy.</span></span>

> <span data-ttu-id="f244d-275">**备注:** 目前上面列出的资源没有返回`Retry-After`页眉`429 Too Many Requests`上答复。</span><span class="sxs-lookup"><span data-stu-id="f244d-275">**Note:** at the moment the resources listed above do not return a `Retry-After` header on `429 Too Many Requests` responses.</span></span>
### <a name="insights-service-limits"></a><span data-ttu-id="f244d-276">见解服务限制</span><span class="sxs-lookup"><span data-stu-id="f244d-276">Insights service limits</span></span>

<span data-ttu-id="f244d-277">以下限制适用于 `me/insights`或`users/{id}/insights` 上的所有请求。</span><span class="sxs-lookup"><span data-stu-id="f244d-277">The following limits apply to any request on `me/insights` or `users/{id}/insights`.</span></span>

| <span data-ttu-id="f244d-278">限制</span><span class="sxs-lookup"><span data-stu-id="f244d-278">Limit</span></span>                                                      | <span data-ttu-id="f244d-279">适用对象</span><span class="sxs-lookup"><span data-stu-id="f244d-279">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="f244d-280">10 分钟内的 10,000 个 API 请求</span><span class="sxs-lookup"><span data-stu-id="f244d-280">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="f244d-281">v1.0 和 beta 终结点</span><span class="sxs-lookup"><span data-stu-id="f244d-281">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="f244d-282">4 个并发请求</span><span class="sxs-lookup"><span data-stu-id="f244d-282">4 concurrent requests</span></span>                                      | <span data-ttu-id="f244d-283">v1.0 和 beta 终结点</span><span class="sxs-lookup"><span data-stu-id="f244d-283">v1.0 and beta endpoints</span></span>   |

### <a name="microsoft-graph-reports-service-limits"></a><span data-ttu-id="f244d-284">Microsoft Graph 报告的服务限制</span><span class="sxs-lookup"><span data-stu-id="f244d-284">Microsoft Graph reports service limits</span></span>

<span data-ttu-id="f244d-285">以下限制适用于 `/reports` 上的所有请求。</span><span class="sxs-lookup"><span data-stu-id="f244d-285">The following limits apply to any request on `/reports`.</span></span>

| <span data-ttu-id="f244d-286">操作</span><span class="sxs-lookup"><span data-stu-id="f244d-286">Operation</span></span>                 | <span data-ttu-id="f244d-287">每个租户每个应用限制</span><span class="sxs-lookup"><span data-stu-id="f244d-287">Limit per app per tenant</span></span>     | <span data-ttu-id="f244d-288">每个租户的使用限制</span><span class="sxs-lookup"><span data-stu-id="f244d-288">Limit per tenant</span></span>           |
|---------------------------|------------------------------|----------------------------|
| <span data-ttu-id="f244d-289">任何请求（CSV）</span><span class="sxs-lookup"><span data-stu-id="f244d-289">Any request (CSV)</span></span>         | <span data-ttu-id="f244d-290">每10分钟14个请求</span><span class="sxs-lookup"><span data-stu-id="f244d-290">14 requests per 10 minutes</span></span>   | <span data-ttu-id="f244d-291">每10分钟40个请求</span><span class="sxs-lookup"><span data-stu-id="f244d-291">40 requests per 10 minutes</span></span> |
| <span data-ttu-id="f244d-292">任何请求（JSON、beta）</span><span class="sxs-lookup"><span data-stu-id="f244d-292">Any request (JSON, beta)</span></span>  | <span data-ttu-id="f244d-293">每10分钟100个请求</span><span class="sxs-lookup"><span data-stu-id="f244d-293">100 requests per 10 minutes</span></span>  | <span data-ttu-id="f244d-294">不适用</span><span class="sxs-lookup"><span data-stu-id="f244d-294">n/a</span></span>                        |

<span data-ttu-id="f244d-295">上述限制分别适用于每个报表 API。</span><span class="sxs-lookup"><span data-stu-id="f244d-295">The preceding limits apply individually to each report API.</span></span> <span data-ttu-id="f244d-296">例如，在10分钟内分别有对 Microsoft Teams 用户活动报告API的请求及对 Outlook 用户活动报告API的请求，将分别被视为14个请求中的1个请求，而不是14个请求中的2个请求。</span><span class="sxs-lookup"><span data-stu-id="f244d-296">For example a request to Microsoft Teams user activity report API and a request to Outlook user activity report API within 10 minutes will count as 1 request out of 14 for each API, not 2 requests out of 14 for both.</span></span>

### <a name="invitation-manager-service-limits"></a><span data-ttu-id="f244d-297">邀请管理器服务限制</span><span class="sxs-lookup"><span data-stu-id="f244d-297">Invitation manager service limits</span></span>

<span data-ttu-id="f244d-298">以下限制适用于 `/invitations` 上的所有请求。</span><span class="sxs-lookup"><span data-stu-id="f244d-298">The following limits apply to any request on `/invitations`.</span></span>

| <span data-ttu-id="f244d-299">操作</span><span class="sxs-lookup"><span data-stu-id="f244d-299">Operation</span></span>                 | <span data-ttu-id="f244d-300">每个租户的使用限制</span><span class="sxs-lookup"><span data-stu-id="f244d-300">Limit per tenant</span></span>             |
|---------------------------|------------------------------|
| <span data-ttu-id="f244d-301">任何操作</span><span class="sxs-lookup"><span data-stu-id="f244d-301">Any operation</span></span>             | <span data-ttu-id="f244d-302">每 5 秒 150 个请求</span><span class="sxs-lookup"><span data-stu-id="f244d-302">150 requests per 5 seconds</span></span>   |

<!-- { "blockType": "throttlinggenstart" } -->
### <a name="education-service-limits"></a><span data-ttu-id="f244d-303">教育版服务限制</span><span class="sxs-lookup"><span data-stu-id="f244d-303">Education service limits</span></span>

[!INCLUDE [Education rostering APIS throttling documentation](../includes/throttling-education-rostering-apis.md)]

### <a name="excel-service-limits"></a><span data-ttu-id="f244d-304">Excel 服务限制</span><span class="sxs-lookup"><span data-stu-id="f244d-304">Excel service limits</span></span>

[!INCLUDE [Excel throttling documentation](../includes/throttling-excel.md)]

### <a name="identity-and-access-audit-logs-service-limits"></a><span data-ttu-id="f244d-305">标识和访问审核日志的服务限制</span><span class="sxs-lookup"><span data-stu-id="f244d-305">Identity and access audit logs service limits</span></span>

[!INCLUDE [Identity and access audit logs throttling documentation](../includes/throttling-Identity-and-access-audit-logs.md)]

### <a name="identity-providers-service-limits"></a><span data-ttu-id="f244d-306">身份提供程序的服务限制</span><span class="sxs-lookup"><span data-stu-id="f244d-306">Identity providers service limits</span></span>

[!INCLUDE [CPIM throttling documentation](../includes/throttling-cpim.md)]

### <a name="intune-service-limits"></a><span data-ttu-id="f244d-307">Intune服务限制</span><span class="sxs-lookup"><span data-stu-id="f244d-307">Intune service limits</span></span>

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

### <a name="skype-service-limits"></a><span data-ttu-id="f244d-308">Skype 服务限制</span><span class="sxs-lookup"><span data-stu-id="f244d-308">Skype service limits</span></span>

[!INCLUDE [Skype calling throttling documentation](../includes/throttling-skype-calling.md)]

### <a name="subscription-service-limits"></a><span data-ttu-id="f244d-309">订阅服务</span><span class="sxs-lookup"><span data-stu-id="f244d-309">Subscription service limits</span></span>

[!INCLUDE [Subscription services throttling documentation](../includes/throttling-subscription-services.md)]

<!-- { "blockType": "throttlinggenend" } -->
