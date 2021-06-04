---
title: 使用 Microsoft Graph API
description: Microsoft Graph 一种是可让你访问 Microsoft 云服务资源的 REST 风格的 Web API。在你注册应用并获取身份验证令牌以用于用户或服务后，可以向 Microsoft Graph API 发送请求。
author: jackson-woods
localization_priority: Priority
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: 1a478adb9053face3537a445e25dd69a908b2525
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732145"
---
# <a name="use-the-microsoft-graph-api"></a><span data-ttu-id="8420f-104">使用 Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="8420f-104">Use the Microsoft Graph API</span></span>

<span data-ttu-id="8420f-p102">Microsoft Graph 一种是可让你访问 Microsoft 云服务资源的 REST 风格的 Web API。在你[注册应用](auth-register-app-v2.md)并[获取身份验证令牌以用于用户](auth-v2-user.md)或[服务](auth-v2-service.md)后，可以向 Microsoft Graph API 发送请求。</span><span class="sxs-lookup"><span data-stu-id="8420f-p102">Microsoft Graph is a RESTful web API that enables you to access Microsoft Cloud service resources. After you [register your app](auth-register-app-v2.md) and [get authentication tokens for a user](auth-v2-user.md) or [service](auth-v2-service.md), you can make requests to the Microsoft Graph API.</span></span>

> <span data-ttu-id="8420f-107">**重要说明：** 条件访问策略应用于 Microsoft Graph 的方式在发生变化。</span><span class="sxs-lookup"><span data-stu-id="8420f-107">**Important:**  How conditional access policies apply to Microsoft Graph is changing.</span></span> <span data-ttu-id="8420f-108">应用程序需要进行更新以处理配置了条件访问策略的应用场景。</span><span class="sxs-lookup"><span data-stu-id="8420f-108">Applications need to be updated to handle scenarios where conditional access policies are configured.</span></span> <span data-ttu-id="8420f-109">有关详细信息和指南，请参阅 [Azure Active Directory 条件访问开发人员指南](/azure/active-directory/develop/active-directory-conditional-access-developer)。</span><span class="sxs-lookup"><span data-stu-id="8420f-109">For more information and guidance, see [Developer Guidance for Azure Active Directory Conditional Access](/azure/active-directory/develop/active-directory-conditional-access-developer).</span></span>

## <a name="odata-namespace"></a><span data-ttu-id="8420f-110">OData 命名空间</span><span class="sxs-lookup"><span data-stu-id="8420f-110">OData namespace</span></span>

<span data-ttu-id="8420f-111">Microsoft Graph API 在 [Microsoft Graph 元数据](traverse-the-graph.md#microsoft-graph-api-metadata)的 OData 命名空间 `microsoft.graph` 中，定义它的大多数资源、方法和枚举。</span><span class="sxs-lookup"><span data-stu-id="8420f-111">The Microsoft Graph API defines most of its resources, methods, and enumerations in the OData namespace, `microsoft.graph`, in the [Microsoft Graph metadata](traverse-the-graph.md#microsoft-graph-api-metadata).</span></span> <span data-ttu-id="8420f-112">少量的 API 集在其子命名空间中定义，例如[调用记录 API](/graph/api/resources/callrecords-api-overview) 定义诸如 `microsoft.graph.callRecords`中的 [callRecord](/graph/api/resources/callrecords-callrecord) 等资源。</span><span class="sxs-lookup"><span data-stu-id="8420f-112">A small number of API sets are defined in their sub-namespaces, such as the [call records API](/graph/api/resources/callrecords-api-overview) which defines resources like [callRecord](/graph/api/resources/callrecords-callrecord) in `microsoft.graph.callRecords`.</span></span> 

<span data-ttu-id="8420f-113">除非在相应主题中明确指定，否则假定类型、方法和枚举是 `microsoft.graph` 命名空间的一部分。</span><span class="sxs-lookup"><span data-stu-id="8420f-113">Unless explicitly specified in the corresponding topic, assume types, methods, and enumerations are part of the `microsoft.graph` namespace.</span></span>

## <a name="call-a-rest-api-method"></a><span data-ttu-id="8420f-114">调用 REST API 方法</span><span class="sxs-lookup"><span data-stu-id="8420f-114">Call a REST API method</span></span>

<span data-ttu-id="8420f-115">要在资源（如用户或电子邮件）中读取或写入资源，可以创建如下请求：</span><span class="sxs-lookup"><span data-stu-id="8420f-115">To read from or write to a resource such as a user or an email message, you construct a request that looks like the following:</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
{HTTP method} https://graph.microsoft.com/{version}/{resource}?{query-parameters}
```

<span data-ttu-id="8420f-116">请求的组成部分包括：</span><span class="sxs-lookup"><span data-stu-id="8420f-116">The components of a request include:</span></span>

* <span data-ttu-id="8420f-117">[{HTTP method}](#http-methods) - 在 Microsoft Graph 请求上所使用的 HTTP 方法。</span><span class="sxs-lookup"><span data-stu-id="8420f-117">[{HTTP method}](#http-methods) - The HTTP method used on the request to Microsoft Graph.</span></span>
* <span data-ttu-id="8420f-118">[{version}](#version) - 你的应用程序正在使用的 Microsoft Graph API 版本。</span><span class="sxs-lookup"><span data-stu-id="8420f-118">[{version}](#version) - The version of the Microsoft Graph API your application is using.</span></span>
* <span data-ttu-id="8420f-119">[{resource}](#resource) - 你正在引用的 Microsoft Graph 中的资源。</span><span class="sxs-lookup"><span data-stu-id="8420f-119">[{resource}](#resource) - The resource in Microsoft Graph that you're referencing.</span></span> 
* <span data-ttu-id="8420f-120">[{query-parameters}](#query-parameters) - 可自定义响应的可选 OData 查询选项或 REST 方法参数。</span><span class="sxs-lookup"><span data-stu-id="8420f-120">[{query-parameters}](#query-parameters) - Optional OData query options or REST method parameters that customize the response.</span></span>

<span data-ttu-id="8420f-121">在你发出请求后，响应便会返回，其中包括：</span><span class="sxs-lookup"><span data-stu-id="8420f-121">After you make a request, a response is returned that includes:</span></span> 

* <span data-ttu-id="8420f-p105">状态代码 - 表示成功或失败的 HTTP 状态代码。若要详细了解 HTTP 错误代码，请参阅[错误](errors.md)。</span><span class="sxs-lookup"><span data-stu-id="8420f-p105">Status code - An HTTP status code that indicates success or failure. For details about HTTP error codes, see [Errors](errors.md).</span></span>
* <span data-ttu-id="8420f-p106">响应消息 - 请求获取的数据或操作结果。对于某些操作，响应消息可能为空。</span><span class="sxs-lookup"><span data-stu-id="8420f-p106">Response message - The data that you requested or the result of the operation. The response message can be empty for some operations.</span></span>
* <span data-ttu-id="8420f-p107">`nextLink` - 如果请求返回大量数据，则需要使用 `@odata.nextLink` 中返回的 URL 对其进行翻页。有关详细信息，请参阅[分页](paging.md)。</span><span class="sxs-lookup"><span data-stu-id="8420f-p107">`nextLink` - If your request returns a lot of data, you need to page through it by using the URL returned in `@odata.nextLink`. For details, see [Paging](paging.md).</span></span>

## <a name="http-methods"></a><span data-ttu-id="8420f-128">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="8420f-128">HTTP methods</span></span>

<span data-ttu-id="8420f-p108">Microsoft Graph 使用请求上的 HTTP 方法来确定请求正在执行的操作。API 支持以下方法。</span><span class="sxs-lookup"><span data-stu-id="8420f-p108">Microsoft Graph uses the HTTP method on your request to determine what your request is doing. The API supports the following methods.</span></span>

|<span data-ttu-id="8420f-131">**方法**</span><span class="sxs-lookup"><span data-stu-id="8420f-131">**Method**</span></span> |<span data-ttu-id="8420f-132">**说明**</span><span class="sxs-lookup"><span data-stu-id="8420f-132">**Description**</span></span>                             |
| :----- | :------------------------------------------- |
| <span data-ttu-id="8420f-133">GET</span><span class="sxs-lookup"><span data-stu-id="8420f-133">GET</span></span>    | <span data-ttu-id="8420f-134">从资源中读取数据。</span><span class="sxs-lookup"><span data-stu-id="8420f-134">Read data from a resource.</span></span>                   |
| <span data-ttu-id="8420f-135">POST</span><span class="sxs-lookup"><span data-stu-id="8420f-135">POST</span></span>   | <span data-ttu-id="8420f-136">创建新的资源，或执行某个操作。</span><span class="sxs-lookup"><span data-stu-id="8420f-136">Create a new resource, or perform an action.</span></span> |
| <span data-ttu-id="8420f-137">PATCH</span><span class="sxs-lookup"><span data-stu-id="8420f-137">PATCH</span></span>  | <span data-ttu-id="8420f-138">用新值更新资源。</span><span class="sxs-lookup"><span data-stu-id="8420f-138">Update a resource with new values.</span></span>           |
| <span data-ttu-id="8420f-139">PUT</span><span class="sxs-lookup"><span data-stu-id="8420f-139">PUT</span></span>    | <span data-ttu-id="8420f-140">替换为新资源。</span><span class="sxs-lookup"><span data-stu-id="8420f-140">Replace a resource with a new one.</span></span>           |
| <span data-ttu-id="8420f-141">DELETE</span><span class="sxs-lookup"><span data-stu-id="8420f-141">DELETE</span></span> | <span data-ttu-id="8420f-142">删除资源。</span><span class="sxs-lookup"><span data-stu-id="8420f-142">Remove a resource.</span></span>                           |

* <span data-ttu-id="8420f-143">对于 CRUD 方法 `GET` 和 `DELETE`，不需要任何请求正文。</span><span class="sxs-lookup"><span data-stu-id="8420f-143">For the CRUD methods `GET` and `DELETE`, no request body is required.</span></span>
* <span data-ttu-id="8420f-144">`POST`、`PATCH` 和 `PUT` 方法需要通常以 JSON 格式指定的请求正文，此正文包含了其他信息，如资源的属性值。</span><span class="sxs-lookup"><span data-stu-id="8420f-144">The `POST`, `PATCH`, and `PUT` methods require a request body, usually specified in JSON format, that contains additional information, such as the values for properties of the resource.</span></span>

## <a name="version"></a><span data-ttu-id="8420f-145">版本</span><span class="sxs-lookup"><span data-stu-id="8420f-145">Version</span></span>

<span data-ttu-id="8420f-146">Microsoft Graph 目前支持以下两种版本：`v1.0` 和 `beta`。</span><span class="sxs-lookup"><span data-stu-id="8420f-146">Microsoft Graph currently supports two versions: `v1.0` and `beta`.</span></span>

* <span data-ttu-id="8420f-p109">`v1.0` 包括正式可用 API。请对所有生产应用使用 v1.0 版本。</span><span class="sxs-lookup"><span data-stu-id="8420f-p109">`v1.0` includes generally available APIs. Use the v1.0 version for all production apps.</span></span>
* <span data-ttu-id="8420f-p110">`beta` 包括目前处于预览中的 API。因为我们可能会为试用的 API引入更大更改，我们建议你仅对开发中的测试应用使用试用版；请勿在生产应用中使用试用版 API。</span><span class="sxs-lookup"><span data-stu-id="8420f-p110">`beta` includes APIs that are currently in preview. Because we might introduce breaking changes to our beta APIs, we recommend that you use the beta version only to test apps that are in development; do not use beta APIs in your production apps.</span></span>

<span data-ttu-id="8420f-p111">我们一直在寻求有关试用版 API 的反馈。若要提供反馈或请求功能，请参阅 [Microsoft 365 开发者平台创意论坛](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph)。</span><span class="sxs-lookup"><span data-stu-id="8420f-p111">We are always looking for feedback on our beta APIs. To provide feedback or request features, see our [Microsoft 365 Developer Platform ideas forum](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph).</span></span>

<span data-ttu-id="8420f-153">若要详细了解 API 版本，请参阅[版本控制和支持](versioning-and-support.md)。</span><span class="sxs-lookup"><span data-stu-id="8420f-153">For more information about API versions, see [Versioning and support](versioning-and-support.md).</span></span>

## <a name="resource"></a><span data-ttu-id="8420f-154">Resource</span><span class="sxs-lookup"><span data-stu-id="8420f-154">Resource</span></span>

<span data-ttu-id="8420f-155">资源可以是实体或复杂类型，通常使用属性定义。</span><span class="sxs-lookup"><span data-stu-id="8420f-155">A resource can be an entity or complex type, commonly defined with properties.</span></span> <span data-ttu-id="8420f-156">实体与复杂类型的不同之处在于前者始终包含 **id** 属性。</span><span class="sxs-lookup"><span data-stu-id="8420f-156">Entities differ from complex types by always including an **id** property.</span></span>

<span data-ttu-id="8420f-p113">你的 URL 将包含你正在请求中与之交互的资源，如`me`、**用户**、**组**、**驱动器** 和 **网站**。通常，顶级资源还包括可以用来访问其他资源的 _关系_（如 `me/messages` 或 `me/drive`）。你还可以使用 _方法_ 与资源交互；例如，要发送电子邮件，则使用 `me/sendMail`。有关详细信息，请参阅[通过导航 Microsoft Graph 访问数据和方法](traverse-the-graph.md)。</span><span class="sxs-lookup"><span data-stu-id="8420f-p113">Your URL will include the resource you are interacting with in the request, such as `me`, **user**, **group**, **drive**, and **site**. Often, top-level resources also include _relationships_, which you can use to access additional resources, like `me/messages` or `me/drive`. You can also interact with resources using _methods_; for example, to send an email, use `me/sendMail`. For more information, see [Access data and methods by navigating Microsoft Graph](traverse-the-graph.md).</span></span>

<span data-ttu-id="8420f-p114">每个资源可能需要不同的权限来访问它。通常，你需要用来创建或更新资源的权限比读取时要求的权限更高。有关所需权限的详细信息，请参见方法引用主题。</span><span class="sxs-lookup"><span data-stu-id="8420f-p114">Each resource might require different permissions to access it. You will often need a higher level of permissions to create or update a resource than to read it. For details about required permissions, see the method reference topic.</span></span> 

<span data-ttu-id="8420f-164">有关权限的详细信息，请参阅[权限引用](permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="8420f-164">For details about permissions, see [Permissions reference](permissions-reference.md).</span></span>

## <a name="query-parameters"></a><span data-ttu-id="8420f-165">查询参数</span><span class="sxs-lookup"><span data-stu-id="8420f-165">Query parameters</span></span>

<span data-ttu-id="8420f-166">查询参数可以是 OData 系统查询选项，也可以是方法接受的用于自定义其响应的其他字符串。</span><span class="sxs-lookup"><span data-stu-id="8420f-166">Query parameters can be OData system query options, or other strings that a method accepts to customize its response.</span></span>

<span data-ttu-id="8420f-167">你可以使用可选的 OData 系统查询选项来包含比默认响应更多或更少的属性、过滤与自定义查询匹配的项的响应，或为方法提供其他参数。</span><span class="sxs-lookup"><span data-stu-id="8420f-167">You can use optional OData system query options to include more or fewer properties than the default response, filter the response for items that match a custom query, or provide additional parameters for a method.</span></span>

<span data-ttu-id="8420f-168">例如，添加以下 `filter` 参数会将返回的邮件限制为 `emailAddress` 属性仅为 `jon@contoso.com` 的邮件。</span><span class="sxs-lookup"><span data-stu-id="8420f-168">For example, adding the following `filter` parameter restricts the messages returned to only those with the `emailAddress` property of `jon@contoso.com`.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages?filter=emailAddress eq 'jon@contoso.com'
```

<span data-ttu-id="8420f-169">有关 OData 查询选项的详细信息，请参阅[使用查询参数自定义响应](query-parameters.md)。</span><span class="sxs-lookup"><span data-stu-id="8420f-169">For more information about OData query options, see [Use query parameters to customize responses](query-parameters.md).</span></span>

<span data-ttu-id="8420f-170">除 OData 查询选项之外，某些方法还需要将参数值指定为查询 URL 的一部分。</span><span class="sxs-lookup"><span data-stu-id="8420f-170">Aside from OData query options, some methods require parameter values specified as part of the query URL.</span></span> <span data-ttu-id="8420f-171">例如，你可以通过查询 **用户** 的 **calendarView** 关系，并将时段 `startDateTime` 和 `endDateTime` 值指定为查询参数来获取用户日历中某个时间段内发生的事件的集合：</span><span class="sxs-lookup"><span data-stu-id="8420f-171">For example, you can get a collection of events that occurred during a time period in a user's calendar, by querying the **calendarView** relationship of a **user**, and specifying the period `startDateTime` and `endDateTime` values as query parameters:</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/me/calendarView?startDateTime=2019-09-01T09:00:00.0000000&endDateTime=2019-09-01T17:00:00.0000000
```

## <a name="tools-for-interacting-with-microsoft-graph"></a><span data-ttu-id="8420f-172">用于与 Microsoft Graph 交互的工具</span><span class="sxs-lookup"><span data-stu-id="8420f-172">Tools for interacting with Microsoft Graph</span></span>

### <a name="graph-explorer"></a><span data-ttu-id="8420f-173">Graph 浏览器</span><span class="sxs-lookup"><span data-stu-id="8420f-173">Graph Explorer</span></span>

<span data-ttu-id="8420f-p116">Graph 浏览器是一个基于 Web 的工具，可用于通过 Microsoft Graph API 构建和测试请求。可在以下位置访问 Graph Explorer：[https://developer.microsoft.com/graph/graph-explorer](https://developer.microsoft.com/graph/graph-explorer)。</span><span class="sxs-lookup"><span data-stu-id="8420f-p116">Graph Explorer is a web-based tool that you can use to build and test requests using Microsoft Graph APIs. You can access Graph Explorer at: [https://developer.microsoft.com/graph/graph-explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

<span data-ttu-id="8420f-p117">可在不登录的情况下访问演示数据，或者可登录自己的租户。请按照以下步骤生成请求：</span><span class="sxs-lookup"><span data-stu-id="8420f-p117">You can either access demo data without signing in, or you can sign in to a tenant of your own. Use the following steps to build the request:</span></span>

1. <span data-ttu-id="8420f-178">选择 HTTP 方法。</span><span class="sxs-lookup"><span data-stu-id="8420f-178">Select the HTTP method.</span></span>
2. <span data-ttu-id="8420f-179">选择要使用的 API 版本。</span><span class="sxs-lookup"><span data-stu-id="8420f-179">Select the version of API that you want to use.</span></span>
3. <span data-ttu-id="8420f-180">在请求文本框中键入查询。</span><span class="sxs-lookup"><span data-stu-id="8420f-180">Type the query in the request text box.</span></span>
4. <span data-ttu-id="8420f-181">选择“**运行查询**”。</span><span class="sxs-lookup"><span data-stu-id="8420f-181">Select **Run Query**.</span></span> 

<span data-ttu-id="8420f-182">以下示例显示返回演示租户中的用户相关信息的请求：</span><span class="sxs-lookup"><span data-stu-id="8420f-182">The following example shows a request that returns information about users in the demo tenant:</span></span>

![Graph 浏览器屏幕截图，突出显示 GET 用户请求](./images/graph-explorer.png)

<span data-ttu-id="8420f-184">Graph 浏览器中提供了示例查询，让你能够更快地运行常见请求。</span><span class="sxs-lookup"><span data-stu-id="8420f-184">Sample queries are provided in Graph Explorer to enable you to more quickly run common requests.</span></span> <span data-ttu-id="8420f-185">若要查看可用示例，请选择“**显示更多示例**”。</span><span class="sxs-lookup"><span data-stu-id="8420f-185">To see the samples that are available, select **show more samples**.</span></span> <span data-ttu-id="8420f-186">对于要查看的示例集选择“**打开**”，然后在关闭选择窗口后，应会看到预定义的请求列表。</span><span class="sxs-lookup"><span data-stu-id="8420f-186">Select **On** for the set of samples that you want to see, and then after closing the selection window, you should see a list of predefined requests.</span></span>

<span data-ttu-id="8420f-187">发送请求后将显示状态代码和消息，并在“**响应预览**”选项卡中显示响应。</span><span class="sxs-lookup"><span data-stu-id="8420f-187">A status code and message are displayed after a request is sent and the response is shown in the **Response Preview** tab.</span></span>

### <a name="postman"></a><span data-ttu-id="8420f-188">Postman</span><span class="sxs-lookup"><span data-stu-id="8420f-188">Postman</span></span>

<span data-ttu-id="8420f-189">Postman 浏览器是一款可用于使用 Microsoft Graph API 构建和测试请求的工具。</span><span class="sxs-lookup"><span data-stu-id="8420f-189">Postman is a tool that you can use to build and test requests using the Microsoft Graph APIs.</span></span> <span data-ttu-id="8420f-190">可在以下位置下载 Postman：[https://www.getpostman.com/](https://www.getpostman.com/)。</span><span class="sxs-lookup"><span data-stu-id="8420f-190">You can download Postman at: [https://www.getpostman.com/](https://www.getpostman.com/).</span></span> <span data-ttu-id="8420f-191">若要在 Postman 中与 Microsoft Graph 进行交互，请使用 Microsoft Graph 集合。</span><span class="sxs-lookup"><span data-stu-id="8420f-191">To interact with Microsoft Graph in Postman, you use the Microsoft Graph collection.</span></span>

<span data-ttu-id="8420f-192">有关详细信息，请参阅[结合使用 Postman 和 Microsoft Graph API](./use-postman.md)。</span><span class="sxs-lookup"><span data-stu-id="8420f-192">For more information, see [Use Postman with the Microsoft Graph API](./use-postman.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="8420f-193">后续步骤</span><span class="sxs-lookup"><span data-stu-id="8420f-193">Next steps</span></span>

<span data-ttu-id="8420f-p120">你可以随时开始使用和运行 Microsoft Graph。请尝试“[快速入门](https://developer.microsoft.com/graph/quick-start)”或开始使用我们的其中一个 [SDK 和代码示例](https://developer.microsoft.com/graph/code-samples-and-sdks)。</span><span class="sxs-lookup"><span data-stu-id="8420f-p120">You're ready to get up and running with Microsoft Graph. Try the [Quick Start](https://developer.microsoft.com/graph/quick-start), or get started using one of our [SDKs and code samples](https://developer.microsoft.com/graph/code-samples-and-sdks).</span></span>
