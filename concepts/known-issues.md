---
title: Microsoft Graph 已知问题
description: 本文介绍了 Microsoft Graph 已知问题。若要了解最新更新，请参阅 Microsoft Graph 更改日志。
author: jthake-msft
localization_priority: Priority
ms.openlocfilehash: 351b02e3d423458fba8dbaec2050530ccaba4df0
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576785"
---
# <a name="known-issues-with-microsoft-graph"></a><span data-ttu-id="8415d-104">Microsoft Graph 已知问题</span><span class="sxs-lookup"><span data-stu-id="8415d-104">Known issues with Microsoft Graph</span></span>

<span data-ttu-id="8415d-p102">本文介绍了 Microsoft Graph 已知问题。若要了解最新更新，请参阅 [Microsoft Graph 更改日志](changelog.md)。</span><span class="sxs-lookup"><span data-stu-id="8415d-p102">This article describes known issues with Microsoft Graph. For information about the latest updates, see the [Microsoft Graph changelog](changelog.md).</span></span>

## <a name="users"></a><span data-ttu-id="8415d-107">用户</span><span class="sxs-lookup"><span data-stu-id="8415d-107">Users</span></span>

### <a name="no-instant-access-after-creation"></a><span data-ttu-id="8415d-108">创建后无法即时访问</span><span class="sxs-lookup"><span data-stu-id="8415d-108">No instant access after creation</span></span>

<span data-ttu-id="8415d-p103">可通过在用户实体上使用 POST 来即时创建用户。必须先向用户分配 Office 365 许可证，然后用户才能访问 Office 365 服务。尽管如此，由于服务具有分散特性，因此用户可能需要先等待 15 分钟，然后才能通过 Microsoft Graph API 使用文件、邮件和事件实体。在此期间，应用会收到一个 404 HTTP 错误响应。</span><span class="sxs-lookup"><span data-stu-id="8415d-p103">Users can be created immediately through a POST on the user entity. An Office 365 license must first be assigned to a user, in order to get access to Office 365 services. Even then, due to the distributed nature of the service, it might take 15 minutes before files, messages and events entities are available for use for this user, through the Microsoft Graph API. During this time, apps will receive a 404 HTTP error response.</span></span>

### <a name="photo-restrictions"></a><span data-ttu-id="8415d-113">照片限制</span><span class="sxs-lookup"><span data-stu-id="8415d-113">Photo restrictions</span></span>

<span data-ttu-id="8415d-p104">只有当用户有邮箱时，才能读取和更新用户的个人资料照片。另外，之前*可能*使用 **thumbnailPhoto** 属性（使用 Office 365 统一 API 预览或 Azure AD Graph，或通过 AD Connect 同步）存储的所有照片无法再通过[用户](/graph/api/resources/user?view=graph-rest-1.0)资源的 Microsoft Graph **照片**属性进行访问。在这种情况下，无法读取或更新照片会生成以下错误：</span><span class="sxs-lookup"><span data-stu-id="8415d-p104">Reading and updating a user's profile photo is only possible if the user has a mailbox. Additionally, any photos that *may* have been previously stored using the **thumbnailPhoto** property (using the Office 365 unified API preview, or the Azure AD Graph, or through AD Connect synchronization) are no longer accessible through the Microsoft Graph **photo** property of the [user](/graph/api/resources/user?view=graph-rest-1.0) resource. Failure to read or update a photo, in this case, would result in the following error:</span></span>

```javascript
    {
      "error": {
        "code": "ErrorNonExistentMailbox",
        "message": "The SMTP address has no mailbox associated with it."
      }
    }
```

### <a name="using-delta-query"></a><span data-ttu-id="8415d-117">使用 delta 查询</span><span class="sxs-lookup"><span data-stu-id="8415d-117">Using delta query</span></span>

<span data-ttu-id="8415d-118">有关使用 delta 查询方面的已知问题，请参阅本文中的[“delta 查询”部分](#delta-query)。</span><span class="sxs-lookup"><span data-stu-id="8415d-118">For known issues using delta query, see the [delta query section](#delta-query) in this article.</span></span>

## <a name="microsoft-teams"></a><span data-ttu-id="8415d-119">Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="8415d-119">Microsoft Teams</span></span>

### <a name="create-chat-thread-api"></a><span data-ttu-id="8415d-120">创建聊天线程 API</span><span class="sxs-lookup"><span data-stu-id="8415d-120">Create chat thread API</span></span>

<span data-ttu-id="8415d-121">当前用于[创建聊天线程](/graph/api/channel-post-chatthreads?view=graph-rest-beta)的 API 将被替换为，与用于[列出频道消息](/graph/api/channel-list-messages?view=graph-rest-beta)的架构一致的更丰富 API。</span><span class="sxs-lookup"><span data-stu-id="8415d-121">The current API to [create a chat thread](/graph/api/channel-post-chatthreads?view=graph-rest-beta) will be replaced with a richer API that is consistent with the schema for [listing channel messages](/graph/api/channel-list-messages?view=graph-rest-beta).</span></span>

### <a name="graph-explorer-and-global-admins"></a><span data-ttu-id="8415d-122">Graph 浏览器和全局管理员</span><span class="sxs-lookup"><span data-stu-id="8415d-122">Graph Explorer and global admins</span></span>

<span data-ttu-id="8415d-123">目前，Graph 浏览器允许全局管理员管理他们不拥有或不所属的团队；但如果当前用户不是团队的成员或所有者，其他应用便无法尝试执行相同的 API 调用。</span><span class="sxs-lookup"><span data-stu-id="8415d-123">Currently, Graph Explorer allows global admins to manipulate teams they are not an owner or member of, but other apps attempting to make the same API calls will fail if the current user is not a member or owner of the team.</span></span>

### <a name="get-teams-and-post-teams-are-not-supported"></a><span data-ttu-id="8415d-124">不支持 GET /teams 和 POST /teams</span><span class="sxs-lookup"><span data-stu-id="8415d-124">GET /teams and POST /teams are not supported</span></span>

<span data-ttu-id="8415d-125">若要获取团队列表，请参阅[列出所有团队](teams-list-all-teams.md)和[列出团队](/graph/api/user-list-joinedteams?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="8415d-125">See [list all teams](teams-list-all-teams.md) and [list your teams](/graph/api/user-list-joinedteams?view=graph-rest-1.0) to get a list of teams.</span></span>
<span data-ttu-id="8415d-126">若要创建团队，请参阅[创建团队](/graph/api/team-put-teams?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="8415d-126">See [create team](/graph/api/team-put-teams?view=graph-rest-1.0) for creating teams.</span></span>

### <a name="missing-teams-in-list-all-teams"></a><span data-ttu-id="8415d-127">“列出所有团队”没有列出的团队</span><span class="sxs-lookup"><span data-stu-id="8415d-127">Missing teams in list all teams</span></span>

<span data-ttu-id="8415d-128">[列出所有团队](teams-list-all-teams.md)没有列出过去创建但 Microsoft Teams 用户最近未使用的一些团队。</span><span class="sxs-lookup"><span data-stu-id="8415d-128">Some teams that were created in the past but haven't been used recently by a Microsoft Teams user aren't listed by [list all teams](teams-list-all-teams.md).</span></span>
<span data-ttu-id="8415d-129">新团队会被列出。</span><span class="sxs-lookup"><span data-stu-id="8415d-129">New teams will be listed.</span></span>
<span data-ttu-id="8415d-130">一些旧团队没有包含“Team”的 **resourceProvisioningOptions** 属性，但新创建的团队和在 Microsoft Teams 中被访问的团队有此属性。</span><span class="sxs-lookup"><span data-stu-id="8415d-130">Certain old teams don't have a **resourceProvisioningOptions** property that contains "Team", which is set on newly created teams and teams that are visited in Microsoft Teams.</span></span>
<span data-ttu-id="8415d-131">今后，我们将对尚未在 Microsoft Teams 中打开的现有团队设置 **resourceProvisioningOptions**。</span><span class="sxs-lookup"><span data-stu-id="8415d-131">In the future, we will set **resourceProvisioningOptions** on existing teams that have not been opened in Microsoft Teams.</span></span>

## <a name="groups"></a><span data-ttu-id="8415d-132">组</span><span class="sxs-lookup"><span data-stu-id="8415d-132">Groups</span></span>

### <a name="permissions-for-groups-and-microsoft-teams"></a><span data-ttu-id="8415d-133">组和 Microsoft Teams 的权限</span><span class="sxs-lookup"><span data-stu-id="8415d-133">Permissions for groups and Microsoft Teams</span></span>

<span data-ttu-id="8415d-134">Microsoft Graph 为组和 Microsoft Teams 公开了两个用于访问 API 的权限（[*Group.Read.All*](permissions-reference.md#group-permissions) 和 [*Group.ReadWrite.All*](permissions-reference.md#group-permissions)）。</span><span class="sxs-lookup"><span data-stu-id="8415d-134">Microsoft Graph exposes two permissions ([*Group.Read.All*](permissions-reference.md#group-permissions) and [*Group.ReadWrite.All*](permissions-reference.md#group-permissions)) for access to the APIs for groups and Microsoft Teams.</span></span>
<span data-ttu-id="8415d-135">管理员必须同意授予这些权限。</span><span class="sxs-lookup"><span data-stu-id="8415d-135">These permissions must be consented to by an administrator.</span></span>
<span data-ttu-id="8415d-136">今后，我们计划新增用户可同意授予的组和团队权限。</span><span class="sxs-lookup"><span data-stu-id="8415d-136">In the future, we plan to add new permissions for groups and teams that users can consent to.</span></span>

<span data-ttu-id="8415d-p108">此外，只有与核心组管理和管理相关的 API 才支持使用委派权限或仅限应用权限进行访问。其他所有的组 API 功能仅支持委派权限。</span><span class="sxs-lookup"><span data-stu-id="8415d-p108">Also, only the API for core group administration and management supports access using delegated or app-only permissions. All other features of the group API support only delegated permissions.</span></span>

<span data-ttu-id="8415d-139">同时支持委派权限和仅限应用权限的组功能示例：</span><span class="sxs-lookup"><span data-stu-id="8415d-139">Examples of group features that support delegated and app-only permissions:</span></span>

* <span data-ttu-id="8415d-140">创建和删除组</span><span class="sxs-lookup"><span data-stu-id="8415d-140">Creating and deleting groups</span></span>
* <span data-ttu-id="8415d-141">获取和更新与组管理或管理相关的组属性</span><span class="sxs-lookup"><span data-stu-id="8415d-141">Getting and updating group properties pertaining to group administration or management</span></span>
* <span data-ttu-id="8415d-142">组[目录设置](/graph/api/resources/directoryobject?view=graph-rest-1.0)、类型和同步</span><span class="sxs-lookup"><span data-stu-id="8415d-142">Group [directory settings](/graph/api/resources/directoryobject?view=graph-rest-1.0), type, and synchronization</span></span>
* <span data-ttu-id="8415d-143">组所有者和成员</span><span class="sxs-lookup"><span data-stu-id="8415d-143">Group owners and membership</span></span>

<span data-ttu-id="8415d-144">仅支持委派权限的组功能示例：</span><span class="sxs-lookup"><span data-stu-id="8415d-144">Examples of group features that support only delegated permissions:</span></span>

* <span data-ttu-id="8415d-145">组对话、事件和照片</span><span class="sxs-lookup"><span data-stu-id="8415d-145">Group conversations, events, photo</span></span>
* <span data-ttu-id="8415d-146">外部发件人、被接受或拒绝的发件人、组订阅</span><span class="sxs-lookup"><span data-stu-id="8415d-146">External senders, accepted or rejected senders, group subscription</span></span>
* <span data-ttu-id="8415d-147">用户收藏夹和未看计数</span><span class="sxs-lookup"><span data-stu-id="8415d-147">User favorites and unseen count</span></span>

### <a name="policy"></a><span data-ttu-id="8415d-148">策略</span><span class="sxs-lookup"><span data-stu-id="8415d-148">Policy</span></span>

<span data-ttu-id="8415d-149">使用 Microsoft Graph 创建并命名 Office 365 组会忽略通过 Outlook Web App 配置的所有 Office 365 组策略。</span><span class="sxs-lookup"><span data-stu-id="8415d-149">Using Microsoft Graph to create and name an Office 365 group bypasses any Office 365 group policies that are configured through Outlook Web App.</span></span>

### <a name="adding-and-getting-attachments-of-group-posts"></a><span data-ttu-id="8415d-150">添加和获取组帖子的附件</span><span class="sxs-lookup"><span data-stu-id="8415d-150">Adding and getting attachments of group posts</span></span>

<span data-ttu-id="8415d-p109">向组帖子 [添加](/graph/api/post-post-attachments?view=graph-rest-1.0) 附件、[列出](/graph/api/post-list-attachments?view=graph-rest-1.0) 和获取组帖子的附件目前返回错误消息“OData 请求不受支持”。已经为 `/v1.0` 和 `/beta` 版本推出修复程序，并预计到 2016 年 1 月底会广泛推出。</span><span class="sxs-lookup"><span data-stu-id="8415d-p109">[Adding](/graph/api/post-post-attachments?view=graph-rest-1.0) attachments to group posts, [listing](/graph/api/post-list-attachments?view=graph-rest-1.0) and getting attachments of group posts currently return the error message "The OData request is not supported." A fix has been rolled out for both the `/v1.0` and `/beta` versions, and is expected to be widely available by the end of January 2016.</span></span>

### <a name="setting-the-allowexternalsenders-property"></a><span data-ttu-id="8415d-153">设置 allowExternalSenders 属性</span><span class="sxs-lookup"><span data-stu-id="8415d-153">Setting the allowExternalSenders property</span></span>

<span data-ttu-id="8415d-154">目前，`/v1.0` 和 `/beta` 中均存在一个问题，即会阻止在 POST 或 PATCH 操作中设置组的属性 **allowExternalSenders**。</span><span class="sxs-lookup"><span data-stu-id="8415d-154">There is currently an issue that prevents setting the **allowExternalSenders** property of a group in a POST or PATCH operation, in both `/v1.0` and `/beta`.</span></span>

### <a name="using-delta-query"></a><span data-ttu-id="8415d-155">使用 delta 查询</span><span class="sxs-lookup"><span data-stu-id="8415d-155">Using delta query</span></span>

<span data-ttu-id="8415d-156">有关使用 delta 查询的已知问题，请参阅本文中的 [delta 查询部分](#delta-query)。</span><span class="sxs-lookup"><span data-stu-id="8415d-156">For known issues using delta query, see the [delta query section](#delta-query) in this article.</span></span>

## <a name="bookings"></a><span data-ttu-id="8415d-157">预订</span><span class="sxs-lookup"><span data-stu-id="8415d-157">Bookings</span></span>

### <a name="errorexceededfindcountlimit-when-querying-bookingbusinesses"></a><span data-ttu-id="8415d-158">查询 bookingBusinesses 时出现 ErrorExceededFindCountLimit</span><span class="sxs-lookup"><span data-stu-id="8415d-158">ErrorExceededFindCountLimit when querying bookingBusinesses</span></span>

<span data-ttu-id="8415d-159">当组织拥有多个预订业务且提出请求的帐户不是管理员时，获取 `bookingBusinesses` 列表会失败，并显示以下错误代码：</span><span class="sxs-lookup"><span data-stu-id="8415d-159">Getting the list of `bookingBusinesses` fails with the following error code when an organization has several Bookings businesses and the account making the request is not an administrator:</span></span>

```json
{
  "error": {
    "code": "ErrorExceededFindCountLimit",
    "message":
      "The GetBookingMailboxes request returned too many results. Please specify a query to limit the results.",
  }
}
```

<span data-ttu-id="8415d-160">解决方法是，可以通过加入 `query` 参数来限制请求返回的业务集，例如：</span><span class="sxs-lookup"><span data-stu-id="8415d-160">As a workaround, you can limit the set of businesses returned by the request by including a `query` parameter, for example:</span></span>

```
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Fabrikam
```


## <a name="calendars"></a><span data-ttu-id="8415d-161">日历</span><span class="sxs-lookup"><span data-stu-id="8415d-161">Calendars</span></span>

### <a name="accessing-a-shared-calendar"></a><span data-ttu-id="8415d-162">访问共享日历</span><span class="sxs-lookup"><span data-stu-id="8415d-162">Accessing a shared calendar</span></span>

<span data-ttu-id="8415d-163">使用以下操作尝试访问其他用户共享的日历中的事件时：</span><span class="sxs-lookup"><span data-stu-id="8415d-163">When attempting to access events in a calendar that has been shared by another user using the following operation:</span></span>

```http
GET \users('{id}')\calendars('{id}')\events
```

<span data-ttu-id="8415d-p110">可能会看到错误代码为 `ErrorInternalServerTransientError` 的 HTTP 500。导致错误发生的原因是：</span><span class="sxs-lookup"><span data-stu-id="8415d-p110">You may get HTTP 500 with the error code `ErrorInternalServerTransientError`. The error occurs because:</span></span>

- <span data-ttu-id="8415d-166">过去，日历共享的实现方法有两种。为了加以区分，将它们称为“旧”方法和“新”方法。</span><span class="sxs-lookup"><span data-stu-id="8415d-166">Historically, there are two ways that calendar sharing has been implemented, which, for the purpose of differentiating them, are referred to as the "old" approach and "new" approach.</span></span>
- <span data-ttu-id="8415d-167">新方法当前可用于通过查看或编辑权限共享日历，但无法通过委派权限进行共享。</span><span class="sxs-lookup"><span data-stu-id="8415d-167">The new approach is currently available for sharing calendars with view or edit permissions, but not with delegate permissions.</span></span>
- <span data-ttu-id="8415d-168">只有使用**新**方法共享日历后，才能使用日历 REST API 查看或编辑共享日历。</span><span class="sxs-lookup"><span data-stu-id="8415d-168">You can use the calendar REST API to view or edit shared calendars only if the calendars were shared using the **new** approach.</span></span>
- <span data-ttu-id="8415d-169">如果使用**旧**方法共享日历，则无法使用日历 REST API 查看或编辑此类日历（或其事件）。</span><span class="sxs-lookup"><span data-stu-id="8415d-169">You cannot use the calendar REST API to view or edit such calendars (or their events) if the calendars were shared using the **old** approach.</span></span>


<span data-ttu-id="8415d-170">如果日历是通过查看或编辑权限共享，但使用的是旧方法，现在可以修复错误，手动将日历共享升级为使用新方法。</span><span class="sxs-lookup"><span data-stu-id="8415d-170">If a calendar was shared with view or edit permissions but using the old approach, you can now work around the error and manually upgrade the calendar sharing to use the new approach.</span></span>
<span data-ttu-id="8415d-171">随着时间的推移，Outlook 将把所有共享日历（包括通过委托权限共享的日历）自动升级为使用新方法。</span><span class="sxs-lookup"><span data-stu-id="8415d-171">Over time, Outlook will automatically upgrade all shared calendars to use the new approach, including calendars shared with delegate permissions.</span></span>

<span data-ttu-id="8415d-172">若要手动将共享日历升级为使用新方法，请按照以下步骤操作：</span><span class="sxs-lookup"><span data-stu-id="8415d-172">To manually upgrade a shared calendar to use the new approach, follow these steps:</span></span>
1.  <span data-ttu-id="8415d-173">收件人删除以前与他们共享的日历。</span><span class="sxs-lookup"><span data-stu-id="8415d-173">The recipient removes the calendar that was previously shared to them.</span></span>
2.  <span data-ttu-id="8415d-174">日历所有者在 Outlook 网页版、iOS 版或 Android 版中重新共享日历。</span><span class="sxs-lookup"><span data-stu-id="8415d-174">The calendar owner re-shares the calendar in Outlook on the web, Outlook on iOS, or Outlook on Android.</span></span>
3.  <span data-ttu-id="8415d-p112">收件人使用 Outlook 网页版重新接受共享日历。（很快就可以使用其他 Outlook 客户端了。）</span><span class="sxs-lookup"><span data-stu-id="8415d-p112">The recipient re-accepts the shared calendar using Outlook on the web. (It will be possible to use other Outlook clients soon.)</span></span>
4.  <span data-ttu-id="8415d-177">收件人可以在 Outlook iOS 版或 Android 版中查看共享日历，从而验证是否已成功使用新方法重新共享日历。</span><span class="sxs-lookup"><span data-stu-id="8415d-177">The recipient verifies that the calendar has been re-shared successfully using the new approach by being able to view the shared calendar in Outlook on iOS or Outlook on Android.</span></span>

<span data-ttu-id="8415d-p113">使用新方法共享的日历看起来与邮箱中的其他日历一样。可以使用日历 REST API 查看或编辑共享日历中的事件，就像查看或编辑自己日历中的事件一样。示例：</span><span class="sxs-lookup"><span data-stu-id="8415d-p113">A calendar shared with you in the new approach appears as just another calendar in your mailbox. You can use the calendar REST API to view or edit events in the shared calendar, as if it's your own calendar. As an example:</span></span>

```http
GET \me\calendars('{id}')\events
```

### <a name="adding-and-accessing-ics-based-calendars-in-users-mailbox"></a><span data-ttu-id="8415d-181">在用户邮箱中添加和访问基于 ICS 的日历</span><span class="sxs-lookup"><span data-stu-id="8415d-181">Adding and accessing ICS-based calendars in user's mailbox</span></span>

<span data-ttu-id="8415d-182">目前，还有部分支持基于 Internet 日历订阅 (ICS) 的日历：</span><span class="sxs-lookup"><span data-stu-id="8415d-182">Currently, there is partial support for a calendar based on an Internet Calendar Subscription (ICS):</span></span>

* <span data-ttu-id="8415d-183">你可以通过用户界面，而不是通过 Microsoft Graph API 为用户邮箱添加基于 ICS 的日历。</span><span class="sxs-lookup"><span data-stu-id="8415d-183">You can add an ICS-based calendar to a user mailbox through the user interface, but not through the Microsoft Graph API.</span></span>
* <span data-ttu-id="8415d-p114">[列出用户的日历](/graph/api/user-list-calendars?view=graph-rest-1.0)允许你获取用户默认日历组中或指定日历组中的每个 [日历](/graph/api/resources/calendar?view=graph-rest-1.0)的**名称**、**颜色**和 **id** 属性，包括所有基于 ICS 的日历。你无法存储或访问日历资源中的 ICS URL。</span><span class="sxs-lookup"><span data-stu-id="8415d-p114">[Listing the user's calendars](/graph/api/user-list-calendars?view=graph-rest-1.0) lets you get the **name**, **color** and **id** properties of each [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) in the user's default calendar group, or a specified calendar group, including any ICS-based calendars. You cannot store or access the ICS URL in the calendar resource.</span></span>
* <span data-ttu-id="8415d-186">还可以[列出基于 ICS 的日历事件](/graph/api/calendar-list-events?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="8415d-186">You can also [list the events](/graph/api/calendar-list-events?view=graph-rest-1.0) of an ICS-based calendar.</span></span>

### <a name="onlinemeetingurl-property-support-for-microsoft-teams"></a><span data-ttu-id="8415d-187">Microsoft Teams 的 onlineMeetingUrl 属性支持</span><span class="sxs-lookup"><span data-stu-id="8415d-187">onlineMeetingUrl property support for Microsoft Teams</span></span>

<span data-ttu-id="8415d-188">目前，Skype 会议[事件](/graph/api/resources/event?view=graph-rest-1.0)的 **onlineMeetingUrl** 属性指明联机会议 URL。</span><span class="sxs-lookup"><span data-stu-id="8415d-188">Currently, the **onlineMeetingUrl** property of a Skype meeting [event](/graph/api/resources/event?view=graph-rest-1.0) would indicate the online meeting URL.</span></span> <span data-ttu-id="8415d-189">不过，对于 Microsoft Teams 会议事件，此属性设置为 NULL。</span><span class="sxs-lookup"><span data-stu-id="8415d-189">However, that property for a Microsoft Teams meeting event is set to null.</span></span>

## <a name="calls-and-online-meetings"></a><span data-ttu-id="8415d-190">呼叫和联机会议</span><span class="sxs-lookup"><span data-stu-id="8415d-190">Calls and online meetings</span></span>

> <span data-ttu-id="8415d-191">**注意**：呼叫和联机会议暂处于预览阶段，仅适用于 Microsoft Graph beta 终结点。</span><span class="sxs-lookup"><span data-stu-id="8415d-191">**Note** Calling and online meetings are currently in preview and are available only in the Microsoft Graph beta endpoint.</span></span>

- <span data-ttu-id="8415d-192">导航路径 `/applications/{id}` 不受支持。</span><span class="sxs-lookup"><span data-stu-id="8415d-192">Navigation path `/applications/{id}` is not supported.</span></span> <span data-ttu-id="8415d-193">禁止通过全局应用节点转到应用，即使是你自己的应用，也不例外。</span><span class="sxs-lookup"><span data-stu-id="8415d-193">Navigating through the global applications node to the application, even your own, is not allowed.</span></span> <span data-ttu-id="8415d-194">请仅使用 `/app` 导航。</span><span class="sxs-lookup"><span data-stu-id="8415d-194">Please use the `/app` navigation only.</span></span>

## <a name="contacts"></a><span data-ttu-id="8415d-195">联系人</span><span class="sxs-lookup"><span data-stu-id="8415d-195">Contacts</span></span>

### <a name="organization-contacts-available-in-only-beta"></a><span data-ttu-id="8415d-196">仅 beta 版支持组织联系人。</span><span class="sxs-lookup"><span data-stu-id="8415d-196">Organization contacts available in only beta</span></span>

<span data-ttu-id="8415d-p117">目前只支持个人联系人。`/v1.0` 中目前暂不支持组织联系人，但可以在 `/beta` 中找到组织联系人。</span><span class="sxs-lookup"><span data-stu-id="8415d-p117">Only personal contacts are currently supported. Organizational contacts are not currently supported in `/v1.0`, but can be found in `/beta`.</span></span>

### <a name="default-contacts-folder"></a><span data-ttu-id="8415d-199">默认联系人文件夹</span><span class="sxs-lookup"><span data-stu-id="8415d-199">Default contacts folder</span></span>

<span data-ttu-id="8415d-200">在 `/v1.0` 版本中，`GET /me/contactFolders` 不包括用户的默认联系人文件夹。</span><span class="sxs-lookup"><span data-stu-id="8415d-200">In the `/v1.0` version, `GET /me/contactFolders` does not include the user's default contacts folder.</span></span>

<span data-ttu-id="8415d-p118">将会提供修复程序。同时，您还可以使用以下[列出联系人](/graph/api/user-list-contacts?view=graph-rest-1.0)查询和 **parentFolderId** 属性作为一种解决方法，来获取默认联系人文件夹的文件夹 ID：</span><span class="sxs-lookup"><span data-stu-id="8415d-p118">A fix will be made available. Meanwhile, you can use the following [list contacts](/graph/api/user-list-contacts?view=graph-rest-1.0) query and the **parentFolderId** property as a workaround to get the folder ID of the default contacts folder:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/contacts?$top=1&$select=parentFolderId
```

<span data-ttu-id="8415d-203">在上面的查询中：</span><span class="sxs-lookup"><span data-stu-id="8415d-203">In the above query:</span></span>

1. <span data-ttu-id="8415d-204">`/me/contacts?$top=1` 获取默认联系人文件夹中 [联系人](/graph/api/resources/contact?view=graph-rest-1.0) 的属性。</span><span class="sxs-lookup"><span data-stu-id="8415d-204">`/me/contacts?$top=1` gets the properties of a [contact](/graph/api/resources/contact?view=graph-rest-1.0) in the default contacts folder.</span></span>
2. <span data-ttu-id="8415d-205">附加 `&$select=parentFolderId` 仅返回联系人的 **parentFolderId** 属性，即默认联系人文件夹的 ID。</span><span class="sxs-lookup"><span data-stu-id="8415d-205">Appending `&$select=parentFolderId` returns only the contact's **parentFolderId** property, which is the ID of the default contacts folder.</span></span>


### <a name="accessing-contacts-via-a-contact-folder-in-beta"></a><span data-ttu-id="8415d-206">在 beta 版中通过联系人文件夹访问联系人</span><span class="sxs-lookup"><span data-stu-id="8415d-206">Accessing contacts via a contact folder in beta</span></span>

<span data-ttu-id="8415d-207">目前，`/beta` 版中存在一个问题，即会在 REST 请求 URL 中指定父文件夹，进而阻止访问[联系人](/graph/api/resources/contact?view=graph-rest-beta)，如以下 2 个方案所示。</span><span class="sxs-lookup"><span data-stu-id="8415d-207">In the `/beta` version, there is currently an issue that prevents accessing a [contact](/graph/api/resources/contact?view=graph-rest-beta) by specifying its parent folder in the REST request URL, as shown in the 2 scenarios below.</span></span>

* <span data-ttu-id="8415d-208">从用户的顶级 [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-beta) 访问联系人。</span><span class="sxs-lookup"><span data-stu-id="8415d-208">Accessing a contact from a top level [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-beta) of the user's.</span></span>

```http
GET /me/contactfolders/{id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```

* <span data-ttu-id="8415d-p119">访问 **contactFolder** 的子文件夹中的联系人。下面的示例展示了一级嵌套，但可以在子文件夹的子级等对象中访问联系人。</span><span class="sxs-lookup"><span data-stu-id="8415d-p119">Accessing a contact contained in a child folder of a **contactFolder**.  The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>

```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```

<span data-ttu-id="8415d-211">或者，如下所示，只需指定联系人 ID 即可[获取](/graph/api/contact-get?view=graph-rest-beta)此联系人，因为在 `/beta` 版中 GET /contacts 适用于用户邮箱中的所有联系人：</span><span class="sxs-lookup"><span data-stu-id="8415d-211">As an alternative, you can simply [get](/graph/api/contact-get?view=graph-rest-beta) the contact by specifying its ID as shown below, since GET /contacts in the `/beta` version applies to all the contacts in the user's mailbox:</span></span>

```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```

## <a name="messages"></a><span data-ttu-id="8415d-212">邮件</span><span class="sxs-lookup"><span data-stu-id="8415d-212">Messages</span></span>

### <a name="the-comment-parameter-for-creating-a-draft"></a><span data-ttu-id="8415d-213">用于创建草稿的注释参数</span><span class="sxs-lookup"><span data-stu-id="8415d-213">The comment parameter for creating a draft</span></span>

<span data-ttu-id="8415d-214">用于创建答复或转发草稿的**注释**参数（[createReply](/graph/api/message-createreply?view=graph-rest-1.0)、[createReplyAll](/graph/api/message-createreplyall?view=graph-rest-1.0)、[createForward](/graph/api/message-createforward?view=graph-rest-1.0)）不会成为最终的邮件草稿正文的一部分。</span><span class="sxs-lookup"><span data-stu-id="8415d-214">The **comment** parameter for creating a reply or forward draft ([createReply](/graph/api/message-createreply?view=graph-rest-1.0), [createReplyAll](/graph/api/message-createreplyall?view=graph-rest-1.0), [createForward](/graph/api/message-createforward?view=graph-rest-1.0)) does not become part of the body of the resultant message draft.</span></span>

### <a name="get-messages-returns-chats-in-microsoft-teams"></a><span data-ttu-id="8415d-215">GET 消息返回 Microsoft Teams 中的聊天</span><span class="sxs-lookup"><span data-stu-id="8415d-215">GET messages returns chats in Microsoft Teams</span></span>

<span data-ttu-id="8415d-216">在 v1 和 beta 终结点中，`GET /users/id/messages` 的响应包含出现在团队或通道范围外的用户的 Microsoft Teams 聊天。</span><span class="sxs-lookup"><span data-stu-id="8415d-216">In both the v1 and beta endpoints, the response of `GET /users/id/messages` includes the user's Microsoft Teams chats that occurred outside the scope of a team or channel.</span></span> <span data-ttu-id="8415d-217">这些聊天消息具有“即时信息”作为其主题。</span><span class="sxs-lookup"><span data-stu-id="8415d-217">These chat messages have "IM" as their subject.</span></span>


## <a name="drives-files-and-content-streaming"></a><span data-ttu-id="8415d-218">驱动器、文件和内容流式传输</span><span class="sxs-lookup"><span data-stu-id="8415d-218">Drives, files and content streaming</span></span>

* <span data-ttu-id="8415d-219">在通过浏览器访问个人站点之前，用户首次通过 Microsoft Graph 访问个人驱动器会生成 401 响应。</span><span class="sxs-lookup"><span data-stu-id="8415d-219">First time access to a user's personal drive through the Microsoft Graph before the user accesses their personal site through a browser leads to a 401 response.</span></span>

## <a name="query-parameter-limitations"></a><span data-ttu-id="8415d-220">查询参数限制</span><span class="sxs-lookup"><span data-stu-id="8415d-220">Query parameter limitations</span></span>

* <span data-ttu-id="8415d-221">不支持多个命名空间。</span><span class="sxs-lookup"><span data-stu-id="8415d-221">Multiple namespaces are not supported.</span></span>
* <span data-ttu-id="8415d-222">在用户、组、设备、服务主体和应用程序上，不支持对 `$ref` 执行 GET 操作和投影。</span><span class="sxs-lookup"><span data-stu-id="8415d-222">GETs on `$ref` and casting is not supported on users, groups, devices, service principals and applications.</span></span>
* <span data-ttu-id="8415d-p121">不支持 `@odata.bind`。也就是说，开发者无法正确地在组上设置 `Accepted` 或 `RejectedSenders`。</span><span class="sxs-lookup"><span data-stu-id="8415d-p121">`@odata.bind` is not supported.  This means that developers won’t be able to properly set the `Accepted` or `RejectedSenders` on a group.</span></span>
* <span data-ttu-id="8415d-225">使用极少的元数据时，非包容导航（如邮件）上不存在 `@odata.id`。</span><span class="sxs-lookup"><span data-stu-id="8415d-225">`@odata.id` is not present on non-containment navigations (like messages) when using minimal metadata.</span></span>
* <span data-ttu-id="8415d-226">`$expand`:</span><span class="sxs-lookup"><span data-stu-id="8415d-226">`$expand`:</span></span>
  * <span data-ttu-id="8415d-227">不支持 `nextLink`</span><span class="sxs-lookup"><span data-stu-id="8415d-227">No support for `nextLink`</span></span>
  * <span data-ttu-id="8415d-228">不支持 1 级以上扩展</span><span class="sxs-lookup"><span data-stu-id="8415d-228">No support for more than 1 level of expand</span></span>
  * <span data-ttu-id="8415d-229">不支持其他参数（`$filter`、`$select`）</span><span class="sxs-lookup"><span data-stu-id="8415d-229">No support with extra parameters (`$filter`, `$select`)</span></span>
* <span data-ttu-id="8415d-230">`$filter`:</span><span class="sxs-lookup"><span data-stu-id="8415d-230">`$filter`:</span></span>
  * <span data-ttu-id="8415d-231">`/attachments` 终结点不支持筛选器。</span><span class="sxs-lookup"><span data-stu-id="8415d-231">`/attachments` endpoint does not support filters.</span></span> <span data-ttu-id="8415d-232">如果存在，将忽略 `$filter` 参数。</span><span class="sxs-lookup"><span data-stu-id="8415d-232">If present, the `$filter` parameter is ignored.</span></span>
  * <span data-ttu-id="8415d-233">不支持跨工作负载筛选。</span><span class="sxs-lookup"><span data-stu-id="8415d-233">Cross-workload filtering is not supported.</span></span>
* <span data-ttu-id="8415d-234">`$search`:</span><span class="sxs-lookup"><span data-stu-id="8415d-234">`$search`:</span></span>
  * <span data-ttu-id="8415d-235">全文搜索仅对实体子集（如邮件）可用。</span><span class="sxs-lookup"><span data-stu-id="8415d-235">Full-text search is only available for a subset of entities such as messages.</span></span>
  * <span data-ttu-id="8415d-236">不支持跨工作负载搜索。</span><span class="sxs-lookup"><span data-stu-id="8415d-236">Cross-workload searching is not supported.</span></span>

## <a name="delta-query"></a><span data-ttu-id="8415d-237">Delta 查询</span><span class="sxs-lookup"><span data-stu-id="8415d-237">Delta query</span></span>

* <span data-ttu-id="8415d-238">跟踪关系更改时，OData 上下文有时无法正确返回。</span><span class="sxs-lookup"><span data-stu-id="8415d-238">OData context is sometimes returned incorrectly when tracking changes to relationships.</span></span>
* <span data-ttu-id="8415d-239">架构扩展（旧版）未使用 $select 语句返回，而是在无 $select 的情况下返回。</span><span class="sxs-lookup"><span data-stu-id="8415d-239">Schema extensions (legacy) are not returned with $select statement, but are returned without $select.</span></span>
* <span data-ttu-id="8415d-240">客户端无法跟踪开放扩展或已注册架构扩展的变化。</span><span class="sxs-lookup"><span data-stu-id="8415d-240">Clients cannot track changes to open extensions or registered schema extensions.</span></span>

## <a name="application-and-serviceprincipal-api-changes"></a><span data-ttu-id="8415d-241">应用程序和 servicePrincipal API 更改</span><span class="sxs-lookup"><span data-stu-id="8415d-241">Application and servicePrincipal API changes</span></span>

<span data-ttu-id="8415d-p123">当前处于开发阶段的 [application](/graph/api/resources/application?view=graph-rest-beta) 和 [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) 实体有变化。下面总结了当前限制和处于开发阶段的 API 功能。</span><span class="sxs-lookup"><span data-stu-id="8415d-p123">There are changes to the [application](/graph/api/resources/application?view=graph-rest-beta) and [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) entities currently in development. The following is a summary of current limitations and in-development API features.</span></span>

<span data-ttu-id="8415d-244">当前限制：</span><span class="sxs-lookup"><span data-stu-id="8415d-244">Current limitations:</span></span>

* <span data-ttu-id="8415d-245">只有在所有更改完成后，一些应用属性（如 appRoles 和 addIns）才可用。</span><span class="sxs-lookup"><span data-stu-id="8415d-245">Some application properties (such as appRoles and addIns) will not be available until all changes are completed.</span></span>
* <span data-ttu-id="8415d-246">只能注册多租户应用。</span><span class="sxs-lookup"><span data-stu-id="8415d-246">Only multi-tenant apps can be registered.</span></span>
* <span data-ttu-id="8415d-247">更新应用仅限于在首次 beta更新后注册的应用。</span><span class="sxs-lookup"><span data-stu-id="8415d-247">Updating apps is restricted to apps registered after the initial beta update.</span></span>
* <span data-ttu-id="8415d-248">Azure Active Directory 用户可以注册应用并添加其他所有者。</span><span class="sxs-lookup"><span data-stu-id="8415d-248">Azure Active Directory users can register apps and add additional owners.</span></span>
* <span data-ttu-id="8415d-249">支持 OpenID Connect 和 OAuth 协议。</span><span class="sxs-lookup"><span data-stu-id="8415d-249">Support for OpenID Connect and OAuth protocols.</span></span>
* <span data-ttu-id="8415d-250">无法向应用分配策略。</span><span class="sxs-lookup"><span data-stu-id="8415d-250">Policy assignments to an application fail.</span></span>
* <span data-ttu-id="8415d-251">无法对需要 appId 的 ownedObjects 执行操作（例如，users/{id|userPrincipalName}/ownedObjects/{id}/...）</span><span class="sxs-lookup"><span data-stu-id="8415d-251">Operations on ownedObjects that require appId fail (For example, users/{id|userPrincipalName}/ownedObjects/{id}/...).</span></span>

<span data-ttu-id="8415d-252">处于开发阶段的功能：</span><span class="sxs-lookup"><span data-stu-id="8415d-252">In development:</span></span>

* <span data-ttu-id="8415d-253">可以注册单租户应用。</span><span class="sxs-lookup"><span data-stu-id="8415d-253">Ability to register single tenant apps.</span></span>
* <span data-ttu-id="8415d-254">更新 servicePrincipal。</span><span class="sxs-lookup"><span data-stu-id="8415d-254">Updates to servicePrincipal.</span></span>
* <span data-ttu-id="8415d-255">将现有 Azure AD 应用迁移到更新后的模型中。</span><span class="sxs-lookup"><span data-stu-id="8415d-255">Migration of existing Azure AD apps to updated model.</span></span>
* <span data-ttu-id="8415d-256">支持 appRoles、预授权客户端、可选声明、组成员身份声明和品牌塑造</span><span class="sxs-lookup"><span data-stu-id="8415d-256">Support for appRoles, pre-authorized clients, optional claims, group membership claims, and branding</span></span>
* <span data-ttu-id="8415d-257">Microsoft 帐户 (MSA) 用户可以注册应用。</span><span class="sxs-lookup"><span data-stu-id="8415d-257">Microsoft account (MSA) users can register apps.</span></span>
* <span data-ttu-id="8415d-258">支持 SAML 和 WsFed 协议。</span><span class="sxs-lookup"><span data-stu-id="8415d-258">Support for SAML and WsFed protocols.</span></span>

## <a name="extensions"></a><span data-ttu-id="8415d-259">扩展</span><span class="sxs-lookup"><span data-stu-id="8415d-259">Extensions</span></span>

### <a name="change-tracking-is-not-supported"></a><span data-ttu-id="8415d-260">不支持更改跟踪</span><span class="sxs-lookup"><span data-stu-id="8415d-260">Change tracking is not supported</span></span>

<span data-ttu-id="8415d-261">开放扩展或架构扩展属性不支持更改跟踪（Delta 查询）。</span><span class="sxs-lookup"><span data-stu-id="8415d-261">Change tracking (delta query) is not supported for open or schema extension properties.</span></span>

### <a name="creating-a-resource-and-open-extension-at-the-same-time"></a><span data-ttu-id="8415d-262">同时创建资源和开放扩展</span><span class="sxs-lookup"><span data-stu-id="8415d-262">Creating a resource and open extension at the same time</span></span>

<span data-ttu-id="8415d-p124">无法在创建**管理单元**、**设备**、**组**、**组织**或**用户**的实例的同时指定开放扩展。必须首先创建实例，然后在该实例的后续 ``POST`` 请求中指定开放扩展数据。</span><span class="sxs-lookup"><span data-stu-id="8415d-p124">You cannot specify an open extension at the same time you create an instance of **administrativeUnit**, **device**, **group**, **organization** or **user**. You must first create the instance and then specify the open extension data in a subsequent ``POST`` request on that instance.</span></span>

### <a name="creating-a-resource-instance-and-adding-schema-extension-data-at-the-same-time"></a><span data-ttu-id="8415d-265">创建资源实例的同时添加架构扩展数据</span><span class="sxs-lookup"><span data-stu-id="8415d-265">Creating a resource instance and adding schema extension data at the same time</span></span>

<span data-ttu-id="8415d-266">不能在创建 **contact**、**event**、**message** 或 **post** 实例的同一个操作中指定架构扩展。</span><span class="sxs-lookup"><span data-stu-id="8415d-266">You cannot specify a schema extension in the same operation as creating an instance of **contact**, **event**, **message**, or **post**.</span></span>
<span data-ttu-id="8415d-267">必须先创建资源实例，然后再对此实例执行 `PATCH`，从而添加架构扩展和自定义数据。</span><span class="sxs-lookup"><span data-stu-id="8415d-267">You must first create the resource instance and then do a `PATCH` to that instance to add a schema extension and custom data.</span></span>

### <a name="limit-of-100-schema-extension-property-values-allowed-per-resource-instance"></a><span data-ttu-id="8415d-268">每资源实例最多可以添加 100 个架构扩展属性值</span><span class="sxs-lookup"><span data-stu-id="8415d-268">Limit of 100 schema extension property values allowed per resource instance</span></span>

<span data-ttu-id="8415d-269">目录资源（如**设备**、**组**和**用户**）目前将可在资源实例上设置的架构扩展属性值的总数限制为 100。</span><span class="sxs-lookup"><span data-stu-id="8415d-269">Directory resources, such as **device**, **group** and **user**, currently limit the total number of schema extension property values that can be set on a resource instance, to 100.</span></span>

### <a name="filtering-on-schema-extension-properties-not-supported-on-all-entity-types"></a><span data-ttu-id="8415d-270">并非所有实体类型都支持对架构扩展属性进行筛选</span><span class="sxs-lookup"><span data-stu-id="8415d-270">Filtering on schema extension properties not supported on all entity types</span></span>

<span data-ttu-id="8415d-271">Outlook 实体类型不支持对架构扩展属性进行筛选（使用 `$filter` 表达式）- **联系人**、**事件**、**消息**或**帖子**。</span><span class="sxs-lookup"><span data-stu-id="8415d-271">Filtering on schema extension properties (using the `$filter` expresssion) is not supported for Outlook entity types - **contact**, **event**, **message**, or **post**.</span></span>

## <a name="json-batching"></a><span data-ttu-id="8415d-272">JSON 批处理</span><span class="sxs-lookup"><span data-stu-id="8415d-272">JSON Batching</span></span>

### <a name="no-nested-batch"></a><span data-ttu-id="8415d-273">无嵌套批处理</span><span class="sxs-lookup"><span data-stu-id="8415d-273">No nested batch</span></span>

<span data-ttu-id="8415d-274">JSON 批处理请求中不得包含任何嵌套批处理请求。</span><span class="sxs-lookup"><span data-stu-id="8415d-274">JSON batch requests must not contain any nested batch requests.</span></span>

### <a name="all-individual-requests-must-be-synchronous"></a><span data-ttu-id="8415d-275">所有单个请求必须同步</span><span class="sxs-lookup"><span data-stu-id="8415d-275">All individual requests must be synchronous</span></span>

<span data-ttu-id="8415d-p126">批处理请求中包含的所有请求都必须同步执行。如果存在，将忽略 `respond-async` 首选项。</span><span class="sxs-lookup"><span data-stu-id="8415d-p126">All requests contained in a batch request must be executed synchronously. If present, the `respond-async` preference will be ignored.</span></span>

### <a name="no-transactions"></a><span data-ttu-id="8415d-278">无事务</span><span class="sxs-lookup"><span data-stu-id="8415d-278">No transactions</span></span>

<span data-ttu-id="8415d-p127">Microsoft Graph 当前不支持单个请求的事务处理。将忽略单个请求的 `atomicityGroup` 属性。</span><span class="sxs-lookup"><span data-stu-id="8415d-p127">Microsoft Graph does not currently support transactional processing of individual requests. The `atomicityGroup` property on individual requests will be ignored.</span></span>

### <a name="uris-must-be-relative"></a><span data-ttu-id="8415d-281">URI 必须相对</span><span class="sxs-lookup"><span data-stu-id="8415d-281">URIs must be relative</span></span>

<span data-ttu-id="8415d-p128">始终在批处理请求中指定相对的 URI。Microsoft Graph 将使用批处理 URL 中包含的版本终结点使这些 URL 绝对。</span><span class="sxs-lookup"><span data-stu-id="8415d-p128">Always specify relative URIs in batch requests. Microsoft Graph then makes these URLs absolute by using the version endpoint included in the batch URL.</span></span>

### <a name="limit-on-batch-size"></a><span data-ttu-id="8415d-284">限制批处理大小</span><span class="sxs-lookup"><span data-stu-id="8415d-284">Limit on batch size</span></span>

<span data-ttu-id="8415d-285">JSON 批处理请求目前限定为 20 个单独请求。</span><span class="sxs-lookup"><span data-stu-id="8415d-285">JSON batch requests are currently limited to 20 individual requests.</span></span>

### <a name="simplified-dependencies"></a><span data-ttu-id="8415d-286">简化的依赖项</span><span class="sxs-lookup"><span data-stu-id="8415d-286">Simplified dependencies</span></span>

<span data-ttu-id="8415d-p129">单独请求可以依赖其他单独请求。目前，请求只能依赖于单个其他请求，并且必须遵循下面的三种模式之一：</span><span class="sxs-lookup"><span data-stu-id="8415d-p129">Individual requests can depend on other individual requests. Currently, requests can only depend on a single other request, and must follow one of these three patterns:</span></span>

1. <span data-ttu-id="8415d-289">平行 - 没有单独的请求在 `dependsOn` 属性中声明依赖项。</span><span class="sxs-lookup"><span data-stu-id="8415d-289">Parallel - no individual request states a dependency in the `dependsOn` property.</span></span>
2. <span data-ttu-id="8415d-290">串行 - 所有单独请求都依赖于之前的单独请求。</span><span class="sxs-lookup"><span data-stu-id="8415d-290">Serial - all individual requests depend on the previous individual request.</span></span>
3. <span data-ttu-id="8415d-291">相同 - 在 `dependsOn` 属性中声明依赖项的所有单独请求均声明了相同的依赖项。</span><span class="sxs-lookup"><span data-stu-id="8415d-291">Same - all individual requests that state a dependency in the `dependsOn` property, state the same dependency.</span></span>

<span data-ttu-id="8415d-292">随着 JSON 批处理技术日臻成熟，这些限制将会被取消。</span><span class="sxs-lookup"><span data-stu-id="8415d-292">As JSON batching matures, these limitations will be removed.</span></span>

## <a name="cloud-solution-provider-apps"></a><span data-ttu-id="8415d-293">云解决方案提供商应用</span><span class="sxs-lookup"><span data-stu-id="8415d-293">Cloud Solution Provider apps</span></span>

### <a name="csp-apps-must-use-azure-ad-endpoint"></a><span data-ttu-id="8415d-294">CSP 应用必须使用 Azure AD 终结点</span><span class="sxs-lookup"><span data-stu-id="8415d-294">CSP apps must use Azure AD endpoint</span></span>

<span data-ttu-id="8415d-p130">云解决方案提供商 (CSP) 应用必须从 Azure AD (v1) 终结点中获取令牌，才能在其合作伙伴托管的客户中成功调用 Microsoft Graph。目前，不支持通过较新的 Azure AD v2.0 终结点获取令牌。</span><span class="sxs-lookup"><span data-stu-id="8415d-p130">Cloud solution provider (CSP) apps must acquire tokens from the Azure AD (v1) endpoints to successfully call Microsoft Graph in their partner-managed customers. Currently, acquiring a token through the newer Azure AD v2.0 endpoint is not supported.</span></span>

### <a name="pre-consent-for-csp-apps-doesnt-work-in-some-customer-tenants"></a><span data-ttu-id="8415d-297">对 CSP 应用的预授权不适用于一些客户租户</span><span class="sxs-lookup"><span data-stu-id="8415d-297">Pre-consent for CSP apps doesn't work in some customer tenants</span></span>

<span data-ttu-id="8415d-298">在某些情况下，对 CSP 应用的预授权可能不适用于一些客户租户。</span><span class="sxs-lookup"><span data-stu-id="8415d-298">Under certain circumstances, pre-consent for CSP apps may not work for some of your customer tenants.</span></span>

- <span data-ttu-id="8415d-299">对于使用委派权限的应用，首次将此应用用于新客户租户时，登录后可能会看到以下错误：`AADSTS50000: There was an error issuing a token`。</span><span class="sxs-lookup"><span data-stu-id="8415d-299">For apps using delegated permissions, when using the app for the first time with a new customer tenant you might receive this error after sign-in: `AADSTS50000: There was an error issuing a token`.</span></span>
- <span data-ttu-id="8415d-300">对于使用应用权限的应用，应用可以获取令牌，但在调用 Microsoft Graph 时会意外看到“拒绝访问”消息。</span><span class="sxs-lookup"><span data-stu-id="8415d-300">For apps using application permissions, your app can acquire a token, but unexpectedly gets an access denied message when calling Microsoft Graph.</span></span>

<span data-ttu-id="8415d-301">我们正在努力工作，以尽快解决此问题，让预授权适用于所有客户租户。</span><span class="sxs-lookup"><span data-stu-id="8415d-301">We are working to fix this issue as soon as possible, so that pre-consent will work for all your customer tenants.</span></span>

<span data-ttu-id="8415d-302">同时，若要取消阻止开发和测试，可使用以下解决方法。</span><span class="sxs-lookup"><span data-stu-id="8415d-302">In the meantime, to unblock development and testing you can use the following workaround.</span></span>

><span data-ttu-id="8415d-p131">**注意：** 这不是永久性解决方案，仅用于取消阻止开发。一旦上述问题得到解决，便无需使用此解决方案。在问题得到解决后，无需撤消此解决方法。</span><span class="sxs-lookup"><span data-stu-id="8415d-p131">**NOTE:** This is not a permanent solution and is only intended to unblock development.  This workaround will not be required once the aforementioned issue is fixed.  This workaround does not need to be undone once the fix is in place.</span></span>

1. <span data-ttu-id="8415d-p132">打开 Azure AD v2 PowerShell 会话，然后在登录窗口中输入管理员凭据，以连接 `customer` 租户。可以单击[此处](https://www.powershellgallery.com/packages/AzureAD)，下载并安装 Azure AD PowerShell V2。</span><span class="sxs-lookup"><span data-stu-id="8415d-p132">Open an Azure AD v2 PowerShell session and connect to your `customer` tenant by entering your admin credentials into the sign-in window. You can download and install Azure AD PowerShell V2 from [here](https://www.powershellgallery.com/packages/AzureAD).</span></span>

    ```PowerShell
    Connect-AzureAd -TenantId {customerTenantIdOrDomainName}
    ```

2. <span data-ttu-id="8415d-308">创建 Microsoft Graph 服务主体。</span><span class="sxs-lookup"><span data-stu-id="8415d-308">Create the Microsoft Graph service principal.</span></span>

    ```PowerShell
    New-AzureADServicePrincipal -AppId 00000003-0000-0000-c000-000000000000
    ```

## <a name="functionality-available-only-in-office-365-rest-or-azure-ad-graph-apis"></a><span data-ttu-id="8415d-309">只有 Office 365 REST 或 Azure AD Graph API 才具有的功能</span><span class="sxs-lookup"><span data-stu-id="8415d-309">Functionality available only in Office 365 REST or Azure AD Graph APIs</span></span>

<span data-ttu-id="8415d-p133">某些功能尚未在 Microsoft Graph 中提供。如果找不到所需的功能，请使用特定于终结点的 [Office 365 REST API](https://msdn.microsoft.com/office/office365/api/api-catalog)。有关 Azure Active Directory，请参考 [Microsoft Graph 或 Azure AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) 博客文章，获取只能通过 Azure AD Graph API 提供的功能。</span><span class="sxs-lookup"><span data-stu-id="8415d-p133">Some functionality is not yet available in Microsoft Graph. If you don't see the functionality you're looking for, you can use the endpoint-specific [Office 365 REST APIs](https://msdn.microsoft.com/office/office365/api/api-catalog). For Azure Active Directory, please refer to the [Microsoft Graph or Azure AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) blog post on the features that are only available through Azure AD Graph API.</span></span>

