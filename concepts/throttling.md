# <a name="microsoft-graph-throttling-guidance"></a><span data-ttu-id="2dbf3-101">Microsoft Graph 限制指南</span><span class="sxs-lookup"><span data-stu-id="2dbf3-101">Microsoft Graph throttling guidance</span></span>


<span data-ttu-id="2dbf3-p101">限制可调节并发调用服务的数量，以防止资源的过度使用。Microsoft Graph 旨在用于处理大量的请求。如果出现过多请求，限制将有助于保持 Microsoft Graph 的最佳性能和服务的可靠性。</span><span class="sxs-lookup"><span data-stu-id="2dbf3-p101">Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span></span>

<span data-ttu-id="2dbf3-p102">根据该方案，执行的限制会有所不同。例如，如果你正在执行大量的写入操作，限制的可能性会比仅执行读取时要高。</span><span class="sxs-lookup"><span data-stu-id="2dbf3-p102">Throttling limits vary based on the scenario. For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span></span>

## <a name="what-happens-when-throttling-occurs"></a><span data-ttu-id="2dbf3-107">在限制时，会发生什么情况？</span><span class="sxs-lookup"><span data-stu-id="2dbf3-107">What happens when throttling occurs?</span></span>

<span data-ttu-id="2dbf3-p103">超出限制阈值后，Microsoft Graph 会在一段时间内限制来自该客户端的任何进一步的请求。发生限制时，Microsoft Graph 将返回 HTTP 状态代码 429（请求过多），同时请求失败。在失败的请求的响应标头中返回建议的等待时间。限制行为取决于请求的类型和数量。例如，如果你有大量的请求，则所有请求类型受限。阈值限制根据请求类型而有所不同。因此，你可能会遇到这样一种场景，在场景中，写入被限制，但仍允许读取。</span><span class="sxs-lookup"><span data-stu-id="2dbf3-p103">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time. When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail. A suggested wait time is returned in the response header of the failed request. Throttling behavior can depend on the type and number of requests. For example, if you have a high volume of requests, all requests types are throttled. Threshold limits vary based on the request type. Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span> 

## <a name="common-throttling-scenarios"></a><span data-ttu-id="2dbf3-115">常见的限制场景</span><span class="sxs-lookup"><span data-stu-id="2dbf3-115">Common throttling scenarios</span></span>

<span data-ttu-id="2dbf3-116">客户端受限的最常见原因包括：</span><span class="sxs-lookup"><span data-stu-id="2dbf3-116">The most common causes of throttling of clients include:</span></span>

* <span data-ttu-id="2dbf3-117">来自租户中所有应用程序的请求太多。</span><span class="sxs-lookup"><span data-stu-id="2dbf3-117">A large number of requests across all applications in a tenant.</span></span>
* <span data-ttu-id="2dbf3-118">来自所有租户中特定应用程序的请求太多。</span><span class="sxs-lookup"><span data-stu-id="2dbf3-118">A large number of requests from a particular application across all tenants.</span></span>

## <a name="best-practices-to-handle-throttling"></a><span data-ttu-id="2dbf3-119">处理限制的最佳实践</span><span class="sxs-lookup"><span data-stu-id="2dbf3-119">Best practices to handle throttling</span></span>

<span data-ttu-id="2dbf3-120">以下是处理限制的最佳做法：</span><span class="sxs-lookup"><span data-stu-id="2dbf3-120">The following are best practices for handling throttling:</span></span>

* <span data-ttu-id="2dbf3-121">减少每个请求的操作数量。</span><span class="sxs-lookup"><span data-stu-id="2dbf3-121">Reduce the number of operations per request.</span></span>
* <span data-ttu-id="2dbf3-122">减少调用频率。</span><span class="sxs-lookup"><span data-stu-id="2dbf3-122">Reduce the frequency of calls.</span></span>
* <span data-ttu-id="2dbf3-123">避免立即重试，因为所有请求都会计入使用限制。</span><span class="sxs-lookup"><span data-stu-id="2dbf3-123">Avoid immediate retries, because all requests accrue against your usage limits.</span></span>

<span data-ttu-id="2dbf3-124">进行错误处理时，使用 HTTP 错误代码 429 检测限制。</span><span class="sxs-lookup"><span data-stu-id="2dbf3-124">When you implement error handling, use the HTTP error code 429 to detect throttling.</span></span> <span data-ttu-id="2dbf3-125">失败响应的响应头中有“重试间隔”**字段。</span><span class="sxs-lookup"><span data-stu-id="2dbf3-125">The failed response includes the *Retry-After* field in the response header.</span></span> <span data-ttu-id="2dbf3-126">使用*重试间隔*延迟回退请求是从限制中恢复的最快速方式，因为 Microsoft Graph 会在客户端受限时继续记录资源使用状况。</span><span class="sxs-lookup"><span data-stu-id="2dbf3-126">When you implement error handling, use the HTTP error code 429 to detect throttling. The failed response includes the Retry-After field in the response header. Backing off requests using the *Retry-After* delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span></span>

1. <span data-ttu-id="2dbf3-127">等待“重试间隔”**字段中指定的秒数。</span><span class="sxs-lookup"><span data-stu-id="2dbf3-127">Wait the number of seconds specified in the *Retry-After* field.</span></span>
2. <span data-ttu-id="2dbf3-128">重试请求。</span><span class="sxs-lookup"><span data-stu-id="2dbf3-128">Retry the request.</span></span>
3. <span data-ttu-id="2dbf3-p105">如果请求再次失败，并显示 429 错误代码，则表示你仍然受限。继续使用建议的重试间隔延迟并重试请求直到成功。</span><span class="sxs-lookup"><span data-stu-id="2dbf3-p105">If the request fails again with a 429 error code, you are still being throttled. Continue to use the recommended Retry-After delay and retry the request until it succeeds.</span></span>

<span data-ttu-id="2dbf3-131">下列资源目前提供“重试间隔”头：</span><span class="sxs-lookup"><span data-stu-id="2dbf3-131">The following resources currently provide a retry-after header:</span></span>
- [<span data-ttu-id="2dbf3-132">用户</span><span class="sxs-lookup"><span data-stu-id="2dbf3-132">User</span></span>](../api-reference/v1.0/resources/user.md)
- [<span data-ttu-id="2dbf3-133">照片</span><span class="sxs-lookup"><span data-stu-id="2dbf3-133">Photo</span></span>](../api-reference/v1.0/resources/profilephoto.md)
- [<span data-ttu-id="2dbf3-134">邮件</span><span class="sxs-lookup"><span data-stu-id="2dbf3-134">mail</span></span>](../api-reference/v1.0/resources/message.md)
- [<span data-ttu-id="2dbf3-135">日历（用户和组）</span><span class="sxs-lookup"><span data-stu-id="2dbf3-135">Calendar (users and groups)</span></span>](../api-reference/v1.0/resources/event.md)
- [<span data-ttu-id="2dbf3-136">联系人</span><span class="sxs-lookup"><span data-stu-id="2dbf3-136">Contact</span></span>](../api-reference/v1.0/resources/contact.md)
- [<span data-ttu-id="2dbf3-137">附件</span><span class="sxs-lookup"><span data-stu-id="2dbf3-137">Attachment</span></span>](../api-reference/v1.0/resources/attachment.md)
- [<span data-ttu-id="2dbf3-138">组对话</span><span class="sxs-lookup"><span data-stu-id="2dbf3-138">Group conversations</span></span>](../api-reference/v1.0/resources/conversation.md)
- [<span data-ttu-id="2dbf3-139">人员和社交活动</span><span class="sxs-lookup"><span data-stu-id="2dbf3-139">People and social</span></span>](../api-reference/beta/resources/social_overview.md)
- [<span data-ttu-id="2dbf3-140">Drive (OneDrive)</span><span class="sxs-lookup"><span data-stu-id="2dbf3-140">Drive (OneDrive)</span></span>](../api-reference/v1.0/resources/drive.md)

<span data-ttu-id="2dbf3-141">有关 Microsoft 云限制的更广泛讨论，请参阅[限制模式]((https://msdn.microsoft.com/zh-CN/library/office/dn589798.aspx))。</span><span class="sxs-lookup"><span data-stu-id="2dbf3-141">For a broader discussion of throttling on the Microsoft Cloud, see [Throttling Pattern]((https://msdn.microsoft.com/zh-CN/library/office/dn589798.aspx)).</span></span>
