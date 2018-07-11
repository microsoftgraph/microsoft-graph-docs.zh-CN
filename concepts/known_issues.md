# <a name="known-issues-with-microsoft-graph"></a><span data-ttu-id="afaf6-101">Microsoft Graph 已知问题</span><span class="sxs-lookup"><span data-stu-id="afaf6-101">Known issues with Microsoft Graph</span></span>

<span data-ttu-id="afaf6-p101">本文介绍了 Microsoft Graph 已知问题。若要了解最新更新，请参阅 [Microsoft Graph 更改日志](changelog.md)。</span><span class="sxs-lookup"><span data-stu-id="afaf6-p101">This article describes known issues with Microsoft Graph. For information about the latest updates, see the [Microsoft Graph changelog](changelog.md).</span></span>

## <a name="users"></a><span data-ttu-id="afaf6-104">用户</span><span class="sxs-lookup"><span data-stu-id="afaf6-104">Users</span></span>

### <a name="no-instant-access-after-creation"></a><span data-ttu-id="afaf6-105">创建后无法即时访问</span><span class="sxs-lookup"><span data-stu-id="afaf6-105">No instant access after creation</span></span>

<span data-ttu-id="afaf6-p102">可通过在用户实体上使用 POST 来即时创建用户。必须先向用户分配 Office 365 许可证，然后用户才能访问 Office 365 服务。尽管如此，由于服务具有分散特性，因此用户可能需要先等待 15 分钟，然后才能通过 Microsoft Graph API 使用文件、邮件和事件实体。在此期间，应用会收到一个 404 HTTP 错误响应。</span><span class="sxs-lookup"><span data-stu-id="afaf6-p102">Users can be created immediately through a POST on the user entity. An Office 365 license must first be assigned to a user, in order to get access to Office 365 services. Even then, due to the distributed nature of the service, it might take 15 minutes before files, messages and events entities are available for use for this user, through the Microsoft Graph API. During this time, apps will receive a 404 HTTP error response.</span></span>

### <a name="photo-restrictions"></a><span data-ttu-id="afaf6-110">照片限制</span><span class="sxs-lookup"><span data-stu-id="afaf6-110">Photo restrictions</span></span>

<span data-ttu-id="afaf6-p103">只有当用户有邮箱时，才能读取和更新用户的个人资料照片。另外，之前*可能*使用 **thumbnailPhoto** 属性（使用 Office 365 统一 API 预览或 Azure AD Graph，或通过 AD Connect 同步）存储的所有照片无法再通过[用户](../api-reference/v1.0/resources/user.md)资源的 Microsoft Graph **照片**属性进行访问。在这种情况下，无法读取或更新照片会生成以下错误：</span><span class="sxs-lookup"><span data-stu-id="afaf6-p103">Reading and updating a user's profile photo is only possible if the user has a mailbox. Additionally, any photos that *may* have been previously stored using the **thumbnailPhoto** property (using the Office 365 unified API preview, or the Azure AD Graph, or through AD Connect synchronization) are no longer accessible through the Microsoft Graph **photo** property of the [user](../api-reference/v1.0/resources/user.md) resource. Failure to read or update a photo, in this case, would result in the following error:</span></span>

```javascript
    {
      "error": {
        "code": "ErrorNonExistentMailbox",
        "message": "The SMTP address has no mailbox associated with it."
      }
    }
```


### <a name="using-delta-query"></a><span data-ttu-id="afaf6-114">使用 delta 查询</span><span class="sxs-lookup"><span data-stu-id="afaf6-114">Using delta query</span></span>

<span data-ttu-id="afaf6-115">有关使用 delta 查询的已知问题，请参阅本文中的 [delta 查询部分](#delta-query)。</span><span class="sxs-lookup"><span data-stu-id="afaf6-115">For known issues using delta query, see the [delta query section](#delta-query) in this article.</span></span>

## <a name="groups-and-microsoft-teams"></a><span data-ttu-id="afaf6-116">组和 Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="afaf6-116">Groups and Microsoft Teams</span></span>

><span data-ttu-id="afaf6-117">**注意**：Microsoft Teams 当前处于预览阶段，仅在 Microsoft Graph beta 终结点中可用。</span><span class="sxs-lookup"><span data-stu-id="afaf6-117">**Note** Microsoft Teams is currently in preview and is available only in the Microsoft Graph beta endpoint.</span></span>

### <a name="policy"></a><span data-ttu-id="afaf6-118">策略</span><span class="sxs-lookup"><span data-stu-id="afaf6-118">Policy</span></span>

<span data-ttu-id="afaf6-119">使用 Microsoft Graph 创建并命名 Office 365 组会忽略通过 Outlook Web App 配置的所有 Office 365 组策略。</span><span class="sxs-lookup"><span data-stu-id="afaf6-119">Using Microsoft Graph to create and name an Office 365 group bypasses any Office 365 group policies that are configured through Outlook Web App.</span></span>

### <a name="permissions-for-groups-and-microsoft-teams"></a><span data-ttu-id="afaf6-120">组和 Microsoft Teams 的权限</span><span class="sxs-lookup"><span data-stu-id="afaf6-120">Permissions for groups and Microsoft Teams</span></span>

<span data-ttu-id="afaf6-p104">Microsoft Graph 公开了两个权限（*Group.Read.All* 和 *Group.ReadWrite.All*），用于访问组和 Microsoft Teams 的 API。必须征得管理员同意，才能使用这些权限（不同于预览版）。我们计划在将来新增只需征得用户同意的组和团队权限。</span><span class="sxs-lookup"><span data-stu-id="afaf6-p104">Microsoft Graph exposes two permissions (*Group.Read.All* and *Group.ReadWrite.All*) for access to the APIs for groups and Microsoft Teams. These permissions must be consented to by an administrator (which is a change from preview).  In the future, we plan to add new permissions for groups and teams that users can consent to.</span></span>

<span data-ttu-id="afaf6-p105">此外，只有与核心组管理和管理相关的 API 才支持使用委派权限或仅限应用权限进行访问。其他所有的组 API 功能仅支持委派权限。</span><span class="sxs-lookup"><span data-stu-id="afaf6-p105">Also, only the API for core group administration and management supports access using delegated or app-only permissions. All other features of the group API support only delegated permissions.</span></span>

<span data-ttu-id="afaf6-126">同时支持委派权限和仅限应用权限的组功能示例：</span><span class="sxs-lookup"><span data-stu-id="afaf6-126">Examples of group features that support delegated and app-only permissions:</span></span>

* <span data-ttu-id="afaf6-127">创建和删除组</span><span class="sxs-lookup"><span data-stu-id="afaf6-127">Creating and deleting groups</span></span>
* <span data-ttu-id="afaf6-128">获取和更新与组管理或管理相关的组属性</span><span class="sxs-lookup"><span data-stu-id="afaf6-128">Getting and updating group properties pertaining to group administration or management</span></span>
* <span data-ttu-id="afaf6-129">组[目录设置](../api-reference/v1.0/resources/directoryobject.md)、类型和同步</span><span class="sxs-lookup"><span data-stu-id="afaf6-129">Group [directory settings](../api-reference/v1.0/resources/directoryobject.md), type, and synchronization</span></span>
* <span data-ttu-id="afaf6-130">组所有者和成员</span><span class="sxs-lookup"><span data-stu-id="afaf6-130">Group owners and membership</span></span>

<span data-ttu-id="afaf6-131">仅支持委派权限的组功能示例：</span><span class="sxs-lookup"><span data-stu-id="afaf6-131">Examples of group features that support only delegated permissions:</span></span>

* <span data-ttu-id="afaf6-132">组对话、事件和照片</span><span class="sxs-lookup"><span data-stu-id="afaf6-132">Group conversations, events, photo</span></span>
* <span data-ttu-id="afaf6-133">外部发件人、被接受或拒绝的发件人、组订阅</span><span class="sxs-lookup"><span data-stu-id="afaf6-133">External senders, accepted or rejected senders, group subscription</span></span>
* <span data-ttu-id="afaf6-134">用户收藏夹和未读计数</span><span class="sxs-lookup"><span data-stu-id="afaf6-134">User favorites and unseen count</span></span>
* <span data-ttu-id="afaf6-135">Microsoft Teams 频道和聊天</span><span class="sxs-lookup"><span data-stu-id="afaf6-135">Microsoft Teams channels and chats</span></span>

### <a name="teams-in-microsoft-teams-preview"></a><span data-ttu-id="afaf6-136">Microsoft Teams 中的团队（预览阶段）</span><span class="sxs-lookup"><span data-stu-id="afaf6-136">Teams in Microsoft Teams (preview)</span></span>

<span data-ttu-id="afaf6-p106">Microsoft Teams 和 Office 365 组的[功能相似](../api-reference/beta/resources/teams_api_overview.md)。所有组 API 均可用于团队，暂不允许创建团队的创建组 API 除外。今后发布的 API 版本将支持此功能。</span><span class="sxs-lookup"><span data-stu-id="afaf6-p106">Microsoft Teams and Office 365 groups [share similar functionality](../api-reference/beta/resources/teams_api_overview.md). All group APIs can be used with teams, with the exception that the Create group API does not currently allow you to create a team.  Future API releases will support this.</span></span>

### <a name="microsoft-teams-channels-preview"></a><span data-ttu-id="afaf6-140">Microsoft Teams 频道（预览）</span><span class="sxs-lookup"><span data-stu-id="afaf6-140">Microsoft Teams channels (preview)</span></span>

<span data-ttu-id="afaf6-p107">目前，你可以读取和创建频道，但无法更新或删除频道。将来的 API 版本将支持此功能。</span><span class="sxs-lookup"><span data-stu-id="afaf6-p107">Currently, you can read and create channels, but you cannot update or delete them.  Future API releases will support this.</span></span>

### <a name="microsoft-teams-chat-threads-and-chat-messages-preview"></a><span data-ttu-id="afaf6-143">Microsoft Teams 聊天会话和聊天消息（预览）</span><span class="sxs-lookup"><span data-stu-id="afaf6-143">Microsoft Teams chat threads and chat messages (preview)</span></span>

<span data-ttu-id="afaf6-p108">目前，可以在通道中创建聊天会话，但无法读取现有聊天会话，也无法添加对它们的答复。此外，还无法读取或写入与团队或频道范围外的用户之间的直接聊天。今后发布的 API 版本将在这一领域新增其他功能。</span><span class="sxs-lookup"><span data-stu-id="afaf6-p108">Currently, you can create chat threads in channels, but you cannot read existing chat threads or add replies to them. Also, you cannot read or write direct chats between users that are outside the scope of a team or channel.  Future API releases will add additional capabilities in this area.</span></span>

### <a name="microsoft-teams-users-list-of-joined-teams-preview"></a><span data-ttu-id="afaf6-147">Microsoft Teams 用户的已加入团队列表（预览阶段）</span><span class="sxs-lookup"><span data-stu-id="afaf6-147">Microsoft Teams user's list of joined teams (preview)</span></span>

<span data-ttu-id="afaf6-p109">目前，[列出用户已加入的团队](../api-reference/beta/api/user_list_joinedteams.md)仅适用于呼叫者对其拥有[委派权限](permissions_reference.md)的“我”用户。今后发布的版本将支持对任何指定用户 ID 执行此操作。</span><span class="sxs-lookup"><span data-stu-id="afaf6-p109">Currrently, [listing the teams a user has joined](../api-reference/beta/api/user_list_joinedteams.md) only works for the 'me' user for which the caller has [delegated permissions](permissions_reference.md).  Future releases will support this operation for any specified user ID.</span></span>

### <a name="adding-and-getting-attachments-of-group-posts"></a><span data-ttu-id="afaf6-150">添加和获取组帖子的附件</span><span class="sxs-lookup"><span data-stu-id="afaf6-150">Adding and getting attachments of group posts</span></span>

<span data-ttu-id="afaf6-p110">向组帖子 [添加](http://developer.microsoft.com/zh-CN/graph/docs/api-reference/v1.0/api/post_post_attachments) 附件、[列出](http://developer.microsoft.com/zh-CN/graph/docs/api-reference/v1.0/api/post_list_attachments) 和获取组帖子的附件目前返回错误消息“OData 请求不受支持”。已经为 `/v1.0` 和 `/beta` 版本推出修复程序，并预计到 2016 年 1 月底会广泛推出。</span><span class="sxs-lookup"><span data-stu-id="afaf6-p110">[Adding](http://developer.microsoft.com/zh-CN/graph/docs/api-reference/v1.0/api/post_post_attachments) attachments to group posts, [listing](http://developer.microsoft.com/zh-CN/graph/docs/api-reference/v1.0/api/post_list_attachments) and getting attachments of group posts currently return the error message "The OData request is not supported." A fix has been rolled out for both the `/v1.0` and `/beta` versions, and is expected to be widely available by the end of January 2016.</span></span>

### <a name="setting-the-allowexternalsenders-property"></a><span data-ttu-id="afaf6-153">设置 allowExternalSenders 属性</span><span class="sxs-lookup"><span data-stu-id="afaf6-153">Setting the allowExternalSenders property</span></span>

<span data-ttu-id="afaf6-154">目前，`/v1.0` 和 `/beta` 中均存在一个问题，即会阻止在 POST 或 PATCH 操作中设置组的属性 **allowExternalSenders**。</span><span class="sxs-lookup"><span data-stu-id="afaf6-154">There is currently an issue that prevents setting the **allowExternalSenders** property of a group in a POST or PATCH operation, in both `/v1.0` and `/beta`.</span></span>

### <a name="using-delta-query"></a><span data-ttu-id="afaf6-155">使用 delta 查询</span><span class="sxs-lookup"><span data-stu-id="afaf6-155">Using delta query</span></span>

<span data-ttu-id="afaf6-156">有关使用 delta 查询的已知问题，请参阅本文中的 [delta 查询部分](#delta-query)。</span><span class="sxs-lookup"><span data-stu-id="afaf6-156">For known issues using delta query, see the [delta query section](#delta-query) in this article.</span></span>


## <a name="bookings"></a><span data-ttu-id="afaf6-157">预订</span><span class="sxs-lookup"><span data-stu-id="afaf6-157">Bookings</span></span>

### <a name="errorexceededfindcountlimit-when-querying-bookingbusinesses"></a><span data-ttu-id="afaf6-158">查询 bookingBusinesses 时出现 ErrorExceededFindCountLimit</span><span class="sxs-lookup"><span data-stu-id="afaf6-158">ErrorExceededFindCountLimit when querying bookingBusinesses</span></span>

<span data-ttu-id="afaf6-159">当组织拥有多个预订业务且提出请求的帐户不是管理员时，获取 `bookingBusinesses` 列表会失败，并显示以下错误代码：</span><span class="sxs-lookup"><span data-stu-id="afaf6-159">Getting the list of `bookingBusinesses` fails with the following error code when an organization has several booking businesses and the account making the request is not an administrator:</span></span>

```json
{
  "error": {
    "code": "ErrorExceededFindCountLimit",
    "message":
      "The GetBookingMailboxes request returned too many results. Please specify a query to limit the results.",
  }
}
```

<span data-ttu-id="afaf6-160">解决方法是，可以通过加入 `query` 参数来限制请求返回的业务集，例如：</span><span class="sxs-lookup"><span data-stu-id="afaf6-160">As a workaround, you can limit the set of businesses returned by the request by including a `query` parameter, for example:</span></span>

```
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Fabrikam
```


## <a name="calendars"></a><span data-ttu-id="afaf6-161">日历</span><span class="sxs-lookup"><span data-stu-id="afaf6-161">Calendars</span></span>

### <a name="adding-and-accessing-ics-based-calendars-in-users-mailbox"></a><span data-ttu-id="afaf6-162">在用户邮箱中添加和访问基于 ICS 的日历</span><span class="sxs-lookup"><span data-stu-id="afaf6-162">Adding and accessing ICS-based calendars in user's mailbox</span></span>

<span data-ttu-id="afaf6-163">目前，还有部分支持基于 Internet 日历订阅 (ICS) 的日历：</span><span class="sxs-lookup"><span data-stu-id="afaf6-163">Currently, there is partial support for a calendar based on an Internet Calendar Subscription (ICS):</span></span>

* <span data-ttu-id="afaf6-164">你可以通过用户界面，而不是通过 Microsoft Graph API 为用户邮箱添加基于 ICS 的日历。</span><span class="sxs-lookup"><span data-stu-id="afaf6-164">You can add an ICS-based calendar to a user mailbox through the user interface, but not through the Microsoft Graph API.</span></span>
* <span data-ttu-id="afaf6-p111">[列出用户的日历](http://developer.microsoft.com/zh-CN/graph/docs/api-reference/v1.0/api/user_list_calendars)允许你获取用户默认日历组中或指定日历组中的每个 [日历](http://developer.microsoft.com/zh-CN/graph/docs/api-reference/v1.0/resources/calendar)的**名称**、**颜色**和 **id** 属性，包括所有基于 ICS 的日历。你无法存储或访问日历资源中的 ICS URL。</span><span class="sxs-lookup"><span data-stu-id="afaf6-p111">[Listing the user's calendars](http://developer.microsoft.com/zh-CN/graph/docs/api-reference/v1.0/api/user_list_calendars) lets you get the **name**, **color** and **id** properties of each [calendar](http://developer.microsoft.com/zh-CN/graph/docs/api-reference/v1.0/resources/calendar) in the user's default calendar group, or a specified calendar group, including any ICS-based calendars. You cannot store or access the ICS URL in the calendar resource.</span></span>
* <span data-ttu-id="afaf6-167">还可以[列出基于 ICS 的日历事件](http://developer.microsoft.com/zh-CN/graph/docs/api-reference/v1.0/api/calendar_list_events)。</span><span class="sxs-lookup"><span data-stu-id="afaf6-167">You can also [list the events](http://developer.microsoft.com/zh-CN/graph/docs/api-reference/v1.0/api/calendar_list_events) of an ICS-based calendar.</span></span>

### <a name="accessing-a-shared-calendar"></a><span data-ttu-id="afaf6-168">访问共享日历</span><span class="sxs-lookup"><span data-stu-id="afaf6-168">Accessing a shared calendar</span></span>

<span data-ttu-id="afaf6-169">使用以下操作尝试访问其他用户共享的日历中的事件时：</span><span class="sxs-lookup"><span data-stu-id="afaf6-169">When attempting to access events in a calendar that has been shared by another user using the following operation:</span></span>

```http
GET \users('{id}')\calendars('{id}')\events
```

<span data-ttu-id="afaf6-p112">可能会看到错误代码为 `ErrorInternalServerTransientError` 的 HTTP 500。导致错误发生的原因是：</span><span class="sxs-lookup"><span data-stu-id="afaf6-p112">You may get HTTP 500 with the error code `ErrorInternalServerTransientError`. The error occurs because:</span></span>

- <span data-ttu-id="afaf6-172">过去，日历共享的实现方法有两种。为了加以区分，将它们称为“旧”方法和“新”方法。</span><span class="sxs-lookup"><span data-stu-id="afaf6-172">Historically, there are two ways that calendar sharing has been implemented, which, for the purpose of differentiating them, are referred to as the "old" approach and "new" approach.</span></span>
- <span data-ttu-id="afaf6-173">新方法当前可用于通过查看或编辑权限共享日历，但无法通过委派权限进行共享。</span><span class="sxs-lookup"><span data-stu-id="afaf6-173">The new approach is currently available for sharing calendars with view or edit permissions, but not with delegate permissions.</span></span>
- <span data-ttu-id="afaf6-174">只有使用**新**方法共享日历后，才能使用日历 REST API 查看或编辑共享日历。</span><span class="sxs-lookup"><span data-stu-id="afaf6-174">You can use the calendar REST API to view or edit shared calendars only if the calendars were shared using the **new** approach.</span></span>
- <span data-ttu-id="afaf6-175">如果使用**旧**方法共享日历，则无法使用日历 REST API 查看或编辑此类日历（或其事件）。</span><span class="sxs-lookup"><span data-stu-id="afaf6-175">You cannot use the calendar REST API to view or edit such calendars (or their events) if the calendars were shared using the **old** approach.</span></span>


<span data-ttu-id="afaf6-176">如果日历是通过查看或编辑权限共享，但使用的是旧方法，现在可以修复错误，手动将日历共享升级为使用新方法。</span><span class="sxs-lookup"><span data-stu-id="afaf6-176">If a calendar was shared with view or edit permissions but using the old approach, you can now work around the error and manually upgrade the calendar sharing to use the new approach.</span></span>
<span data-ttu-id="afaf6-177">随着时间的推移，Outlook 将把所有共享日历（包括通过委托权限共享的日历）自动升级为使用新方法。</span><span class="sxs-lookup"><span data-stu-id="afaf6-177">Over time, Outlook will automatically upgrade all shared calendars to use the new approach, including calendars shared with delegate permissions.</span></span>

<span data-ttu-id="afaf6-178">若要手动将共享日历升级为使用新方法，请按照以下步骤操作：</span><span class="sxs-lookup"><span data-stu-id="afaf6-178">To manually upgrade a shared calendar to use the new approach, follow these steps:</span></span>
1.  <span data-ttu-id="afaf6-179">收件人删除以前与他们共享的日历。</span><span class="sxs-lookup"><span data-stu-id="afaf6-179">The recipient removes the calendar that was previously shared to them.</span></span>
2.  <span data-ttu-id="afaf6-180">日历所有者在 Outlook 网页版、iOS 版或 Android 版中重新共享日历。</span><span class="sxs-lookup"><span data-stu-id="afaf6-180">The calendar owner re-shares the calendar in Outlook on the web, Outlook on iOS, or Outlook on Android.</span></span>
3.  <span data-ttu-id="afaf6-p114">收件人使用 Outlook 网页版重新接受共享日历。（很快就可以使用其他 Outlook 客户端了。）</span><span class="sxs-lookup"><span data-stu-id="afaf6-p114">The recipient re-accepts the shared calendar using Outlook on the web. (It will be possible to use other Outlook clients soon.)</span></span>
4.  <span data-ttu-id="afaf6-183">收件人可以在 Outlook iOS 版或 Android 版中查看共享日历，从而验证是否已成功使用新方法重新共享日历。</span><span class="sxs-lookup"><span data-stu-id="afaf6-183">The recipient verifies that the calendar has been re-shared successfully using the new approach by being able to view the shared calendar in Outlook on iOS or Outlook on Android.</span></span>

<span data-ttu-id="afaf6-p115">使用新方法共享的日历看起来与邮箱中的其他日历一样。可以使用日历 REST API 查看或编辑共享日历中的事件，就像查看或编辑自己日历中的事件一样。示例：</span><span class="sxs-lookup"><span data-stu-id="afaf6-p115">A calendar shared with you in the new approach appears as just another calendar in your mailbox. You can use the calendar REST API to view or edit events in the shared calendar, as if it's your own calendar. As an example:</span></span>

```http
GET \me\calendars('{id}')\events
```


## <a name="contacts"></a><span data-ttu-id="afaf6-187">Contacts</span><span class="sxs-lookup"><span data-stu-id="afaf6-187">Contacts</span></span>

### <a name="organization-contacts-available-in-only-beta"></a><span data-ttu-id="afaf6-188">仅 beta 版支持组织联系人。</span><span class="sxs-lookup"><span data-stu-id="afaf6-188">Organization contacts available in only beta</span></span>

<span data-ttu-id="afaf6-p116">目前只支持个人联系人。`/v1.0` 中目前暂不支持组织联系人，但可以在 `/beta` 中找到组织联系人。</span><span class="sxs-lookup"><span data-stu-id="afaf6-p116">Only personal contacts are currently supported. Organizational contacts are not currently supported in `/v1.0`, but can be found in `/beta`.</span></span>

### <a name="default-contacts-folder"></a><span data-ttu-id="afaf6-191">默认联系人文件夹</span><span class="sxs-lookup"><span data-stu-id="afaf6-191">Default contacts folder</span></span>

<span data-ttu-id="afaf6-192">在 `/v1.0` 版本中，`GET /me/contactFolders` 不包括用户的默认联系人文件夹。</span><span class="sxs-lookup"><span data-stu-id="afaf6-192">In the `/v1.0` version, `GET /me/contactFolders` does not include the user's default contacts folder.</span></span>

<span data-ttu-id="afaf6-p117">将会提供修复程序。同时，您还可以使用以下[列出联系人](http://developer.microsoft.com/zh-CN/graph/docs/api-reference/v1.0/api/user_list_contacts)查询和 **parentFolderId** 属性作为一种解决方法，来获取默认联系人文件夹的文件夹 ID：</span><span class="sxs-lookup"><span data-stu-id="afaf6-p117">A fix will be made available. Meanwhile, you can use the following [list contacts](http://developer.microsoft.com/zh-CN/graph/docs/api-reference/v1.0/api/user_list_contacts) query and the **parentFolderId** property as a workaround to get the folder ID of the default contacts folder:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/contacts?$top=1&$select=parentFolderId
```

<span data-ttu-id="afaf6-195">在上面的查询中：</span><span class="sxs-lookup"><span data-stu-id="afaf6-195">In the above query:</span></span>

1. <span data-ttu-id="afaf6-196">`/me/contacts?$top=1` 获取默认联系人文件夹中 [联系人](http://developer.microsoft.com/zh-CN/graph/docs/api-reference/v1.0/resources/contact) 的属性。</span><span class="sxs-lookup"><span data-stu-id="afaf6-196">`/me/contacts?$top=1` gets the properties of a [contact](http://developer.microsoft.com/zh-CN/graph/docs/api-reference/v1.0/resources/contact) in the default contacts folder.</span></span>
2. <span data-ttu-id="afaf6-197">附加 `&$select=parentFolderId` 仅返回联系人的 **parentFolderId** 属性，即默认联系人文件夹的 ID。</span><span class="sxs-lookup"><span data-stu-id="afaf6-197">Appending `&$select=parentFolderId` returns only the contact's **parentFolderId** property, which is the ID of the default contacts folder.</span></span>


### <a name="accessing-contacts-via-a-contact-folder-in-beta"></a><span data-ttu-id="afaf6-198">在 beta 版中通过联系人文件夹访问联系人</span><span class="sxs-lookup"><span data-stu-id="afaf6-198">Accessing contacts via a contact folder in beta</span></span>

<span data-ttu-id="afaf6-199">目前，`/beta` 版中存在一个问题，即会在 REST 请求 URL 中指定父文件夹，进而阻止访问[联系人](../api-reference/beta/resources/contact.md)，如以下 2 个方案所示。</span><span class="sxs-lookup"><span data-stu-id="afaf6-199">In the `/beta` version, there is currently an issue that prevents accessing a [contact](../api-reference/beta/resources/contact.md) by specifying its parent folder in the REST request URL, as shown in the 2 scenarios below.</span></span>

* <span data-ttu-id="afaf6-200">从用户的顶级 [contactFolder](../api-reference/beta/resources/contactfolder.md) 访问联系人。</span><span class="sxs-lookup"><span data-stu-id="afaf6-200">Accessing a contact from a top level [contactFolder](../api-reference/beta/resources/contactfolder.md) of the user's.</span></span>

```http
GET /me/contactfolders/{id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```

* <span data-ttu-id="afaf6-p118">访问 **contactFolder** 的子文件夹中的联系人。下面的示例展示了一级嵌套，但可以在子文件夹的子级等对象中访问联系人。</span><span class="sxs-lookup"><span data-stu-id="afaf6-p118">Accessing a contact contained in a child folder of a **contactFolder**.  The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>

```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```

<span data-ttu-id="afaf6-203">或者，如下所示，只需指定联系人 ID 即可[获取](../api-reference/beta/api/contact_get.md)此联系人，因为在 `/beta` 版中 GET /contacts 适用于用户邮箱中的所有联系人：</span><span class="sxs-lookup"><span data-stu-id="afaf6-203">As an alternative, you can simply [get](../api-reference/beta/api/contact_get.md) the contact by specifying its ID as shown below, since GET /contacts in the `/beta` version applies to all the contacts in the user's mailbox:</span></span>

```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```

## <a name="messages"></a><span data-ttu-id="afaf6-204">邮件</span><span class="sxs-lookup"><span data-stu-id="afaf6-204">Messages</span></span>

### <a name="the-comment-parameter-for-creating-a-draft"></a><span data-ttu-id="afaf6-205">用于创建草稿的注释参数</span><span class="sxs-lookup"><span data-stu-id="afaf6-205">The comment parameter for creating a draft</span></span>

<span data-ttu-id="afaf6-206">用于创建答复或转发草稿的**注释**参数（[createReply](../api-reference/v1.0/api/message_createreply.md)、[createReplyAll](../api-reference/v1.0/api/message_createreplyall.md)、[createForward](../api-reference/v1.0/api/message_createforward.md)）不会成为最终的邮件草稿正文的一部分。</span><span class="sxs-lookup"><span data-stu-id="afaf6-206">The **comment** parameter for creating a reply or forward draft ([createReply](../api-reference/v1.0/api/message_createreply.md), [createReplyAll](../api-reference/v1.0/api/message_createreplyall.md), [createForward](../api-reference/v1.0/api/message_createforward.md)) does not become part of the body of the resultant message draft.</span></span>


## <a name="drives-files-and-content-streaming"></a><span data-ttu-id="afaf6-207">驱动器、文件和内容流式传输</span><span class="sxs-lookup"><span data-stu-id="afaf6-207">Drives, files and content streaming</span></span>

* <span data-ttu-id="afaf6-208">在通过浏览器访问个人站点之前，用户首次通过 Microsoft Graph 访问个人驱动器会生成 401 响应。</span><span class="sxs-lookup"><span data-stu-id="afaf6-208">First time access to a user's personal drive through the Microsoft Graph before the user accesses their personal site through a browser leads to a 401 response.</span></span>

## <a name="query-parameter-limitations"></a><span data-ttu-id="afaf6-209">查询参数限制</span><span class="sxs-lookup"><span data-stu-id="afaf6-209">Query parameter limitations</span></span>

* <span data-ttu-id="afaf6-210">不支持多个命名空间。</span><span class="sxs-lookup"><span data-stu-id="afaf6-210">Multiple namespaces are not supported.</span></span>
* <span data-ttu-id="afaf6-211">在用户、组、设备、服务主体和应用程序上，不支持对 `$ref` 执行 GET 操作和投影。</span><span class="sxs-lookup"><span data-stu-id="afaf6-211">GETs on `$ref` and casting is not supported on users, groups, devices, service principals and applications.</span></span>
* <span data-ttu-id="afaf6-p119">不支持 `@odata.bind`。也就是说，开发者无法正确地在组上设置 `Accepted` 或 `RejectedSenders`。</span><span class="sxs-lookup"><span data-stu-id="afaf6-p119">`@odata.bind` is not supported.  This means that developers won’t be able to properly set the `Accepted` or `RejectedSenders` on a group.</span></span>
* <span data-ttu-id="afaf6-214">使用极少的元数据时，非包容导航（如邮件）上不存在 `@odata.id`。</span><span class="sxs-lookup"><span data-stu-id="afaf6-214">`@odata.id` is not present on non-containment navigations (like messages) when using minimal metadata.</span></span>
* <span data-ttu-id="afaf6-215">`$expand`:</span><span class="sxs-lookup"><span data-stu-id="afaf6-215">`$expand`:</span></span>
  * <span data-ttu-id="afaf6-216">不支持 `nextLink`</span><span class="sxs-lookup"><span data-stu-id="afaf6-216">No support for `nextLink`</span></span>
  * <span data-ttu-id="afaf6-217">不支持 1 级以上扩展</span><span class="sxs-lookup"><span data-stu-id="afaf6-217">No support for more than 1 level of expand</span></span>
  * <span data-ttu-id="afaf6-218">不支持其他参数（`$filter`、`$select`）</span><span class="sxs-lookup"><span data-stu-id="afaf6-218">No support with extra parameters (`$filter`, `$select`)</span></span>
* <span data-ttu-id="afaf6-219">`$filter`:</span><span class="sxs-lookup"><span data-stu-id="afaf6-219">`$filter`:</span></span>
  * <span data-ttu-id="afaf6-220">`/attachments` 终结点不支持筛选器。</span><span class="sxs-lookup"><span data-stu-id="afaf6-220">`/attachments` endpoint does not support filters.</span></span> <span data-ttu-id="afaf6-221">如果存在，将忽略 `$filter` 参数。</span><span class="sxs-lookup"><span data-stu-id="afaf6-221">If present, the `$filter` parameter is ignored.</span></span>
  * <span data-ttu-id="afaf6-222">不支持跨工作负载筛选。</span><span class="sxs-lookup"><span data-stu-id="afaf6-222">Cross-workload filtering is not supported.</span></span>
* <span data-ttu-id="afaf6-223">`$search`:</span><span class="sxs-lookup"><span data-stu-id="afaf6-223">`$search`:</span></span>
  * <span data-ttu-id="afaf6-224">全文搜索仅对实体子集（如邮件）可用。</span><span class="sxs-lookup"><span data-stu-id="afaf6-224">Full-text search is only available for a subset of entities such as messages.</span></span>
  * <span data-ttu-id="afaf6-225">不支持跨工作负载搜索。</span><span class="sxs-lookup"><span data-stu-id="afaf6-225">Cross-workload searching is not supported.</span></span>

## <a name="delta-query"></a><span data-ttu-id="afaf6-226">Delta 查询</span><span class="sxs-lookup"><span data-stu-id="afaf6-226">Delta query</span></span>

* <span data-ttu-id="afaf6-227">跟踪关系更改时，OData 上下文有时无法正确返回。</span><span class="sxs-lookup"><span data-stu-id="afaf6-227">OData context is sometimes returned incorrectly when tracking changes to relationships.</span></span>
* <span data-ttu-id="afaf6-228">架构扩展（旧版）未使用 $select 语句返回，而是在无 $select 的情况下返回。</span><span class="sxs-lookup"><span data-stu-id="afaf6-228">Schema extensions (legacy) are not returned with $select statement, but are returned without $select.</span></span>
* <span data-ttu-id="afaf6-229">客户端无法跟踪开放扩展或已注册架构扩展的变化。</span><span class="sxs-lookup"><span data-stu-id="afaf6-229">Clients cannot track changes to open extensions or registered schema extensions.</span></span>

## <a name="application-and-serviceprincipal-api-changes"></a><span data-ttu-id="afaf6-230">应用程序和 servicePrincipal API 更改</span><span class="sxs-lookup"><span data-stu-id="afaf6-230">Application and servicePrincipal API changes</span></span>

<span data-ttu-id="afaf6-p121">当前处于开发阶段的 [application](../api-reference/beta/resources/application.md) 和 [servicePrincipal](../api-reference/beta/resources/serviceprincipal.md) 实体有变化。下面总结了当前限制和处于开发阶段的 API 功能。</span><span class="sxs-lookup"><span data-stu-id="afaf6-p121">There are changes to the [application](../api-reference/beta/resources/application.md) and [servicePrincipal](../api-reference/beta/resources/serviceprincipal.md) entities currently in development. The following is a summary of current limitations and in-development API features.</span></span>

<span data-ttu-id="afaf6-233">当前限制：</span><span class="sxs-lookup"><span data-stu-id="afaf6-233">Current limitations:</span></span>

* <span data-ttu-id="afaf6-234">只有在所有更改完成后，一些应用属性（如 appRoles 和 addIns）才可用。</span><span class="sxs-lookup"><span data-stu-id="afaf6-234">Some application properties (such as appRoles and addIns) will not be available until all changes are completed.</span></span>
* <span data-ttu-id="afaf6-235">只能注册多租户应用。</span><span class="sxs-lookup"><span data-stu-id="afaf6-235">Only multi-tenant apps can be registered.</span></span>
* <span data-ttu-id="afaf6-236">更新应用仅限于在首次 beta更新后注册的应用。</span><span class="sxs-lookup"><span data-stu-id="afaf6-236">Updating apps is restricted to apps registered after the initial beta update.</span></span>
* <span data-ttu-id="afaf6-237">Azure Active Directory 用户可以注册应用并添加其他所有者。</span><span class="sxs-lookup"><span data-stu-id="afaf6-237">Azure Active Directory users can register apps and add additional owners.</span></span>
* <span data-ttu-id="afaf6-238">支持 OpenID Connect 和 OAuth 协议。</span><span class="sxs-lookup"><span data-stu-id="afaf6-238">Support for OpenID Connect and OAuth protocols.</span></span>
* <span data-ttu-id="afaf6-239">无法向应用分配策略。</span><span class="sxs-lookup"><span data-stu-id="afaf6-239">Policy assignments to an application fail.</span></span>
* <span data-ttu-id="afaf6-240">无法对需要 appId 的 ownedObjects 执行操作（例如，users/{id|userPrincipalName}/ownedObjects/{id}/...）</span><span class="sxs-lookup"><span data-stu-id="afaf6-240">Operations on ownedObjects that require appId fail (For example, users/{id|userPrincipalName}/ownedObjects/{id}/...).</span></span>

<span data-ttu-id="afaf6-241">处于开发阶段的功能：</span><span class="sxs-lookup"><span data-stu-id="afaf6-241">In development:</span></span>

* <span data-ttu-id="afaf6-242">可以注册单租户应用。</span><span class="sxs-lookup"><span data-stu-id="afaf6-242">Ability to register single tenant apps.</span></span>
* <span data-ttu-id="afaf6-243">更新 servicePrincipal。</span><span class="sxs-lookup"><span data-stu-id="afaf6-243">Updates to servicePrincipal.</span></span>
* <span data-ttu-id="afaf6-244">将现有 Azure AD 应用迁移到更新后的模型中。</span><span class="sxs-lookup"><span data-stu-id="afaf6-244">Migration of existing Azure AD apps to updated model.</span></span>
* <span data-ttu-id="afaf6-245">支持 appRoles、预授权客户端、可选声明、组成员身份声明和品牌塑造</span><span class="sxs-lookup"><span data-stu-id="afaf6-245">Support for appRoles, pre-authorized clients, optional claims, group membership claims, and branding</span></span>
* <span data-ttu-id="afaf6-246">Microsoft 帐户 (MSA) 用户可以注册应用。</span><span class="sxs-lookup"><span data-stu-id="afaf6-246">Microsoft account (MSA) users can register apps.</span></span>
* <span data-ttu-id="afaf6-247">支持 SAML 和 WsFed 协议。</span><span class="sxs-lookup"><span data-stu-id="afaf6-247">Support for SAML and WsFed protocols.</span></span>

## <a name="extensions"></a><span data-ttu-id="afaf6-248">扩展</span><span class="sxs-lookup"><span data-stu-id="afaf6-248">Extensions</span></span>

### <a name="change-tracking-is-not-supported"></a><span data-ttu-id="afaf6-249">不支持更改跟踪</span><span class="sxs-lookup"><span data-stu-id="afaf6-249">Change tracking is not supported</span></span>

<span data-ttu-id="afaf6-250">开放扩展或架构扩展属性不支持更改跟踪（Delta 查询）。</span><span class="sxs-lookup"><span data-stu-id="afaf6-250">Change tracking (delta query) is not supported for open or schema extension properties.</span></span>

### <a name="creating-a-resource-and-open-extension-at-the-same-time"></a><span data-ttu-id="afaf6-251">同时创建资源和开放扩展</span><span class="sxs-lookup"><span data-stu-id="afaf6-251">Creating a resource and open extension at the same time</span></span>

<span data-ttu-id="afaf6-p122">无法在创建**管理单元**、**设备**、**组**、**组织**或**用户**的实例的同时指定开放扩展。必须首先创建实例，然后在该实例的后续 ``POST`` 请求中指定开放扩展数据。</span><span class="sxs-lookup"><span data-stu-id="afaf6-p122">You cannot specify an open extension at the same time you create an instance of **administrativeUnit**, **device**, **group**, **organization** or **user**. You must first create the instance and then specify the open extension data in a subsequent ``POST`` request on that instance.</span></span>

### <a name="creating-a-resource-instance-and-adding-schema-extension-data-at-the-same-time"></a><span data-ttu-id="afaf6-254">创建资源实例的同时添加架构扩展数据</span><span class="sxs-lookup"><span data-stu-id="afaf6-254">Creating a resource instance and adding schema extension data at the same time</span></span>

<span data-ttu-id="afaf6-255">不能在创建 **contact**、**event**、**message** 或 **post** 实例的同一个操作中指定架构扩展。</span><span class="sxs-lookup"><span data-stu-id="afaf6-255">You cannot specify a schema extension in the same operation as creating an instance of **contact**, **event**, **message**, or **post**.</span></span>
<span data-ttu-id="afaf6-256">必须先创建资源实例，然后再对此实例执行 `PATCH`，从而添加架构扩展和自定义数据。</span><span class="sxs-lookup"><span data-stu-id="afaf6-256">You must first create the resource instance and then do a `PATCH` to that instance to add a schema extension and custom data.</span></span>

### <a name="limit-of-100-schema-extension-property-values-allowed-per-resource-instance"></a><span data-ttu-id="afaf6-257">每资源实例最多可以添加 100 个架构扩展属性值</span><span class="sxs-lookup"><span data-stu-id="afaf6-257">Limit of 100 schema extension property values allowed per resource instance</span></span>

<span data-ttu-id="afaf6-258">目录资源（如**设备**、**组**和**用户**）目前将可在资源实例上设置的架构扩展属性值的总数限制为 100。</span><span class="sxs-lookup"><span data-stu-id="afaf6-258">Directory resources, such as **device**, **group** and **user**, currently limit the total number of schema extension property values that can be set on a resource instance, to 100.</span></span>

### <a name="filtering-on-schema-extension-properties-not-supported-on-all-entity-types"></a><span data-ttu-id="afaf6-259">并非所有实体类型都支持对架构扩展属性进行筛选</span><span class="sxs-lookup"><span data-stu-id="afaf6-259">Filtering on schema extension properties not supported on all entity types</span></span>

<span data-ttu-id="afaf6-260">Outlook 实体类型不支持对架构扩展属性进行筛选（使用 `$filter` 表达式）- **联系人**、**事件**、**消息**或**帖子**。</span><span class="sxs-lookup"><span data-stu-id="afaf6-260">Filtering on schema extension properties (using the `$filter` expresssion) is not supported for Outlook entity types - **contact**, **event**, **message**, or **post**.</span></span>

## <a name="json-batching"></a><span data-ttu-id="afaf6-261">JSON 批处理</span><span class="sxs-lookup"><span data-stu-id="afaf6-261">JSON Batching</span></span>

### <a name="no-nested-batch"></a><span data-ttu-id="afaf6-262">无嵌套批处理</span><span class="sxs-lookup"><span data-stu-id="afaf6-262">No nested batch</span></span>

<span data-ttu-id="afaf6-263">JSON 批处理请求中不得包含任何嵌套批处理请求。</span><span class="sxs-lookup"><span data-stu-id="afaf6-263">JSON batch requests must not contain any nested batch requests.</span></span>

### <a name="all-individual-requests-must-be-synchronous"></a><span data-ttu-id="afaf6-264">所有单个请求必须同步</span><span class="sxs-lookup"><span data-stu-id="afaf6-264">All individual requests must be synchronous</span></span>

<span data-ttu-id="afaf6-p124">批处理请求中包含的所有请求都必须同步执行。如果存在，将忽略 `respond-async` 首选项。</span><span class="sxs-lookup"><span data-stu-id="afaf6-p124">All requests contained in a batch request must be executed synchronously. If present, the `respond-async` preference will be ignored.</span></span>

### <a name="no-transactions"></a><span data-ttu-id="afaf6-267">无事务</span><span class="sxs-lookup"><span data-stu-id="afaf6-267">No transactions</span></span>

<span data-ttu-id="afaf6-p125">Microsoft Graph 当前不支持单个请求的事务处理。将忽略单个请求的 `atomicityGroup` 属性。</span><span class="sxs-lookup"><span data-stu-id="afaf6-p125">Microsoft Graph does not currently support transactional processing of individual requests. The `atomicityGroup` property on individual requests will be ignored.</span></span>

### <a name="uris-must-be-relative"></a><span data-ttu-id="afaf6-270">URI 必须相对</span><span class="sxs-lookup"><span data-stu-id="afaf6-270">URIs must be relative</span></span>

<span data-ttu-id="afaf6-p126">始终在批处理请求中指定相对的 URI。Microsoft Graph 将使用批处理 URL 中包含的版本终结点使这些 URL 绝对。</span><span class="sxs-lookup"><span data-stu-id="afaf6-p126">Always specify relative URIs in batch requests. Microsoft Graph then makes these URLs absolute by using the version endpoint included in the batch URL.</span></span>

### <a name="limit-on-batch-size"></a><span data-ttu-id="afaf6-273">限制批处理大小</span><span class="sxs-lookup"><span data-stu-id="afaf6-273">Limit on batch size</span></span>

<span data-ttu-id="afaf6-274">JSON 批处理请求目前限定为 20 个单独请求。</span><span class="sxs-lookup"><span data-stu-id="afaf6-274">JSON batch requests are currently limited to 20 individual requests.</span></span>

### <a name="simplified-dependencies"></a><span data-ttu-id="afaf6-275">简化的依赖项</span><span class="sxs-lookup"><span data-stu-id="afaf6-275">Simplified dependencies</span></span>

<span data-ttu-id="afaf6-p127">单独请求可以依赖其他单独请求。目前，请求只能依赖于单个其他请求，并且必须遵循下面的三种模式之一：</span><span class="sxs-lookup"><span data-stu-id="afaf6-p127">Individual requests can depend on other individual requests. Currently, requests can only depend on a single other request, and must follow one of these three patterns:</span></span>

1. <span data-ttu-id="afaf6-278">平行 - 没有单独的请求在 `dependsOn` 属性中声明依赖项。</span><span class="sxs-lookup"><span data-stu-id="afaf6-278">Parallel - no individual request states a dependency in the `dependsOn` property.</span></span>
2. <span data-ttu-id="afaf6-279">串行 - 所有单独请求都依赖于之前的单独请求。</span><span class="sxs-lookup"><span data-stu-id="afaf6-279">Serial - all individual requests depend on the previous individual request.</span></span>
3. <span data-ttu-id="afaf6-280">相同 - 在 `dependsOn` 属性中声明依赖项的所有单独请求均声明了相同的依赖项。</span><span class="sxs-lookup"><span data-stu-id="afaf6-280">Same - all individual requests that state a dependency in the `dependsOn` property, state the same dependency.</span></span>

<span data-ttu-id="afaf6-281">随着 JSON 批处理技术日臻成熟，这些限制将会被取消。</span><span class="sxs-lookup"><span data-stu-id="afaf6-281">As JSON batching matures, these limitations will be removed.</span></span>

## <a name="cloud-solution-provider-apps"></a><span data-ttu-id="afaf6-282">云解决方案提供商应用</span><span class="sxs-lookup"><span data-stu-id="afaf6-282">Cloud Solution Provider apps</span></span>

### <a name="csp-apps-must-use-azure-ad-endpoint"></a><span data-ttu-id="afaf6-283">CSP 应用必须使用 Azure AD 终结点</span><span class="sxs-lookup"><span data-stu-id="afaf6-283">CSP apps must use Azure AD endpoint</span></span>

<span data-ttu-id="afaf6-p128">云解决方案提供商 (CSP) 应用必须从 Azure AD (v1) 终结点中获取令牌，才能在其合作伙伴托管的客户中成功调用 Microsoft Graph。目前，不支持通过较新的 Azure AD v2.0 终结点获取令牌。</span><span class="sxs-lookup"><span data-stu-id="afaf6-p128">Cloud solution provider (CSP) apps must acquire tokens from the Azure AD (v1) endpoints to successfully call Microsoft Graph in their partner-managed customers. Currently, acquiring a token through the newer Azure AD v2.0 endpoint is not supported.</span></span>

### <a name="pre-consent-for-csp-apps-doesnt-work-in-some-customer-tenants"></a><span data-ttu-id="afaf6-286">对 CSP 应用的预授权不适用于一些客户租户</span><span class="sxs-lookup"><span data-stu-id="afaf6-286">Pre-consent for CSP apps doesn't work in some customer tenants</span></span>

<span data-ttu-id="afaf6-287">在某些情况下，对 CSP 应用的预授权可能不适用于一些客户租户。</span><span class="sxs-lookup"><span data-stu-id="afaf6-287">Under certain circumstances, pre-consent for CSP apps may not work for some of your customer tenants.</span></span>

- <span data-ttu-id="afaf6-288">对于使用委派权限的应用，首次将此应用用于新客户租户时，登录后可能会看到以下错误：`AADSTS50000: There was an error issuing a token`。</span><span class="sxs-lookup"><span data-stu-id="afaf6-288">For apps using delegated permissions, when using the app for the first time with a new customer tenant you might receive this error after sign-in: `AADSTS50000: There was an error issuing a token`.</span></span>
- <span data-ttu-id="afaf6-289">对于使用应用权限的应用，应用可以获取令牌，但在调用 Microsoft Graph 时会意外看到“拒绝访问”消息。</span><span class="sxs-lookup"><span data-stu-id="afaf6-289">For apps using application permissions, your app can acquire a token, but unexpectedly gets an access denied message when calling Microsoft Graph.</span></span>

<span data-ttu-id="afaf6-290">我们正在努力工作，以尽快解决此问题，让预授权适用于所有客户租户。</span><span class="sxs-lookup"><span data-stu-id="afaf6-290">We are working to fix this issue as soon as possible, so that pre-consent will work for all your customer tenants.</span></span>

<span data-ttu-id="afaf6-291">同时，若要取消阻止开发和测试，可使用以下解决方法。</span><span class="sxs-lookup"><span data-stu-id="afaf6-291">In the meantime, to unblock development and testing you can use the following workaround.</span></span>

><span data-ttu-id="afaf6-p129">**注意：** 这不是永久性解决方案，仅用于取消阻止开发。一旦上述问题得到解决，便无需使用此解决方案。在问题得到解决后，无需撤消此解决方法。</span><span class="sxs-lookup"><span data-stu-id="afaf6-p129">**NOTE:** This is not a permanent solution and is only intended to unblock development.  This workaround will not be required once the aforementioned issue is fixed.  This workaround does not need to be undone once the fix is in place.</span></span>

1. <span data-ttu-id="afaf6-p130">打开 Azure AD v2 PowerShell 会话，然后在登录窗口中输入管理员凭据，以连接 `customer` 租户。可以单击[此处](https://www.powershellgallery.com/packages/AzureAD)，下载并安装 Azure AD PowerShell V2。</span><span class="sxs-lookup"><span data-stu-id="afaf6-p130">Open an Azure AD v2 PowerShell session and connect to your `customer` tenant by entering your admin credentials into the sign-in window. You can download and install Azure AD PowerShell V2 from [here](https://www.powershellgallery.com/packages/AzureAD).</span></span>

    ```PowerShell
    Connect-AzureAd -TenantId {customerTenantIdOrDomainName}
    ```

2. <span data-ttu-id="afaf6-297">创建 Microsoft Graph 服务主体。</span><span class="sxs-lookup"><span data-stu-id="afaf6-297">Create the Microsoft Graph service principal.</span></span>

    ```PowerShell
    New-AzureADServicePrincipal -AppId 00000003-0000-0000-c000-000000000000
    ```

## <a name="functionality-available-only-in-office-365-rest-or-azure-ad-graph-apis"></a><span data-ttu-id="afaf6-298">只有 Office 365 REST 或 Azure AD Graph API 才具有的功能</span><span class="sxs-lookup"><span data-stu-id="afaf6-298">Functionality available only in Office 365 REST or Azure AD Graph APIs</span></span>

<span data-ttu-id="afaf6-p131">某些功能尚未在 Microsoft Graph 中提供。如果找不到所需的功能，请使用特定于终结点的 [Office 365 REST API](https://msdn.microsoft.com/zh-CN/office/office365/api/api-catalog)。有关 Azure Active Directory，请参考 [Microsoft Graph 或 Azure AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) 博客文章，获取只能通过 Azure AD Graph API 提供的功能。</span><span class="sxs-lookup"><span data-stu-id="afaf6-p131">Some functionality is not yet available in Microsoft Graph. If you don't see the functionality you're looking for, you can use the endpoint-specific [Office 365 REST APIs](https://msdn.microsoft.com/zh-CN/office/office365/api/api-catalog). For Azure Active Directory, please refer to the [Microsoft Graph or Azure AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) blog post on the features that are only available through Azure AD Graph API.</span></span>

## <a name="feedback"></a><span data-ttu-id="afaf6-302">反馈</span><span class="sxs-lookup"><span data-stu-id="afaf6-302">Feedback</span></span>

> <span data-ttu-id="afaf6-p132">我们非常重视你的反馈意见。请在 [Stack Overflow](http://stackoverflow.com/questions/tagged/microsoftgraph) 上与我们联系。</span><span class="sxs-lookup"><span data-stu-id="afaf6-p132">Your feedback is important to us. Connect with us on [Stack Overflow](http://stackoverflow.com/questions/tagged/microsoftgraph).</span></span>
