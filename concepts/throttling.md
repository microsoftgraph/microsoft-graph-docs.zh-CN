---
title: Microsoft Graph 限制指南
description: 限制可调节并发调用服务的数量，以防止资源的过度使用。Microsoft Graph 旨在用于处理大量的请求。如果出现过多请求，限制将有助于保持 Microsoft Graph 的最佳性能和服务的可靠性。
author: piotrci
localization_priority: Priority
ms.openlocfilehash: 8b3b8c5b0ec5a5209ad96f87dc677f4331c24e0b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580979"
---
# <a name="microsoft-graph-throttling-guidance"></a><span data-ttu-id="c32d4-105">Microsoft Graph 限制指南</span><span class="sxs-lookup"><span data-stu-id="c32d4-105">Microsoft Graph throttling guidance</span></span>


<span data-ttu-id="c32d4-p102">限制可调节并发调用服务的数量，以防止资源的过度使用。Microsoft Graph 旨在用于处理大量的请求。如果出现过多请求，限制将有助于保持 Microsoft Graph 的最佳性能和服务的可靠性。</span><span class="sxs-lookup"><span data-stu-id="c32d4-p102">Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span></span>

<span data-ttu-id="c32d4-p103">根据该方案，执行的限制会有所不同。例如，如果你正在执行大量的写入操作，限制的可能性会比仅执行读取时要高。</span><span class="sxs-lookup"><span data-stu-id="c32d4-p103">Throttling limits vary based on the scenario. For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span></span>

## <a name="what-happens-when-throttling-occurs"></a><span data-ttu-id="c32d4-111">在限制时，会发生什么情况？</span><span class="sxs-lookup"><span data-stu-id="c32d4-111">What happens when throttling occurs?</span></span>

<span data-ttu-id="c32d4-p104">超出限制阈值后，Microsoft Graph 会在一段时间内限制来自该客户端的任何进一步的请求。发生限制时，Microsoft Graph 将返回 HTTP 状态代码 429（请求过多），同时请求失败。在失败的请求的响应标头中返回建议的等待时间。限制行为取决于请求的类型和数量。例如，如果你有大量的请求，则所有请求类型受限。阈值限制根据请求类型而有所不同。因此，你可能会遇到这样一种场景，在场景中，写入被限制，但仍允许读取。</span><span class="sxs-lookup"><span data-stu-id="c32d4-p104">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time. When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail. A suggested wait time is returned in the response header of the failed request. Throttling behavior can depend on the type and number of requests. For example, if you have a high volume of requests, all requests types are throttled. Threshold limits vary based on the request type. Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span> 

## <a name="common-throttling-scenarios"></a><span data-ttu-id="c32d4-119">常见的限制场景</span><span class="sxs-lookup"><span data-stu-id="c32d4-119">Common throttling scenarios</span></span>

<span data-ttu-id="c32d4-120">客户端受限的最常见原因包括：</span><span class="sxs-lookup"><span data-stu-id="c32d4-120">The most common causes of throttling of clients include:</span></span>

* <span data-ttu-id="c32d4-121">来自租户中所有应用程序的请求太多。</span><span class="sxs-lookup"><span data-stu-id="c32d4-121">A large number of requests across all applications in a tenant.</span></span>
* <span data-ttu-id="c32d4-122">来自所有租户中特定应用程序的请求太多。</span><span class="sxs-lookup"><span data-stu-id="c32d4-122">A large number of requests from a particular application across all tenants.</span></span>

## <a name="best-practices-to-handle-throttling"></a><span data-ttu-id="c32d4-123">处理限制的最佳实践</span><span class="sxs-lookup"><span data-stu-id="c32d4-123">Best practices to handle throttling</span></span>

<span data-ttu-id="c32d4-124">以下是处理限制的最佳做法：</span><span class="sxs-lookup"><span data-stu-id="c32d4-124">The following are best practices for handling throttling:</span></span>

* <span data-ttu-id="c32d4-125">减少每个请求的操作数量。</span><span class="sxs-lookup"><span data-stu-id="c32d4-125">Reduce the number of operations per request.</span></span>
* <span data-ttu-id="c32d4-126">减少调用频率。</span><span class="sxs-lookup"><span data-stu-id="c32d4-126">Reduce the frequency of calls.</span></span>
* <span data-ttu-id="c32d4-127">不要立即重试，因为所有请求都会计入使用限制。</span><span class="sxs-lookup"><span data-stu-id="c32d4-127">Avoid immediate retries, because all requests accrue against your usage limits.</span></span>

<span data-ttu-id="c32d4-p105">进行错误处理时，使用 HTTP 错误代码 429 检测限制。失败的响应包括响应标头中的*重试间隔*字段。使用*重试间隔*延迟回退请求是从限制中恢复的最快速的方式，因为 Microsoft Graph 会在客户端受限时继续记录资源使用状况。</span><span class="sxs-lookup"><span data-stu-id="c32d4-p105">When you implement error handling, use the HTTP error code 429 to detect throttling. The failed response includes the *Retry-After* field in the response header. Backing off requests using the *Retry-After* delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span></span>

1. <span data-ttu-id="c32d4-131">等待“重试间隔”\*\* 字段中指定的秒数。</span><span class="sxs-lookup"><span data-stu-id="c32d4-131">Wait the number of seconds specified in the *Retry-After* field.</span></span>
2. <span data-ttu-id="c32d4-132">重试请求。</span><span class="sxs-lookup"><span data-stu-id="c32d4-132">Retry the request.</span></span>
3. <span data-ttu-id="c32d4-p106">如果请求再次失败，并显示 429 错误代码，则表示你仍然受限。继续使用建议的重试间隔延迟并重试请求直到成功。</span><span class="sxs-lookup"><span data-stu-id="c32d4-p106">If the request fails again with a 429 error code, you are still being throttled. Continue to use the recommended Retry-After delay and retry the request until it succeeds.</span></span>

<span data-ttu-id="c32d4-135">下列资源目前提供“重试间隔”头：</span><span class="sxs-lookup"><span data-stu-id="c32d4-135">The following resources currently provide a retry-after header:</span></span>
- [<span data-ttu-id="c32d4-136">用户</span><span class="sxs-lookup"><span data-stu-id="c32d4-136">User</span></span>](/graph/api/resources/user?view=graph-rest-1.0)
- [<span data-ttu-id="c32d4-137">照片</span><span class="sxs-lookup"><span data-stu-id="c32d4-137">Photo</span></span>](/graph/api/resources/profilephoto?view=graph-rest-1.0)
- [<span data-ttu-id="c32d4-138">邮件</span><span class="sxs-lookup"><span data-stu-id="c32d4-138">Mail</span></span>](/graph/api/resources/message?view=graph-rest-1.0)
- [<span data-ttu-id="c32d4-139">日历（用户和组）</span><span class="sxs-lookup"><span data-stu-id="c32d4-139">Calendar (users and groups)</span></span>](/graph/api/resources/event?view=graph-rest-1.0)
- [<span data-ttu-id="c32d4-140">联系人</span><span class="sxs-lookup"><span data-stu-id="c32d4-140">Contact</span></span>](/graph/api/resources/contact?view=graph-rest-1.0)
- [<span data-ttu-id="c32d4-141">附件</span><span class="sxs-lookup"><span data-stu-id="c32d4-141">Attachment</span></span>](/graph/api/resources/attachment?view=graph-rest-1.0)
- [<span data-ttu-id="c32d4-142">组对话</span><span class="sxs-lookup"><span data-stu-id="c32d4-142">Group conversations</span></span>](/graph/api/resources/conversation?view=graph-rest-1.0)
- [<span data-ttu-id="c32d4-143">人员和社交活动</span><span class="sxs-lookup"><span data-stu-id="c32d4-143">People and social</span></span>](/graph/api/resources/social-overview?view=graph-rest-beta)
- [<span data-ttu-id="c32d4-144">Drive (OneDrive)</span><span class="sxs-lookup"><span data-stu-id="c32d4-144">Drive (OneDrive)</span></span>](/graph/api/resources/drive?view=graph-rest-1.0)

<span data-ttu-id="c32d4-145">有关 Microsoft 云限制的更广泛讨论，请参阅[限制模式](https://msdn.microsoft.com/library/office/dn589798.aspx)。</span><span class="sxs-lookup"><span data-stu-id="c32d4-145">For a broader discussion of throttling on the Microsoft Cloud, see [Throttling Pattern](https://msdn.microsoft.com/library/office/dn589798.aspx).</span></span>
