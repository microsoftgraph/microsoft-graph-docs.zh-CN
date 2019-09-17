---
title: Microsoft Graph 限制指南
description: 限制可调节并发调用服务的数量，以防止资源的过度使用。Microsoft Graph 旨在用于处理大量的请求。如果出现过多请求，限制将有助于保持 Microsoft Graph 的最佳性能和服务的可靠性。
author: piotrci
localization_priority: Priority
ms.openlocfilehash: 780beda25a05675a77a933496dcce6fe5cd1a453
ms.sourcegitcommit: c739cbfab42181adfcda409ca12514ab7f4832b1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2019
ms.locfileid: "36982864"
---
# <a name="microsoft-graph-throttling-guidance"></a><span data-ttu-id="00657-105">Microsoft Graph 限制指南</span><span class="sxs-lookup"><span data-stu-id="00657-105">Microsoft Graph throttling guidance</span></span>

<span data-ttu-id="00657-p102">限制可调节并发调用服务的数量，以防止资源的过度使用。Microsoft Graph 旨在用于处理大量的请求。如果出现过多请求，限制将有助于保持 Microsoft Graph 的最佳性能和服务的可靠性。</span><span class="sxs-lookup"><span data-stu-id="00657-p102">Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span></span>

<span data-ttu-id="00657-p103">根据该方案，执行的限制会有所不同。例如，如果你正在执行大量的写入操作，限制的可能性会比仅执行读取时要高。</span><span class="sxs-lookup"><span data-stu-id="00657-p103">Throttling limits vary based on the scenario. For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span></span>

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a><span data-ttu-id="00657-111">在限制时，会发生什么情况？</span><span class="sxs-lookup"><span data-stu-id="00657-111">What happens when throttling occurs?</span></span>
<!-- markdownlint-enable MD026 -->

<span data-ttu-id="00657-p104">超出限制阈值后，Microsoft Graph 会在一段时间内限制来自该客户端的任何进一步的请求。发生限制时，Microsoft Graph 将返回 HTTP 状态代码 429（请求过多），同时请求失败。在失败的请求的响应标头中返回建议的等待时间。限制行为取决于请求的类型和数量。例如，如果你有大量的请求，则所有请求类型受限。阈值限制根据请求类型而有所不同。因此，你可能会遇到这样一种场景，在场景中，写入被限制，但仍允许读取。</span><span class="sxs-lookup"><span data-stu-id="00657-p104">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time. When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail. A suggested wait time is returned in the response header of the failed request. Throttling behavior can depend on the type and number of requests. For example, if you have a high volume of requests, all requests types are throttled. Threshold limits vary based on the request type. Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span>

## <a name="common-throttling-scenarios"></a><span data-ttu-id="00657-119">常见的限制场景</span><span class="sxs-lookup"><span data-stu-id="00657-119">Common throttling scenarios</span></span>

<span data-ttu-id="00657-120">客户端受限的最常见原因包括：</span><span class="sxs-lookup"><span data-stu-id="00657-120">The most common causes of throttling of clients include:</span></span>

- <span data-ttu-id="00657-121">来自租户中所有应用程序的请求太多。</span><span class="sxs-lookup"><span data-stu-id="00657-121">A large number of requests across all applications in a tenant.</span></span>
- <span data-ttu-id="00657-122">来自所有租户中特定应用程序的请求太多。</span><span class="sxs-lookup"><span data-stu-id="00657-122">A large number of requests from a particular application across all tenants.</span></span>

## <a name="best-practices-to-handle-throttling"></a><span data-ttu-id="00657-123">处理限制的最佳实践</span><span class="sxs-lookup"><span data-stu-id="00657-123">Best practices to handle throttling</span></span>

<span data-ttu-id="00657-124">以下是处理限制的最佳做法：</span><span class="sxs-lookup"><span data-stu-id="00657-124">The following are best practices for handling throttling:</span></span>

- <span data-ttu-id="00657-125">减少每个请求的操作数量。</span><span class="sxs-lookup"><span data-stu-id="00657-125">Reduce the number of operations per request.</span></span>
- <span data-ttu-id="00657-126">减少调用频率。</span><span class="sxs-lookup"><span data-stu-id="00657-126">Reduce the frequency of calls.</span></span>
- <span data-ttu-id="00657-127">不要立即重试，因为所有请求都会计入使用限制。</span><span class="sxs-lookup"><span data-stu-id="00657-127">Avoid immediate retries, because all requests accrue against your usage limits.</span></span>

<span data-ttu-id="00657-p105">进行错误处理时，使用 HTTP 错误代码 429 检测限制。失败的响应包括 `Retry-After` 响应标头。使用 `Retry-After` 延迟回退请求是从限制中恢复的最快速的方式，因为 Microsoft Graph 会在客户端受限时继续记录资源使用状况。</span><span class="sxs-lookup"><span data-stu-id="00657-p105">When you implement error handling, use the HTTP error code 429 to detect throttling. The failed response includes the `Retry-After` field in the response header. Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span></span>

1. <span data-ttu-id="00657-131">等待 `Retry-After` 标头中指定的秒数。</span><span class="sxs-lookup"><span data-stu-id="00657-131">Wait the number of seconds specified in the `Retry-After` field.</span></span>
2. <span data-ttu-id="00657-132">请重试请求。</span><span class="sxs-lookup"><span data-stu-id="00657-132">Retry the request.</span></span>
3. <span data-ttu-id="00657-p106">如果请求再次失败，并显示 429 错误代码，则表示你仍然受限。继续使用建议的 `Retry-After` 延迟并重试请求直到成功。</span><span class="sxs-lookup"><span data-stu-id="00657-p106">If the request fails again with a 429 error code, you are still being throttled. Continue to use the recommended Retry-After delay and retry the request until it succeeds.</span></span>

<span data-ttu-id="00657-135">下列资源目前提供 `Retry-After` 标头：</span><span class="sxs-lookup"><span data-stu-id="00657-135">The following resources currently provide a retry-after header:</span></span>

- [<span data-ttu-id="00657-136">用户</span><span class="sxs-lookup"><span data-stu-id="00657-136">User</span></span>](/graph/api/resources/user?view=graph-rest-1.0)
- [<span data-ttu-id="00657-137">照片</span><span class="sxs-lookup"><span data-stu-id="00657-137">Photo</span></span>](/graph/api/resources/profilephoto?view=graph-rest-1.0)
- [<span data-ttu-id="00657-138">邮件</span><span class="sxs-lookup"><span data-stu-id="00657-138">Mail</span></span>](/graph/api/resources/message?view=graph-rest-1.0)
- [<span data-ttu-id="00657-139">日历（用户和组）</span><span class="sxs-lookup"><span data-stu-id="00657-139">Calendar (users and groups)</span></span>](/graph/api/resources/event?view=graph-rest-1.0)
- [<span data-ttu-id="00657-140">联系人</span><span class="sxs-lookup"><span data-stu-id="00657-140">Contact</span></span>](/graph/api/resources/contact?view=graph-rest-1.0)
- [<span data-ttu-id="00657-141">附件</span><span class="sxs-lookup"><span data-stu-id="00657-141">Attachment</span></span>](/graph/api/resources/attachment?view=graph-rest-1.0)
- [<span data-ttu-id="00657-142">组对话</span><span class="sxs-lookup"><span data-stu-id="00657-142">Group conversations</span></span>](/graph/api/resources/conversation?view=graph-rest-1.0)
- [<span data-ttu-id="00657-143">人员和社交活动</span><span class="sxs-lookup"><span data-stu-id="00657-143">People and social</span></span>](/graph/api/resources/social-overview?view=graph-rest-beta)
- [<span data-ttu-id="00657-144">Drive (OneDrive)</span><span class="sxs-lookup"><span data-stu-id="00657-144">Drive (OneDrive)</span></span>](/graph/api/resources/drive?view=graph-rest-1.0)

<span data-ttu-id="00657-145">有关 Microsoft 云限制的更广泛讨论，请参阅[限制模式](https://msdn.microsoft.com/library/office/dn589798.aspx)。</span><span class="sxs-lookup"><span data-stu-id="00657-145">For a broader discussion of throttling on the Microsoft Cloud, see [Throttling Pattern](https://msdn.microsoft.com/library/office/dn589798.aspx).</span></span>

## <a name="service-specific-limits"></a><span data-ttu-id="00657-146">服务特定限制</span><span class="sxs-lookup"><span data-stu-id="00657-146">Service-specific limits</span></span>

<span data-ttu-id="00657-147">借助 Microsoft Graph，用户可访问[多个服务](overview-major-services.md)中的数据，如 Outlook 或 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="00657-147">Microsoft Graph allows you to access data in [multiple services](overview-major-services.md), such as Outlook or Azure Active Directory.</span></span> <span data-ttu-id="00657-148">这些服务实施自己的限制，这些限制会影响使用 Microsoft Graph 访问它们的应用程序。</span><span class="sxs-lookup"><span data-stu-id="00657-148">These services impose their own throttling limits that affect applications that use Microsoft Graph to access them.</span></span>

> [!NOTE]
> <span data-ttu-id="00657-149">此处所述的具体限制可能会发生更改。</span><span class="sxs-lookup"><span data-stu-id="00657-149">The specific limits described here are subject to change.</span></span>

### <a name="outlook-service-limits"></a><span data-ttu-id="00657-150">Outlook 服务限制</span><span class="sxs-lookup"><span data-stu-id="00657-150">Outlook service limits</span></span>

<span data-ttu-id="00657-151">将评估每个应用 ID 和邮箱组合的 Outlook 服务限制。</span><span class="sxs-lookup"><span data-stu-id="00657-151">Outlook service limits are evaluated for each app ID and mailbox combination.</span></span> <span data-ttu-id="00657-152">换言之，上述限制适用于访问特定邮箱（用户或组）的特定应用。</span><span class="sxs-lookup"><span data-stu-id="00657-152">In other words, the limits described apply to a specific app accessing a specific mailbox (user or group).</span></span> <span data-ttu-id="00657-153">如果一个邮箱的应用程序超过限制，不会影响访问另一个邮箱的功能。</span><span class="sxs-lookup"><span data-stu-id="00657-153">If an application exceeds the limit in one mailbox, it does not affect the ability to access another mailbox.</span></span>

| <span data-ttu-id="00657-154">限制</span><span class="sxs-lookup"><span data-stu-id="00657-154">Limit</span></span>                                                      | <span data-ttu-id="00657-155">适用对象</span><span class="sxs-lookup"><span data-stu-id="00657-155">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="00657-156">10 分钟内的 10,000 个 API 请求</span><span class="sxs-lookup"><span data-stu-id="00657-156">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="00657-157">v1.0 和 beta 终结点</span><span class="sxs-lookup"><span data-stu-id="00657-157">v1.0 and beta</span></span> |
| <span data-ttu-id="00657-158">4 个并发请求</span><span class="sxs-lookup"><span data-stu-id="00657-158">4 concurrent requests</span></span>                                      | <span data-ttu-id="00657-159">Beta 终结点</span><span class="sxs-lookup"><span data-stu-id="00657-159">Beta endpoint</span></span>   |
| <span data-ttu-id="00657-160">30 秒内的 15 兆位上传（PATCH、POST、PUT）</span><span class="sxs-lookup"><span data-stu-id="00657-160">15 megabit upload (PATCH, POST, PUT) in a 30 second period</span></span> | <span data-ttu-id="00657-161">Beta 终结点</span><span class="sxs-lookup"><span data-stu-id="00657-161">Beta endpoint</span></span>   |

#### <a name="outlook-service-resources"></a><span data-ttu-id="00657-162">Outlook 服务资源</span><span class="sxs-lookup"><span data-stu-id="00657-162">Outlook service resources</span></span>

<span data-ttu-id="00657-163">Outlook 服务提供以下资源。</span><span class="sxs-lookup"><span data-stu-id="00657-163">The following resources are provided by the Outlook service.</span></span>

##### <a name="calendar-api-resources"></a><span data-ttu-id="00657-164">日历 API 资源</span><span class="sxs-lookup"><span data-stu-id="00657-164">Calendar API resources</span></span>

- [<span data-ttu-id="00657-165">event</span><span class="sxs-lookup"><span data-stu-id="00657-165">event</span></span>](/graph/api/resources/event)
- [<span data-ttu-id="00657-166">eventMessage</span><span class="sxs-lookup"><span data-stu-id="00657-166">eventMessage</span></span>](/graph/api/resources/eventmessage)
- [<span data-ttu-id="00657-167">calendar</span><span class="sxs-lookup"><span data-stu-id="00657-167">calendar</span></span>](/graph/api/resources/calendar)
- [<span data-ttu-id="00657-168">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="00657-168">calendarGroup</span></span>](/graph/api/resources/calendargroup)
- [<span data-ttu-id="00657-169">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="00657-169">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="00657-170">attachment</span><span class="sxs-lookup"><span data-stu-id="00657-170">attachment</span></span>](/graph/api/resources/attachment)
- [<span data-ttu-id="00657-171">place（预览）</span><span class="sxs-lookup"><span data-stu-id="00657-171">place (preview)</span></span>](/graph/api/resources/place)

##### <a name="mail-api-resources"></a><span data-ttu-id="00657-172">邮件 API 资源</span><span class="sxs-lookup"><span data-stu-id="00657-172">Mail API resources</span></span>

- [<span data-ttu-id="00657-173">message</span><span class="sxs-lookup"><span data-stu-id="00657-173">message</span></span>](/graph/api/resources/message)
- [<span data-ttu-id="00657-174">mailFolder</span><span class="sxs-lookup"><span data-stu-id="00657-174">mailFolder</span></span>](/graph/api/resources/mailfolder)
- <span data-ttu-id="00657-175">[mailSearchFolder](/graph/api/resources/mailsearchfolder)</span><span class="sxs-lookup"><span data-stu-id="00657-175">Added [mailSearchFolder](/graph/api/resources/mailsearchfolder).</span></span>
- [<span data-ttu-id="00657-176">messageRule</span><span class="sxs-lookup"><span data-stu-id="00657-176">messageRule</span></span>](/graph/api/resources/messagerule)
- [<span data-ttu-id="00657-177">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="00657-177">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="00657-178">attachment</span><span class="sxs-lookup"><span data-stu-id="00657-178">attachment</span></span>](/graph/api/resources/attachment)

##### <a name="personal-contacts-api-resources"></a><span data-ttu-id="00657-179">个人联系人 API 资源</span><span class="sxs-lookup"><span data-stu-id="00657-179">Personal contacts API resources</span></span>

- [<span data-ttu-id="00657-180">contact</span><span class="sxs-lookup"><span data-stu-id="00657-180">contact</span></span>](/graph/api/resources/contact)
- [<span data-ttu-id="00657-181">contactFolder</span><span class="sxs-lookup"><span data-stu-id="00657-181">contactFolder</span></span>](/graph/api/resources/contactfolder)
- [<span data-ttu-id="00657-182">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="00657-182">outlookCategory</span></span>](/graph/api/resources/outlookcategory)

##### <a name="social-and-workplace-intelligence-resources"></a><span data-ttu-id="00657-183">社交和工作区智能资源</span><span class="sxs-lookup"><span data-stu-id="00657-183">Social and workplace intelligence resources</span></span>

- [<span data-ttu-id="00657-184">person</span><span class="sxs-lookup"><span data-stu-id="00657-184">person</span></span>](/graph/api/resources/person)

##### <a name="to-do-tasks-api-preview-resources"></a><span data-ttu-id="00657-185">待办任务 API（预览）资源</span><span class="sxs-lookup"><span data-stu-id="00657-185">To-do tasks API (preview) resources</span></span>

- [<span data-ttu-id="00657-186">outlookTask</span><span class="sxs-lookup"><span data-stu-id="00657-186">outlookTask</span></span>](/graph/api/resources/outlooktask)
- [<span data-ttu-id="00657-187">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="00657-187">outlookTaskFolder</span></span>](/graph/api/resources/outlooktaskfolder)
- [<span data-ttu-id="00657-188">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="00657-188">outlookTaskGroup</span></span>](/graph/api/resources/outlooktaskgroup)
- [<span data-ttu-id="00657-189">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="00657-189">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="00657-190">attachment</span><span class="sxs-lookup"><span data-stu-id="00657-190">attachment</span></span>](/graph/api/resources/attachment)
