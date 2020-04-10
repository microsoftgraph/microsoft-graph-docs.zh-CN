---
title: Microsoft Graph 工具包：由 Microsoft Graph 提供支持的 Web 组件
description: Microsoft Graph 工具包是 resuable、框架不可知的 web 组件以及用于访问和使用 Microsoft Graph 的帮助程序的集合。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 2ba11a66dcec1eaec276b3fe71427fcf356cbcde
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181614"
---
# <a name="microsoft-graph-toolkit-web-components-powered-by-microsoft-graph"></a><span data-ttu-id="5c951-103">Microsoft Graph 工具包：由 Microsoft Graph 提供支持的 Web 组件</span><span class="sxs-lookup"><span data-stu-id="5c951-103">Microsoft Graph Toolkit: Web Components powered by Microsoft Graph</span></span>

<span data-ttu-id="5c951-104">Microsoft Graph 工具包是用于访问和使用 Microsoft Graph 的可重用、框架不可知 web 组件和帮助器的集合。</span><span class="sxs-lookup"><span data-stu-id="5c951-104">The Microsoft Graph Toolkit is a collection of reusable, framework-agnostic web components and helpers for accessing and working with Microsoft Graph.</span></span> <span data-ttu-id="5c951-105">组件在现成的功能中完全正常，内置提供程序，可通过 Microsoft Graph 中的数据进行身份验证和获取数据。</span><span class="sxs-lookup"><span data-stu-id="5c951-105">The components are fully functional right of out of the box, with built in providers that authenticate with and fetch data from Microsoft Graph.</span></span>

<span data-ttu-id="5c951-106">使用 Microsoft Graph 工具包，可以轻松地在应用程序中使用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="5c951-106">The Microsoft Graph Toolkit makes it easy to use Microsoft Graph in your application.</span></span> <span data-ttu-id="5c951-107">在下面的示例中，查看登录用户及其日历事件如何使用[登录](./components/login.md)和[议程](./components/agenda.md)组件仅显示两行代码。</span><span class="sxs-lookup"><span data-stu-id="5c951-107">In the example below, see how a signed in user and their calendar events are displayed with just two lines of code by using the [Login](./components/login.md) and [Agenda](./components/agenda.md) components.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=samples-general--login-to-show-agenda&source=docs&source=docs" height="400"></iframe>

[<span data-ttu-id="5c951-108">在 "dev" 中打开此示例</span><span class="sxs-lookup"><span data-stu-id="5c951-108">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/samples-general--login-to-show-agenda&source=docs)

## <a name="whats-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="5c951-109">Microsoft Graph 工具包中的内容是什么？</span><span class="sxs-lookup"><span data-stu-id="5c951-109">What's in the Microsoft Graph Toolkit?</span></span>

### <a name="components"></a><span data-ttu-id="5c951-110">组件</span><span class="sxs-lookup"><span data-stu-id="5c951-110">Components</span></span>

<span data-ttu-id="5c951-111">Microsoft Graph 工具包包含一系列 web 组件，用于 Microsoft Graph Api 所支持的最常见的构建体验。</span><span class="sxs-lookup"><span data-stu-id="5c951-111">The Microsoft Graph Toolkit includes a collection of web components for the most commonly built experiences powered by Microsoft Graph APIs.</span></span>

|<span data-ttu-id="5c951-112">组件</span><span class="sxs-lookup"><span data-stu-id="5c951-112">Component</span></span>|<span data-ttu-id="5c951-113">说明</span><span class="sxs-lookup"><span data-stu-id="5c951-113">Description</span></span>|
|---------|-----------|
|[<span data-ttu-id="5c951-114">登录</span><span class="sxs-lookup"><span data-stu-id="5c951-114">Login</span></span>](./components/login.md)|<span data-ttu-id="5c951-115">一个按钮和一个浮出控件，用于对用户进行身份验证，以使用 Microsoft 标识平台并在登录时显示用户的配置文件信息。</span><span class="sxs-lookup"><span data-stu-id="5c951-115">A button and a flyout control to authenticate a user with the Microsoft Identity platform and display the user's profile information on sign in.</span></span>|
|[<span data-ttu-id="5c951-116">人员</span><span class="sxs-lookup"><span data-stu-id="5c951-116">Person</span></span>](./components/person.md)|<span data-ttu-id="5c951-117">按照片、姓名和/或电子邮件地址显示人员或联系人。</span><span class="sxs-lookup"><span data-stu-id="5c951-117">Displays a person or contact by their photo, name, and/or email address.</span></span>|
|[<span data-ttu-id="5c951-118">人员</span><span class="sxs-lookup"><span data-stu-id="5c951-118">People</span></span>](./components/people.md)|<span data-ttu-id="5c951-119">按照片或缩写显示一组人或联系人。</span><span class="sxs-lookup"><span data-stu-id="5c951-119">Displays a group of people or contacts by their photos or initials.</span></span>|
|[<span data-ttu-id="5c951-120">日程</span><span class="sxs-lookup"><span data-stu-id="5c951-120">Agenda</span></span>](./components/agenda.md)|<span data-ttu-id="5c951-121">显示用户或组的日历中的事件。</span><span class="sxs-lookup"><span data-stu-id="5c951-121">Displays events in a user or group's calendar.</span></span>|
|[<span data-ttu-id="5c951-122">任务</span><span class="sxs-lookup"><span data-stu-id="5c951-122">Tasks</span></span>](./components/tasks.md)|<span data-ttu-id="5c951-123">显示并允许添加、删除、完成或编辑 Microsoft Planner 或 Microsoft To Do 中的任务。</span><span class="sxs-lookup"><span data-stu-id="5c951-123">Displays and enables adding, removing, completing, or editing of tasks from Microsoft Planner or Microsoft To-Do.</span></span>|
|[<span data-ttu-id="5c951-124">人员选取器</span><span class="sxs-lookup"><span data-stu-id="5c951-124">People picker</span></span>](./components/people-picker.md)|<span data-ttu-id="5c951-125">提供搜索人员并呈现结果列表的功能。</span><span class="sxs-lookup"><span data-stu-id="5c951-125">Provides the ability to search for people and renders the list of results.</span></span>|
|[<span data-ttu-id="5c951-126">个人卡片</span><span class="sxs-lookup"><span data-stu-id="5c951-126">Person card</span></span>](./components/person-card.md)|<span data-ttu-id="5c951-127">在 person 组件上使用的浮出控件，用于显示有关用户的更多配置文件信息。</span><span class="sxs-lookup"><span data-stu-id="5c951-127">A flyout used on the person component to display more profile information about a user.</span></span>|
|[<span data-ttu-id="5c951-128">获取</span><span class="sxs-lookup"><span data-stu-id="5c951-128">Get</span></span>](./components/get.md)|<span data-ttu-id="5c951-129">在 HTML 中直接向任何 Microsoft Graph API 发出 GET 查询。</span><span class="sxs-lookup"><span data-stu-id="5c951-129">Make a GET query to any Microsoft Graph API directly in your HTML.</span></span>|
|[<span data-ttu-id="5c951-130">频道选取器</span><span class="sxs-lookup"><span data-stu-id="5c951-130">Channel picker</span></span>](./components/teams-channel-picker.md)|<span data-ttu-id="5c951-131">提供搜索 Microsoft 团队频道以从呈现的结果列表中选择频道的功能。</span><span class="sxs-lookup"><span data-stu-id="5c951-131">Provides the ability to search for Microsoft Teams channels to select a channel from a rendered list of results.</span></span>|

### <a name="providers"></a><span data-ttu-id="5c951-132">提供程序</span><span class="sxs-lookup"><span data-stu-id="5c951-132">Providers</span></span>

<span data-ttu-id="5c951-133">与[提供程序](/providers/providers.md)配合使用时，组件的工作效果最佳。</span><span class="sxs-lookup"><span data-stu-id="5c951-133">The components work best when used with a [provider](/providers/providers.md).</span></span> <span data-ttu-id="5c951-134">提供程序启用身份验证，并提供用于获取调用 Microsoft Graph Api 的访问令牌的实现。</span><span class="sxs-lookup"><span data-stu-id="5c951-134">Providers enable authentication and provide the implementation for acquiring the access tokens for calling the Microsoft Graph APIs.</span></span>

|<span data-ttu-id="5c951-135">提供程序</span><span class="sxs-lookup"><span data-stu-id="5c951-135">Providers</span></span>|<span data-ttu-id="5c951-136">Description</span><span class="sxs-lookup"><span data-stu-id="5c951-136">Description</span></span>|
|---------|-----------|
|[<span data-ttu-id="5c951-137">Msal</span><span class="sxs-lookup"><span data-stu-id="5c951-137">Msal</span></span>](./providers/msal.md)|<span data-ttu-id="5c951-138">使用 MSAL 登录用户并获取令牌以用于 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="5c951-138">Uses MSAL.js to sign in users and acquire tokens to use with Microsoft Graph.</span></span>|
|[<span data-ttu-id="5c951-139">SharePoint</span><span class="sxs-lookup"><span data-stu-id="5c951-139">SharePoint</span></span>](./providers/sharepoint.md)|<span data-ttu-id="5c951-140">对 SharePoint web 部件内的组件进行身份验证并提供 Microsoft Graph 访问权限。</span><span class="sxs-lookup"><span data-stu-id="5c951-140">Authenticates and provides Microsoft Graph access to components inside of SharePoint web parts.</span></span>|
|[<span data-ttu-id="5c951-141">Teams</span><span class="sxs-lookup"><span data-stu-id="5c951-141">Teams</span></span>](./providers/teams.md)|<span data-ttu-id="5c951-142">对 Microsoft 团队选项卡内的组件进行身份验证并提供 Microsoft Graph 访问权限。</span><span class="sxs-lookup"><span data-stu-id="5c951-142">Authenticates and provides Microsoft Graph access to components inside of Microsoft Teams tabs.</span></span>|
|[<span data-ttu-id="5c951-143">代理</span><span class="sxs-lookup"><span data-stu-id="5c951-143">Proxy</span></span>](./providers/proxy.md)|<span data-ttu-id="5c951-144">通过将对 Microsoft Graph 的所有调用通过后端路由，允许使用后端身份验证。</span><span class="sxs-lookup"><span data-stu-id="5c951-144">Allows the use of backend authentication by routing all calls to Microsoft Graph through your backend.</span></span>|
|[<span data-ttu-id="5c951-145">自定义</span><span class="sxs-lookup"><span data-stu-id="5c951-145">Custom</span></span>](./providers/custom.md)|<span data-ttu-id="5c951-146">创建自定义提供程序，以便通过应用程序的现有身份验证代码启用对 Microsoft Graph 的身份验证和访问。</span><span class="sxs-lookup"><span data-stu-id="5c951-146">Create a custom provider to enable authentication and access to Microsoft Graph with your application's existing authentication code.</span></span>|

## <a name="why-use-the-microsoft-graph-toolkit"></a><span data-ttu-id="5c951-147">为什么要使用 Microsoft Graph 工具包？</span><span class="sxs-lookup"><span data-stu-id="5c951-147">Why use the Microsoft Graph Toolkit?</span></span>

<span data-ttu-id="5c951-148">Microsoft Graph 工具包将 Microsoft Graph 所支持的常见体验集成到您自己的应用程序中，快速轻松地实现。</span><span class="sxs-lookup"><span data-stu-id="5c951-148">The Microsoft Graph Toolkit makes integrating common experiences powered by Microsoft Graph into your own application quick and easy.</span></span>

:::row:::
   :::column span="":::
    <span data-ttu-id="5c951-149">**缩短开发时间**</span><span class="sxs-lookup"><span data-stu-id="5c951-149">**Cut Development Time**</span></span>

    <span data-ttu-id="5c951-150">连接到 Microsoft Graph Api 并在 UI 中呈现数据的工作在外观和感觉像 Microsoft365 体验的 UI 中，无需进行自定义。</span><span class="sxs-lookup"><span data-stu-id="5c951-150">The work to connect to Microsoft Graph APIs and render the data in a UI that looks and feels like a Microsoft365 experience is done for you, with no customization required.</span></span>
  :::column-end:::
  :::column span="":::
    <span data-ttu-id="5c951-151">**随处工作**</span><span class="sxs-lookup"><span data-stu-id="5c951-151">**Works Everywhere**</span></span>

    <span data-ttu-id="5c951-152">所有组件都基于 web 标准，并可与任何新式浏览器和 web 框架无缝协作（反应、角度、Vue 等）。</span><span class="sxs-lookup"><span data-stu-id="5c951-152">All components are based on web standards and work seamlessly with any modern browser and web framework (React, Angular, Vue, etc.).</span></span> 
  :::column-end:::
  :::column span="":::
    <span data-ttu-id="5c951-153">**漂亮但灵活**</span><span class="sxs-lookup"><span data-stu-id="5c951-153">**Beautiful but Flexible**</span></span>

    <span data-ttu-id="5c951-154">这些组件设计为外观和感觉像 Microsoft365，但也可以使用[CSS 自定义属性](./style.md)和[模板](./templates.md)进行自定义。</span><span class="sxs-lookup"><span data-stu-id="5c951-154">The components are designed to look and feel like Microsoft365 experiences, but are also customizable using [CSS custom properties](./style.md) and [templating](./templates.md).</span></span>
  :::column-end:::
:::row-end:::

## <a name="who-should-use-it"></a><span data-ttu-id="5c951-155">谁应使用它？</span><span class="sxs-lookup"><span data-stu-id="5c951-155">Who should use it?</span></span>

<span data-ttu-id="5c951-156">Microsoft Graph 工具包非常适合于开发用于开发 web 应用程序、Microsoft 团队选项卡或 SharePoint web 部件的所有体验级别，这些应用程序将连接到 Microsoft Graph 中的数据并对其进行访问。</span><span class="sxs-lookup"><span data-stu-id="5c951-156">The Microsoft Graph Toolkit is great for developers of all experience levels looking to develop a web application, Microsoft Teams tab, or SharePoint web part that connects to and accesses data from Microsoft Graph.</span></span>

## <a name="where-can-i-use-it"></a><span data-ttu-id="5c951-157">在哪里可以使用它？</span><span class="sxs-lookup"><span data-stu-id="5c951-157">Where can I use it?</span></span>

<span data-ttu-id="5c951-158">以下浏览器支持 Microsoft Graph 工具包。</span><span class="sxs-lookup"><span data-stu-id="5c951-158">The Microsoft Graph Toolkit is supported in the following browsers.</span></span>

|![Microsoft Edge](images/edgeIcon.png)|![Internet Explorer 11](images/internetExplorerIcon.png)|![Firefox](images/firefoxIcon.png)|![Chrome](images/chromeIcon.png)|![Safari](images/safariIcon.png)|![Opera](images/operaIcon.png)|![Samsung Internet](images/samsungInternetIcon.png)|
|----|----|----|----|----|----|----|
|<span data-ttu-id="5c951-166">**Microsoft Edge**</span><span class="sxs-lookup"><span data-stu-id="5c951-166">**Edge**</span></span>|<span data-ttu-id="5c951-167">**IE 11**</span><span class="sxs-lookup"><span data-stu-id="5c951-167">**IE 11**</span></span>|<span data-ttu-id="5c951-168">**Firefox**</span><span class="sxs-lookup"><span data-stu-id="5c951-168">**Firefox**</span></span>|<span data-ttu-id="5c951-169">**Chrome**</span><span class="sxs-lookup"><span data-stu-id="5c951-169">**Chrome**</span></span>|<span data-ttu-id="5c951-170">**Safari**</span><span class="sxs-lookup"><span data-stu-id="5c951-170">**Safari**</span></span>|<span data-ttu-id="5c951-171">**Opera**</span><span class="sxs-lookup"><span data-stu-id="5c951-171">**Opera**</span></span>|<span data-ttu-id="5c951-172">**Samsung**</span><span class="sxs-lookup"><span data-stu-id="5c951-172">**Samsung**</span></span>|

## <a name="next-steps"></a><span data-ttu-id="5c951-173">后续步骤</span><span class="sxs-lookup"><span data-stu-id="5c951-173">Next steps</span></span>

- <span data-ttu-id="5c951-174">尝试[样本](https://mgt.dev)中的组件。</span><span class="sxs-lookup"><span data-stu-id="5c951-174">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="5c951-175">[开始](get-started.md)使用 Microsoft Graph 工具包。</span><span class="sxs-lookup"><span data-stu-id="5c951-175">[Get started](get-started.md) with the Microsoft Graph Toolkit.</span></span>
