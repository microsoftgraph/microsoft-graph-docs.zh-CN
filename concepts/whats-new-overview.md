---
title: Microsoft Graph 新增功能
description: Microsoft Graph 新增功能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: ea123de2fea1efdc4647238f6a953e21d49901db
ms.sourcegitcommit: f23cc661a0e30d01a6b59cfdae90768c55b80ae2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/08/2019
ms.locfileid: "37418208"
---
# <a name="whats-new-in-microsoft-graph"></a><span data-ttu-id="9c2e0-103">Microsoft Graph 新增功能</span><span class="sxs-lookup"><span data-stu-id="9c2e0-103">What's new in Microsoft Graph</span></span>

<span data-ttu-id="9c2e0-104">你是否知道 Microsoft Graph 中的一些新功能来源于开发人员社区的热门请求？</span><span class="sxs-lookup"><span data-stu-id="9c2e0-104">Did you know some new features in Microsoft Graph originate as popular requests from the developer community?</span></span> 

<span data-ttu-id="9c2e0-105">Microsoft Graph 团队会定期评估客户需求，并按以下顺序发布新功能：</span><span class="sxs-lookup"><span data-stu-id="9c2e0-105">The Microsoft Graph team regularly evaluates customer needs and releases new features in the following order:</span></span>

1. <span data-ttu-id="9c2e0-106">处于**_预览_** 状态的 Debut。</span><span class="sxs-lookup"><span data-stu-id="9c2e0-106">Debut in **_preview_** status.</span></span> <span data-ttu-id="9c2e0-107">任何相关的 REST API 更新都在 beta 终结点 (`https://graph.microsoft.com/beta`) 中。</span><span class="sxs-lookup"><span data-stu-id="9c2e0-107">Any related REST API updates are in the beta endpoint (`https://graph.microsoft.com/beta`).</span></span>  

2. <span data-ttu-id="9c2e0-108">如果有足够的反馈表明具有可行性，则提升为 **_正式发布_ (GA)** 状态。</span><span class="sxs-lookup"><span data-stu-id="9c2e0-108">Promoted to **_general availability_ (GA)** status, if sufficient feedback indicates viability.</span></span> <span data-ttu-id="9c2e0-109">任何相关的 REST API 更新都添加到 v1.0 终结点 (`https://graph.microsoft.com/v1.0`)。</span><span class="sxs-lookup"><span data-stu-id="9c2e0-109">Any related REST API updates are added to the v1.0 endpoint (`https://graph.microsoft.com/v1.0`).</span></span> 

<span data-ttu-id="9c2e0-110">在下面查看 Microsoft Graph 中新增功能要点，并查看你可如何[分享你的想法](#want-to-stay-in-the-loop)。</span><span class="sxs-lookup"><span data-stu-id="9c2e0-110">Below, see highlights of what's new in Microsoft Graph, and how you can [share your ideas](#want-to-stay-in-the-loop).</span></span> <span data-ttu-id="9c2e0-111">如需了解 API 更新的更多详情，请参阅 API 更改日志的 [9 月](changelog.md#september-2019)和 [8 月](changelog.md#august-2019)部分。</span><span class="sxs-lookup"><span data-stu-id="9c2e0-111">For details of API updates, see the [September](changelog.md#september-2019) and [August](changelog.md#august-2019) sections of the API changelog.</span></span> 


## <a name="october-2019-new-and-generally-available"></a><span data-ttu-id="9c2e0-112">2019 年 10 月：新版本和正式版</span><span class="sxs-lookup"><span data-stu-id="9c2e0-112">September 2019: New and generally available</span></span>

### <a name="mail"></a><span data-ttu-id="9c2e0-113">邮件</span><span class="sxs-lookup"><span data-stu-id="9c2e0-113">Mail</span></span>
<span data-ttu-id="9c2e0-114">使用新的 **message** 参数更新[回复](/graph/api/message-reply?view=graph-rest-1.0)邮件时任何可写的 [message](/graph/api/resources/message?view=graph-rest-1.0) 属性，例如 [将收件人添加到回复](/graph/api/message-reply#example ?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="9c2e0-114">Use the new **message** parameter to update any writeable [message](/graph/api/resources/message?view=graph-rest-1.0) properties when [replying](/graph/api/message-reply?view=graph-rest-1.0) to a message, for example, [adding a recipient to the reply](/graph/api/message-reply#example ?view=graph-rest-1.0).</span></span>

### <a name="users"></a><span data-ttu-id="9c2e0-115">用户</span><span class="sxs-lookup"><span data-stu-id="9c2e0-115">Users</span></span>
<span data-ttu-id="9c2e0-116">[获取](/graph/api/user-get-mailboxsettings?view=graph-rest-1.0)或[设置](/graph/api/user-update-mailboxsettings?view=graph-rest-1.0)[用户邮箱](/graph/api/resources/mailboxsettings?view=graph-rest-1.0)的用户首选日期和时间格式设置。</span><span class="sxs-lookup"><span data-stu-id="9c2e0-116">Get or update a user's preferred date and time format settings for the mailbox.</span></span> 

## <a name="october-2019-new-in-preview"></a><span data-ttu-id="9c2e0-117">2019 年 10 月：预览版中的新增功能</span><span class="sxs-lookup"><span data-stu-id="9c2e0-117">August 2019: New in preview</span></span>

> [!IMPORTANT]
> <span data-ttu-id="9c2e0-118">_预览_状态下的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为 GA 状态。</span><span class="sxs-lookup"><span data-stu-id="9c2e0-118">Features, including APIs and tools, in _preview_ status may change without notice, and some may never be promoted to GA status.</span></span> <span data-ttu-id="9c2e0-119">请不要在生产应用中使用它们。</span><span class="sxs-lookup"><span data-stu-id="9c2e0-119">Do not use them in production apps.</span></span>

### <a name="groups"></a><span data-ttu-id="9c2e0-120">组</span><span class="sxs-lookup"><span data-stu-id="9c2e0-120">Groups</span></span>
<span data-ttu-id="9c2e0-121">使用 **hideFromAddressLists** 和 **hideFromOutlookClients** 属性在 Outlook 用户界面的某些部分或 Outlook 客户端中控制[组](/graph/api/resources/group?view=graph-rest-beta)的可见性。</span><span class="sxs-lookup"><span data-stu-id="9c2e0-121">Use the **hideFromAddressLists** and **hideFromOutlookClients** properties to control the visibility of a [group](/graph/api/resources/group?view=graph-rest-beta) in certain parts of the Outlook user interface or in an Outlook client.</span></span>

## <a name="september-2019-new-and-generally-available"></a><span data-ttu-id="9c2e0-122">2019 年 9 月：新版本和正式版</span><span class="sxs-lookup"><span data-stu-id="9c2e0-122">September 2019: New and generally available</span></span>

### <a name="calendar-mail-and-group"></a><span data-ttu-id="9c2e0-123">日历、邮件和组</span><span class="sxs-lookup"><span data-stu-id="9c2e0-123">Calendar, mail, and group</span></span>
<span data-ttu-id="9c2e0-124">[获取文件的原始内容或项目的 MIME 内容](/graph/api/attachment-get?view=graph-rest-1.0#get-the-raw-contents-of-a-file-or-item-attachment)，该项目已作为[附件](/graph/api/resources/attachment?view=graph-rest-1.0)添加到[事件](/graph/api/resources/event?view=graph-rest-1.0)、[邮件](/graph/api/resources/message?view=graph-rest-1.0)或组[帖子](/graph/api/resources/post?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="9c2e0-124">[Get the raw content of a file, or the MIME content of an item](/graph/api/attachment-get?view=graph-rest-1.0#get-the-raw-contents-of-a-file-or-item-attachment) that has been added as an [attachment](/graph/api/resources/attachment?view=graph-rest-1.0) to an [event](/graph/api/resources/event?view=graph-rest-1.0), [message](/graph/api/resources/message?view=graph-rest-1.0), or group [post](/graph/api/resources/post?view=graph-rest-1.0).</span></span>

### <a name="calendar-mail-outlook-task-personal-contact"></a><span data-ttu-id="9c2e0-125">日历、邮件、Outlook 任务、个人联系人</span><span class="sxs-lookup"><span data-stu-id="9c2e0-125">Calendar, mail, Outlook task, personal contact</span></span>
<span data-ttu-id="9c2e0-126">使用 [translateExchangeId](/graph/api/user-translateexchangeids?view=graph-rest-1.0) 函数在受支持的[格式](/graph/api/user-translateexchangeids?view=graph-rest-1.0#exchangeidformat-values)之间转换 Outlook 项目 ID，包括 Microsoft Graph 默认 ID 格式和不可变的 ID 格式。</span><span class="sxs-lookup"><span data-stu-id="9c2e0-126">Use the [translateExchangeId](/graph/api/user-translateexchangeids?view=graph-rest-1.0) function to convert an Outlook item ID between supported [formats](/graph/api/user-translateexchangeids?view=graph-rest-1.0#exchangeidformat-values), including the Microsoft Graph default ID format and immutable ID format.</span></span> 

<span data-ttu-id="9c2e0-127">以下资源支持 ID 格式转换：</span><span class="sxs-lookup"><span data-stu-id="9c2e0-127">The following resources support ID format conversion:</span></span>

- [<span data-ttu-id="9c2e0-128">附件</span><span class="sxs-lookup"><span data-stu-id="9c2e0-128">attachment</span></span>](/graph/api/resources/attachment?view=graph-rest-1.0)
- [<span data-ttu-id="9c2e0-129">联系人</span><span class="sxs-lookup"><span data-stu-id="9c2e0-129">contact</span></span>](/graph/api/resources/contact?view=graph-rest-1.0)
- [<span data-ttu-id="9c2e0-130">事件</span><span class="sxs-lookup"><span data-stu-id="9c2e0-130">event</span></span>](/graph/api/resources/event?view=graph-rest-1.0)
- [<span data-ttu-id="9c2e0-131">eventMessage</span><span class="sxs-lookup"><span data-stu-id="9c2e0-131">eventMessage</span></span>](/graph/api/resources/eventmessage?view=graph-rest-1.0)
- [<span data-ttu-id="9c2e0-132">邮件</span><span class="sxs-lookup"><span data-stu-id="9c2e0-132">message</span></span>](/graph/api/resources/message?view=graph-rest-1.0)
- [<span data-ttu-id="9c2e0-133">outlookTask</span><span class="sxs-lookup"><span data-stu-id="9c2e0-133">outlookTask</span></span>](/graph/api/resources/outlooktask?view=graph-rest-1.0)

### <a name="mail"></a><span data-ttu-id="9c2e0-134">邮件</span><span class="sxs-lookup"><span data-stu-id="9c2e0-134">Mail</span></span>
<span data-ttu-id="9c2e0-135">[获取邮件的 MIME 内容](outlook-get-mime-message.md)。</span><span class="sxs-lookup"><span data-stu-id="9c2e0-135">[Get the MIME content of a message](outlook-get-mime-message.md).</span></span>

### <a name="microsoft-graph-toolkit"></a><span data-ttu-id="9c2e0-136">Microsoft Graph 工具包</span><span class="sxs-lookup"><span data-stu-id="9c2e0-136">Microsoft Graph Toolkit</span></span>
<span data-ttu-id="9c2e0-137">使用 [Microsoft Graph 工具包](toolkit/overview.md)开发生产应用，该应用提供一致的 Microsoft 365 外观，可以节省从 Microsoft Graph 进行身份验证和访问数据的时间。</span><span class="sxs-lookup"><span data-stu-id="9c2e0-137">Use the [Microsoft Graph Toolkit](toolkit/overview.md) to develop production apps that offer a consistent Microsoft 365 look-and-feel, and save time in authenticating and accessing data from Microsoft Graph.</span></span>

## <a name="september-2019-new-in-preview"></a><span data-ttu-id="9c2e0-138">2019 年 9 月：预览版中的新增功能</span><span class="sxs-lookup"><span data-stu-id="9c2e0-138">September 2019: New in preview</span></span>

> [!IMPORTANT]
> <span data-ttu-id="9c2e0-139">_预览_状态下的功能（包括 API 和工具）可能会发生更改，恕不另行通知，有些功能可能永远不会提升为 GA 状态。</span><span class="sxs-lookup"><span data-stu-id="9c2e0-139">Features, including APIs and tools, in _preview_ status may change without notice, and some may never be promoted to GA status.</span></span> <span data-ttu-id="9c2e0-140">请不要在成品应用中使用它们。</span><span class="sxs-lookup"><span data-stu-id="9c2e0-140">Do not use them in production apps.</span></span>

### <a name="devices-and-apps"></a><span data-ttu-id="9c2e0-141">设备和应用</span><span class="sxs-lookup"><span data-stu-id="9c2e0-141">Devices and apps</span></span>
<span data-ttu-id="9c2e0-142">Intune [9 月](changelog.md#september-2019)更新</span><span class="sxs-lookup"><span data-stu-id="9c2e0-142">Intune [September](changelog.md#september-2019) updates</span></span>

### <a name="files"></a><span data-ttu-id="9c2e0-143">文件</span><span class="sxs-lookup"><span data-stu-id="9c2e0-143">Files</span></span>
- <span data-ttu-id="9c2e0-144">增强的同步支持：</span><span class="sxs-lookup"><span data-stu-id="9c2e0-144">Enhanced synchronization support:</span></span>

  - <span data-ttu-id="9c2e0-145">使用新的 **pendingOperations** 属性标识可能影响 [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) 的二进制内容的操作。</span><span class="sxs-lookup"><span data-stu-id="9c2e0-145">Use the new **pendingOperations** property to identify operations that may affect the binary content of a [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta).</span></span>
  - <span data-ttu-id="9c2e0-146">[还原](/graph/api/driveitem-restore?view=graph-rest-beta)已删除的 **driveItem**。</span><span class="sxs-lookup"><span data-stu-id="9c2e0-146">Restore a deleted mailbox</span></span> 
- <span data-ttu-id="9c2e0-147">使用安全哈希算法 (SHA-256) 增强[文件](/graph/api/resources/file?view=graph-rest-beta)数据安全性和完整性。</span><span class="sxs-lookup"><span data-stu-id="9c2e0-147">Use Secure Hash Algorithm (SHA-256) to enhance [file](/graph/api/resources/file?view=graph-rest-beta) data security and integrity.</span></span>
- <span data-ttu-id="9c2e0-148">获取或设置[照片](/graph/api/resources/photo?view=graph-rest-beta)的方向。</span><span class="sxs-lookup"><span data-stu-id="9c2e0-148">Get or set the orientation of a [photo](/graph/api/resources/photo?view=graph-rest-beta).</span></span> <span data-ttu-id="9c2e0-149">OneDrive 个人版上支持设置。</span><span class="sxs-lookup"><span data-stu-id="9c2e0-149">Setting is supported on OneDrive Personal.</span></span>

### <a name="identity-and-access"></a><span data-ttu-id="9c2e0-150">标识和访问</span><span class="sxs-lookup"><span data-stu-id="9c2e0-150">Identity and access</span></span>
- <span data-ttu-id="9c2e0-151">使用新的 **identities** 属性并获取[用户](/graph/api/resources/user?view=graph-rest-beta)可用于登录帐户的标识。</span><span class="sxs-lookup"><span data-stu-id="9c2e0-151">Use the new **identities** property and get the identities that a [user](/graph/api/resources/user?view=graph-rest-beta) can use to sign in to an account.</span></span> <span data-ttu-id="9c2e0-152">这些标识可由组织或诸如 Facebook、Google 和 Microsoft 等社交标识提供者提供。</span><span class="sxs-lookup"><span data-stu-id="9c2e0-152">These identities can be provided by business organizations, or by social identity providers such as Facebook, Google, and Microsoft.</span></span>
- <span data-ttu-id="9c2e0-153">用于在租户的云应用程序中[同步标识](/graph/api/resources/synchronization-overview?view=graph-rest-beta)的增强功能：</span><span class="sxs-lookup"><span data-stu-id="9c2e0-153">Incremental enhancements for [synchronizing identities](/graph/api/resources/synchronization-overview?view=graph-rest-beta) in a cloud application for a tenant:</span></span>

  - <span data-ttu-id="9c2e0-154">存储[同步作业](/graph/api/resources/synchronization-synchronizationjob?view=graph-rest-beta)的设置</span><span class="sxs-lookup"><span data-stu-id="9c2e0-154">To store settings for a [synchronization job](/graph/api/resources/synchronization-synchronizationjob?view=graph-rest-beta)</span></span>
  - <span data-ttu-id="9c2e0-155">指定对同步作业施加[隔离](/graph/api/resources/synchronization-quarantine?view=graph-rest-beta)的原因</span><span class="sxs-lookup"><span data-stu-id="9c2e0-155">To specify a reason to impose [quarantine](/graph/api/resources/synchronization-quarantine?view=graph-rest-beta) on a synchronization job</span></span>

### <a name="teamwork"></a><span data-ttu-id="9c2e0-156">团队合作</span><span class="sxs-lookup"><span data-stu-id="9c2e0-156">Teamwork</span></span>
<span data-ttu-id="9c2e0-157">使用[团队](/graph/api/resources/team?view=graph-rest-beta)的**常规**频道或自定义[成员设置](/graph/api/resources/teammembersettings?view=graph-rest-beta)，让团队成员在**团队**中创建专用频道。</span><span class="sxs-lookup"><span data-stu-id="9c2e0-157">Programmatic support for the **General** channel of a [team](/graph/api/resources/team?view=graph-rest-beta), and for customizing [member settings](/graph/api/resources/teammembersettings?view=graph-rest-beta) to let team members create private channels in the **team**.</span></span>

### <a name="users"></a><span data-ttu-id="9c2e0-158">用户</span><span class="sxs-lookup"><span data-stu-id="9c2e0-158">Users</span></span>
- <span data-ttu-id="9c2e0-159">获取或更新[用户](/graph/api/resources/user?view=graph-rest-beta)用于登录帐户的标识。</span><span class="sxs-lookup"><span data-stu-id="9c2e0-159">Get or update the identities with which a [user](/graph/api/resources/user?view=graph-rest-beta) can sign in to an account.</span></span> <span data-ttu-id="9c2e0-160">这些标识可由商业组织或诸如 Facebook、Google 和 Microsoft 等社交标识提供者提供。</span><span class="sxs-lookup"><span data-stu-id="9c2e0-160">These identities can be provided by business organizations, or by social identity providers such as Facebook, Google, and Microsoft.</span></span>
- <span data-ttu-id="9c2e0-161">获取或更新用户的[邮箱首选日期和时间格式设置](/graph/api/resources/mailboxsettings?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="9c2e0-161">Get or update a user's preferred date and time format [settings for the mailbox](/graph/api/resources/mailboxsettings?view=graph-rest-beta).</span></span>


## <a name="want-to-stay-in-the-loop"></a><span data-ttu-id="9c2e0-162">保持循环</span><span class="sxs-lookup"><span data-stu-id="9c2e0-162">Want to stay in the loop?</span></span>
- <span data-ttu-id="9c2e0-163">是否有希望 Microsoft Graph 支持的方案？</span><span class="sxs-lookup"><span data-stu-id="9c2e0-163">Are there scenarios you'd like Microsoft Graph to support?</span></span> <span data-ttu-id="9c2e0-164">在 [Microsoft Graph 用户心声](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)中建议新功能并进行投票。</span><span class="sxs-lookup"><span data-stu-id="9c2e0-164">Suggest and vote for new features at [Microsoft Graph User Voice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).</span></span>
- <span data-ttu-id="9c2e0-165">成为 Microsoft Graph 社区中的活跃成员!</span><span class="sxs-lookup"><span data-stu-id="9c2e0-165">Be an active member in the Microsoft Graph community!</span></span> <span data-ttu-id="9c2e0-166">[参与](https://aka.ms/microsoftgraphcall)Microsoft Graph 社区每月通话。</span><span class="sxs-lookup"><span data-stu-id="9c2e0-166">[Join](https://aka.ms/microsoftgraphcall) the monthly Microsoft Graph community call.</span></span>
- <span data-ttu-id="9c2e0-167">注册 [office 365 开发人员计划](https://developer.microsoft.com/zh-CN/office/dev-program)，免费订阅 Office 365, 然后开始开发! </span><span class="sxs-lookup"><span data-stu-id="9c2e0-167">Sign up for the [Office 365 developer program](https://developer.microsoft.com/zh-CN/office/dev-program), get a free Office 365 subscription, and start developing!</span></span>


## <a name="see-also"></a><span data-ttu-id="9c2e0-168">另请参阅</span><span class="sxs-lookup"><span data-stu-id="9c2e0-168">See also</span></span>
- <span data-ttu-id="9c2e0-169">定期查看 [Microsoft Graph 开发人员博客](https://developer.microsoft.com/zh-CN/graph/blogs/), 了解发布公告和有帮助的资源。 </span><span class="sxs-lookup"><span data-stu-id="9c2e0-169">Check out the [Microsoft Graph developer blog](https://developer.microsoft.com/zh-CN/graph/blogs/) periodically for release announcements and helpful resources.</span></span>
- <span data-ttu-id="9c2e0-170">浏览 Microsoft Graph API 新增功能的详细信息, 以及[changelog](changelog.md)中的 API 行为更新。</span><span class="sxs-lookup"><span data-stu-id="9c2e0-170">Browse details of Microsoft Graph API additions, and API behavior updates in the [changelog](changelog.md).</span></span>
- <span data-ttu-id="9c2e0-171">查找[早期版本的重点内容](whats-new-earlier.md)。</span><span class="sxs-lookup"><span data-stu-id="9c2e0-171">Find [highlights of earlier releases](whats-new-earlier.md).</span></span>
- <span data-ttu-id="9c2e0-172">了解有关 [Microsoft Graph 的版本控制、支持和中断性变更策略](versioning-and-support.md)。</span><span class="sxs-lookup"><span data-stu-id="9c2e0-172">Learn more about [versioning, support, and breaking change policies for Microsoft Graph](versioning-and-support.md).</span></span>

