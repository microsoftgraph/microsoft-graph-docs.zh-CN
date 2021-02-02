---
title: 使用 Graph 浏览器
description: 了解如何使用 Graph 资源管理器中的一些重要功能。
localization_priority: Normal
author: bettirosengugi
ms.openlocfilehash: b4c669ae6983efe2082b623c3de5b019a049311d
ms.sourcegitcommit: 7dc8ca82a8b2c25c5084e6b3121688766c9c14a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/02/2021
ms.locfileid: "50072386"
---
# <a name="working-with-graph-explorer"></a><span data-ttu-id="fff32-103">使用 Graph 浏览器</span><span class="sxs-lookup"><span data-stu-id="fff32-103">Working with Graph Explorer</span></span>

<span data-ttu-id="fff32-104">[Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer/) 是一款开发人员工具，可方便你提出 Microsoft Graph REST API 请求并查看相应的响应。</span><span class="sxs-lookup"><span data-stu-id="fff32-104">[Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/) is a developer tool that lets you conveniently make Microsoft Graph REST API requests and view corresponding responses.</span></span> <span data-ttu-id="fff32-105">本文介绍如何使用 Graph 资源管理器中的一些重要功能。</span><span class="sxs-lookup"><span data-stu-id="fff32-105">This article describes how to use some of the important features in Graph Explorer.</span></span>

## <a name="consent-to-permissions"></a><span data-ttu-id="fff32-106">同意权限</span><span class="sxs-lookup"><span data-stu-id="fff32-106">Consent to permissions</span></span>

<span data-ttu-id="fff32-107">用户或管理员必须通过同意过程授予 Graph 资源管理器访问 Microsoft Graph 中数据的正确权限。</span><span class="sxs-lookup"><span data-stu-id="fff32-107">The user or administrator must grant Graph Explorer the correct permissions via a consent process to access data in Microsoft Graph.</span></span> <span data-ttu-id="fff32-108">登录时，通过"修改权限 **"选项卡或** 配置文件旁边的设置齿轮中的"选择权限"选项同意 Graph 资源管理器中的权限。</span><span class="sxs-lookup"><span data-stu-id="fff32-108">Consent to permissions in Graph Explorer either via the **Modify permissions** tab or the **Select permissions** option in the settings gear next to your profile when you’re signed in.</span></span> <span data-ttu-id="fff32-109">" **修改权限"** 选项卡列出了在地址栏中运行查询所需的所有权限。</span><span class="sxs-lookup"><span data-stu-id="fff32-109">The **Modify permissions** tab lists all permissions you need to run the query in the address bar.</span></span> 

<span data-ttu-id="fff32-110">同意权限：</span><span class="sxs-lookup"><span data-stu-id="fff32-110">To consent to permissions:</span></span>

1.  <span data-ttu-id="fff32-111">选择一个示例查询并运行它。</span><span class="sxs-lookup"><span data-stu-id="fff32-111">Select a sample query and run it.</span></span>
2.  <span data-ttu-id="fff32-112">选择 **"修改权限"** 选项卡。</span><span class="sxs-lookup"><span data-stu-id="fff32-112">Select the **Modify permissions** tab.</span></span>
3.  <span data-ttu-id="fff32-113">请参阅运行查询所需的权限列表。</span><span class="sxs-lookup"><span data-stu-id="fff32-113">See the list of permissions required to run the query.</span></span>
4.  <span data-ttu-id="fff32-114">选择要同意的权限旁边的同意按钮。</span><span class="sxs-lookup"><span data-stu-id="fff32-114">Select the consent button next to the permission you want to consent to.</span></span> 

![Graph 资源管理器屏幕截图，其中突出显示了同意权限的步骤](./images/modify-permissions.png)

<span data-ttu-id="fff32-116">" **修改权限"** 功能当前处于预览阶段，并且某些查询可能缺少权限。</span><span class="sxs-lookup"><span data-stu-id="fff32-116">The **Modify  permissions** feature is currently in preview, and some queries might be missing permissions.</span></span> <span data-ttu-id="fff32-117">如果查询缺少权限，则配置文件旁边的设置齿轮中的"选择权限"选项将包含所有可用权限的列表：</span><span class="sxs-lookup"><span data-stu-id="fff32-117">If permissions are missing for a query, the **Select permissions** option in the settings gear next to your profile contains the list of all available permissions:</span></span>

1.  <span data-ttu-id="fff32-118">转到设置齿轮，然后单击 **"选择权限"** 选项。</span><span class="sxs-lookup"><span data-stu-id="fff32-118">Go the settings gear and click the **Select permissions** option.</span></span> <span data-ttu-id="fff32-119">此选项包含所有可用权限的列表。</span><span class="sxs-lookup"><span data-stu-id="fff32-119">This option contains the list of all available permissions.</span></span>
2.  <span data-ttu-id="fff32-120">从所有权限列表中，同意所需的权限。</span><span class="sxs-lookup"><span data-stu-id="fff32-120">From the list of all the permissions, consent to the ones you want.</span></span>

![突出显示"选择权限"选项的图形资源管理器屏幕截图](./images/select-permissions.png)

## <a name="get-an-access-or-authentication-token"></a><span data-ttu-id="fff32-122">获取访问或身份验证令牌</span><span class="sxs-lookup"><span data-stu-id="fff32-122">Get an access or authentication token</span></span>

<span data-ttu-id="fff32-123">Graph 资源管理器包含 **一个访问令牌** 选项卡，可显示登录时的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="fff32-123">Graph Explorer includes an **Access token** tab that shows your access token when you are signed in.</span></span> <span data-ttu-id="fff32-124">在 **"访问令牌** "选项卡上，如果需要在常用 REST 客户端应用程序中使用它，可以复制令牌。</span><span class="sxs-lookup"><span data-stu-id="fff32-124">On the **Access token** tab, you can copy the token if you need to use it in your favorite REST client application.</span></span>

![Graph 资源管理器中"访问令牌"选项卡的屏幕截图，其中突出显示了"复制"按钮](./images/access-token.png)

## <a name="copy-code-snippets"></a><span data-ttu-id="fff32-126">复制代码段</span><span class="sxs-lookup"><span data-stu-id="fff32-126">Copy code snippets</span></span>

<span data-ttu-id="fff32-127">对于你在 Graph 资源管理器中选择或输入的每个 REST API 查询，你可以找到如何在代码段选项卡 -C#、Java、JavaScript 和 Objective-C 下展示的四种语言中调用该 API。 </span><span class="sxs-lookup"><span data-stu-id="fff32-127">For each REST API query you select or enter in Graph Explorer, you can find how to call that API in each of the four languages showcased under the **Code snippets** tab - C#, Java, JavaScript, and Objective-C.</span></span> 

![突出显示代码段选项卡的 Graph 资源管理器屏幕截图](./images/code-snippets.png)

## <a name="ui-component-integration"></a><span data-ttu-id="fff32-129">UI 组件集成</span><span class="sxs-lookup"><span data-stu-id="fff32-129">UI component integration</span></span>

<span data-ttu-id="fff32-130">Graph 资源管理器包括多个功能，以便更轻松地实现 UI。</span><span class="sxs-lookup"><span data-stu-id="fff32-130">Graph Explorer includes several features to make implementing UI easier.</span></span> <span data-ttu-id="fff32-131">在应用中也重复使用这些组件。</span><span class="sxs-lookup"><span data-stu-id="fff32-131">Reuse these components in your apps too.</span></span>

### <a name="microsoft-graph-toolkit-integration"></a><span data-ttu-id="fff32-132">Microsoft Graph Toolkit集成</span><span class="sxs-lookup"><span data-stu-id="fff32-132">Microsoft Graph Toolkit integration</span></span>

<span data-ttu-id="fff32-133">[Microsoft Graph Toolkit](/graph/toolkit/overview)是可重用的、与框架无关的 Web 组件和帮助程序的集合，用于访问和使用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="fff32-133">The [Microsoft Graph Toolkit](/graph/toolkit/overview) is a collection of reusable, framework-agnostic web components and helpers for accessing and working with Microsoft Graph.</span></span> <span data-ttu-id="fff32-134">这些组件具有功能齐全的功能，内置提供程序使用 Microsoft Graph 进行身份验证并提取数据。</span><span class="sxs-lookup"><span data-stu-id="fff32-134">The components are fully functional, with built in providers that authenticate with and fetch data from Microsoft Graph.</span></span>

<span data-ttu-id="fff32-135">Graph 资源管理器提供与 Microsoft Graph 和组件Toolkit REST API 查询。</span><span class="sxs-lookup"><span data-stu-id="fff32-135">Graph Explorer provides sample REST API queries that correspond to Microsoft Graph Toolkit components.</span></span> <span data-ttu-id="fff32-136">Toolkit **组件** 选项卡上的一个蓝点指示Toolkit在 Graph 资源管理器中为当前指定的 REST API 查询提供组件。</span><span class="sxs-lookup"><span data-stu-id="fff32-136">A blue dot on the **Toolkit component** tab indicates that the Toolkit provides a component for the currently specified REST API query in Graph Explorer.</span></span> <span data-ttu-id="fff32-137">你可以方便地将组件的代码复制到你的应用。</span><span class="sxs-lookup"><span data-stu-id="fff32-137">You can conveniently copy the code for the component to your app.</span></span>

<span data-ttu-id="fff32-138">下表列出了当前包含应用程序组件的示例Toolkit查询。</span><span class="sxs-lookup"><span data-stu-id="fff32-138">The following table lists the sample queries that currently include a Toolkit component.</span></span>

| <span data-ttu-id="fff32-139">**Graph 浏览器示例查询**</span><span class="sxs-lookup"><span data-stu-id="fff32-139">**Graph Explorer sample query**</span></span> | <span data-ttu-id="fff32-140">**Toolkit iFrame URL 示例**</span><span class="sxs-lookup"><span data-stu-id="fff32-140">**Toolkit sample iFrame URL**</span></span> |
| --- | --- |
| <span data-ttu-id="fff32-141">获取我的个人资料</span><span class="sxs-lookup"><span data-stu-id="fff32-141">GET my profile</span></span> | [<span data-ttu-id="fff32-142"> https://mgt.dev/iframe.html?id=components-mgt-person-card—person-card-hover</span><span class="sxs-lookup"><span data-stu-id="fff32-142">https://mgt.dev/iframe.html?id=components-mgt-person-card—person-card-hover</span></span>](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-person-card--person-card-hover&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083362882%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=9FvGlMZNc78EE66JiY7hrusYVuGUm2NeflYlVgwTVwo%3D&amp;reserved=0) |
| <span data-ttu-id="fff32-143">获取我合作的人</span><span class="sxs-lookup"><span data-stu-id="fff32-143">GET people I work with</span></span> | [<span data-ttu-id="fff32-144"> https://mgt.dev/iframe.html?id=components-mgt-people—people</span><span class="sxs-lookup"><span data-stu-id="fff32-144">https://mgt.dev/iframe.html?id=components-mgt-people—people</span></span>](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-people--people&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083372878%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=yMF3X0M%2FmvWTUfhMdNYkG5I7fDMXpPHS6Fwea%2B3ycPs%3D&amp;reserved=0) |
| <span data-ttu-id="fff32-145">获取我的所有规划器任务</span><span class="sxs-lookup"><span data-stu-id="fff32-145">GET all my planner tasks</span></span> | [<span data-ttu-id="fff32-146"> https://mgt.dev/iframe.html?id=components-mgt-tasks—tasks</span><span class="sxs-lookup"><span data-stu-id="fff32-146">https://mgt.dev/iframe.html?id=components-mgt-tasks—tasks</span></span>](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-tasks--tasks&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083382869%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=Vk5IhPb%2FNbni7c6bteEveIdQNn%2BPm6AchwewCJ%2Fkmzk%3D&amp;reserved=0) |
| <span data-ttu-id="fff32-147">获取下一周的事件</span><span class="sxs-lookup"><span data-stu-id="fff32-147">GET my events for the next week</span></span> | [<span data-ttu-id="fff32-148"> https://mgt.dev/iframe.html?id=components-mgt-agenda—get-events-for-next-week</span><span class="sxs-lookup"><span data-stu-id="fff32-148">https://mgt.dev/iframe.html?id=components-mgt-agenda—get-events-for-next-week</span></span>](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-agenda--get-events-for-next-week&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083382869%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=VVFcx3gXMmg%2B%2BdQCZXjAmkCk5zKcrntK6fI35jbdN94%3D&amp;reserved=0) |
| <span data-ttu-id="fff32-149">获取我的照片	</span><span class="sxs-lookup"><span data-stu-id="fff32-149">GET my photo</span></span> | [<span data-ttu-id="fff32-150"> https://mgt.dev/iframe.html?id=components-mgt-person—仅个人照片</span><span class="sxs-lookup"><span data-stu-id="fff32-150">https://mgt.dev/iframe.html?id=components-mgt-person—person-photo-only</span></span>](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-person--person-photo-only&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083392872%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=aI%2BUqciLPOxEqlIpbjT8wtWBgcaJWM6sqooRlLVspZ0%3D&amp;reserved=0) |

![Screenshot showing the Toolkit components tab with the code to generate the component highlighted](./images/get-graph-toolkit-card.png)

### <a name="adaptive-cards-integration"></a><span data-ttu-id="fff32-152">自适应卡片集成</span><span class="sxs-lookup"><span data-stu-id="fff32-152">Adaptive cards integration</span></span>

<span data-ttu-id="fff32-153">[自适应卡片](https://adaptivecards.io/) 是 UI 的与平台无关的代码段，在 JSON 中创作，应用和服务可以公开交换。</span><span class="sxs-lookup"><span data-stu-id="fff32-153">[Adaptive cards](https://adaptivecards.io/) are platform-agnostic snippets of UI, authored in JSON, that apps and services can openly exchange.</span></span> <span data-ttu-id="fff32-154">运行查询且自适应卡片可用时，自适应卡片选项卡上会显示一个 **蓝色** 点。</span><span class="sxs-lookup"><span data-stu-id="fff32-154">When you run a query and an adaptive card is available, a blue dot appears on the **Adaptive cards** tab.</span></span>

![Graph 资源管理器中自适应卡片选项卡的屏幕截图，其中突出显示了响应详细信息](./images/adaptive-cards.png)

## <a name="customize-the-theme-in-graph-explorer"></a><span data-ttu-id="fff32-156">在 Graph 资源管理器中自定义主题</span><span class="sxs-lookup"><span data-stu-id="fff32-156">Customize the theme in Graph Explorer</span></span>

<span data-ttu-id="fff32-157">通过选择设置齿轮下的"更改主题" **选项，** 为 Graph 浏览器选择主题。</span><span class="sxs-lookup"><span data-stu-id="fff32-157">Choose the theme for Graph Explorer by selecting the **Change theme** option under the settings gear.</span></span> <span data-ttu-id="fff32-158">主题选项为浅色、深色和高对比度。</span><span class="sxs-lookup"><span data-stu-id="fff32-158">Theme options are Light, Dark, and High contrast.</span></span>

![Graph 资源管理器中"更改主题"选项的屏幕截图，其中突出显示了主题选项](./images/change-theme.png)

## <a name="storing-and-sharing-queries"></a><span data-ttu-id="fff32-160">存储和共享查询</span><span class="sxs-lookup"><span data-stu-id="fff32-160">Storing and sharing queries</span></span>

<span data-ttu-id="fff32-161">在 Graph 资源管理器中运行的查询在"历史记录"选项卡中保存 30 **天。** 在"历史记录"选项卡上，您可以：</span><span class="sxs-lookup"><span data-stu-id="fff32-161">Queries run in Graph Explorer are saved for 30 days in the **History** tab. On the History tab, you can:</span></span>

1.  <span data-ttu-id="fff32-162">导出 .har 格式的所有历史记录项。</span><span class="sxs-lookup"><span data-stu-id="fff32-162">Export all history items in .har format.</span></span>
2.  <span data-ttu-id="fff32-163">删除所有历史记录项。</span><span class="sxs-lookup"><span data-stu-id="fff32-163">Delete all history items.</span></span>
3.  <span data-ttu-id="fff32-164">查看此历史记录项。</span><span class="sxs-lookup"><span data-stu-id="fff32-164">View this history item.</span></span>
4.  <span data-ttu-id="fff32-165">运行此查询。</span><span class="sxs-lookup"><span data-stu-id="fff32-165">Run this query.</span></span>
5.  <span data-ttu-id="fff32-166">以 .har 格式导出此历史记录项。</span><span class="sxs-lookup"><span data-stu-id="fff32-166">Export this history item in .har format.</span></span>
6.  <span data-ttu-id="fff32-167">删除此历史记录项。</span><span class="sxs-lookup"><span data-stu-id="fff32-167">Delete this history item.</span></span>

![突出显示选项的"历史记录"选项卡的屏幕截图](./images/storing-and-sharing-queries.png)

<span data-ttu-id="fff32-169">若要共享您运行的查询，请单击响应窗格中的"共享查询"按钮，然后单击"复制 **"。**</span><span class="sxs-lookup"><span data-stu-id="fff32-169">To share queries that you run, click the share query button in the response pane and click **copy**.</span></span> <span data-ttu-id="fff32-170">这会复制要共享的链接，并允许其他人查看查询和结果。</span><span class="sxs-lookup"><span data-stu-id="fff32-170">This copies a link to share and allow others to see your query and the results.</span></span>

![突出显示"共享和复制"选项的 Graph 浏览器屏幕截图](./images/share-query.png)

## <a name="graph-explorer-ui-features"></a><span data-ttu-id="fff32-172">Graph 浏览器 UI 功能</span><span class="sxs-lookup"><span data-stu-id="fff32-172">Graph Explorer UI features</span></span>

<span data-ttu-id="fff32-173">当你想要扩大请求和响应区域时，在 Graph 资源管理器中折叠并展开边栏组件。</span><span class="sxs-lookup"><span data-stu-id="fff32-173">Collapse and expand the sidebar component in Graph Explorer when you want to widen the request and response area.</span></span> <span data-ttu-id="fff32-174">若要折叠边栏组件，请选择边栏左上方的汉堡包图标。</span><span class="sxs-lookup"><span data-stu-id="fff32-174">To collapse the sidebar component, select the hamburger icon on the top left of the sidebar.</span></span>

![突出显示展开和折叠选项的 Graph 资源管理器屏幕截图](./images/expand-collapse-sidebar-component.png)

<span data-ttu-id="fff32-176">通过选择响应预览窗口中的展开箭头展开和折叠响应预览。</span><span class="sxs-lookup"><span data-stu-id="fff32-176">Expand and collapse the response preview by selecting the expand arrow in the response preview window.</span></span>

![突出显示展开和折叠选项的响应窗格屏幕截图](./images/expand-collapse-response-preview.png)

<span data-ttu-id="fff32-178">通过 Graph 浏览器 UI 方便地访问 Microsoft 365 开发人员计划网站，获取包含要试验的示例数据的免费沙盒。</span><span class="sxs-lookup"><span data-stu-id="fff32-178">Conveniently access the Microsoft 365 Developer Program site from the Graph Explorer UI to get a free sandbox with sample data to experiment with.</span></span> <span data-ttu-id="fff32-179">在设置齿轮下，选择 **"获取包含示例数据的沙盒"。**</span><span class="sxs-lookup"><span data-stu-id="fff32-179">Under the setting gear, select **Get a sandbox with sample data**.</span></span>

![突出显示了"获取包含示例数据"选项的沙盒的 Graph 资源管理器屏幕截图](./images/link-to-m365-dev-program.png)


## <a name="next-steps"></a><span data-ttu-id="fff32-181">后续步骤</span><span class="sxs-lookup"><span data-stu-id="fff32-181">Next steps</span></span>

- <span data-ttu-id="fff32-182">访问 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer/) 并浏览示例查询。</span><span class="sxs-lookup"><span data-stu-id="fff32-182">Visit [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/) and explore sample queries.</span></span>
- <span data-ttu-id="fff32-183">浏览 [Microsoft Graph Toolkit文档](/graph/toolkit/overview)。</span><span class="sxs-lookup"><span data-stu-id="fff32-183">Explore the [Microsoft Graph Toolkit documentation](/graph/toolkit/overview).</span></span>
- <span data-ttu-id="fff32-184">在 Graph 资源管理器 [GitHub](https://github.com/microsoftgraph/microsoft-graph-explorer-v4/issues/new/choose)存储库中参与或提供反馈。</span><span class="sxs-lookup"><span data-stu-id="fff32-184">Contribute or provide feedback in the [Graph Explorer GitHub repo](https://github.com/microsoftgraph/microsoft-graph-explorer-v4/issues/new/choose).</span></span>
