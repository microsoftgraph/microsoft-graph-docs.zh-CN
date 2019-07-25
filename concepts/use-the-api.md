---
title: 使用 Microsoft Graph API
description: Microsoft Graph 一种是可让你访问 Microsoft 云服务资源的 REST 风格的 Web API。在你注册应用并获取身份验证令牌以用于用户或服务后，可以向 Microsoft Graph API 发送请求。
author: jackson-woods
localization_priority: Priority
ms.openlocfilehash: 18de281cc0becfacfdabe5fb81a68358f04c3747
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840640"
---
# <a name="use-the-microsoft-graph-api"></a><span data-ttu-id="675bb-104">使用 Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="675bb-104">Use the Microsoft Graph API</span></span>

<span data-ttu-id="675bb-p102">Microsoft Graph 一种是可让你访问 Microsoft 云服务资源的 REST 风格的 Web API。在你[注册应用](auth-register-app-v2.md)并[获取身份验证令牌以用于用户](auth-v2-user.md)或[服务](auth-v2-service.md)后，可以向 Microsoft Graph API 发送请求。</span><span class="sxs-lookup"><span data-stu-id="675bb-p102">Microsoft Graph is a RESTful web API that enables you to access Microsoft Cloud service resources. After you [register your app](auth-register-app-v2.md) and [get authentication tokens for a user](auth-v2-user.md) or [service](auth-v2-service.md), you can make requests to the Microsoft Graph API.</span></span>

> <span data-ttu-id="675bb-107">**重要说明：** 条件访问策略应用于 Microsoft Graph 的方式在发生变化。</span><span class="sxs-lookup"><span data-stu-id="675bb-107">**Important:**  How conditional access policies apply to Microsoft Graph is changing.</span></span> <span data-ttu-id="675bb-108">应用程序需要进行更新以处理配置了条件访问策略的应用场景。</span><span class="sxs-lookup"><span data-stu-id="675bb-108">Applications need to be updated to handle scenarios where conditional access policies are configured.</span></span> <span data-ttu-id="675bb-109">有关详细信息和指南，请参阅 [Azure Active Directory 条件访问开发人员指南](https://docs.microsoft.com/azure/active-directory/develop/active-directory-conditional-access-developer)。</span><span class="sxs-lookup"><span data-stu-id="675bb-109">For more information and guidance, see [Developer Guidance for Azure Active Directory Conditional Access](https://docs.microsoft.com/azure/active-directory/develop/active-directory-conditional-access-developer).</span></span>

<span data-ttu-id="675bb-110">要在资源（如用户或电子邮件）中读取或写入资源，可以创建如下请求：</span><span class="sxs-lookup"><span data-stu-id="675bb-110">To read from or write to a resource such as a user or an email message, you construct a request that looks like the following.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
{HTTP method} https://graph.microsoft.com/{version}/{resource}?{query-parameters}
```

<span data-ttu-id="675bb-111">请求的组成部分包括：</span><span class="sxs-lookup"><span data-stu-id="675bb-111">The components of a request include:</span></span>

* <span data-ttu-id="675bb-112">[{HTTP method}](#http-methods) - 在 Microsoft Graph 请求上所使用的 HTTP 方法。</span><span class="sxs-lookup"><span data-stu-id="675bb-112">[HTTP method](#http-methods) - The HTTP method used on the request to Microsoft Graph.</span></span>
* <span data-ttu-id="675bb-113">[{version}](#version) - 你的应用程序正在使用的 Microsoft Graph API 版本。</span><span class="sxs-lookup"><span data-stu-id="675bb-113">   - The version of the Microsoft Graph API your application is using.</span></span>
* <span data-ttu-id="675bb-114">[{resource}](#resource) - 你正在引用的 Microsoft Graph 中的资源。</span><span class="sxs-lookup"><span data-stu-id="675bb-114">   - The resource in Microsoft Graph that you're referencing.</span></span> 
* <span data-ttu-id="675bb-115">[{query-parameters}](#query-parameters-optional) - 可自定义响应的可选 OData 查询选项或 REST 方法参数。</span><span class="sxs-lookup"><span data-stu-id="675bb-115">[{query-parameters}](#query-parameters-optional) - Optional OData query options or REST method parameters that customize the response.</span></span>

<span data-ttu-id="675bb-116">在你发出请求后，响应便会返回，其中包括：</span><span class="sxs-lookup"><span data-stu-id="675bb-116">After you make a request, a response is returned that includes:</span></span> 

* <span data-ttu-id="675bb-p104">状态代码 - 表示成功或失败的 HTTP 状态代码。若要详细了解 HTTP 错误代码，请参阅[错误](errors.md)。</span><span class="sxs-lookup"><span data-stu-id="675bb-p104">Status code - An HTTP status code that indicates success or failure. For details about HTTP error codes, see [Errors](errors.md).</span></span>
* <span data-ttu-id="675bb-p105">响应消息 - 请求获取的数据或操作结果。对于某些操作，响应消息可能为空。</span><span class="sxs-lookup"><span data-stu-id="675bb-p105">Response message - The data that you requested or the result of the operation. The response message can be empty for some operations.</span></span>
* <span data-ttu-id="675bb-p106">`nextLink` - 如果请求返回大量数据，则需要使用 `@odata.nextLink` 中返回的 URL 对其进行翻页。有关详细信息，请参阅[分页](paging.md)。</span><span class="sxs-lookup"><span data-stu-id="675bb-p106">`nextLink` link - If your request returns a lot of data, you need to page through it by choosing `@odata.nextLink`. For details, see [Paging](paging.md).</span></span>

## <a name="http-methods"></a><span data-ttu-id="675bb-123">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="675bb-123">HTTP methods</span></span>

<span data-ttu-id="675bb-p107">Microsoft Graph 使用请求上的 HTTP 方法来确定请求正在执行的操作。API 支持以下方法。</span><span class="sxs-lookup"><span data-stu-id="675bb-p107">Microsoft Graph uses the HTTP method on your request to determine what your request is doing. The API supports the following methods.</span></span>


|<span data-ttu-id="675bb-126">**方法**</span><span class="sxs-lookup"><span data-stu-id="675bb-126">**Method**</span></span> |<span data-ttu-id="675bb-127">**说明**</span><span class="sxs-lookup"><span data-stu-id="675bb-127">**Description**</span></span>                             |
| :----- | :------------------------------------------- |
| <span data-ttu-id="675bb-128">GET</span><span class="sxs-lookup"><span data-stu-id="675bb-128">GET</span></span>    | <span data-ttu-id="675bb-129">从资源中读取数据。</span><span class="sxs-lookup"><span data-stu-id="675bb-129">Read data from a resource.</span></span>                   |
| <span data-ttu-id="675bb-130">POST</span><span class="sxs-lookup"><span data-stu-id="675bb-130">POST</span></span>   | <span data-ttu-id="675bb-131">创建新的资源，或执行某个操作。</span><span class="sxs-lookup"><span data-stu-id="675bb-131">Create a new resource, or perform an action.</span></span> |
| <span data-ttu-id="675bb-132">PATCH</span><span class="sxs-lookup"><span data-stu-id="675bb-132">PATCH</span></span>  | <span data-ttu-id="675bb-133">用新值更新资源。</span><span class="sxs-lookup"><span data-stu-id="675bb-133">Update a resource with new values.</span></span>           |
| <span data-ttu-id="675bb-134">PUT</span><span class="sxs-lookup"><span data-stu-id="675bb-134">PUT</span></span>    | <span data-ttu-id="675bb-135">替换为新资源。</span><span class="sxs-lookup"><span data-stu-id="675bb-135">Replace a resource with a new one.</span></span>           |
| <span data-ttu-id="675bb-136">DELETE</span><span class="sxs-lookup"><span data-stu-id="675bb-136">DELETE</span></span> | <span data-ttu-id="675bb-137">删除资源。</span><span class="sxs-lookup"><span data-stu-id="675bb-137">Remove a resource.</span></span>                           |

* <span data-ttu-id="675bb-138">对于 CRUD 方法 `GET` 和 `DELETE`，不需要任何请求正文。</span><span class="sxs-lookup"><span data-stu-id="675bb-138">For the methods `GET` and `DELETE`, no request body is required.</span></span>
* <span data-ttu-id="675bb-139">`POST`、`PATCH` 和 `PUT` 方法需要通常以 JSON 格式指定的请求正文，此正文包含了其他信息，如资源的属性值。</span><span class="sxs-lookup"><span data-stu-id="675bb-139">The `POST`, `PATCH`, and `PUT` methods require a request body, usually specified in JSON format, that contains additional information, such as the values for properties of the resource.</span></span>

## <a name="version"></a><span data-ttu-id="675bb-140">版本</span><span class="sxs-lookup"><span data-stu-id="675bb-140">Version</span></span>

<span data-ttu-id="675bb-141">Microsoft Graph 目前支持以下两种版本：`v1.0` 和 `beta`。</span><span class="sxs-lookup"><span data-stu-id="675bb-141">Microsoft Graph currently supports two versions: `v1.0` and `beta`.</span></span>

* <span data-ttu-id="675bb-p108">`v1.0` 包括正式可用 API。请对所有生产应用使用 v1.0 版本。</span><span class="sxs-lookup"><span data-stu-id="675bb-p108">`v1.0` includes generally available APIs. Use the v1.0 version for all production apps.</span></span>
* <span data-ttu-id="675bb-p109">`beta` 包括目前处于预览中的 API。因为我们可能会为试用的 API引入更大更改，我们建议你仅对开发中的测试应用使用试用版；请勿在生产应用中使用试用版 API。</span><span class="sxs-lookup"><span data-stu-id="675bb-p109">`beta` includes APIs that are currently in preview. Because we might introduce breaking changes to our beta APIs, we recommend that you use the beta version only to test apps that are in development; do not use beta APIs in your production apps.</span></span>

<span data-ttu-id="675bb-p110">我们一直期待用户提供 beta API 反馈。若要提供反馈或申请功能，请参阅 [UserVoice](https://officespdev.uservoice.com/) 页。</span><span class="sxs-lookup"><span data-stu-id="675bb-p110">We are always looking for feedback on our beta APIs. To provide feedback or request features, see our [UserVoice](https://officespdev.uservoice.com/) page.</span></span>

<span data-ttu-id="675bb-148">若要详细了解 API 版本，请参阅[版本控制和支持](versioning-and-support.md)。</span><span class="sxs-lookup"><span data-stu-id="675bb-148">For more information about API versions, see [Versioning and support](versioning-and-support.md).</span></span>

## <a name="resource"></a><span data-ttu-id="675bb-149">Resource</span><span class="sxs-lookup"><span data-stu-id="675bb-149">Resource</span></span>

<span data-ttu-id="675bb-150">资源可以是实体或复杂类型，通常使用属性定义。</span><span class="sxs-lookup"><span data-stu-id="675bb-150">A resource can be an entity or complex type, commonly defined with properties.</span></span> <span data-ttu-id="675bb-151">实体与复杂类型的不同之处在于前者始终包含 **id** 属性。</span><span class="sxs-lookup"><span data-stu-id="675bb-151">Entities differ from complex types by always including an **id** property.</span></span>

<span data-ttu-id="675bb-152">你的 URL 将包含你正在请求中与之交互的资源，如`me`、**用户**、**组**、**驱动器**和**网站**。</span><span class="sxs-lookup"><span data-stu-id="675bb-152">Your URL will include the resource or resources you are interacting with in the request, such as `me`, \*\*\*\*, \*\*\*\*, \*\*\*\*, and \*\*\*\*.</span></span> <span data-ttu-id="675bb-153">通常，顶级资源还包括可以用来访问其他资源的_关系_（如 `me/messages` 或 `me/drive`）。</span><span class="sxs-lookup"><span data-stu-id="675bb-153">Each of the top-level resources also include _relationships_, which you can use to access additional resources, like `me/messages` or `me/drive`.</span></span> <span data-ttu-id="675bb-154">还可以使用_方法_与资源交互；例如，若要发送电子邮件，可以使用 `me/sendMail`。</span><span class="sxs-lookup"><span data-stu-id="675bb-154">You can also interact with resources using _methods_; for example, to send an email, use `me/sendMail`.</span></span> <span data-ttu-id="675bb-155">有关详细信息，请参阅[通过导航 Microsoft Graph 访问数据和方法](traverse-the-graph.md)。</span><span class="sxs-lookup"><span data-stu-id="675bb-155">For more information, see [Access data and methods by navigating Microsoft Graph](traverse-the-graph.md).</span></span>

<span data-ttu-id="675bb-p113">每个资源可能需要不同的权限来访问它。通常，你需要用来创建或更新资源的权限比读取时要求的权限更高。有关所需权限的详细信息，请参见方法引用主题。</span><span class="sxs-lookup"><span data-stu-id="675bb-p113">Each resource might require different permissions to access it. You will often need a higher level of permissions to create or update a resource than to read it. For details about required permissions, see the method reference topic.</span></span> 

<span data-ttu-id="675bb-159">有关权限的详细信息，请参阅[权限引用](permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="675bb-159">For details about permissions, see [Permissions reference](permissions-reference.md).</span></span>

## <a name="query-parameters"></a><span data-ttu-id="675bb-160">查询参数</span><span class="sxs-lookup"><span data-stu-id="675bb-160">Query parameters</span></span>

<span data-ttu-id="675bb-161">查询参数可以是 OData 系统查询选项，也可以是方法接受的用于自定义其响应的其他字符串。</span><span class="sxs-lookup"><span data-stu-id="675bb-161">Query parameters can be OData system query options, or other strings that a method accepts to customize its response.</span></span>

<span data-ttu-id="675bb-162">你可以使用可选的 OData 系统查询选项来包含比默认响应更多或更少的属性、过滤与自定义查询匹配的项的响应，或为方法提供其他参数。</span><span class="sxs-lookup"><span data-stu-id="675bb-162">You can use optional query parameters to customize the response in your Microsoft Graph app. Use query parameters to include more or fewer properties than the default response, filter the response for items that match a custom query, or provide additional parameters for a method.</span></span>

<span data-ttu-id="675bb-163">例如，添加以下 `filter` 参数会将返回的邮件限制为 `emailAddress` 属性仅为 `jon@contoso.com` 的邮件。</span><span class="sxs-lookup"><span data-stu-id="675bb-163">For example, adding the following filter parameter restricts the messages returned to only those with the  property of .</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages?filter=emailAddress eq 'jon@contoso.com'
```

<span data-ttu-id="675bb-164">有关 OData 查询选项的详细信息，请参阅[使用查询参数自定义响应](query-parameters.md)。</span><span class="sxs-lookup"><span data-stu-id="675bb-164">For more information about OData query options, see [Use query parameters to customize responses](query-parameters.md).</span></span>

<span data-ttu-id="675bb-165">除 OData 查询选项之外，某些方法还需要将参数值指定为查询 URL 的一部分。</span><span class="sxs-lookup"><span data-stu-id="675bb-165">Aside from OData query options, some methods require parameter values specified as part of the query URL.</span></span> <span data-ttu-id="675bb-166">例如，你可以通过查询**用户**的 **calendarView** 关系，并将时段 `startDateTime` 和 `endDateTime` 值指定为查询参数来获取用户日历中某个时间段内发生的事件的集合：</span><span class="sxs-lookup"><span data-stu-id="675bb-166">For example, you can get a collection of events that occurred during a time period in a user's calendar, by querying the **calendarView** relationship of a **user**, and specifying the period `startDateTime` and `endDateTime` values as query parameters:</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/me/calendarView?startDateTime=2019-09-01T09:00:00.0000000&endDateTime=2019-09-01T17:00:00.0000000
```

## <a name="next-steps"></a><span data-ttu-id="675bb-167">后续步骤</span><span class="sxs-lookup"><span data-stu-id="675bb-167">Next steps</span></span>

<span data-ttu-id="675bb-p115">你可以随时开始使用和运行 Microsoft Graph。若要了解详细信息，请转到 [Graph 资源管理器](https://developer.microsoft.com/graph/graph-explorer)尝试发出某些请求、尝试[快速启动](https://developer.microsoft.com/graph/quick-start)，或使用 [SDK 和代码示例](https://developer.microsoft.com/graph/code-samples-and-sdks)之一开始使用。</span><span class="sxs-lookup"><span data-stu-id="675bb-p115">You're ready to get up and running with Microsoft Graph. To learn more, go to the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) to try out some requests, try the [Quick Start](https://developer.microsoft.com/graph/quick-start), or get started using one of our [SDKs and code samples](https://developer.microsoft.com/graph/code-samples-and-sdks).</span></span>
