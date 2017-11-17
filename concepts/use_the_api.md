# <a name="use-the-microsoft-graph-api"></a><span data-ttu-id="10b61-101">使用 Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="10b61-101">Use the Microsoft Graph API</span></span>

<span data-ttu-id="10b61-102">Microsoft Graph 一种是可让你访问 Microsoft 云服务资源的 REST 风格的 Web API.</span><span class="sxs-lookup"><span data-stu-id="10b61-102">Microsoft Graph is a RESTful web API that enables you to access Microsoft Cloud service resources.</span></span> <span data-ttu-id="10b61-103">在[注册应用](auth_register_app_v2.md)并[获取身份验证令牌以用于用户](auth_v2_user.md)或[服务](auth_v2_service.md)后，可以向 Microsoft Graph API 发送请求。</span><span class="sxs-lookup"><span data-stu-id="10b61-103">Microsoft Graph is a RESTful web API that enables you to access Microsoft Cloud service resources. After you [register your app](auth_register_app_v2.md) and [get authentication tokens for a user](auth_v2_user.md) or [service](auth_v2_service.md), you can make requests to the Microsoft Graph API.</span></span>

> <span data-ttu-id="10b61-104">**重要说明：**条件访问策略应用于 Microsoft Graph 的方式正在发生变化。</span><span class="sxs-lookup"><span data-stu-id="10b61-104">**Important:**  How conditional access policies apply to Microsoft Graph is changing.</span></span> <span data-ttu-id="10b61-105">应用程序需要进行更新以处理配置了条件访问策略的应用场景。</span><span class="sxs-lookup"><span data-stu-id="10b61-105">Applications need to be updated to handle scenarios where conditional access policies are configured.</span></span> <span data-ttu-id="10b61-106">有关详细信息和指南，请参阅 [Azure Active Directory 条件访问开发人员指南](https://docs.microsoft.com/azure/active-directory/develop/active-directory-conditional-access-developer)。</span><span class="sxs-lookup"><span data-stu-id="10b61-106">For more information and guidance, see [Developer Guidance for Azure Active Directory Conditional Access](https://docs.microsoft.com/azure/active-directory/develop/active-directory-conditional-access-developer).</span></span>

<span data-ttu-id="10b61-107">要在资源（如用户或电子邮件）中读取或写入资源，可以创建如下请求：</span><span class="sxs-lookup"><span data-stu-id="10b61-107">To read from or write to a resource such as a user or an email message, you construct a request that looks like the following.</span></span>

```http
https://graph.microsoft.com/{version}/{resource}?query-parameters
```

<span data-ttu-id="10b61-108">请求的组成部分包括：</span><span class="sxs-lookup"><span data-stu-id="10b61-108">The components of a request include:</span></span>

* <span data-ttu-id="10b61-109">[HTTP 方法](#http-methods) - 在 Microsoft Graph 请求上所使用的 HTTP 方法。</span><span class="sxs-lookup"><span data-stu-id="10b61-109">[HTTP method](#http-methods) - The HTTP method used on the request to Microsoft Graph.</span></span>
* <span data-ttu-id="10b61-110">[`{version}`](#version) - 你的应用程序正在使用的 Microsoft Graph API 版本。</span><span class="sxs-lookup"><span data-stu-id="10b61-110">[`{version}`](#version) - The version of the Microsoft Graph API your application is using.</span></span>
* <span data-ttu-id="10b61-111">[`{resource}`](#resource) - 你正在引用的 Microsoft Graph 中的资源。</span><span class="sxs-lookup"><span data-stu-id="10b61-111">[`{resource}`](#resource) - The resource in Microsoft Graph that you're referencing.</span></span>
* <span data-ttu-id="10b61-112">[查询参数](#query-parameters-optional) - 一组用于修改请求或响应的可选参数。</span><span class="sxs-lookup"><span data-stu-id="10b61-112">[query-parameters](#query-parameters-optional) - An optional set of parameters to modify the request or response.</span></span>

<span data-ttu-id="10b61-113">发出请求后，返回一个响应，其中包括：</span><span class="sxs-lookup"><span data-stu-id="10b61-113">After you make a request, a response is returned that includes:</span></span> 

* <span data-ttu-id="10b61-114">状态代码 - 表示成功或失败的 HTTP 状态代码。</span><span class="sxs-lookup"><span data-stu-id="10b61-114">Status code - An HTTP status code that indicates success or failure. For details about HTTP error codes, see Errors.</span></span> <span data-ttu-id="10b61-115">有关 HTTP 错误代码的详细信息，请参阅[错误](errors.md)。</span><span class="sxs-lookup"><span data-stu-id="10b61-115">For details about HTTP error codes, see [Errors](errors.md).</span></span>
* <span data-ttu-id="10b61-p104">响应消息 - 所请求的数据或操作结果。对于某些操作，响应消息可以为空。</span><span class="sxs-lookup"><span data-stu-id="10b61-p104">Response message - The data that you requested or the result of the operation. The response message can be empty for some operations.</span></span>
* <span data-ttu-id="10b61-118">**下一步**链接 - 如果请求返回大量数据，则需要通过选择“下一步”****浏览。</span><span class="sxs-lookup"><span data-stu-id="10b61-118">**Next** link - If your request returns a lot of data, you need to page through it by choosing **Next. For details, see Paging**.</span></span> <span data-ttu-id="10b61-119">有关详细信息，请参阅[分页](paging.md)。</span><span class="sxs-lookup"><span data-stu-id="10b61-119">For details, see [Paging](paging.md).</span></span>

## <a name="http-methods"></a><span data-ttu-id="10b61-120">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="10b61-120">HTTP methods</span></span>

<span data-ttu-id="10b61-p106">Microsoft Graph 使用请求上的 HTTP 方法来确定请求正在执行的操作。API 支持以下方法。</span><span class="sxs-lookup"><span data-stu-id="10b61-p106">Microsoft Graph uses the HTTP method on your request to determine what your request is doing. The API supports the following methods.</span></span>


|<span data-ttu-id="10b61-123">**方法**</span><span class="sxs-lookup"><span data-stu-id="10b61-123">**Method**</span></span> |<span data-ttu-id="10b61-124">**说明**</span><span class="sxs-lookup"><span data-stu-id="10b61-124">**Description**</span></span>                             |
| :----- | :------------------------------------------- |
| <span data-ttu-id="10b61-125">GET</span><span class="sxs-lookup"><span data-stu-id="10b61-125">GET</span></span>    | <span data-ttu-id="10b61-126">从资源中读取数据。</span><span class="sxs-lookup"><span data-stu-id="10b61-126">Read data from a resource.</span></span>                   |
| <span data-ttu-id="10b61-127">POST</span><span class="sxs-lookup"><span data-stu-id="10b61-127">POST</span></span>   | <span data-ttu-id="10b61-128">创建新的资源，或执行某个操作。</span><span class="sxs-lookup"><span data-stu-id="10b61-128">Create a new resource, or perform an action.</span></span> |
| <span data-ttu-id="10b61-129">PATCH</span><span class="sxs-lookup"><span data-stu-id="10b61-129">PATCH</span></span>  | <span data-ttu-id="10b61-130">用新值更新资源。</span><span class="sxs-lookup"><span data-stu-id="10b61-130">Update a resource with new values.</span></span>           |
| <span data-ttu-id="10b61-131">PUT</span><span class="sxs-lookup"><span data-stu-id="10b61-131">PUT</span></span>    | <span data-ttu-id="10b61-132">替换为新资源。</span><span class="sxs-lookup"><span data-stu-id="10b61-132">Replace a resource with a new one.</span></span>           |
| <span data-ttu-id="10b61-133">DELETE</span><span class="sxs-lookup"><span data-stu-id="10b61-133">DELETE</span></span> | <span data-ttu-id="10b61-134">删除资源。</span><span class="sxs-lookup"><span data-stu-id="10b61-134">Remove a resource.</span></span>                           |

* <span data-ttu-id="10b61-135">对于 **GET** 和 **DELETE** 方法，不需要任何请求正文。</span><span class="sxs-lookup"><span data-stu-id="10b61-135">For the methods **GET** and **DELETE**, no request body is required.</span></span>
* <span data-ttu-id="10b61-136">**POST**、**PATCH** 和 **PUT** 方法需要通常以 JSON 格式指定的请求正文，此正文包含了其他信息，如资源的属性值。</span><span class="sxs-lookup"><span data-stu-id="10b61-136">The **POST**, **PATCH**, and **PUT** methods require a request body, usually specified in JSON format, that contains additional information, such as the values for properties of the resource.</span></span>

## <a name="version"></a><span data-ttu-id="10b61-137">版本</span><span class="sxs-lookup"><span data-stu-id="10b61-137">Version</span></span>

<span data-ttu-id="10b61-138">Microsoft Graph 目前支持两种版本：`v1.0` 和 `beta`。</span><span class="sxs-lookup"><span data-stu-id="10b61-138">Microsoft Graph currently supports two versions: `v1.0` and `beta`.</span></span>

* <span data-ttu-id="10b61-139">`v1.0` 包括通常可用的 API。</span><span class="sxs-lookup"><span data-stu-id="10b61-139">`v1.0` includes generally available APIs.</span></span> <span data-ttu-id="10b61-140">为所有生产应用使用 v1.0 版本。</span><span class="sxs-lookup"><span data-stu-id="10b61-140"> includes generally available APIs. Use the v1.0 version for all production apps.</span></span>
* <span data-ttu-id="10b61-141">`beta` 包括目前处于预览中的 API。</span><span class="sxs-lookup"><span data-stu-id="10b61-141">`beta` includes APIs that are currently in preview.</span></span> <span data-ttu-id="10b61-142">因为我们可能会为试用的 API引入更大更改，我们建议你仅对开发中的测试应用使用试用版；请勿在生产应用中使用试用版 API。</span><span class="sxs-lookup"><span data-stu-id="10b61-142"> includes APIs that are currently in preview. Because we might introduce breaking changes to our beta APIs, we recommend that you use the beta version only to test apps that are in development; do not use beta APIs in your production apps.</span></span>

<span data-ttu-id="10b61-143">我们一直在寻求有关试用版 API 的反馈。</span><span class="sxs-lookup"><span data-stu-id="10b61-143">We are always looking for feedback on our beta APIs. To provide feedback or request features, see our UserVoice page.</span></span> <span data-ttu-id="10b61-144">要提供反馈或开通功能，请参阅 [UserVoice](https://officespdev.uservoice.com/) 页面。</span><span class="sxs-lookup"><span data-stu-id="10b61-144">We are always looking for feedback on our beta APIs. To provide feedback or request features, see our [UserVoice](https://officespdev.uservoice.com/) page.</span></span>

<span data-ttu-id="10b61-145">有关 API 版本的详细信息，请参阅[版本控制和支持](versioning_and_support.md)。</span><span class="sxs-lookup"><span data-stu-id="10b61-145">For more information about API versions, see [Versioning and support](versioning_and_support.md).</span></span>

## <a name="resource"></a><span data-ttu-id="10b61-146">资源</span><span class="sxs-lookup"><span data-stu-id="10b61-146">Resource</span></span>

<span data-ttu-id="10b61-147">你的 URL 将包含你正在请求中与之交互的一个或多个资源，如 `me`、`users`、`groups`、`drives` 和 `sites`。</span><span class="sxs-lookup"><span data-stu-id="10b61-147">Your URL will include the resource or resources you are interacting with in the request, such as `me`, `users`, `groups`, `drives`, and `sites`.</span></span> <span data-ttu-id="10b61-148">每个顶级资源也包括可以用来访问其他资源的**关系**（如 `me/messages` 或 `me/drive`）。</span><span class="sxs-lookup"><span data-stu-id="10b61-148">Each of the top-level resources also include **relationships**, which you can use to access additional resources, like `me/messages` or `me/drive`.</span></span> <span data-ttu-id="10b61-149">还可以使用**方法**与资源交互；例如，要发送电子邮件，则使用 `me/sendMail`。</span><span class="sxs-lookup"><span data-stu-id="10b61-149">You can also interact with resources using **methods**; for example, to send an email, use `me/sendMail`.</span></span>

<span data-ttu-id="10b61-150">有关如何导航资源关系和方法的详细信息，请参阅“遍历图”。</span><span class="sxs-lookup"><span data-stu-id="10b61-150">For more information about how to navigate resource relationships and methods, see Traverse the graph.</span></span> 

<span data-ttu-id="10b61-p111">每个资源可能需要不同的权限来访问它。通常，你需要用来创建或更新资源的权限比读取时要求的权限更高。有关所需权限的详细信息，请参见方法引用主题。</span><span class="sxs-lookup"><span data-stu-id="10b61-p111">Each resource might require different permissions to access it. You will often need a higher level of permissions to create or update a resource than to read it. For details about required permissions, see the method reference topic.</span></span> 

<span data-ttu-id="10b61-154">有关权限的详细信息，请参阅[权限引用](permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="10b61-154">For details about permissions, see [Permissions reference](permissions_reference.md).</span></span>

## <a name="query-parameters-optional"></a><span data-ttu-id="10b61-155">查询参数（可选）</span><span class="sxs-lookup"><span data-stu-id="10b61-155">Query parameters (optional)</span></span>

<span data-ttu-id="10b61-p112">你可以使用可选的查询参数，在 Microsoft Graph 应用中自定义响应。使用查询参数来包含比默认响应更多或更少的属性、过滤匹配自定义查询项目的响应，或为方法提供其他参数。</span><span class="sxs-lookup"><span data-stu-id="10b61-p112">You can use optional query parameters to customize the response in your Microsoft Graph app. Use query parameters to include more or fewer properties than the default response, filter the response for items that match a custom query, or provide additional parameters for a method.</span></span>

<span data-ttu-id="10b61-158">例如，添加以下筛选器参数会将返回的邮件限制为仅 `emailAddress` 属性为 `jon@contoso.com` 的邮件。</span><span class="sxs-lookup"><span data-stu-id="10b61-158">For example, adding the following filter parameter restricts the messages returned to only those with the `emailAddress` property of `jon@contoso.com`.</span></span>

```http
https://graph.microsoft.com/v1.0/me/messages?filter=emailAddress eq 'jon@contoso.com'
```

<span data-ttu-id="10b61-159">有关查询参数的详细信息，请参阅[自定义响应](query_parameters.md)。</span><span class="sxs-lookup"><span data-stu-id="10b61-159">For more information about query parameters, see [Customize responses](query_parameters.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="10b61-160">后续步骤</span><span class="sxs-lookup"><span data-stu-id="10b61-160">Next steps</span></span>

<span data-ttu-id="10b61-161">你可以随时开始使用和运行 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="10b61-161">You're ready to get up and running with Microsoft Graph.</span></span> <span data-ttu-id="10b61-162">若要了解详细信息，请转到 [Graph 资源管理器](https://developer.microsoft.com/en-us/graph/graph-explorer)尝试发出某些请求、尝试[快速启动](https://developer.microsoft.com/en-us/graph/quick-start)，或使用 [SDK 和代码示例](https://developer.microsoft.com/en-us/graph/code-samples-and-sdks)之一开始使用。</span><span class="sxs-lookup"><span data-stu-id="10b61-162">You're ready to get up and running with Microsoft Graph. To learn more, go to the [Graph Explorer](https://developer.microsoft.com/en-us/graph/graph-explorer) to try out some requests, try the [Quick Start](https://developer.microsoft.com/en-us/graph/quick-start), or get started using one of our [SDKs and code samples](https://developer.microsoft.com/en-us/graph/code-samples-and-sdks).</span></span>