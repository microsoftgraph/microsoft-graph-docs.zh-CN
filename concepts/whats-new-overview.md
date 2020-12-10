---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 69cc7d0ba5232770bb3b014690991ffefff6df02
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597170"
---
# <a name="whats-new-in-microsoft-graph"></a><span data-ttu-id="218d8-103">Microsoft Graph 新增功能</span><span class="sxs-lookup"><span data-stu-id="218d8-103">What's new in Microsoft Graph</span></span>

<span data-ttu-id="218d8-104">查看 Microsoft Graph 中的最近两个月新增功能要点、[以前增加的内容](whats-new-earlier.md)以及如何[分享你的想法](#want-to-stay-in-the-loop)。</span><span class="sxs-lookup"><span data-stu-id="218d8-104">See highlights of what's new in the recent two months in Microsoft Graph, [what's added earlier](whats-new-earlier.md), and how you can [share your ideas](#want-to-stay-in-the-loop).</span></span> <span data-ttu-id="218d8-105">有关 API 级更新的详细列表，请参见 [API更改日志](changelog.md)。</span><span class="sxs-lookup"><span data-stu-id="218d8-105">For a detailed list of API-level updates, see the [API changelog](changelog.md).</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="218d8-106">_预览_ 状态下的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为正式发布 (GA) 状态。</span><span class="sxs-lookup"><span data-stu-id="218d8-106">Features, including APIs and tools, in _preview_ status may change without notice, and some may never be promoted to generally available (GA) status.</span></span> <span data-ttu-id="218d8-107">不要在成品应用中使用预览功能。</span><span class="sxs-lookup"><span data-stu-id="218d8-107">Do not use preview features in production apps.</span></span>

## <a name="december-2020-new-and-generally-available"></a><span data-ttu-id="218d8-108">2020 年 12 月：新版本和正式版</span><span class="sxs-lookup"><span data-stu-id="218d8-108">December 2020: New and generally available</span></span>

### <a name="cloud-communications"></a><span data-ttu-id="218d8-109">云通信</span><span class="sxs-lookup"><span data-stu-id="218d8-109">Cloud communications</span></span>
<span data-ttu-id="218d8-110">[状态](/graph/api/resources/presence) 资源的 GA，允许获取一个或多个用户的状态。</span><span class="sxs-lookup"><span data-stu-id="218d8-110">GA of the [presence](/graph/api/resources/presence) resource, allowing getting the presence information of one or more users.</span></span>

### <a name="teamwork"></a><span data-ttu-id="218d8-111">团队合作</span><span class="sxs-lookup"><span data-stu-id="218d8-111">Teamwork</span></span>
- <span data-ttu-id="218d8-112">[API 管理 Teams 应用安装](/graph/api/resources/teamsappinstallation) 的 GA，包括获取团队或用户个人范围内的 应用，或者添加、删除或更新该应用。</span><span class="sxs-lookup"><span data-stu-id="218d8-112">GA of the [API to manage the installation of a Teams app](/graph/api/resources/teamsappinstallation), including getting installed apps, or adding, removing, or upgrading of the app in a team or in the personal scope of a user.</span></span>
- <span data-ttu-id="218d8-113">[获取用户和 Teams 应用间的聊天](/graph/api/userscopeteamsappinstallation-get-chat)。</span><span class="sxs-lookup"><span data-stu-id="218d8-113">[Get a chat between a user and a Teams app](/graph/api/userscopeteamsappinstallation-get-chat).</span></span>

## <a name="december-2020-new-in-preview-only"></a><span data-ttu-id="218d8-114">2020 年 12 月：仅限预览版的新增功能</span><span class="sxs-lookup"><span data-stu-id="218d8-114">December 2020: New in preview only</span></span>

### <a name="identity-and-access"></a><span data-ttu-id="218d8-115">身份和访问</span><span class="sxs-lookup"><span data-stu-id="218d8-115">Identity and access</span></span>
<span data-ttu-id="218d8-116">获取或设置 Azure AD 的版本和创建元数据 [使用条款](/graph/api/resources/agreement?view=graph-rest-beta&preserve-view=true) [协议](/graph/api/resources/agreement?view=graph-rest-beta&preserve-view=true), [协议文件](/graph/api/resources/agreementfile?view=graph-rest-beta&preserve-view=true)，以及 [协议文件位置](/graph/api/resources/agreementfilelocalization?view=graph-rest-beta&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="218d8-116">Get or set the version and creation metadata for an Azure AD [terms of use](/graph/api/resources/agreement?view=graph-rest-beta&preserve-view=true) [agreement](/graph/api/resources/agreement?view=graph-rest-beta&preserve-view=true), [agreement file](/graph/api/resources/agreementfile?view=graph-rest-beta&preserve-view=true), and [agreementfilelocalization](/graph/api/resources/agreementfilelocalization?view=graph-rest-beta&preserve-view=true)</span></span>

## <a name="november-2020-new-and-generally-available"></a><span data-ttu-id="218d8-117">2020年 11 月：新版本和正式版</span><span class="sxs-lookup"><span data-stu-id="218d8-117">November 2020: New and generally available</span></span>

### <a name="cloud-communications"></a><span data-ttu-id="218d8-118">云通信</span><span class="sxs-lookup"><span data-stu-id="218d8-118">Cloud communications</span></span>
- <span data-ttu-id="218d8-119">[meetingParticipantInfo](/graph/api/resources/meetingParticipantInfo) 类型的 **role** 属性 GA，将[在线会议](/graph/api/resources/onlinemeeting) 中的参会者角色区分为与会者或报告者。</span><span class="sxs-lookup"><span data-stu-id="218d8-119">GA of the **role** property of the [meetingParticipantInfo](/graph/api/resources/meetingParticipantInfo) type, that distinguishes the role of a participant in an [online meeting](/graph/api/resources/onlinemeeting) as an attendee or presenter.</span></span>
- <span data-ttu-id="218d8-120">**lobbyBypassSettings** 属性 GA 以及其 [值](/graph/api/resources/lobbybypasssettings#lobbybypassscope-values) 许可用户加入在线会议。</span><span class="sxs-lookup"><span data-stu-id="218d8-120">GA of the **lobbyBypassSettings** property and its [values](/graph/api/resources/lobbybypasssettings#lobbybypassscope-values) to admit users to an online meeting.</span></span>
- <span data-ttu-id="218d8-121">**isEntryExitAnnounced** 属性 GA 自定义设置宣布召集者加入或离开在线会议。</span><span class="sxs-lookup"><span data-stu-id="218d8-121">GA of the **isEntryExitAnnounced** property to customize settings for announcing callers joining or leaving an online meeting.</span></span>
- <span data-ttu-id="218d8-122">**allowedPresenters** 属性 GA 允许会议中特定报告者。</span><span class="sxs-lookup"><span data-stu-id="218d8-122">GA of the **allowedPresenters** property to allow specific presenters in the meeting.</span></span>

### <a name="search"></a><span data-ttu-id="218d8-123">搜索</span><span class="sxs-lookup"><span data-stu-id="218d8-123">Search</span></span>
- <span data-ttu-id="218d8-124">Microsoft 搜索 [查询 API](/graph/api/resources/search-api-overview)的 GA，支持以下类型数据的范围搜索：</span><span class="sxs-lookup"><span data-stu-id="218d8-124">GA of the Microsoft Search [query API](/graph/api/resources/search-api-overview), supporting scoped searching of the following types of data:</span></span>
  - [<span data-ttu-id="218d8-125">Outlook 邮件</span><span class="sxs-lookup"><span data-stu-id="218d8-125">Outlook messages</span></span>](/graph/search-concept-messages)
  - [<span data-ttu-id="218d8-126">Outlook 日历事件</span><span class="sxs-lookup"><span data-stu-id="218d8-126">Outlook calendar events</span></span>](/graph/search-concept-events)
  - <span data-ttu-id="218d8-127">[OneDrive 和 SharePoint 资源](/graph/search-concept-files)。</span><span class="sxs-lookup"><span data-stu-id="218d8-127">[OneDrive and SharePoint resources](/graph/search-concept-files).</span></span>

### <a name="teamwork"></a><span data-ttu-id="218d8-128">团队合作</span><span class="sxs-lookup"><span data-stu-id="218d8-128">Teamwork</span></span>

- <span data-ttu-id="218d8-129">特定资源 GA 允许（RSC）权限。</span><span class="sxs-lookup"><span data-stu-id="218d8-129">GA of resource-specific consent (RSC) permissions.</span></span> <span data-ttu-id="218d8-130">RSC 权限允许团队所有者向生产应用授予精确同意，以便访问和/或修改团队的特定数据，例如读取团队的设置，或者修改频道的名称、说明及其他设置。</span><span class="sxs-lookup"><span data-stu-id="218d8-130">RSC permissions allow team owners to grant granular consent to a production app to access and/or modify specific data of a team, for example, reading the team's settings, or modifying channel names, descriptions, and other settings.</span></span>
- <span data-ttu-id="218d8-131">适用于 [频道](/graph/api/resources/channel) 或频道内的邮件 Api 的 GA。</span><span class="sxs-lookup"><span data-stu-id="218d8-131">GA of APIs that apply to a [channel](/graph/api/resources/channel) or messages within a channel.</span></span> <span data-ttu-id="218d8-132">Api 包括：</span><span class="sxs-lookup"><span data-stu-id="218d8-132">The APIs include:</span></span>
  - <span data-ttu-id="218d8-133">[创建](/graph/api/conversationmember-add) 或 从频道中[删除](/graph/api/conversationmember-delete) 对话成员。</span><span class="sxs-lookup"><span data-stu-id="218d8-133">[Create](/graph/api/conversationmember-add) or [delete](/graph/api/conversationmember-delete) a conversation member from a channel.</span></span>
  - <span data-ttu-id="218d8-134">[更新频道中成员](/graph/api/conversationmember-update) 的角色。</span><span class="sxs-lookup"><span data-stu-id="218d8-134">[Update the role of a member](/graph/api/conversationmember-update) in a channel.</span></span>
  - <span data-ttu-id="218d8-135">获取频道中的特定邮件或所有邮件。</span><span class="sxs-lookup"><span data-stu-id="218d8-135">Get a specific message or all messages in a channel.</span></span>
  - <span data-ttu-id="218d8-136">获取频道中的特定回复或所有回复。</span><span class="sxs-lookup"><span data-stu-id="218d8-136">Get a specific reply or all replies in a channel.</span></span>
  - <span data-ttu-id="218d8-137">[在频道中跟踪新增的或者已更新的邮件](/graph/api/chatmessage-delta)。</span><span class="sxs-lookup"><span data-stu-id="218d8-137">[Track new or updated messages in a channel](/graph/api/chatmessage-delta).</span></span>


## <a name="november-2020-new-in-preview-only"></a><span data-ttu-id="218d8-138">2020 年 11 月：仅限预览版的新增功能</span><span class="sxs-lookup"><span data-stu-id="218d8-138">November 2020: New in preview only</span></span>

### <a name="devices-and-apps--cloud-pc"></a><span data-ttu-id="218d8-139">设备和应用 | 云电脑</span><span class="sxs-lookup"><span data-stu-id="218d8-139">Devices and apps | Cloud PC</span></span>
<span data-ttu-id="218d8-140">[云电脑 API](/graph/api/resources/virtualendpoint?view=graph-rest-beta&preserve-view=true) 首次上线，使组织可以预配和管理员工的虚拟桌面。</span><span class="sxs-lookup"><span data-stu-id="218d8-140">Debut of the [cloud PC API](/graph/api/resources/virtualendpoint?view=graph-rest-beta&preserve-view=true) that lets organizations provision and manage virtual desktops for employees.</span></span> <span data-ttu-id="218d8-141">与 Intune API 配合使用来管理物理和虚拟终结点。</span><span class="sxs-lookup"><span data-stu-id="218d8-141">Use it in conjunction with the Intune API to manage physical and virtual endpoints.</span></span>

### <a name="devices-and-apps--cloud-printing"></a><span data-ttu-id="218d8-142">设备和应用 | 云打印</span><span class="sxs-lookup"><span data-stu-id="218d8-142">Devices and apps | Cloud printing</span></span>
<span data-ttu-id="218d8-143">在 [打印任务定义](/graph/api/resources/printtaskdefinition?view=graph-rest-beta&preserve-view=true)上[订阅更改通知](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="218d8-143">[Subscribe to change notifications](webhooks.md) on a [print task definition](/graph/api/resources/printtaskdefinition?view=graph-rest-beta&preserve-view=true).</span></span>

### <a name="devices-and-apps--corporate-management"></a><span data-ttu-id="218d8-144">设备和应用 | 公司管理</span><span class="sxs-lookup"><span data-stu-id="218d8-144">Devices and apps | Corporate management</span></span>
<span data-ttu-id="218d8-145">Intune beta 版[11 月](changelog.md#november-2020)更新。</span><span class="sxs-lookup"><span data-stu-id="218d8-145">Intune [November](changelog.md#november-2020) updates for the beta version.</span></span>

### <a name="identity-and-access"></a><span data-ttu-id="218d8-146">身份和访问</span><span class="sxs-lookup"><span data-stu-id="218d8-146">Identity and access</span></span>
- <span data-ttu-id="218d8-147">在 [应用](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true) 的 **spa** 属性中指定发送登录用户令牌的 URL，以及授权代码和访问令牌的URI。</span><span class="sxs-lookup"><span data-stu-id="218d8-147">Specify URLs for sending sign-in user tokens, and URIs for authorization codes and access tokens, in the **spa** property of [application](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true).</span></span>
- <span data-ttu-id="218d8-148">通过 [组织品牌属性](/graph/api/resources/organizationalbrandingproperties?view=graph-rest-beta&preserve-view=true) 自定义 Azure Active Directory 登录屏幕的界面外观。</span><span class="sxs-lookup"><span data-stu-id="218d8-148">Customize the look and feel of Azure Active Directory sign-in screens through the [organization branding properties](/graph/api/resources/organizationalbrandingproperties?view=graph-rest-beta&preserve-view=true).</span></span> <span data-ttu-id="218d8-149">组织可根据工作地点自定义特定用户。</span><span class="sxs-lookup"><span data-stu-id="218d8-149">Organizations can customize based on locale for specific users.</span></span>

### <a name="identity-and-access--governance"></a><span data-ttu-id="218d8-150">身份和访问 | 治理</span><span class="sxs-lookup"><span data-stu-id="218d8-150">Identity and access | Governance</span></span>
<span data-ttu-id="218d8-151">[组成员资格访问审查 API](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) 首次上线，可以定期审查用户访问，确保只有适当人员用户持续访问权，并有效管理组成员资格。</span><span class="sxs-lookup"><span data-stu-id="218d8-151">Debut of [access review API for group membership](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) to review user access regularly, make sure only the right people have continued access, and efficiently manage group memberships.</span></span>

### <a name="search"></a><span data-ttu-id="218d8-152">搜索</span><span class="sxs-lookup"><span data-stu-id="218d8-152">Search</span></span>
<span data-ttu-id="218d8-153">可以聚合数值或字符串类型的搜索结果，[Microsoft Graph 连接器](/microsoftsearch/connectors-overview)导入这些结果，并将其在[架构](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true)中设置为可精简。</span><span class="sxs-lookup"><span data-stu-id="218d8-153">You can aggregate numeric or string type search results that are imported by [Microsoft Graph connectors](/microsoftsearch/connectors-overview) and that are set to be refinable in the [schema](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true).</span></span> <span data-ttu-id="218d8-154">查看更多有关 [使用聚合优化搜索结果](search-concept-aggregation.md)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="218d8-154">See more information about [refining search results using aggregations](search-concept-aggregation.md).</span></span>


## <a name="want-to-stay-in-the-loop"></a><span data-ttu-id="218d8-155">保持循环</span><span class="sxs-lookup"><span data-stu-id="218d8-155">Want to stay in the loop?</span></span>

<span data-ttu-id="218d8-156">我们可以通过以下方式进行参与：</span><span class="sxs-lookup"><span data-stu-id="218d8-156">Here are some ways we can engage:</span></span>

- <span data-ttu-id="218d8-157">是否有希望 Microsoft Graph 支持的方案？</span><span class="sxs-lookup"><span data-stu-id="218d8-157">Are there scenarios you'd like Microsoft Graph to support?</span></span> <span data-ttu-id="218d8-158">在 [Microsoft Graph 用户心声](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)中建议新功能并进行投票。</span><span class="sxs-lookup"><span data-stu-id="218d8-158">Suggest and vote for new features at [Microsoft Graph User Voice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).</span></span>
    <span data-ttu-id="218d8-159">某些新功能来源于开发人员社区的热门请求。</span><span class="sxs-lookup"><span data-stu-id="218d8-159">Some new features originate as popular requests from the developer community.</span></span> <span data-ttu-id="218d8-160">Microsoft Graph 团队会定期评估客户需求，并按以下顺序发布新功能：</span><span class="sxs-lookup"><span data-stu-id="218d8-160">The Microsoft Graph team regularly evaluates customer needs and releases new features in the following order:</span></span>

    1. <span data-ttu-id="218d8-161">处于 **_预览_** 状态的 Debut。</span><span class="sxs-lookup"><span data-stu-id="218d8-161">Debut in **_preview_** status.</span></span> <span data-ttu-id="218d8-162">任何相关的 REST API 更新都在 beta 终结点 (`https://graph.microsoft.com/beta`) 中。</span><span class="sxs-lookup"><span data-stu-id="218d8-162">Any related REST API updates are in the beta endpoint (`https://graph.microsoft.com/beta`).</span></span>  

    2. <span data-ttu-id="218d8-163">如果有足够的反馈表明具有可行性，则提升为 **_正式发布_ (GA)** 状态。</span><span class="sxs-lookup"><span data-stu-id="218d8-163">Promoted to **_general availability_ (GA)** status, if sufficient feedback indicates viability.</span></span> <span data-ttu-id="218d8-164">任何相关的 REST API 更新都添加到 v1.0 终结点 (`https://graph.microsoft.com/v1.0`)。</span><span class="sxs-lookup"><span data-stu-id="218d8-164">Any related REST API updates are added to the v1.0 endpoint (`https://graph.microsoft.com/v1.0`).</span></span> 
- <span data-ttu-id="218d8-165">成为 Microsoft Graph 社区中的活跃成员!</span><span class="sxs-lookup"><span data-stu-id="218d8-165">Be an active member in the Microsoft Graph community!</span></span> <span data-ttu-id="218d8-166">[参与](https://aka.ms/microsoftgraphcall)Microsoft Graph 社区每月通话。</span><span class="sxs-lookup"><span data-stu-id="218d8-166">[Join](https://aka.ms/microsoftgraphcall) the monthly Microsoft Graph community call.</span></span>
- <span data-ttu-id="218d8-167">注册 [Microsoft 365 开发人员计划](https://developer.microsoft.com/office/dev-program)，免费订阅 Microsoft 365, 然后开始开发! </span><span class="sxs-lookup"><span data-stu-id="218d8-167">Sign up for the [Microsoft 365 developer program](https://developer.microsoft.com/office/dev-program), get a free Microsoft 365 subscription, and start developing!</span></span>


## <a name="see-also"></a><span data-ttu-id="218d8-168">另请参阅</span><span class="sxs-lookup"><span data-stu-id="218d8-168">See also</span></span>
- <span data-ttu-id="218d8-169">定期查看 [Microsoft Graph 开发人员博客](https://developer.microsoft.com/graph/blogs/), 了解发布公告和有帮助的资源。 </span><span class="sxs-lookup"><span data-stu-id="218d8-169">Check out the [Microsoft Graph developer blog](https://developer.microsoft.com/graph/blogs/) periodically for release announcements and helpful resources.</span></span>
- <span data-ttu-id="218d8-170">浏览 Microsoft Graph API 新增功能的详细信息, 以及[changelog](changelog.md)中的 API 行为更新。</span><span class="sxs-lookup"><span data-stu-id="218d8-170">Browse details of Microsoft Graph API additions, and API behavior updates in the [changelog](changelog.md).</span></span>
- <span data-ttu-id="218d8-171">查找[早期版本的重点内容](whats-new-earlier.md)。</span><span class="sxs-lookup"><span data-stu-id="218d8-171">Find [highlights of earlier releases](whats-new-earlier.md).</span></span>
- <span data-ttu-id="218d8-172">了解有关 [Microsoft Graph 的版本控制、支持和中断性变更策略](versioning-and-support.md)。</span><span class="sxs-lookup"><span data-stu-id="218d8-172">Learn more about [versioning, support, and breaking change policies for Microsoft Graph](versioning-and-support.md).</span></span>
