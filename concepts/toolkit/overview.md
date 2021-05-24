---
title: Microsoft Graph Toolkit：Microsoft Graph 的 UI 组件和身份验证提供程序
description: Microsoft Graph Toolkit是一组身份验证提供程序和可重用的、与框架无关的 Web 组件，用于访问和使用 Microsoft Graph。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 3b9dd368f9fe565164f3025c1f3de81645ad22df
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629159"
---
# <a name="microsoft-graph-toolkit-ui-components-and-authentication-providers-for-microsoft-graph"></a><span data-ttu-id="44069-103">Microsoft Graph Toolkit：Microsoft Graph 的 UI 组件和身份验证提供程序</span><span class="sxs-lookup"><span data-stu-id="44069-103">Microsoft Graph Toolkit: UI Components and Authentication Providers for Microsoft Graph</span></span> 

<span data-ttu-id="44069-104">Microsoft Graph Toolkit是可重用的、与框架无关的组件和身份验证提供程序的集合，用于访问和使用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="44069-104">The Microsoft Graph Toolkit is a collection of reusable, framework-agnostic components and authentication providers for accessing and working with Microsoft Graph.</span></span> <span data-ttu-id="44069-105">这些组件具有开箱即用的功能，内置提供程序使用 Microsoft Graph 进行身份验证和提取数据。</span><span class="sxs-lookup"><span data-stu-id="44069-105">The components are fully functional right of out of the box, with built in providers that authenticate with and fetch data from Microsoft Graph.</span></span>

<span data-ttu-id="44069-106">Microsoft Graph Toolkit使你能够轻松地在应用程序中Graph Microsoft 应用程序。</span><span class="sxs-lookup"><span data-stu-id="44069-106">The Microsoft Graph Toolkit makes it easy to use Microsoft Graph in your application.</span></span> <span data-ttu-id="44069-107">在下面的示例中，登录用户及其日历事件使用 [Login](./components/login.md) 和 [Agenda](./components/agenda.md) 组件只显示两行代码。</span><span class="sxs-lookup"><span data-stu-id="44069-107">In the following example, a signed in user and their calendar events are displayed with just two lines of code by using the [Login](./components/login.md) and [Agenda](./components/agenda.md) components.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=samples-general--login-to-show-agenda&source=docs&source=docs" height="400"></iframe>

[<span data-ttu-id="44069-108">在"打开"mgt.dev</span><span class="sxs-lookup"><span data-stu-id="44069-108">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/samples-general--login-to-show-agenda&source=docs)

## <a name="whats-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="44069-109">Microsoft Graph Toolkit？</span><span class="sxs-lookup"><span data-stu-id="44069-109">What's in the Microsoft Graph Toolkit?</span></span>

### <a name="components"></a><span data-ttu-id="44069-110">组件</span><span class="sxs-lookup"><span data-stu-id="44069-110">Components</span></span>

<span data-ttu-id="44069-111">Microsoft Graph Toolkit包括一组 Web 组件，用于由 Microsoft Graph API 支持的最常用体验。</span><span class="sxs-lookup"><span data-stu-id="44069-111">The Microsoft Graph Toolkit includes a collection of web components for the most commonly built experiences powered by Microsoft Graph APIs.</span></span> 

<span data-ttu-id="44069-112">这些组件还可作为React[组件。](./get-started/mgt-react.md)</span><span class="sxs-lookup"><span data-stu-id="44069-112">The components are also available as [React components](./get-started/mgt-react.md).</span></span>

|<span data-ttu-id="44069-113">组件</span><span class="sxs-lookup"><span data-stu-id="44069-113">Component</span></span>|<span data-ttu-id="44069-114">说明</span><span class="sxs-lookup"><span data-stu-id="44069-114">Description</span></span>|
|---------|-----------|
|[<span data-ttu-id="44069-115">登录</span><span class="sxs-lookup"><span data-stu-id="44069-115">Login</span></span>](./components/login.md)|<span data-ttu-id="44069-116">一个按钮和一个飞出控件，用于使用 Microsoft Identity 平台对用户进行身份验证，在登录时显示用户配置文件信息。</span><span class="sxs-lookup"><span data-stu-id="44069-116">A button and a flyout control to authenticate a user with the Microsoft Identity platform and display the user's profile information on sign in.</span></span>|
|[<span data-ttu-id="44069-117">人员</span><span class="sxs-lookup"><span data-stu-id="44069-117">Person</span></span>](./components/person.md)|<span data-ttu-id="44069-118">按照片、姓名和/或电子邮件地址显示个人或联系人。</span><span class="sxs-lookup"><span data-stu-id="44069-118">Displays a person or contact by their photo, name, and/or email address.</span></span>|
|[<span data-ttu-id="44069-119">人员</span><span class="sxs-lookup"><span data-stu-id="44069-119">People</span></span>](./components/people.md)|<span data-ttu-id="44069-120">按照片或缩写显示一组人员或联系人。</span><span class="sxs-lookup"><span data-stu-id="44069-120">Displays a group of people or contacts by their photos or initials.</span></span>|
|[<span data-ttu-id="44069-121">议程</span><span class="sxs-lookup"><span data-stu-id="44069-121">Agenda</span></span>](./components/agenda.md)|<span data-ttu-id="44069-122">显示用户或组的日历中的事件。</span><span class="sxs-lookup"><span data-stu-id="44069-122">Displays events in a user or group's calendar.</span></span>|
|[<span data-ttu-id="44069-123">人员选取器</span><span class="sxs-lookup"><span data-stu-id="44069-123">People picker</span></span>](./components/people-picker.md)|<span data-ttu-id="44069-124">提供搜索人员并呈现结果列表的能力。</span><span class="sxs-lookup"><span data-stu-id="44069-124">Provides the ability to search for people and renders the list of results.</span></span>|
|[<span data-ttu-id="44069-125">个人卡片</span><span class="sxs-lookup"><span data-stu-id="44069-125">Person card</span></span>](./components/person-card.md)|<span data-ttu-id="44069-126">在人员组件上用于显示有关用户的更多个人资料信息的飞出图。</span><span class="sxs-lookup"><span data-stu-id="44069-126">A flyout used on the person component to display more profile information about a user.</span></span>|
|[<span data-ttu-id="44069-127">文件</span><span class="sxs-lookup"><span data-stu-id="44069-127">File</span></span>](./components/file.md)|<span data-ttu-id="44069-128">表示包含图标、文件名、作者等的文件或文件夹。</span><span class="sxs-lookup"><span data-stu-id="44069-128">Represents a file or folder with icon, filename, author, and more.</span></span>|
|[<span data-ttu-id="44069-129">文件列表</span><span class="sxs-lookup"><span data-stu-id="44069-129">File list</span></span>](./components/file-list.md)|<span data-ttu-id="44069-130">显示多个文件或文件夹的列表。</span><span class="sxs-lookup"><span data-stu-id="44069-130">Displays a list of multiple files or folders.</span></span>|
|[<span data-ttu-id="44069-131">获取</span><span class="sxs-lookup"><span data-stu-id="44069-131">Get</span></span>](./components/get.md)|<span data-ttu-id="44069-132">直接在 HTML 中对任意 Microsoft Graph API 进行 GET 查询。</span><span class="sxs-lookup"><span data-stu-id="44069-132">Make a GET query to any Microsoft Graph API directly in your HTML.</span></span>|
|[<span data-ttu-id="44069-133">通道选取器</span><span class="sxs-lookup"><span data-stu-id="44069-133">Channel picker</span></span>](./components/teams-channel-picker.md)|<span data-ttu-id="44069-134">提供搜索特定Microsoft Teams以从呈现的结果列表中选择通道的能力。</span><span class="sxs-lookup"><span data-stu-id="44069-134">Provides the ability to search for Microsoft Teams channels to select a channel from a rendered list of results.</span></span>|
|[<span data-ttu-id="44069-135">待办事项</span><span class="sxs-lookup"><span data-stu-id="44069-135">To Do</span></span>](./components/todo.md)|<span data-ttu-id="44069-136">显示并启用在任务中添加、删除、完成或编辑任务微软待办。</span><span class="sxs-lookup"><span data-stu-id="44069-136">Displays and enables adding, removing, completing, or editing of tasks from Microsoft To Do.</span></span>|
|[<span data-ttu-id="44069-137">Tasks</span><span class="sxs-lookup"><span data-stu-id="44069-137">Tasks</span></span>](./components/tasks.md)|<span data-ttu-id="44069-138">显示并启用添加、删除、完成或编辑 Microsoft Planner 或 微软待办。</span><span class="sxs-lookup"><span data-stu-id="44069-138">Displays and enables adding, removing, completing, or editing of tasks from Microsoft Planner or Microsoft To Do.</span></span>|

### <a name="providers"></a><span data-ttu-id="44069-139">提供程序</span><span class="sxs-lookup"><span data-stu-id="44069-139">Providers</span></span>

<span data-ttu-id="44069-140">[提供程序](/providers/providers.md)启用身份验证并提供用于在各种平台上获取访问令牌的实现，并公开用于调用 Microsoft Graph API 的 Microsoft Graph 客户端。</span><span class="sxs-lookup"><span data-stu-id="44069-140">[Providers](/providers/providers.md) enable authentication and provide the implementation for acquiring access tokens on various platforms and expose a Microsoft Graph client for calling the Microsoft Graph APIs.</span></span> <span data-ttu-id="44069-141">这些组件在用于提供程序时效果最佳，但提供程序可自行使用。</span><span class="sxs-lookup"><span data-stu-id="44069-141">The components work best when used with a provider, but the providers can be used on their own.</span></span>

|<span data-ttu-id="44069-142">提供程序</span><span class="sxs-lookup"><span data-stu-id="44069-142">Providers</span></span>|<span data-ttu-id="44069-143">说明</span><span class="sxs-lookup"><span data-stu-id="44069-143">Description</span></span>|
|---------|-----------|
|[<span data-ttu-id="44069-144">Msal</span><span class="sxs-lookup"><span data-stu-id="44069-144">Msal</span></span>](./providers/msal.md)|<span data-ttu-id="44069-145">使用 MSAL.js 登录用户并获取与 Microsoft Graph 一Graph。</span><span class="sxs-lookup"><span data-stu-id="44069-145">Uses MSAL.js to sign in users and acquire tokens to use with Microsoft Graph.</span></span>|
|[<span data-ttu-id="44069-146">Msal 2.0</span><span class="sxs-lookup"><span data-stu-id="44069-146">Msal 2.0</span></span>](./providers/msal2.md)| <span data-ttu-id="44069-147">使用 msal-browser 登录用户并获取与 Microsoft Graph 一Graph。</span><span class="sxs-lookup"><span data-stu-id="44069-147">Uses msal-browser to sign in users and acquire tokens to use with Microsoft Graph.</span></span>|
|[<span data-ttu-id="44069-148">百年</span><span class="sxs-lookup"><span data-stu-id="44069-148">Electron</span></span>](./providers/electron.md)|<span data-ttu-id="44069-149">通过身份验证并提供 Microsoft Graph访问"一线"应用内的组件</span><span class="sxs-lookup"><span data-stu-id="44069-149">Authenticates and provides Microsoft Graph access to components inside of Electron apps</span></span>|
|[<span data-ttu-id="44069-150">SharePoint</span><span class="sxs-lookup"><span data-stu-id="44069-150">SharePoint</span></span>](./providers/sharepoint.md)|<span data-ttu-id="44069-151">通过身份验证并提供 Microsoft Graph访问 Web 部件内SharePoint权限。</span><span class="sxs-lookup"><span data-stu-id="44069-151">Authenticates and provides Microsoft Graph access to components inside of SharePoint web parts.</span></span>|
|[<span data-ttu-id="44069-152">Teams</span><span class="sxs-lookup"><span data-stu-id="44069-152">Teams</span></span>](./providers/teams.md)|<span data-ttu-id="44069-153">通过身份验证并提供 Microsoft Graph访问选项卡内的组件Microsoft Teams权限。</span><span class="sxs-lookup"><span data-stu-id="44069-153">Authenticates and provides Microsoft Graph access to components inside of Microsoft Teams tabs.</span></span>|
|[<span data-ttu-id="44069-154">代理</span><span class="sxs-lookup"><span data-stu-id="44069-154">Proxy</span></span>](./providers/proxy.md)|<span data-ttu-id="44069-155">允许通过后端将所有调用路由到 Microsoft Graph后端身份验证。</span><span class="sxs-lookup"><span data-stu-id="44069-155">Allows the use of backend authentication by routing all calls to Microsoft Graph through your backend.</span></span>|
|[<span data-ttu-id="44069-156">自定义</span><span class="sxs-lookup"><span data-stu-id="44069-156">Custom</span></span>](./providers/custom.md)|<span data-ttu-id="44069-157">创建自定义提供程序以使用应用程序的现有身份验证代码Graph访问 Microsoft 客户端。</span><span class="sxs-lookup"><span data-stu-id="44069-157">Create a custom provider to enable authentication and access to Microsoft Graph with your application's existing authentication code.</span></span>|

## <a name="why-use-the-microsoft-graph-toolkit"></a><span data-ttu-id="44069-158">为什么使用 Microsoft Graph Toolkit？</span><span class="sxs-lookup"><span data-stu-id="44069-158">Why use the Microsoft Graph Toolkit?</span></span>

<span data-ttu-id="44069-159">Microsoft Graph Toolkit使由 Microsoft 支持的共同体验Graph轻松快速地集成到你自己的应用程序中。</span><span class="sxs-lookup"><span data-stu-id="44069-159">The Microsoft Graph Toolkit makes integrating common experiences powered by Microsoft Graph into your own application quick and easy.</span></span>

:::row:::
   :::column span="":::
    <span data-ttu-id="44069-160">**剪切开发时间**</span><span class="sxs-lookup"><span data-stu-id="44069-160">**Cut Development Time**</span></span>

    <span data-ttu-id="44069-161">连接到 Microsoft Graph API 和在 UI 中呈现数据（外观和感觉就像 Microsoft365 体验）的工作已由你完成，无需进行自定义。</span><span class="sxs-lookup"><span data-stu-id="44069-161">The work to connect to Microsoft Graph APIs and render the data in a UI that looks and feels like a Microsoft365 experience is done for you, with no customization required.</span></span>
  :::column-end:::
  :::column span="":::
    <span data-ttu-id="44069-162">**适用于任何地方**</span><span class="sxs-lookup"><span data-stu-id="44069-162">**Works Everywhere**</span></span>

    <span data-ttu-id="44069-163">所有组件均基于 Web 标准，可与任何新式浏览器和 Web 框架 (React、Angular、Vue 等) 。</span><span class="sxs-lookup"><span data-stu-id="44069-163">All components are based on web standards and work seamlessly with any modern browser and web framework (React, Angular, Vue, etc.).</span></span> 
  :::column-end:::
  :::column span="":::
    <span data-ttu-id="44069-164">**美观但灵活**</span><span class="sxs-lookup"><span data-stu-id="44069-164">**Beautiful but Flexible**</span></span>

    <span data-ttu-id="44069-165">这些组件旨在外观与 Microsoft365 体验类似，但也可使用 [CSS](./customize-components/style.md) 自定义属性和 [模板进行自定义](./customize-components/templates.md)。</span><span class="sxs-lookup"><span data-stu-id="44069-165">The components are designed to look and feel like Microsoft365 experiences, but are also customizable using [CSS custom properties](./customize-components/style.md) and [templating](./customize-components/templates.md).</span></span>
  :::column-end:::
:::row-end:::

## <a name="who-should-use-it"></a><span data-ttu-id="44069-166">Who应该使用它？</span><span class="sxs-lookup"><span data-stu-id="44069-166">Who should use it?</span></span>

<span data-ttu-id="44069-167">Microsoft Graph Toolkit非常适用于希望开发连接到 Microsoft Graph 和访问数据的应用的所有体验级别的开发人员，例如：</span><span class="sxs-lookup"><span data-stu-id="44069-167">The Microsoft Graph Toolkit is great for developers of all experience levels looking to develop an app that connects to and accesses data from Microsoft Graph, such as a:</span></span>
- <span data-ttu-id="44069-168">Web 应用</span><span class="sxs-lookup"><span data-stu-id="44069-168">Web app</span></span>
- <span data-ttu-id="44069-169">Microsoft Teams选项卡</span><span class="sxs-lookup"><span data-stu-id="44069-169">Microsoft Teams tab</span></span>
- <span data-ttu-id="44069-170">渐进式 Web 应用 (PWA) </span><span class="sxs-lookup"><span data-stu-id="44069-170">Progressive Web App (PWA)</span></span>
- <span data-ttu-id="44069-171">中国应用</span><span class="sxs-lookup"><span data-stu-id="44069-171">Electron app</span></span>
- <span data-ttu-id="44069-172">SharePoint Web 部件</span><span class="sxs-lookup"><span data-stu-id="44069-172">SharePoint web part</span></span>

## <a name="where-can-i-use-it"></a><span data-ttu-id="44069-173">在哪里可以使用它？</span><span class="sxs-lookup"><span data-stu-id="44069-173">Where can I use it?</span></span>

<span data-ttu-id="44069-174">以下Graph Toolkit支持 Microsoft 浏览器。</span><span class="sxs-lookup"><span data-stu-id="44069-174">The Microsoft Graph Toolkit is supported in the following browsers.</span></span>

|![Microsoft Edge](images/edgeIcon.png)|![Firefox](images/firefoxIcon.png)|![Chrome](images/chromeIcon.png)|![Safari](images/safariIcon.png)|![Opera](images/operaIcon.png)|![Samsung Internet](images/samsungInternetIcon.png)|
|----|----|----|----|----|----|----|
|<span data-ttu-id="44069-181">**Microsoft Edge**</span><span class="sxs-lookup"><span data-stu-id="44069-181">**Edge**</span></span>|<span data-ttu-id="44069-182">**Firefox**</span><span class="sxs-lookup"><span data-stu-id="44069-182">**Firefox**</span></span>|<span data-ttu-id="44069-183">**Chrome**</span><span class="sxs-lookup"><span data-stu-id="44069-183">**Chrome**</span></span>|<span data-ttu-id="44069-184">**Safari**</span><span class="sxs-lookup"><span data-stu-id="44069-184">**Safari**</span></span>|<span data-ttu-id="44069-185">**Opera**</span><span class="sxs-lookup"><span data-stu-id="44069-185">**Opera**</span></span>|<span data-ttu-id="44069-186">**三星**</span><span class="sxs-lookup"><span data-stu-id="44069-186">**Samsung**</span></span>|

## <a name="next-steps"></a><span data-ttu-id="44069-187">后续步骤</span><span class="sxs-lookup"><span data-stu-id="44069-187">Next steps</span></span>

- <span data-ttu-id="44069-188">尝试在运动场中的 [组件](https://mgt.dev)。</span><span class="sxs-lookup"><span data-stu-id="44069-188">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="44069-189">[开始使用](./get-started/overview.md)Microsoft Graph Toolkit。</span><span class="sxs-lookup"><span data-stu-id="44069-189">[Get started](./get-started/overview.md) with the Microsoft Graph Toolkit.</span></span>
- <span data-ttu-id="44069-190">请查看 Microsoft Graph Toolkit上的[GitHub。](https://aka.ms/mgt)</span><span class="sxs-lookup"><span data-stu-id="44069-190">Check out the Microsoft Graph Toolkit on [GitHub](https://aka.ms/mgt).</span></span>
