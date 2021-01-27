---
title: 使用 Graph 浏览器尝试 Microsoft Graph API
description: 使用 Graph 浏览器在默认示例租户上尝试 Microsoft Graph API 以探索功能，或登录到你自己的租户，并使用它作为原型工具实现你的应用方案。
localization_priority: Normal
author: bettirosengugi
ms.openlocfilehash: 3f957d940d4dde483324492f1778ede970a5aefc
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013743"
---
# <a name="use-graph-explorer-to-try-microsoft-graph-apis"></a><span data-ttu-id="4c29e-103">使用 Graph 浏览器尝试 Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="4c29e-103">Use Graph Explorer to try Microsoft Graph APIs</span></span>

<span data-ttu-id="4c29e-104">[Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer/) 是一款开发人员工具，可方便你提出 Microsoft Graph REST API 请求并查看相应的响应。</span><span class="sxs-lookup"><span data-stu-id="4c29e-104">[Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/) is a developer tool that lets you conveniently make Microsoft Graph REST API requests and view corresponding responses.</span></span> <span data-ttu-id="4c29e-105">使用 Graph 浏览器尝试默认示例租户上的 API 来浏览功能，或登录到你自己的租户，并使用它作为原型制作工具，以完成你的应用方案。</span><span class="sxs-lookup"><span data-stu-id="4c29e-105">Use Graph Explorer to try APIs on the default sample tenant to explore capabilities, or sign in to your own tenant and use it as a prototyping tool to fulfill your app scenarios.</span></span> <span data-ttu-id="4c29e-106">此工具包括有用的功能，如 C#、Java、JavaScript 和目标 C 中的代码段;Microsoft Graph Toolkit和自适应卡片集成;等。</span><span class="sxs-lookup"><span data-stu-id="4c29e-106">This tool includes helpful features such as code snippets in C#, Java, JavaScript, and Objective C; Microsoft Graph Toolkit and adaptive cards integration; and more.</span></span>

<span data-ttu-id="4c29e-107">使用 Graph 浏览器：</span><span class="sxs-lookup"><span data-stu-id="4c29e-107">Use Graph Explorer to:</span></span>

- <span data-ttu-id="4c29e-108">将 Microsoft Graph API 请求 (GET、POST、PUT、PATCH 和 DELETE) 查看响应，包括响应代码以及任何标头和正文。</span><span class="sxs-lookup"><span data-stu-id="4c29e-108">Make Microsoft Graph API requests (GET, POST, PUT, PATCH and DELETE) and see responses including response code and any headers and bodies.</span></span>
- <span data-ttu-id="4c29e-109">同意权限。</span><span class="sxs-lookup"><span data-stu-id="4c29e-109">Consent to permissions.</span></span>
- <span data-ttu-id="4c29e-110">向查询添加请求正文和请求标头。</span><span class="sxs-lookup"><span data-stu-id="4c29e-110">Add a request body and request header to your query.</span></span>
- <span data-ttu-id="4c29e-111">查看和复制访问令牌。</span><span class="sxs-lookup"><span data-stu-id="4c29e-111">View and copy the access token.</span></span>
- <span data-ttu-id="4c29e-112">查看 Microsoft Graph 中不同服务的示例查询。</span><span class="sxs-lookup"><span data-stu-id="4c29e-112">View sample queries for different services in Microsoft Graph.</span></span>
- <span data-ttu-id="4c29e-113">查看、下载或删除最近 30 天内运行的查询。</span><span class="sxs-lookup"><span data-stu-id="4c29e-113">View, download, or delete the queries you ran in the last 30 days.</span></span>
- <span data-ttu-id="4c29e-114">查看和复制在 C#、Java、JavaScript 和目标 C 中运行的每个查询的代码段。</span><span class="sxs-lookup"><span data-stu-id="4c29e-114">View and copy code snippets of each query you run in C#, Java, JavaScript, and Objective C.</span></span>
- <span data-ttu-id="4c29e-115">访问 Microsoft Graph Toolkit组件和自适应卡片，用于一些示例查询。</span><span class="sxs-lookup"><span data-stu-id="4c29e-115">Access Microsoft Graph Toolkit components and adaptive cards for some sample queries.</span></span>
- <span data-ttu-id="4c29e-116">共享查询，包括请求正文和请求标头。</span><span class="sxs-lookup"><span data-stu-id="4c29e-116">Share queries, including the request body and request headers.</span></span>

<span data-ttu-id="4c29e-117">Graph 资源管理器会处理身份验证过程。</span><span class="sxs-lookup"><span data-stu-id="4c29e-117">Graph Explorer handles the authentication process for you.</span></span> <span data-ttu-id="4c29e-118">通过折叠边栏并更改主题来自定义体验。</span><span class="sxs-lookup"><span data-stu-id="4c29e-118">Customize the experience by collapsing the sidebar and changing the theme.</span></span>

## <a name="get-started"></a><span data-ttu-id="4c29e-119">入门</span><span class="sxs-lookup"><span data-stu-id="4c29e-119">Get started</span></span>

<span data-ttu-id="4c29e-120">Graph 浏览器是一个托管在 Microsoft Graph 开发人员中心的 [Web 应用程序](https://developer.microsoft.com/en-us/graph/graph-explorer)。</span><span class="sxs-lookup"><span data-stu-id="4c29e-120">Graph Explorer is a web application hosted on the [Microsoft Graph developer center](https://developer.microsoft.com/en-us/graph/graph-explorer).</span></span> <span data-ttu-id="4c29e-121">这是一个开源项目，欢迎你在 GitHub 存储库中做出 [贡献和提供反馈](https://github.com/microsoftgraph/microsoft-graph-explorer-v4)。</span><span class="sxs-lookup"><span data-stu-id="4c29e-121">It's an open source project,  and we welcome your contributions and feedback in the [GitHub repo](https://github.com/microsoftgraph/microsoft-graph-explorer-v4).</span></span>

<span data-ttu-id="4c29e-122">Graph 资源管理器包括以下元素：</span><span class="sxs-lookup"><span data-stu-id="4c29e-122">Graph Explorer includes the following elements:</span></span>

1. <span data-ttu-id="4c29e-123">HTTP 谓词下拉列表</span><span class="sxs-lookup"><span data-stu-id="4c29e-123">HTTP verb drop-down list</span></span>
2. <span data-ttu-id="4c29e-124">API 版本下拉列表</span><span class="sxs-lookup"><span data-stu-id="4c29e-124">API version drop-down list</span></span>
3. <span data-ttu-id="4c29e-125">请求查询地址栏</span><span class="sxs-lookup"><span data-stu-id="4c29e-125">Request query address bar</span></span>
4. <span data-ttu-id="4c29e-126">示例查询</span><span class="sxs-lookup"><span data-stu-id="4c29e-126">Sample query</span></span>
5. <span data-ttu-id="4c29e-127">示例查询的文档链接</span><span class="sxs-lookup"><span data-stu-id="4c29e-127">Documentation link for the sample query</span></span>

![Graph 浏览器用户界面的屏幕截图](./images/getting-started.png)

### <a name="make-a-get-request-in-graph-explorer"></a><span data-ttu-id="4c29e-129">在 Graph 资源管理器中提出 GET 请求</span><span class="sxs-lookup"><span data-stu-id="4c29e-129">Make a GET request in Graph Explorer</span></span>

<span data-ttu-id="4c29e-130">若要在 Graph 资源管理器中运行 GET 请求，则不必登录。</span><span class="sxs-lookup"><span data-stu-id="4c29e-130">To run a GET request in Graph Explorer, you don’t have to be signed in.</span></span> <span data-ttu-id="4c29e-131">只需单击示例查询，示例数据就会显示在响应预览中。</span><span class="sxs-lookup"><span data-stu-id="4c29e-131">Just click a sample query and sample data will show in the response preview.</span></span> 

![Graph 资源管理器中示例请求的屏幕截图](./images/making-a-get-request.png)

<span data-ttu-id="4c29e-133">若要提出请求，请：</span><span class="sxs-lookup"><span data-stu-id="4c29e-133">To make a request:</span></span>

1. <span data-ttu-id="4c29e-134">选择一个示例查询并运行它。</span><span class="sxs-lookup"><span data-stu-id="4c29e-134">Select a sample query and run it.</span></span>
2. <span data-ttu-id="4c29e-135">获取 HTTP 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4c29e-135">Get the HTTP response code.</span></span>
3. <span data-ttu-id="4c29e-136">使用示例数据查看来自 Microsoft Graph API 的响应。</span><span class="sxs-lookup"><span data-stu-id="4c29e-136">See the response from the Microsoft Graph API with sample data.</span></span>

<span data-ttu-id="4c29e-137">当你登录到 Graph 浏览器并单击同一查询时，响应将返回你登录的租户中的真实数据。</span><span class="sxs-lookup"><span data-stu-id="4c29e-137">When you sign in to Graph Explorer and click the same query, the response will be returned with real data from the tenant you signed in to.</span></span>

### <a name="running-non-get-requests-in-graph-explorer"></a><span data-ttu-id="4c29e-138">在 Graph 资源管理器中运行非 GET 请求</span><span class="sxs-lookup"><span data-stu-id="4c29e-138">Running non-GET requests in Graph Explorer</span></span>

<span data-ttu-id="4c29e-139">若要尝试 POST、PUT、PATCH 和 DELETE 请求，请使用 Microsoft 365 帐户登录到 Graph 资源管理器。这可以是用于测试或演示的组织帐户。</span><span class="sxs-lookup"><span data-stu-id="4c29e-139">To try POST, PUT, PATCH and DELETE requests, sign in to Graph Explorer using a Microsoft 365 account.This can be an organizational account for testing or demonstration purpose.</span></span> <span data-ttu-id="4c29e-140">若要获取免费的 Microsoft 365 E5 开发人员订阅示例，以及可帮助你构建 Microsoft 365 平台解决方案的工具和其他资源，请加入 [Microsoft 365 开发人员计划](https://developer.microsoft.com/microsoft-365/dev-program)。</span><span class="sxs-lookup"><span data-stu-id="4c29e-140">To get a free sample Microsoft 365 E5 developer subscription, along with tools and other resources to help you build solutions for the Microsoft 365 platform, join the [Microsoft 365 Developer Program](https://developer.microsoft.com/microsoft-365/dev-program).</span></span> 

>[!IMPORTANT]
><span data-ttu-id="4c29e-141">如果选择使用组织帐户登录，则运行非 GET 请求可能会影响租户中的数据。</span><span class="sxs-lookup"><span data-stu-id="4c29e-141">If you choose to sign in using your organizational account, running a non-GET request can affect the data in the tenant.</span></span>

<span data-ttu-id="4c29e-142">例如，若要运行 POST 请求，请在 HTTP 谓词的下拉列表中选择 POST，并根据需要添加请求正文和请求标头。</span><span class="sxs-lookup"><span data-stu-id="4c29e-142">For example, to run a POST request, select POST in the drop-down list for the HTTP verb, and add a request body and request headers as appropriate.</span></span>

![Graph 资源管理器中 POST 请求的屏幕截图](./images/making-a-post-request.png)

1. <span data-ttu-id="4c29e-144">选择 POST 示例查询。</span><span class="sxs-lookup"><span data-stu-id="4c29e-144">Select a POST sample query.</span></span>
2. <span data-ttu-id="4c29e-145">更新 **请求正文**;例如，为应用程序命名。</span><span class="sxs-lookup"><span data-stu-id="4c29e-145">Update **Request body**; for example, give the application a name.</span></span>
3. <span data-ttu-id="4c29e-146">单击 **"运行查询"。**</span><span class="sxs-lookup"><span data-stu-id="4c29e-146">Click **Run query**.</span></span>
4. <span data-ttu-id="4c29e-147">查看来自 Microsoft Graph API 的响应。</span><span class="sxs-lookup"><span data-stu-id="4c29e-147">See the response from the Microsoft Graph API.</span></span>

<span data-ttu-id="4c29e-148">若要查看默认 JSON 格式的响应，请选择请求窗格中的"请求标头"选项卡，定义键/值对，然后单击"**添加"。**</span><span class="sxs-lookup"><span data-stu-id="4c29e-148">To view the response in a format other than the default JSON, choose the **Request headers** tab in the request pane, define the key/value pair, and click **Add**.</span></span>

![显示 Graph 资源管理器中的"请求标头"选项卡的屏幕截图](./images/adding-key-value-pairs.png)

## <a name="next-steps"></a><span data-ttu-id="4c29e-150">后续步骤</span><span class="sxs-lookup"><span data-stu-id="4c29e-150">Next steps</span></span>

- <span data-ttu-id="4c29e-151">访问 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer/)。</span><span class="sxs-lookup"><span data-stu-id="4c29e-151">Visit [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/).</span></span>
- <span data-ttu-id="4c29e-152">详细了解 [Graph 浏览器功能](./graph-explorer-features.md)。</span><span class="sxs-lookup"><span data-stu-id="4c29e-152">Learn more about [Graph Explorer features](./graph-explorer-features.md).</span></span>
- <span data-ttu-id="4c29e-153">在 GitHub 存储库中参与或 [提供反馈](https://github.com/microsoftgraph/microsoft-graph-explorer-v4/issues/new/choose)。</span><span class="sxs-lookup"><span data-stu-id="4c29e-153">Contribute or provide feedback in the [GitHub repo](https://github.com/microsoftgraph/microsoft-graph-explorer-v4/issues/new/choose).</span></span>
