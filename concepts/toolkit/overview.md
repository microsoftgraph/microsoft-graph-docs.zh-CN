---
title: Microsoft Graph Toolkit：适用于 Microsoft Graph 的 UI 组件和身份验证提供程序
description: Microsoft Graph Toolkit是身份验证提供程序和可重用的、与框架无关的 Web 组件的集合，用于访问和使用 Microsoft Graph。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 01f406c288ebca1dde5c6b1577fd2acdc7631d5b
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470534"
---
# <a name="microsoft-graph-toolkit-ui-components-and-authentication-providers-for-microsoft-graph"></a><span data-ttu-id="3a331-103">Microsoft Graph Toolkit：适用于 Microsoft Graph 的 UI 组件和身份验证提供程序</span><span class="sxs-lookup"><span data-stu-id="3a331-103">Microsoft Graph Toolkit: UI Components and Authentication Providers for Microsoft Graph</span></span> 

<span data-ttu-id="3a331-104">Microsoft Graph Toolkit是可重用的、与框架无关的组件和身份验证提供程序的集合，用于访问和使用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="3a331-104">The Microsoft Graph Toolkit is a collection of reusable, framework-agnostic components and authentication providers for accessing and working with Microsoft Graph.</span></span> <span data-ttu-id="3a331-105">这些组件具有开箱即用的功能，内置提供程序使用 Microsoft Graph 进行身份验证并提取数据。</span><span class="sxs-lookup"><span data-stu-id="3a331-105">The components are fully functional right of out of the box, with built in providers that authenticate with and fetch data from Microsoft Graph.</span></span>

<span data-ttu-id="3a331-106">Microsoft Graph Toolkit可轻松在应用程序中使用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="3a331-106">The Microsoft Graph Toolkit makes it easy to use Microsoft Graph in your application.</span></span> <span data-ttu-id="3a331-107">在下面的示例中，登录用户及其日历事件使用登录和议程组件只显示两[行代码。](./components/agenda.md) [](./components/login.md)</span><span class="sxs-lookup"><span data-stu-id="3a331-107">In the following example, a signed in user and their calendar events are displayed with just two lines of code by using the [Login](./components/login.md) and [Agenda](./components/agenda.md) components.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=samples-general--login-to-show-agenda&source=docs&source=docs" height="400"></iframe>

[<span data-ttu-id="3a331-108">在 mgt.dev 中打开此示例</span><span class="sxs-lookup"><span data-stu-id="3a331-108">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/samples-general--login-to-show-agenda&source=docs)

## <a name="whats-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="3a331-109">What's in the Microsoft Graph Toolkit?</span><span class="sxs-lookup"><span data-stu-id="3a331-109">What's in the Microsoft Graph Toolkit?</span></span>

### <a name="components"></a><span data-ttu-id="3a331-110">组件</span><span class="sxs-lookup"><span data-stu-id="3a331-110">Components</span></span>

<span data-ttu-id="3a331-111">Microsoft Graph Toolkit包括一组 Web 组件，用于由 Microsoft Graph API 支持的最常用体验。</span><span class="sxs-lookup"><span data-stu-id="3a331-111">The Microsoft Graph Toolkit includes a collection of web components for the most commonly built experiences powered by Microsoft Graph APIs.</span></span> 

<span data-ttu-id="3a331-112">这些组件也作为 [React 组件提供](./get-started/mgt-react.md)。</span><span class="sxs-lookup"><span data-stu-id="3a331-112">The components are also available as [React components](./get-started/mgt-react.md).</span></span>

|<span data-ttu-id="3a331-113">组件</span><span class="sxs-lookup"><span data-stu-id="3a331-113">Component</span></span>|<span data-ttu-id="3a331-114">说明</span><span class="sxs-lookup"><span data-stu-id="3a331-114">Description</span></span>|
|---------|-----------|
|[<span data-ttu-id="3a331-115">登录</span><span class="sxs-lookup"><span data-stu-id="3a331-115">Login</span></span>](./components/login.md)|<span data-ttu-id="3a331-116">一个按钮和一个飞出控件，用于使用 Microsoft Identity 平台对用户进行身份验证，在登录时显示用户配置文件信息。</span><span class="sxs-lookup"><span data-stu-id="3a331-116">A button and a flyout control to authenticate a user with the Microsoft Identity platform and display the user's profile information on sign in.</span></span>|
|[<span data-ttu-id="3a331-117">人员</span><span class="sxs-lookup"><span data-stu-id="3a331-117">Person</span></span>](./components/person.md)|<span data-ttu-id="3a331-118">按个人或联系人的照片、姓名和/或电子邮件地址显示此人或联系人。</span><span class="sxs-lookup"><span data-stu-id="3a331-118">Displays a person or contact by their photo, name, and/or email address.</span></span>|
|[<span data-ttu-id="3a331-119">人员</span><span class="sxs-lookup"><span data-stu-id="3a331-119">People</span></span>](./components/people.md)|<span data-ttu-id="3a331-120">按照片或缩写显示一组人员或联系人。</span><span class="sxs-lookup"><span data-stu-id="3a331-120">Displays a group of people or contacts by their photos or initials.</span></span>|
|[<span data-ttu-id="3a331-121">议程</span><span class="sxs-lookup"><span data-stu-id="3a331-121">Agenda</span></span>](./components/agenda.md)|<span data-ttu-id="3a331-122">显示用户或组的日历中的事件。</span><span class="sxs-lookup"><span data-stu-id="3a331-122">Displays events in a user or group's calendar.</span></span>|
|[<span data-ttu-id="3a331-123">任务</span><span class="sxs-lookup"><span data-stu-id="3a331-123">Tasks</span></span>](./components/tasks.md)|<span data-ttu-id="3a331-124">显示并启用添加、删除、完成或编辑 Microsoft Planner 或 Microsoft To Do 中的任务。</span><span class="sxs-lookup"><span data-stu-id="3a331-124">Displays and enables adding, removing, completing, or editing of tasks from Microsoft Planner or Microsoft To Do.</span></span>|
|[<span data-ttu-id="3a331-125">人员选取器</span><span class="sxs-lookup"><span data-stu-id="3a331-125">People picker</span></span>](./components/people-picker.md)|<span data-ttu-id="3a331-126">提供搜索人员并呈现结果列表的能力。</span><span class="sxs-lookup"><span data-stu-id="3a331-126">Provides the ability to search for people and renders the list of results.</span></span>|
|[<span data-ttu-id="3a331-127">个人卡片</span><span class="sxs-lookup"><span data-stu-id="3a331-127">Person card</span></span>](./components/person-card.md)|<span data-ttu-id="3a331-128">在人员组件上用于显示有关用户的更多配置文件信息的飞出。</span><span class="sxs-lookup"><span data-stu-id="3a331-128">A flyout used on the person component to display more profile information about a user.</span></span>|
|[<span data-ttu-id="3a331-129">获取</span><span class="sxs-lookup"><span data-stu-id="3a331-129">Get</span></span>](./components/get.md)|<span data-ttu-id="3a331-130">直接在 HTML 中对任意 Microsoft Graph API 进行 GET 查询。</span><span class="sxs-lookup"><span data-stu-id="3a331-130">Make a GET query to any Microsoft Graph API directly in your HTML.</span></span>|
|[<span data-ttu-id="3a331-131">通道选取器</span><span class="sxs-lookup"><span data-stu-id="3a331-131">Channel picker</span></span>](./components/teams-channel-picker.md)|<span data-ttu-id="3a331-132">提供搜索 Microsoft Teams 频道以从呈现的结果列表中选择频道的能力。</span><span class="sxs-lookup"><span data-stu-id="3a331-132">Provides the ability to search for Microsoft Teams channels to select a channel from a rendered list of results.</span></span>|
|[<span data-ttu-id="3a331-133">待办事项</span><span class="sxs-lookup"><span data-stu-id="3a331-133">To Do</span></span>](./components/todo.md)|<span data-ttu-id="3a331-134">显示并启用添加、删除、完成或编辑 Microsoft To Do 中的任务。</span><span class="sxs-lookup"><span data-stu-id="3a331-134">Displays and enables adding, removing, completing, or editing of tasks from Microsoft To Do.</span></span>|

### <a name="providers"></a><span data-ttu-id="3a331-135">提供程序</span><span class="sxs-lookup"><span data-stu-id="3a331-135">Providers</span></span>

<span data-ttu-id="3a331-136">[提供程序](/providers/providers.md) 启用身份验证并提供在各种平台上获取访问令牌的实现，并公开用于调用 Microsoft Graph API 的 Microsoft Graph 客户端。</span><span class="sxs-lookup"><span data-stu-id="3a331-136">[Providers](/providers/providers.md) enable authentication and provide the implementation for acquiring access tokens on various platforms and expose a Microsoft Graph client for calling the Microsoft Graph APIs.</span></span> <span data-ttu-id="3a331-137">组件在与提供程序一起使用时效果最佳，但提供程序可以自行使用。</span><span class="sxs-lookup"><span data-stu-id="3a331-137">The components work best when used with a provider, but the providers can be used on their own.</span></span>

|<span data-ttu-id="3a331-138">提供程序</span><span class="sxs-lookup"><span data-stu-id="3a331-138">Providers</span></span>|<span data-ttu-id="3a331-139">说明</span><span class="sxs-lookup"><span data-stu-id="3a331-139">Description</span></span>|
|---------|-----------|
|[<span data-ttu-id="3a331-140">Msal</span><span class="sxs-lookup"><span data-stu-id="3a331-140">Msal</span></span>](./providers/msal.md)|<span data-ttu-id="3a331-141">使用MSAL.js登录用户并获取用于 Microsoft Graph 的令牌。</span><span class="sxs-lookup"><span data-stu-id="3a331-141">Uses MSAL.js to sign in users and acquire tokens to use with Microsoft Graph.</span></span>|
|[<span data-ttu-id="3a331-142">云</span><span class="sxs-lookup"><span data-stu-id="3a331-142">Electron</span></span>](./providers/electron.md)|<span data-ttu-id="3a331-143">验证并提供 Microsoft Graph 对"一线"应用内组件的访问</span><span class="sxs-lookup"><span data-stu-id="3a331-143">Authenticates and provides Microsoft Graph access to components inside of Electron apps</span></span>|
|[<span data-ttu-id="3a331-144">SharePoint</span><span class="sxs-lookup"><span data-stu-id="3a331-144">SharePoint</span></span>](./providers/sharepoint.md)|<span data-ttu-id="3a331-145">对 SharePoint Web 部件内的组件进行身份验证并提供 Microsoft Graph 访问。</span><span class="sxs-lookup"><span data-stu-id="3a331-145">Authenticates and provides Microsoft Graph access to components inside of SharePoint web parts.</span></span>|
|[<span data-ttu-id="3a331-146">Teams</span><span class="sxs-lookup"><span data-stu-id="3a331-146">Teams</span></span>](./providers/teams.md)|<span data-ttu-id="3a331-147">对 Microsoft Teams 选项卡内的组件进行身份验证并提供 Microsoft Graph 访问。</span><span class="sxs-lookup"><span data-stu-id="3a331-147">Authenticates and provides Microsoft Graph access to components inside of Microsoft Teams tabs.</span></span>|
|[<span data-ttu-id="3a331-148">代理</span><span class="sxs-lookup"><span data-stu-id="3a331-148">Proxy</span></span>](./providers/proxy.md)|<span data-ttu-id="3a331-149">允许通过后端路由对 Microsoft Graph 的所有调用来使用后端身份验证。</span><span class="sxs-lookup"><span data-stu-id="3a331-149">Allows the use of backend authentication by routing all calls to Microsoft Graph through your backend.</span></span>|
|[<span data-ttu-id="3a331-150">自定义</span><span class="sxs-lookup"><span data-stu-id="3a331-150">Custom</span></span>](./providers/custom.md)|<span data-ttu-id="3a331-151">创建自定义提供程序以使用应用程序的现有身份验证代码启用身份验证并访问 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="3a331-151">Create a custom provider to enable authentication and access to Microsoft Graph with your application's existing authentication code.</span></span>|

## <a name="why-use-the-microsoft-graph-toolkit"></a><span data-ttu-id="3a331-152">为什么使用 Microsoft Graph Toolkit？</span><span class="sxs-lookup"><span data-stu-id="3a331-152">Why use the Microsoft Graph Toolkit?</span></span>

<span data-ttu-id="3a331-153">Microsoft Graph Toolkit使由 Microsoft Graph 支持的共同体验快速轻松地集成到你自己的应用程序中。</span><span class="sxs-lookup"><span data-stu-id="3a331-153">The Microsoft Graph Toolkit makes integrating common experiences powered by Microsoft Graph into your own application quick and easy.</span></span>

:::row:::
   :::column span="":::
    <span data-ttu-id="3a331-154">**剪切开发时间**</span><span class="sxs-lookup"><span data-stu-id="3a331-154">**Cut Development Time**</span></span>

    <span data-ttu-id="3a331-155">连接到 Microsoft Graph API 和在 UI 中呈现数据（外观和感觉就像 Microsoft365 体验）的工作已由你完成，无需进行自定义。</span><span class="sxs-lookup"><span data-stu-id="3a331-155">The work to connect to Microsoft Graph APIs and render the data in a UI that looks and feels like a Microsoft365 experience is done for you, with no customization required.</span></span>
  :::column-end:::
  :::column span="":::
    <span data-ttu-id="3a331-156">**适用于任何地方**</span><span class="sxs-lookup"><span data-stu-id="3a331-156">**Works Everywhere**</span></span>

    <span data-ttu-id="3a331-157">所有组件均基于 Web 标准，可与 React、Angular、Vue 等 (浏览器和 Web 框架无缝) 。</span><span class="sxs-lookup"><span data-stu-id="3a331-157">All components are based on web standards and work seamlessly with any modern browser and web framework (React, Angular, Vue, etc.).</span></span> 
  :::column-end:::
  :::column span="":::
    <span data-ttu-id="3a331-158">**美观但灵活**</span><span class="sxs-lookup"><span data-stu-id="3a331-158">**Beautiful but Flexible**</span></span>

    <span data-ttu-id="3a331-159">这些组件旨在外观与 Microsoft365 体验类似，但也可使用 [CSS](./customize-components/style.md) 自定义属性和 [模板进行自定义](./customize-components/templates.md)。</span><span class="sxs-lookup"><span data-stu-id="3a331-159">The components are designed to look and feel like Microsoft365 experiences, but are also customizable using [CSS custom properties](./customize-components/style.md) and [templating](./customize-components/templates.md).</span></span>
  :::column-end:::
:::row-end:::

## <a name="who-should-use-it"></a><span data-ttu-id="3a331-160">谁应该使用它？</span><span class="sxs-lookup"><span data-stu-id="3a331-160">Who should use it?</span></span>

<span data-ttu-id="3a331-161">Microsoft Graph Toolkit对于希望开发连接到 Microsoft Graph 和从 Microsoft Graph 访问数据的应用（例如：</span><span class="sxs-lookup"><span data-stu-id="3a331-161">The Microsoft Graph Toolkit is great for developers of all experience levels looking to develop an app that connects to and accesses data from Microsoft Graph, such as a:</span></span>
- <span data-ttu-id="3a331-162">Web 应用</span><span class="sxs-lookup"><span data-stu-id="3a331-162">Web app</span></span>
- <span data-ttu-id="3a331-163">Microsoft Teams 选项卡</span><span class="sxs-lookup"><span data-stu-id="3a331-163">Microsoft Teams tab</span></span>
- <span data-ttu-id="3a331-164">渐进式 Web App (PWA) </span><span class="sxs-lookup"><span data-stu-id="3a331-164">Progressive Web App (PWA)</span></span>
- <span data-ttu-id="3a331-165">光化应用</span><span class="sxs-lookup"><span data-stu-id="3a331-165">Electron app</span></span>
- <span data-ttu-id="3a331-166">SharePoint Web 部件</span><span class="sxs-lookup"><span data-stu-id="3a331-166">SharePoint web part</span></span>

## <a name="where-can-i-use-it"></a><span data-ttu-id="3a331-167">在哪里可以使用？</span><span class="sxs-lookup"><span data-stu-id="3a331-167">Where can I use it?</span></span>

<span data-ttu-id="3a331-168">以下Toolkit支持 Microsoft Graph 浏览器。</span><span class="sxs-lookup"><span data-stu-id="3a331-168">The Microsoft Graph Toolkit is supported in the following browsers.</span></span>

|![Microsoft Edge](images/edgeIcon.png)|![Firefox](images/firefoxIcon.png)|![Chrome](images/chromeIcon.png)|![Safari](images/safariIcon.png)|![Opera](images/operaIcon.png)|![三星 Internet](images/samsungInternetIcon.png)|
|----|----|----|----|----|----|----|
|<span data-ttu-id="3a331-175">**Microsoft Edge**</span><span class="sxs-lookup"><span data-stu-id="3a331-175">**Edge**</span></span>|<span data-ttu-id="3a331-176">**Firefox**</span><span class="sxs-lookup"><span data-stu-id="3a331-176">**Firefox**</span></span>|<span data-ttu-id="3a331-177">**Chrome**</span><span class="sxs-lookup"><span data-stu-id="3a331-177">**Chrome**</span></span>|<span data-ttu-id="3a331-178">**Safari**</span><span class="sxs-lookup"><span data-stu-id="3a331-178">**Safari**</span></span>|<span data-ttu-id="3a331-179">**Opera**</span><span class="sxs-lookup"><span data-stu-id="3a331-179">**Opera**</span></span>|<span data-ttu-id="3a331-180">**Samsung**</span><span class="sxs-lookup"><span data-stu-id="3a331-180">**Samsung**</span></span>|

## <a name="next-steps"></a><span data-ttu-id="3a331-181">后续步骤</span><span class="sxs-lookup"><span data-stu-id="3a331-181">Next steps</span></span>

- <span data-ttu-id="3a331-182">尝试在运动场 [中的组件](https://mgt.dev)。</span><span class="sxs-lookup"><span data-stu-id="3a331-182">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="3a331-183">[Microsoft](./get-started/overview.md) Graph Toolkit。</span><span class="sxs-lookup"><span data-stu-id="3a331-183">[Get started](./get-started/overview.md) with the Microsoft Graph Toolkit.</span></span>
- <span data-ttu-id="3a331-184">查看 GitHub 上的 Microsoft Graph [Toolkit。](https://aka.ms/mgt)</span><span class="sxs-lookup"><span data-stu-id="3a331-184">Check out the Microsoft Graph Toolkit on [GitHub](https://aka.ms/mgt).</span></span>
