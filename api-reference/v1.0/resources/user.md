# <a name="user-resource-type"></a><span data-ttu-id="711a2-101">用户资源类型</span><span class="sxs-lookup"><span data-stu-id="711a2-101">user resource type</span></span>

<span data-ttu-id="711a2-p101">表示 Azure AD 用户帐户。继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="711a2-p101">Represents an Azure AD user account. Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="711a2-104">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="711a2-104">This resource supports:</span></span>

- <span data-ttu-id="711a2-105">使用[扩展](../../../concepts/extensibility_overview.md)将自己的数据添加到自定义属性。</span><span class="sxs-lookup"><span data-stu-id="711a2-105">Adding your own data to custom properties using [extensions](../../../concepts/extensibility_overview.md).</span></span>
- <span data-ttu-id="711a2-106">通过提供 [delta](../api/user_delta.md) 函数使用[增量查询](../../../concepts/delta_query_overview.md)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="711a2-106">Using [delta query](../../../concepts/delta_query_overview.md) to track incremental additions, deletions, and updates, by providing a [delta](../api/user_delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="711a2-107">方法</span><span class="sxs-lookup"><span data-stu-id="711a2-107">Methods</span></span>

| <span data-ttu-id="711a2-108">方法</span><span class="sxs-lookup"><span data-stu-id="711a2-108">Method</span></span>       | <span data-ttu-id="711a2-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="711a2-109">Return Type</span></span>  |<span data-ttu-id="711a2-110">说明</span><span class="sxs-lookup"><span data-stu-id="711a2-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="711a2-111">列举用户</span><span class="sxs-lookup"><span data-stu-id="711a2-111">List users</span></span>](../api/user_list.md) |<span data-ttu-id="711a2-112">[user](user.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-112">[user](user.md) collection</span></span>| <span data-ttu-id="711a2-113">获取用户对象列表。</span><span class="sxs-lookup"><span data-stu-id="711a2-113">Get a list of user objects.</span></span>|
|[<span data-ttu-id="711a2-114">创建用户</span><span class="sxs-lookup"><span data-stu-id="711a2-114">Create user</span></span>](../api/user_post_users.md) |[<span data-ttu-id="711a2-115">用户</span><span class="sxs-lookup"><span data-stu-id="711a2-115">user</span></span>](user.md)| <span data-ttu-id="711a2-116">新建用户对象。</span><span class="sxs-lookup"><span data-stu-id="711a2-116">Create a new user object.</span></span>|
|[<span data-ttu-id="711a2-117">获取用户</span><span class="sxs-lookup"><span data-stu-id="711a2-117">Get user</span></span>](../api/user_get.md) | [<span data-ttu-id="711a2-118">用户</span><span class="sxs-lookup"><span data-stu-id="711a2-118">user</span></span>](user.md) |<span data-ttu-id="711a2-119">读取 user 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="711a2-119">Read properties and relationships of user object.</span></span>|
|[<span data-ttu-id="711a2-120">更新用户</span><span class="sxs-lookup"><span data-stu-id="711a2-120">Update user</span></span>](../api/user_update.md) | [<span data-ttu-id="711a2-121">用户</span><span class="sxs-lookup"><span data-stu-id="711a2-121">user</span></span>](user.md) |<span data-ttu-id="711a2-122">更新 user 对象。</span><span class="sxs-lookup"><span data-stu-id="711a2-122">Update user object.</span></span> |
|[<span data-ttu-id="711a2-123">删除用户</span><span class="sxs-lookup"><span data-stu-id="711a2-123">Delete user</span></span>](../api/user_delete.md) | <span data-ttu-id="711a2-124">无</span><span class="sxs-lookup"><span data-stu-id="711a2-124">None</span></span> |<span data-ttu-id="711a2-125">删除 user 对象。</span><span class="sxs-lookup"><span data-stu-id="711a2-125">Delete user object.</span></span> |
|[<span data-ttu-id="711a2-126">列举消息</span><span class="sxs-lookup"><span data-stu-id="711a2-126">List messages</span></span>](../api/user_list_messages.md) |<span data-ttu-id="711a2-127">[消息](message.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-127">[Message](message.md) collection</span></span>| <span data-ttu-id="711a2-128">获取已登录用户的邮箱中的所有邮件。</span><span class="sxs-lookup"><span data-stu-id="711a2-128">Get all the messages in the signed-in user's mailbox.</span></span>|
|[<span data-ttu-id="711a2-129">创建消息</span><span class="sxs-lookup"><span data-stu-id="711a2-129">Create Message</span></span>](../api/user_post_messages.md) |[<span data-ttu-id="711a2-130">消息</span><span class="sxs-lookup"><span data-stu-id="711a2-130">Message</span></span>](message.md)| <span data-ttu-id="711a2-131">通过发布到邮件集合新建邮件。</span><span class="sxs-lookup"><span data-stu-id="711a2-131">Create a new Message by posting to the messages collection.</span></span>|
|[<span data-ttu-id="711a2-132">列举 mailFolders</span><span class="sxs-lookup"><span data-stu-id="711a2-132">List mailFolders</span></span>](../api/user_list_mailfolders.md) |<span data-ttu-id="711a2-133">[MailFolder](mailfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-133">[MailFolder](mailfolder.md) collection</span></span>| <span data-ttu-id="711a2-134">在已登录用户的根文件夹下获取邮件文件夹集合。</span><span class="sxs-lookup"><span data-stu-id="711a2-134">Get the mail folder collection under the root folder of the signed-in user.</span></span> |
|[<span data-ttu-id="711a2-135">创建 mailFolder</span><span class="sxs-lookup"><span data-stu-id="711a2-135">Create mailFolder</span></span>](../api/user_post_mailfolders.md) |[<span data-ttu-id="711a2-136">MailFolder</span><span class="sxs-lookup"><span data-stu-id="711a2-136">MailFolder</span></span>](mailfolder.md)| <span data-ttu-id="711a2-137">通过发布到 mailFolders 集合创建新 MailFolder。</span><span class="sxs-lookup"><span data-stu-id="711a2-137">Create a new MailFolder by posting to the mailFolders collection.</span></span>|
|[<span data-ttu-id="711a2-138">sendMail</span><span class="sxs-lookup"><span data-stu-id="711a2-138">sendMail</span></span>](../api/user_sendmail.md)|<span data-ttu-id="711a2-139">无</span><span class="sxs-lookup"><span data-stu-id="711a2-139">None</span></span>|<span data-ttu-id="711a2-140">发送请求正文中指定的邮件。</span><span class="sxs-lookup"><span data-stu-id="711a2-140">Send the message specified in the request body.</span></span>|
|[<span data-ttu-id="711a2-141">列举事件</span><span class="sxs-lookup"><span data-stu-id="711a2-141">List events</span></span>](../api/user_list_events.md) |<span data-ttu-id="711a2-142">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-142">[Event](event.md) collection</span></span>| <span data-ttu-id="711a2-p102">获取用户邮箱中的 event 对象列表。该列表包含单个实例会议和系列主控形状。</span><span class="sxs-lookup"><span data-stu-id="711a2-p102">Get a list of event objects in the user's mailbox. The list contains single instance meetings and series masters.</span></span>|
|[<span data-ttu-id="711a2-145">创建事件</span><span class="sxs-lookup"><span data-stu-id="711a2-145">Create event</span></span>](../api/user_post_events.md) |[<span data-ttu-id="711a2-146">事件</span><span class="sxs-lookup"><span data-stu-id="711a2-146">Event</span></span>](event.md)| <span data-ttu-id="711a2-147">通过发布到事件集合创建新事件。</span><span class="sxs-lookup"><span data-stu-id="711a2-147">Create a new Event by posting to the events collection.</span></span>|
|[<span data-ttu-id="711a2-148">列举日历</span><span class="sxs-lookup"><span data-stu-id="711a2-148">List calendars</span></span>](../api/user_list_calendars.md) |<span data-ttu-id="711a2-149">[日历](calendar.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-149">[Calendar](calendar.md) collection</span></span>| <span data-ttu-id="711a2-150">获取 Calendar 对象集合。</span><span class="sxs-lookup"><span data-stu-id="711a2-150">Get a Calendar object collection.</span></span>|
|[<span data-ttu-id="711a2-151">创建日历</span><span class="sxs-lookup"><span data-stu-id="711a2-151">Create calendar</span></span>](../api/user_post_calendars.md) |[<span data-ttu-id="711a2-152">日历</span><span class="sxs-lookup"><span data-stu-id="711a2-152">Calendar</span></span>](calendar.md)| <span data-ttu-id="711a2-153">通过发布到日历集合创建新日历。</span><span class="sxs-lookup"><span data-stu-id="711a2-153">Create a new Calendar by posting to the calendars collection.</span></span>|
|[<span data-ttu-id="711a2-154">列举 calendarGroups</span><span class="sxs-lookup"><span data-stu-id="711a2-154">List calendarGroups</span></span>](../api/user_list_calendargroups.md) |<span data-ttu-id="711a2-155">[CalendarGroup](calendargroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-155">[CalendarGroup](calendargroup.md) collection</span></span>| <span data-ttu-id="711a2-156">获取 CalendarGroup 对象集合。</span><span class="sxs-lookup"><span data-stu-id="711a2-156">Get a CalendarGroup object collection.</span></span>|
|[<span data-ttu-id="711a2-157">创建 calendarGroup</span><span class="sxs-lookup"><span data-stu-id="711a2-157">Create calendarGroup</span></span>](../api/user_post_calendargroups.md) |[<span data-ttu-id="711a2-158">CalendarGroup</span><span class="sxs-lookup"><span data-stu-id="711a2-158">CalendarGroup</span></span>](calendargroup.md)| <span data-ttu-id="711a2-159">通过发布到 calendarGroups 集合新建 CalendarGroup。</span><span class="sxs-lookup"><span data-stu-id="711a2-159">Create a new CalendarGroup by posting to the calendarGroups collection.</span></span>|
|[<span data-ttu-id="711a2-160">列举 calendarView</span><span class="sxs-lookup"><span data-stu-id="711a2-160">List calendarView</span></span>](../api/user_list_calendarview.md) |<span data-ttu-id="711a2-161">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-161">[Event](event.md) collection</span></span>| <span data-ttu-id="711a2-162">获取 Event 对象集合。</span><span class="sxs-lookup"><span data-stu-id="711a2-162">Get a Event object collection.</span></span>|
|[<span data-ttu-id="711a2-163">列举联系人</span><span class="sxs-lookup"><span data-stu-id="711a2-163">List contacts</span></span>](../api/user_list_contacts.md) |<span data-ttu-id="711a2-164">[联系人](contact.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-164">[Contact](contact.md) collection</span></span>| <span data-ttu-id="711a2-165">从已登录用户的默认联系人文件夹中获取联系人集合。</span><span class="sxs-lookup"><span data-stu-id="711a2-165">Get a contact collection from the default Contacts folder of the signed-in user.</span></span>|
|[<span data-ttu-id="711a2-166">创建联系人</span><span class="sxs-lookup"><span data-stu-id="711a2-166">Create Contact</span></span>](../api/user_post_contacts.md) |[<span data-ttu-id="711a2-167">联系人</span><span class="sxs-lookup"><span data-stu-id="711a2-167">Contact</span></span>](contact.md)| <span data-ttu-id="711a2-168">通过发布到联系人集合新建联系人。</span><span class="sxs-lookup"><span data-stu-id="711a2-168">Create a new Contact by posting to the contacts collection.</span></span>|
|[<span data-ttu-id="711a2-169">列举 contactFolders</span><span class="sxs-lookup"><span data-stu-id="711a2-169">List contactFolders</span></span>](../api/user_list_contactfolders.md) |<span data-ttu-id="711a2-170">[ContactFolder](contactfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-170">[ContactFolder](contactfolder.md) collection</span></span>| <span data-ttu-id="711a2-171">获取已登录用户的默认联系人文件夹中的联系人文件夹集合。</span><span class="sxs-lookup"><span data-stu-id="711a2-171">Get the contact folder collection in the default Contacts folder of the signed-in user.</span></span>|
|[<span data-ttu-id="711a2-172">创建 ContactFolder</span><span class="sxs-lookup"><span data-stu-id="711a2-172">Create ContactFolder</span></span>](../api/user_post_contactfolders.md) |[<span data-ttu-id="711a2-173">ContactFolder</span><span class="sxs-lookup"><span data-stu-id="711a2-173">ContactFolder</span></span>](contactfolder.md)| <span data-ttu-id="711a2-174">通过发布到 contactFolders 集合创建新 ContactFolder。</span><span class="sxs-lookup"><span data-stu-id="711a2-174">Create a new ContactFolder by posting to the contactFolders collection.</span></span>|
|[<span data-ttu-id="711a2-175">列举 directReports</span><span class="sxs-lookup"><span data-stu-id="711a2-175">List directReports</span></span>](../api/user_list_directreports.md) |<span data-ttu-id="711a2-176">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-176">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="711a2-177">从 directReports 导航属性中获取向此用户报告的用户和联系人。</span><span class="sxs-lookup"><span data-stu-id="711a2-177">Get the users and contacts that report to the user from the directReports navigation property.</span></span>|
|[<span data-ttu-id="711a2-178">列举管理员</span><span class="sxs-lookup"><span data-stu-id="711a2-178">List manager</span></span>](../api/user_list_manager.md) |[<span data-ttu-id="711a2-179">directoryObject</span><span class="sxs-lookup"><span data-stu-id="711a2-179">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="711a2-180">从 manager 导航属性中获取是此用户的经理的用户或联系人。</span><span class="sxs-lookup"><span data-stu-id="711a2-180">Get the user or contact that is this user's manager from the manager navigation property.</span></span>|
|[<span data-ttu-id="711a2-181">列举 memberOf</span><span class="sxs-lookup"><span data-stu-id="711a2-181">List memberOf</span></span>](../api/user_list_memberof.md) |<span data-ttu-id="711a2-182">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-182">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="711a2-183">从 memberOf 导航属性中获取此用户是其直接成员的组和目录角色。</span><span class="sxs-lookup"><span data-stu-id="711a2-183">Get the groups and directory roles that the user is a direct member of from the memberOf navigation property.</span></span>|
|[<span data-ttu-id="711a2-184">列举 ownedDevices</span><span class="sxs-lookup"><span data-stu-id="711a2-184">List ownedDevices</span></span>](../api/user_list_owneddevices.md) |<span data-ttu-id="711a2-185">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-185">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="711a2-186">从 ownedDevices 导航属性中获取此用户所拥有的设备。</span><span class="sxs-lookup"><span data-stu-id="711a2-186">Get the devices that are owned by the user from the ownedDevices navigation property.</span></span>|
|[<span data-ttu-id="711a2-187">列举 ownedObjects</span><span class="sxs-lookup"><span data-stu-id="711a2-187">List ownedObjects</span></span>](../api/user_list_ownedobjects.md) |<span data-ttu-id="711a2-188">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-188">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="711a2-189">从 ownedObjects 导航属性中获取此用户所拥有的目录对象。</span><span class="sxs-lookup"><span data-stu-id="711a2-189">Get the directory objects that are owned by the user from the ownedObjects navigation property.</span></span>|
|[<span data-ttu-id="711a2-190">列举 registeredDevices</span><span class="sxs-lookup"><span data-stu-id="711a2-190">List registeredDevices</span></span>](../api/user_list_registereddevices.md) |<span data-ttu-id="711a2-191">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-191">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="711a2-192">从 registeredDevices 导航属性中获取为此用户注册的设备。</span><span class="sxs-lookup"><span data-stu-id="711a2-192">Get the devices that are retistered for the user from the registeredDevices navigation property.</span></span>|
|[<span data-ttu-id="711a2-193">列举 createdObjects</span><span class="sxs-lookup"><span data-stu-id="711a2-193">List createdObjects</span></span>](../api/user_list_createdobjects.md) |<span data-ttu-id="711a2-194">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-194">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="711a2-195">从 createdObjects 导航属性中获取此用户创建的目录对象。</span><span class="sxs-lookup"><span data-stu-id="711a2-195">Get the directory objects created by the user from the createdObjects navigation property.</span></span>|
|[<span data-ttu-id="711a2-196">assignLicense</span><span class="sxs-lookup"><span data-stu-id="711a2-196">assignLicense</span></span>](../api/user_assignlicense.md)|[<span data-ttu-id="711a2-197">用户</span><span class="sxs-lookup"><span data-stu-id="711a2-197">user</span></span>](user.md)|<span data-ttu-id="711a2-p103">为用户添加或删除订阅。还可以启用和禁用与订阅相关的特定计划。</span><span class="sxs-lookup"><span data-stu-id="711a2-p103">Add or remove subscriptions for the user. You can also enable and disable specific plans associated with a subscription.</span></span>|
|[<span data-ttu-id="711a2-200">列举 licenseDetails</span><span class="sxs-lookup"><span data-stu-id="711a2-200">List licenseDetails</span></span>](../api/user_list_licensedetails.md) |<span data-ttu-id="711a2-201">[licenseDetails](licensedetails.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-201">[licenseDetails](licensedetails.md) collection</span></span>| <span data-ttu-id="711a2-202">获取 licenseDetails 对象集合。</span><span class="sxs-lookup"><span data-stu-id="711a2-202">Get a licenseDetails object collection.</span></span>|
|[<span data-ttu-id="711a2-203">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="711a2-203">checkMemberGroups</span></span>](../api/user_checkmembergroups.md)|<span data-ttu-id="711a2-204">字符串集合</span><span class="sxs-lookup"><span data-stu-id="711a2-204">String collection</span></span>|<span data-ttu-id="711a2-p104">检查组列表中的成员身份。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="711a2-p104">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="711a2-207">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="711a2-207">getMemberGroups</span></span>](../api/user_getmembergroups.md)|<span data-ttu-id="711a2-208">字符串集合</span><span class="sxs-lookup"><span data-stu-id="711a2-208">String collection</span></span>|<span data-ttu-id="711a2-p105">返回用户是其成员的所有组。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="711a2-p105">Return all the groups that the user is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="711a2-211">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="711a2-211">getMemberObjects</span></span>](../api/user_getmemberobjects.md)|<span data-ttu-id="711a2-212">字符串集合</span><span class="sxs-lookup"><span data-stu-id="711a2-212">String collection</span></span>| <span data-ttu-id="711a2-p106">返回用户所属的所有组和目录角色。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="711a2-p106">Return all of the groups and directory roles that the user is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="711a2-215">reminderView</span><span class="sxs-lookup"><span data-stu-id="711a2-215">reminderView</span></span>](../api/user_reminderview.md)|<span data-ttu-id="711a2-216">[提醒](reminder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-216">[Reminder](reminder.md) collection</span></span>|<span data-ttu-id="711a2-217">返回指定开始时间和结束时间范围内的日历提醒列表。</span><span class="sxs-lookup"><span data-stu-id="711a2-217">Return a list of calendar reminders within the start and end times specified.</span></span>|
|[<span data-ttu-id="711a2-218">增量</span><span class="sxs-lookup"><span data-stu-id="711a2-218">delta</span></span>](../api/user_delta.md)|<span data-ttu-id="711a2-219">用户集合</span><span class="sxs-lookup"><span data-stu-id="711a2-219">user collection</span></span>| <span data-ttu-id="711a2-220">获取用户的增量更改。</span><span class="sxs-lookup"><span data-stu-id="711a2-220">Get incremental changes for users.</span></span> |
|<span data-ttu-id="711a2-221">**开放扩展**</span><span class="sxs-lookup"><span data-stu-id="711a2-221">**Open extensions**</span></span>| | |
|[<span data-ttu-id="711a2-222">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="711a2-222">Create open extension</span></span>](../api/opentypeextension_post_opentypeextension.md) |[<span data-ttu-id="711a2-223">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="711a2-223">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="711a2-224">创建开放扩展，并将自定义属性添加到新资源或现有资源。</span><span class="sxs-lookup"><span data-stu-id="711a2-224">Create an open extension and add custom properties to a new or existing resource.</span></span>|
|[<span data-ttu-id="711a2-225">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="711a2-225">Get open extension</span></span>](../api/opentypeextension_get.md) |<span data-ttu-id="711a2-226">[openTypeExtension](opentypeextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-226">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="711a2-227">获取扩展名称标识的开放扩展。</span><span class="sxs-lookup"><span data-stu-id="711a2-227">Get an open extension identified by the extension name.</span></span>|
|<span data-ttu-id="711a2-228">**架构扩展**</span><span class="sxs-lookup"><span data-stu-id="711a2-228">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="711a2-229">添加架构扩展值</span><span class="sxs-lookup"><span data-stu-id="711a2-229">Add schema extension values</span></span>](../../../concepts/extensibility_schema_groups.md) || <span data-ttu-id="711a2-230">创建架构扩展定义，然后使用它向资源添加自定义键入数据。</span><span class="sxs-lookup"><span data-stu-id="711a2-230">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|

## <a name="properties"></a><span data-ttu-id="711a2-231">属性</span><span class="sxs-lookup"><span data-stu-id="711a2-231">Properties</span></span>

| <span data-ttu-id="711a2-232">属性</span><span class="sxs-lookup"><span data-stu-id="711a2-232">Property</span></span>       | <span data-ttu-id="711a2-233">类型</span><span class="sxs-lookup"><span data-stu-id="711a2-233">Type</span></span>    |<span data-ttu-id="711a2-234">说明</span><span class="sxs-lookup"><span data-stu-id="711a2-234">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="711a2-235">aboutMe</span><span class="sxs-lookup"><span data-stu-id="711a2-235">aboutMe</span></span>|<span data-ttu-id="711a2-236">字符串</span><span class="sxs-lookup"><span data-stu-id="711a2-236">String</span></span>|<span data-ttu-id="711a2-237">任意形式的文本输入字段，用于介绍用户自身。</span><span class="sxs-lookup"><span data-stu-id="711a2-237">A freeform text entry field for the user to describe themselves.</span></span>|
|<span data-ttu-id="711a2-238">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="711a2-238">accountEnabled</span></span>|<span data-ttu-id="711a2-239">布尔</span><span class="sxs-lookup"><span data-stu-id="711a2-239">Boolean</span></span>| <span data-ttu-id="711a2-p107">启用帐户时为 **true**，否则为 **false**。创建用户时此属性是必需的。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="711a2-p107">**true** if the account is enabled; otherwise, **false**. This property is required when a user is created. Supports $filter.</span></span>    |
|<span data-ttu-id="711a2-243">ageGroup</span><span class="sxs-lookup"><span data-stu-id="711a2-243">ageGroup</span></span>|<span data-ttu-id="711a2-244">字符串</span><span class="sxs-lookup"><span data-stu-id="711a2-244">String</span></span>|<span data-ttu-id="711a2-245">设置用户的年龄组。</span><span class="sxs-lookup"><span data-stu-id="711a2-245">Sets the age group of the user.</span></span> <span data-ttu-id="711a2-246">允许值： `null`， `minor`， `notAdult` 和 `adult`。</span><span class="sxs-lookup"><span data-stu-id="711a2-246">Allowed values: `null`, `minor`, `notAdult` and `adult`.</span></span> <span data-ttu-id="711a2-247">请参阅 [法律年龄分组属性定义](#legal-age-group-property-definitions) 以获取详细信息。</span><span class="sxs-lookup"><span data-stu-id="711a2-247">Refer to the [legal age group property definitions](#legal-age-group-property-definitions) for further information.</span></span> |
|<span data-ttu-id="711a2-248">assignedLicenses</span><span class="sxs-lookup"><span data-stu-id="711a2-248">assignedLicenses</span></span>|<span data-ttu-id="711a2-249">[assignedLicense](assignedlicense.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-249">[assignedLicense](assignedlicense.md) collection</span></span>|<span data-ttu-id="711a2-p109">分配给该用户的许可证。不可为 null。</span><span class="sxs-lookup"><span data-stu-id="711a2-p109">The licenses that are assigned to the user. Not nullable.</span></span>            |
|<span data-ttu-id="711a2-252">assignedPlans</span><span class="sxs-lookup"><span data-stu-id="711a2-252">assignedPlans</span></span>|<span data-ttu-id="711a2-253">[assignedPlan](assignedplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-253">[assignedPlan](assignedplan.md) collection</span></span>|<span data-ttu-id="711a2-p110">分配给该用户的计划。只读。不可为 null。</span><span class="sxs-lookup"><span data-stu-id="711a2-p110">The plans that are assigned to the user. Read-only. Not nullable.</span></span> |
|<span data-ttu-id="711a2-257">生日</span><span class="sxs-lookup"><span data-stu-id="711a2-257">birthday</span></span>|<span data-ttu-id="711a2-258">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="711a2-258">DateTimeOffset</span></span>|<span data-ttu-id="711a2-p111">用户的生日。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示： `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="711a2-p111">The birthday of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="711a2-262">businessPhones</span><span class="sxs-lookup"><span data-stu-id="711a2-262">businessPhones</span></span>|<span data-ttu-id="711a2-263">字符串集合</span><span class="sxs-lookup"><span data-stu-id="711a2-263">String collection</span></span>|<span data-ttu-id="711a2-p112">用户的电话号码。注意：虽然这是字符串集合，但是只能为该属性设置一个号码。</span><span class="sxs-lookup"><span data-stu-id="711a2-p112">The telephone numbers for the user. NOTE: Although this is a string collection, only one number can be set for this property.</span></span>|
|<span data-ttu-id="711a2-266">城市</span><span class="sxs-lookup"><span data-stu-id="711a2-266">city</span></span>|<span data-ttu-id="711a2-267">字符串</span><span class="sxs-lookup"><span data-stu-id="711a2-267">String</span></span>|<span data-ttu-id="711a2-p113">用户所在的城市。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="711a2-p113">The city in which the user is located. Supports $filter.</span></span>|
|<span data-ttu-id="711a2-270">companyName</span><span class="sxs-lookup"><span data-stu-id="711a2-270">companyName</span></span>| <span data-ttu-id="711a2-271">字符串</span><span class="sxs-lookup"><span data-stu-id="711a2-271">String</span></span> | <span data-ttu-id="711a2-272">与用户关联的公司名称。</span><span class="sxs-lookup"><span data-stu-id="711a2-272">The company name which the user is associated.</span></span> <span data-ttu-id="711a2-273">只读。</span><span class="sxs-lookup"><span data-stu-id="711a2-273">Read-only.</span></span>
|<span data-ttu-id="711a2-274">consentProvidedForMinor</span><span class="sxs-lookup"><span data-stu-id="711a2-274">consentProvidedForMinor</span></span>|<span data-ttu-id="711a2-275">字符串</span><span class="sxs-lookup"><span data-stu-id="711a2-275">String</span></span>|<span data-ttu-id="711a2-276">设置是否已为未成年人获得许可。</span><span class="sxs-lookup"><span data-stu-id="711a2-276">Sets whether consent has been obtained for minors.</span></span> <span data-ttu-id="711a2-277">允许值： `null`， `granted`， `denied` 和 `notRequired`。</span><span class="sxs-lookup"><span data-stu-id="711a2-277">Allowed values: `null`, `granted`, `denied` and `notRequired`.</span></span> <span data-ttu-id="711a2-278">请参阅 [法律年龄分组属性定义](#legal-age-group-property-definitions) 以获取详细信息。</span><span class="sxs-lookup"><span data-stu-id="711a2-278">Refer to the [legal age group property definitions](#legal-age-group-property-definitions) for further information.</span></span>|
|<span data-ttu-id="711a2-279">国家</span><span class="sxs-lookup"><span data-stu-id="711a2-279">country</span></span>|<span data-ttu-id="711a2-280">字符串</span><span class="sxs-lookup"><span data-stu-id="711a2-280">String</span></span>|<span data-ttu-id="711a2-p116">用户所在的国家/地区；例如，“美国”或“英国”。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="711a2-p116">The country/region in which the user is located; for example, “US” or “UK”. Supports $filter.</span></span>|
|<span data-ttu-id="711a2-283">部门</span><span class="sxs-lookup"><span data-stu-id="711a2-283">department</span></span>|<span data-ttu-id="711a2-284">字符串</span><span class="sxs-lookup"><span data-stu-id="711a2-284">String</span></span>|<span data-ttu-id="711a2-p117">用户工作部门的名称。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="711a2-p117">The name for the department in which the user works. Supports $filter.</span></span>|
|<span data-ttu-id="711a2-287">displayName</span><span class="sxs-lookup"><span data-stu-id="711a2-287">displayName</span></span>|<span data-ttu-id="711a2-288">字符串</span><span class="sxs-lookup"><span data-stu-id="711a2-288">String</span></span>|<span data-ttu-id="711a2-p118">用户通讯簿中显示的名称。这通常是用户名字、中间名首字母和姓氏的组合。此属性在创建用户时是必需的，并且在更新过程中不能清除。支持 $filter 和 $orderby。</span><span class="sxs-lookup"><span data-stu-id="711a2-p118">The name displayed in the address book for the user. This is usually the combination of the user's first name, middle initial and last name. This property is required when a user is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="711a2-293">givenName</span><span class="sxs-lookup"><span data-stu-id="711a2-293">givenName</span></span>|<span data-ttu-id="711a2-294">字符串</span><span class="sxs-lookup"><span data-stu-id="711a2-294">String</span></span>|<span data-ttu-id="711a2-p119">用户的名。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="711a2-p119">The given name (first name) of the user. Supports $filter.</span></span>|
|<span data-ttu-id="711a2-297">hireDate</span><span class="sxs-lookup"><span data-stu-id="711a2-297">hireDate</span></span>|<span data-ttu-id="711a2-298">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="711a2-298">DateTimeOffset</span></span>|<span data-ttu-id="711a2-p120">用户的雇佣日期。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示： `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="711a2-p120">The hire date of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="711a2-302">ID</span><span class="sxs-lookup"><span data-stu-id="711a2-302">id</span></span>|<span data-ttu-id="711a2-303">字符串</span><span class="sxs-lookup"><span data-stu-id="711a2-303">String</span></span>|<span data-ttu-id="711a2-p121">用户的唯一标识符。继承自 [directoryObject](directoryobject.md)。键。不可为 null。只读。</span><span class="sxs-lookup"><span data-stu-id="711a2-p121">The unique identifier for the user. Inherited from [directoryObject](directoryobject.md). Key. Not nullable. Read-only.</span></span>|
|<span data-ttu-id="711a2-309">imAddresses</span><span class="sxs-lookup"><span data-stu-id="711a2-309">imAddresses</span></span>|<span data-ttu-id="711a2-310">字符串集合</span><span class="sxs-lookup"><span data-stu-id="711a2-310">String collection</span></span>|<span data-ttu-id="711a2-p122">用户的即时消息 IP 语音 (VOIP) 会话初始协议 (SIP) 地址。只读。</span><span class="sxs-lookup"><span data-stu-id="711a2-p122">The instant message voice over IP (VOIP) session initiation protocol (SIP) addresses for the user. Read-only.</span></span>|
|<span data-ttu-id="711a2-313">兴趣</span><span class="sxs-lookup"><span data-stu-id="711a2-313">interests</span></span>|<span data-ttu-id="711a2-314">字符串集合</span><span class="sxs-lookup"><span data-stu-id="711a2-314">String collection</span></span>|<span data-ttu-id="711a2-315">用户介绍自身兴趣的列表。</span><span class="sxs-lookup"><span data-stu-id="711a2-315">A list for the user to describe their interests.</span></span>|
|<span data-ttu-id="711a2-316">jobTitle</span><span class="sxs-lookup"><span data-stu-id="711a2-316">jobTitle</span></span>|<span data-ttu-id="711a2-317">字符串</span><span class="sxs-lookup"><span data-stu-id="711a2-317">String</span></span>|<span data-ttu-id="711a2-p123">用户的职务。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="711a2-p123">The user’s job title. Supports $filter.</span></span>|
|<span data-ttu-id="711a2-320">legalAgeGroupClassification</span><span class="sxs-lookup"><span data-stu-id="711a2-320">legalAgeGroupClassification</span></span>|<span data-ttu-id="711a2-321">字符串</span><span class="sxs-lookup"><span data-stu-id="711a2-321">String</span></span>| <span data-ttu-id="711a2-322">企业应用程序用于确定用户的法律年龄组。</span><span class="sxs-lookup"><span data-stu-id="711a2-322">Used by enterprise applications to determine the legal age group of the user.</span></span> <span data-ttu-id="711a2-323">此属性为只读，基于 `ageGroup` 和 `consentProvidedForMinor` 属性计算。</span><span class="sxs-lookup"><span data-stu-id="711a2-323">This property is read-only and calculated based on `ageGroup` and `consentProvidedForMinor` properties.</span></span> <span data-ttu-id="711a2-324">允许值： `null`， `minorWithOutParentalConsent`， `minorWithParentalConsent` 和 `minorNoParentalConsentRequired`。`notAdult` `adult`</span><span class="sxs-lookup"><span data-stu-id="711a2-324">Allowed values: `null`, `minorWithOutParentalConsent`, `minorWithParentalConsent`, `minorNoParentalConsentRequired`, `notAdult` and `adult`.</span></span> <span data-ttu-id="711a2-325">请参阅 [法律年龄分组属性定义](#legal-age-group-property-definitions) i获取详细信息。</span><span class="sxs-lookup"><span data-stu-id="711a2-325">Refer to the [legal age group property definitions](#legal-age-group-property-definitions) for further information.)</span></span>|
|<span data-ttu-id="711a2-326">邮件</span><span class="sxs-lookup"><span data-stu-id="711a2-326">mail</span></span>|<span data-ttu-id="711a2-327">字符串</span><span class="sxs-lookup"><span data-stu-id="711a2-327">String</span></span>|<span data-ttu-id="711a2-p125">用户的 SMTP 地址，例如，“jeff@contoso.onmicrosoft.com”。只读。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="711a2-p125">The SMTP address for the user, for example, "jeff@contoso.onmicrosoft.com". Read-Only. Supports $filter.</span></span>|
|<span data-ttu-id="711a2-331">mailboxSettings</span><span class="sxs-lookup"><span data-stu-id="711a2-331">mailboxSettings</span></span>|[<span data-ttu-id="711a2-332">mailboxSettings</span><span class="sxs-lookup"><span data-stu-id="711a2-332">mailboxSettings</span></span>](mailboxsettings.md)|<span data-ttu-id="711a2-p126">已登录用户的主邮箱的设置。可以[获取](../api/user_get_mailboxsettings.md)或[更新](../api/user_update_mailboxsettings.md)用于向传入邮件发送自动答复、区域设置和时区的设置。</span><span class="sxs-lookup"><span data-stu-id="711a2-p126">Settings for the primary mailbox of the signed-in user. You can [get](../api/user_get_mailboxsettings.md) or [update](../api/user_update_mailboxsettings.md) settings for sending automatic replies to incoming messages, locale and time zone.</span></span>|
|<span data-ttu-id="711a2-335">mailNickname</span><span class="sxs-lookup"><span data-stu-id="711a2-335">mailNickname</span></span>|<span data-ttu-id="711a2-336">字符串</span><span class="sxs-lookup"><span data-stu-id="711a2-336">String</span></span>|<span data-ttu-id="711a2-p127">用户的邮件别名。创建用户时必须指定此属性。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="711a2-p127">The mail alias for the user. This property must be specified when a user is created. Supports $filter.</span></span>|
|<span data-ttu-id="711a2-340">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="711a2-340">mobilePhone</span></span>|<span data-ttu-id="711a2-341">字符串</span><span class="sxs-lookup"><span data-stu-id="711a2-341">String</span></span>|<span data-ttu-id="711a2-342">用户的主要移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="711a2-342">The primary cellular telephone number for the user.</span></span>|
|<span data-ttu-id="711a2-343">mySite</span><span class="sxs-lookup"><span data-stu-id="711a2-343">mySite</span></span>|<span data-ttu-id="711a2-344">字符串</span><span class="sxs-lookup"><span data-stu-id="711a2-344">String</span></span>|<span data-ttu-id="711a2-345">用户个人网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="711a2-345">The URL for the user's personal site.</span></span>|
|<span data-ttu-id="711a2-346">officeLocation</span><span class="sxs-lookup"><span data-stu-id="711a2-346">officeLocation</span></span>|<span data-ttu-id="711a2-347">字符串</span><span class="sxs-lookup"><span data-stu-id="711a2-347">String</span></span>|<span data-ttu-id="711a2-348">用户公司地点的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="711a2-348">The office location in the user's place of business.</span></span>|
|<span data-ttu-id="711a2-349">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="711a2-349">onPremisesImmutableId</span></span>|<span data-ttu-id="711a2-350">字符串</span><span class="sxs-lookup"><span data-stu-id="711a2-350">String</span></span>|<span data-ttu-id="711a2-p128">此属性用于将本地 Active Directory 用户帐户关联到他们的 Azure AD 用户对象。如果对用户的 **userPrincipalName** (UPN) 属性使用联盟域，必须在创建新用户帐户时指定此属性。**重要说明：** 指定该属性时不能使用 **$** 和 **_** 字符。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="711a2-p128">This property is used to associate an on-premises Active Directory user account to their Azure AD user object. This property must be specified when creating a new user account in the Graph if you are using a federated domain for the user’s **userPrincipalName** (UPN) property. **Important:** The **$** and **_** characters cannot be used when specifying this property. Supports $filter.</span></span>                            |
|<span data-ttu-id="711a2-355">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="711a2-355">onPremisesLastSyncDateTime</span></span>|<span data-ttu-id="711a2-356">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="711a2-356">DateTimeOffset</span></span>|<span data-ttu-id="711a2-p129">表示上一次对象与本地目录同步的时间；例如：“2013-02-16T03:04:54Z”。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。</span><span class="sxs-lookup"><span data-stu-id="711a2-p129">Indicates the last time at which the object was synced with the on-premises directory; for example: "2013-02-16T03:04:54Z". The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="711a2-361">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="711a2-361">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="711a2-362">字符串</span><span class="sxs-lookup"><span data-stu-id="711a2-362">String</span></span>|<span data-ttu-id="711a2-p130">包含从本地同步到云的用户的本地安全标识符 (SID)。只读。</span><span class="sxs-lookup"><span data-stu-id="711a2-p130">Contains the on-premises security identifier (SID) for the user that was synchronized from on-premises to the cloud. Read-only.</span></span>|
|<span data-ttu-id="711a2-365">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="711a2-365">onPremisesSyncEnabled</span></span>|<span data-ttu-id="711a2-366">布尔值</span><span class="sxs-lookup"><span data-stu-id="711a2-366">Boolean</span></span>| <span data-ttu-id="711a2-p131">如果此对象从本地目录同步，则为 **true**；如果此对象最初从本地目录同步，但以后不再同步，则为 **false**；如果此对象从未从本地目录同步，则为 **null**（默认值）。只读</span><span class="sxs-lookup"><span data-stu-id="711a2-p131">**true** if this object is synced from an on-premises directory; **false** if this object was originally synced from an on-premises directory but is no longer synced; **null** if this object has never been synced from an on-premises directory (default). Read-only</span></span> |
|<span data-ttu-id="711a2-369">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="711a2-369">passwordPolicies</span></span>|<span data-ttu-id="711a2-370">字符串</span><span class="sxs-lookup"><span data-stu-id="711a2-370">String</span></span>|<span data-ttu-id="711a2-p132">指定用户的密码策略。此值是一个枚举，具有一个可能值“DisableStrongPassword”，允许指定比默认策略弱的密码。还可以指定“DisablePasswordExpiration”。可以同时指定这两个策略；例如：“DisablePasswordExpiration、DisableStrongPassword”。</span><span class="sxs-lookup"><span data-stu-id="711a2-p132">Specifies password policies for the user. This value is an enumeration with one possible value being “DisableStrongPassword”, which allows weaker passwords than the default policy to be specified. “DisablePasswordExpiration” can also be specified. The two may be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".</span></span>|
|<span data-ttu-id="711a2-375">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="711a2-375">passwordProfile</span></span>|[<span data-ttu-id="711a2-376">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="711a2-376">PasswordProfile</span></span>](passwordprofile.md)|<span data-ttu-id="711a2-p133">指定用户的密码配置文件。配置文件包含用户的密码。创建用户时此属性是必需的。配置文件中的密码必须满足 **passwordPolicies** 属性指定的最低要求。默认情况下，必须使用强密码。</span><span class="sxs-lookup"><span data-stu-id="711a2-p133">Specifies the password profile for the user. The profile contains the user’s password. This property is required when a user is created. The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property. By default, a strong password is required.</span></span>|
|<span data-ttu-id="711a2-382">pastProjects</span><span class="sxs-lookup"><span data-stu-id="711a2-382">pastProjects</span></span>|<span data-ttu-id="711a2-383">字符串集合</span><span class="sxs-lookup"><span data-stu-id="711a2-383">String collection</span></span>|<span data-ttu-id="711a2-384">供用户枚举其过去项目的列表。</span><span class="sxs-lookup"><span data-stu-id="711a2-384">A list for the user to enumerate their past projects.</span></span>|
|<span data-ttu-id="711a2-385">postalCode</span><span class="sxs-lookup"><span data-stu-id="711a2-385">postalCode</span></span>|<span data-ttu-id="711a2-386">字符串</span><span class="sxs-lookup"><span data-stu-id="711a2-386">String</span></span>|<span data-ttu-id="711a2-p134">用户邮政地址的邮政编码。邮政编码特定于用户所在的国家/地区。在美国，此属性包含邮政编码。</span><span class="sxs-lookup"><span data-stu-id="711a2-p134">The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.</span></span>|
|<span data-ttu-id="711a2-390">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="711a2-390">preferredLanguage</span></span>|<span data-ttu-id="711a2-391">字符串</span><span class="sxs-lookup"><span data-stu-id="711a2-391">String</span></span>|<span data-ttu-id="711a2-p135">用户的首选语言。应遵循 ISO 639-1 代码；例如“EN-US”。</span><span class="sxs-lookup"><span data-stu-id="711a2-p135">The preferred language for the user. Should follow ISO 639-1 Code; for example "en-US".</span></span>|
|<span data-ttu-id="711a2-394">preferredName</span><span class="sxs-lookup"><span data-stu-id="711a2-394">preferredName</span></span>|<span data-ttu-id="711a2-395">字符串</span><span class="sxs-lookup"><span data-stu-id="711a2-395">String</span></span>|<span data-ttu-id="711a2-396">用户的首选名称。</span><span class="sxs-lookup"><span data-stu-id="711a2-396">The preferred name for the user.</span></span>|
|<span data-ttu-id="711a2-397">provisionedPlans</span><span class="sxs-lookup"><span data-stu-id="711a2-397">provisionedPlans</span></span>|<span data-ttu-id="711a2-398">[ProvisionedPlan](provisionedplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-398">[ProvisionedPlan](provisionedplan.md) collection</span></span>|<span data-ttu-id="711a2-p136">为用户设置的计划。只读。不可为 null。</span><span class="sxs-lookup"><span data-stu-id="711a2-p136">The plans that are provisioned for the user. Read-only. Not nullable.</span></span> |
|<span data-ttu-id="711a2-402">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="711a2-402">proxyAddresses</span></span>|<span data-ttu-id="711a2-403">字符串集合</span><span class="sxs-lookup"><span data-stu-id="711a2-403">String collection</span></span>|<span data-ttu-id="711a2-p137">例如：`["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` 需要多值属性筛选器表达式的 **any** 运算符。只读，不可为 Null。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="711a2-p137">For example: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` The **any** operator is required for filter expressions on multi-valued properties. Read-only, Not nullable. Supports $filter.</span></span>          |
|<span data-ttu-id="711a2-407">责任</span><span class="sxs-lookup"><span data-stu-id="711a2-407">responsibilities</span></span>|<span data-ttu-id="711a2-408">字符串集合</span><span class="sxs-lookup"><span data-stu-id="711a2-408">String collection</span></span>|<span data-ttu-id="711a2-409">供用户枚举其职责的列表。</span><span class="sxs-lookup"><span data-stu-id="711a2-409">A list for the user to enumerate their responsibilities.</span></span>|
|<span data-ttu-id="711a2-410">学校</span><span class="sxs-lookup"><span data-stu-id="711a2-410">schools</span></span>|<span data-ttu-id="711a2-411">字符串集合</span><span class="sxs-lookup"><span data-stu-id="711a2-411">String collection</span></span>|<span data-ttu-id="711a2-412">供用户枚举其学习过的学校列表。</span><span class="sxs-lookup"><span data-stu-id="711a2-412">A list for the user to enumerate the schools they have attended.</span></span>|
|<span data-ttu-id="711a2-413">技能</span><span class="sxs-lookup"><span data-stu-id="711a2-413">skills</span></span>|<span data-ttu-id="711a2-414">字符串集合</span><span class="sxs-lookup"><span data-stu-id="711a2-414">String collection</span></span>|<span data-ttu-id="711a2-415">供用户枚举其技能的列表。</span><span class="sxs-lookup"><span data-stu-id="711a2-415">A list for the user to enumerate their skills.</span></span>|
|<span data-ttu-id="711a2-416">省份</span><span class="sxs-lookup"><span data-stu-id="711a2-416">state</span></span>|<span data-ttu-id="711a2-417">字符串</span><span class="sxs-lookup"><span data-stu-id="711a2-417">String</span></span>|<span data-ttu-id="711a2-p138">用户地址中的省/市/自治区或省。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="711a2-p138">The state or province in the user's address. Supports $filter.</span></span>|
|<span data-ttu-id="711a2-420">streetAddress</span><span class="sxs-lookup"><span data-stu-id="711a2-420">streetAddress</span></span>|<span data-ttu-id="711a2-421">字符串</span><span class="sxs-lookup"><span data-stu-id="711a2-421">String</span></span>|<span data-ttu-id="711a2-422">用户公司地点的街道地址。</span><span class="sxs-lookup"><span data-stu-id="711a2-422">The street address of the user's place of business.</span></span>|
|<span data-ttu-id="711a2-423">姓</span><span class="sxs-lookup"><span data-stu-id="711a2-423">surname</span></span>|<span data-ttu-id="711a2-424">字符串</span><span class="sxs-lookup"><span data-stu-id="711a2-424">String</span></span>|<span data-ttu-id="711a2-p139">用户的姓氏。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="711a2-p139">The user's surname (family name or last name). Supports $filter.</span></span>|
|<span data-ttu-id="711a2-427">usageLocation</span><span class="sxs-lookup"><span data-stu-id="711a2-427">usageLocation</span></span>|<span data-ttu-id="711a2-428">字符串</span><span class="sxs-lookup"><span data-stu-id="711a2-428">String</span></span>|<span data-ttu-id="711a2-p140">两个字母的国家/地区代码（ISO 标准 3166）。为检查服务在国家/地区的可用性，这对根据法律要求将分配许可证的用户而言是必需的。示例包括：“US”、“JP”和“GB”。不可为 null。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="711a2-p140">A two letter country code (ISO standard 3166). Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries.  Examples include: "US", "JP", and "GB". Not nullable. Supports $filter.</span></span>|
|<span data-ttu-id="711a2-434">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="711a2-434">userPrincipalName</span></span>|<span data-ttu-id="711a2-435">字符串</span><span class="sxs-lookup"><span data-stu-id="711a2-435">String</span></span>|<span data-ttu-id="711a2-p141">用户的用户主体名称 (UPN)。UPN 是用户基于 Internet 标准 RFC 822 的 Internet 式登录名。按照惯例，此名称应映射到用户的电子邮件名称。常规格式是 alias@domain，其中，domain 必须位于租户的已验证域集合中。创建用户时此属性是必需的。可从 [组织](organization.md) 的 **verifiedDomains** 属性访问租户的已验证域。支持 $filter 和 $orderby。</span><span class="sxs-lookup"><span data-stu-id="711a2-p141">The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains. This property is required when a user is created. The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](organization.md). Supports $filter and $orderby.</span></span>
|<span data-ttu-id="711a2-443">userType</span><span class="sxs-lookup"><span data-stu-id="711a2-443">userType</span></span>|<span data-ttu-id="711a2-444">字符串</span><span class="sxs-lookup"><span data-stu-id="711a2-444">String</span></span>|<span data-ttu-id="711a2-p142">可用于对目录中的用户类型分类的字符串值，例如“成员”和“访客”。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="711a2-p142">A string value that can be used to classify user types in your directory, such as “Member” and “Guest”. Supports $filter.</span></span>          |

### <a name="legal-age-group-property-definitions"></a><span data-ttu-id="711a2-447">法律年龄分组属性定义</span><span class="sxs-lookup"><span data-stu-id="711a2-447">Legal age group property definitions</span></span>

<span data-ttu-id="711a2-448">本节介绍如何三个由 Azure AD 管理员和企业应用程序开发人员使用以满足期限相关法规的年龄分组属性 (`legalAgeGroupClassification`, `ageGroup` 和 `consentProvidedForMinor`) 。</span><span class="sxs-lookup"><span data-stu-id="711a2-448">This section explains how the three age group properties (`legalAgeGroupClassification`, `ageGroup` and `consentProvidedForMinor`) are used by Azure AD administrators and enterprise application developers to meet age-related regulations.</span></span>

<span data-ttu-id="711a2-449">例如： Cameron 是英国 Holyport 小学目录的管理员。</span><span class="sxs-lookup"><span data-stu-id="711a2-449">For example: Cameron is administrator of a directory for an elementary school in Holyport in the United Kingdom.</span></span> <span data-ttu-id="711a2-450">本学年开始，据英国与年龄相关的法规要求，他使用入学通知书获得未成年人父母的许可。</span><span class="sxs-lookup"><span data-stu-id="711a2-450">At the beginning of the school year he uses the admissions paperwork to obtain consent from the minor's parents based on the age-related regulations of the United Kingdom.</span></span> <span data-ttu-id="711a2-451">获得父母许可以允许 Holyport 学校和 Microsoft 应用程序使用未成年人的帐户。</span><span class="sxs-lookup"><span data-stu-id="711a2-451">The consent obtained from the parent allows the minor's account to be used by Holyport school and Microsoft apps.</span></span> <span data-ttu-id="711a2-452">随后，Cameron创建所有帐户，并设置为"未成年人"ageGroup 和 consentProvidedForMinor 为"已获授权"。</span><span class="sxs-lookup"><span data-stu-id="711a2-452">Cameron then creates all the accounts and sets ageGroup to "minor" and consentProvidedForMinor to "granted".</span></span> <span data-ttu-id="711a2-453">学生使用的应用程序可以禁用部分不未成年人的功能。</span><span class="sxs-lookup"><span data-stu-id="711a2-453">Applications used by his students are then able to suppress features that are not suitable for minors.</span></span>

#### <a name="legal-age-group-classification"></a><span data-ttu-id="711a2-454">法律年龄分组分类</span><span class="sxs-lookup"><span data-stu-id="711a2-454">Legal age group classification</span></span>

<span data-ttu-id="711a2-455">企业应用程序开发人员使用只读属性以确保基于所属法律年龄分组用户的正确处理。</span><span class="sxs-lookup"><span data-stu-id="711a2-455">This read-only property is used by enterprise application developers to ensure the correct handling of a user based on their legal age group.</span></span> <span data-ttu-id="711a2-456">计算基于用户的 `ageGroup` 和 `consentProvidedForMinor` 属性。</span><span class="sxs-lookup"><span data-stu-id="711a2-456">It is calculated based on the user's `ageGroup` and `consentProvidedForMinor` properties.</span></span>

| <span data-ttu-id="711a2-457">值</span><span class="sxs-lookup"><span data-stu-id="711a2-457">Value</span></span>    | #  |<span data-ttu-id="711a2-458">说明</span><span class="sxs-lookup"><span data-stu-id="711a2-458">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="711a2-459">空</span><span class="sxs-lookup"><span data-stu-id="711a2-459">null</span></span>|<span data-ttu-id="711a2-460">0</span><span class="sxs-lookup"><span data-stu-id="711a2-460">{0}</span></span>|<span data-ttu-id="711a2-461">默认值，无 `ageGroup` 已经作为用户设置。</span><span class="sxs-lookup"><span data-stu-id="711a2-461">Default value, no `ageGroup` has been set for the user.</span></span>|
|<span data-ttu-id="711a2-462">minorWithoutParentalConsent</span><span class="sxs-lookup"><span data-stu-id="711a2-462">minorWithoutParentalConsent</span></span> |<span data-ttu-id="711a2-463">1</span><span class="sxs-lookup"><span data-stu-id="711a2-463">-1</span></span>|<span data-ttu-id="711a2-464">(预留备用)</span><span class="sxs-lookup"><span data-stu-id="711a2-464">Reserved for future use.</span></span>|
|<span data-ttu-id="711a2-465">minorWithParentalConsent</span><span class="sxs-lookup"><span data-stu-id="711a2-465">minorWithParentalConsent</span></span>|<span data-ttu-id="711a2-466">2</span><span class="sxs-lookup"><span data-stu-id="711a2-466">-2</span></span>| <span data-ttu-id="711a2-467">基于其所在国家/地区的年龄相关规定，用户被视为未成年人，同时帐户管理员已从f父母之一或监护人获取适当许可。</span><span class="sxs-lookup"><span data-stu-id="711a2-467">The user is considered a minor based on the age-related regulations of their country or region and the administrator of the account has obtained appropriate consent from a parent or guardian.</span></span>|
|<span data-ttu-id="711a2-468">成人</span><span class="sxs-lookup"><span data-stu-id="711a2-468">Adult.</span></span>|<span data-ttu-id="711a2-469">3</span><span class="sxs-lookup"><span data-stu-id="711a2-469">-3</span></span>|<span data-ttu-id="711a2-470">基于所在国家或地区的年龄相关法规，用户被视为成人。</span><span class="sxs-lookup"><span data-stu-id="711a2-470">The user considered an adult based on the age-related regulations of their country or region.</span></span>|
|<span data-ttu-id="711a2-471">notAdult</span><span class="sxs-lookup"><span data-stu-id="711a2-471">notAdult</span></span>|<span data-ttu-id="711a2-472">4</span><span class="sxs-lookup"><span data-stu-id="711a2-472">-4</span></span>|<span data-ttu-id="711a2-473">用户所在家或地区实施有其他年龄相关法规 （如美国、英国、欧盟或韩国），并且用户年龄处于未成年人和成人年龄之间 （根据所在国家或地区规定）。</span><span class="sxs-lookup"><span data-stu-id="711a2-473">The user is from a country or region that has additional age-related regulations (such as the United States, United Kingdom, European Union or South Korea), and the user's age is between a minor and an adult age (as stipulated based on country or region).</span></span> <span data-ttu-id="711a2-474">一般来说，这意味着青少年都会被视为处于 `notAdult` 监管国家。</span><span class="sxs-lookup"><span data-stu-id="711a2-474">Generally, this means that teenagers are considered as `notAdult` in regulated countries.</span></span>|
|<span data-ttu-id="711a2-475">minorNoParentalConsentRequired</span><span class="sxs-lookup"><span data-stu-id="711a2-475">minorNoParentalConsentRequired</span></span>|<span data-ttu-id="711a2-476">5</span><span class="sxs-lookup"><span data-stu-id="711a2-476">-5</span></span>|<span data-ttu-id="711a2-477">用户为未成年人，但所在国家或地区不存在与年龄相关的法规。</span><span class="sxs-lookup"><span data-stu-id="711a2-477">The user is a minor but is from a country or region that has no age-related regulations.</span></span>|

#### <a name="age-group-and-minor-consent"></a><span data-ttu-id="711a2-478">年龄分组和未成年人同意</span><span class="sxs-lookup"><span data-stu-id="711a2-478">Age group and minor consent</span></span>

<span data-ttu-id="711a2-479">年龄分组和未成年人同意属性是 Azure AD 管理员可选属性，在根据用户所在国家或地区与年龄相关的管理法规，用于帮助确保正确处理帐户的使用。</span><span class="sxs-lookup"><span data-stu-id="711a2-479">The age group and minor consent properties are optional properties used by Azure AD administrators to help ensure the use of an account is handled correctly based on the age-related regulatory rules governing the user's country or region.</span></span>

#### <a name="agegroup-property"></a><span data-ttu-id="711a2-480">ageGroup 属性</span><span class="sxs-lookup"><span data-stu-id="711a2-480">ageGroup property</span></span>

| <span data-ttu-id="711a2-481">值</span><span class="sxs-lookup"><span data-stu-id="711a2-481">Value</span></span>    | #  |<span data-ttu-id="711a2-482">说明</span><span class="sxs-lookup"><span data-stu-id="711a2-482">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="711a2-483">空</span><span class="sxs-lookup"><span data-stu-id="711a2-483">null</span></span>|<span data-ttu-id="711a2-484">0</span><span class="sxs-lookup"><span data-stu-id="711a2-484">{0}</span></span>|<span data-ttu-id="711a2-485">默认值，无 `ageGroup` 已经作为用户设置。</span><span class="sxs-lookup"><span data-stu-id="711a2-485">Default value, no `ageGroup` has been set for the user.</span></span>|
|<span data-ttu-id="711a2-486">未成年人</span><span class="sxs-lookup"><span data-stu-id="711a2-486">Minor</span></span>|<span data-ttu-id="711a2-487">1</span><span class="sxs-lookup"><span data-stu-id="711a2-487">-1</span></span>|<span data-ttu-id="711a2-488">用户视为未成年人。</span><span class="sxs-lookup"><span data-stu-id="711a2-488">The user is consider a minor.</span></span>|
|<span data-ttu-id="711a2-489">notAdult</span><span class="sxs-lookup"><span data-stu-id="711a2-489">notAdult</span></span>|<span data-ttu-id="711a2-490">2</span><span class="sxs-lookup"><span data-stu-id="711a2-490">-2</span></span>|<span data-ttu-id="711a2-491">用户来自有法定法规的国家（美国、英国、欧盟或韩国），并且用户年龄高于儿童年龄（根据国家/地区规定）的上限，并低于成人年龄的下限 （根据国家/地区规定）。</span><span class="sxs-lookup"><span data-stu-id="711a2-491">The user is from a country that has statutory regulations  United States, United Kingdom, European Union or South Korea) and user’s age is more than the upper limit of kid age (as per country) and less than lower limit of adult age (as stipulated based on country or region).</span></span> <span data-ttu-id="711a2-492">基本上，青少年视为在 `notAdult` 监管国家。</span><span class="sxs-lookup"><span data-stu-id="711a2-492">So basically, teenagers are considered as `notAdult` in regulated countries.</span></span>|
|<span data-ttu-id="711a2-493">成人</span><span class="sxs-lookup"><span data-stu-id="711a2-493">Adult.</span></span>|<span data-ttu-id="711a2-494">3</span><span class="sxs-lookup"><span data-stu-id="711a2-494">-3</span></span>|<span data-ttu-id="711a2-495">用户应作为成人处理。</span><span class="sxs-lookup"><span data-stu-id="711a2-495">The user should be a treated as an adult.</span></span>|

#### <a name="consentprovidedforminor-property"></a><span data-ttu-id="711a2-496">consentProvidedForMinor 属性</span><span class="sxs-lookup"><span data-stu-id="711a2-496">consentProvidedForMinor property</span></span>

| <span data-ttu-id="711a2-497">值</span><span class="sxs-lookup"><span data-stu-id="711a2-497">Value</span></span>    | #  |<span data-ttu-id="711a2-498">说明</span><span class="sxs-lookup"><span data-stu-id="711a2-498">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="711a2-499">空</span><span class="sxs-lookup"><span data-stu-id="711a2-499">null</span></span>|<span data-ttu-id="711a2-500">0</span><span class="sxs-lookup"><span data-stu-id="711a2-500">{0}</span></span>|<span data-ttu-id="711a2-501">默认值，无 `consentProvidedForMinor` 已经作为用户设置。</span><span class="sxs-lookup"><span data-stu-id="711a2-501">Default value, no `consentProvidedForMinor` has been set for the user.</span></span>|
|<span data-ttu-id="711a2-502">已获授权</span><span class="sxs-lookup"><span data-stu-id="711a2-502">Permissions granted</span></span>|<span data-ttu-id="711a2-503">1</span><span class="sxs-lookup"><span data-stu-id="711a2-503">-1</span></span>|<span data-ttu-id="711a2-504">用户已经获得配置账户许可。</span><span class="sxs-lookup"><span data-stu-id="711a2-504">Consent has been obtained for the user to have an account.</span></span>|
|<span data-ttu-id="711a2-505">拒绝</span><span class="sxs-lookup"><span data-stu-id="711a2-505">denied</span></span>|<span data-ttu-id="711a2-506">2</span><span class="sxs-lookup"><span data-stu-id="711a2-506">-2</span></span>|<span data-ttu-id="711a2-507">已为用户获得许可配置账户。</span><span class="sxs-lookup"><span data-stu-id="711a2-507">Consent has not been obtained for the user to have an account.</span></span>|
|<span data-ttu-id="711a2-508">notRequired</span><span class="sxs-lookup"><span data-stu-id="711a2-508">notRequired</span></span>|<span data-ttu-id="711a2-509">3</span><span class="sxs-lookup"><span data-stu-id="711a2-509">-3</span></span>|<span data-ttu-id="711a2-510">用户所在地不要求获得同意。</span><span class="sxs-lookup"><span data-stu-id="711a2-510">The user is from a location that does not require consent.</span></span>|
 
## <a name="relationships"></a><span data-ttu-id="711a2-511">关系</span><span class="sxs-lookup"><span data-stu-id="711a2-511">Relationships</span></span>

| <span data-ttu-id="711a2-512">关系</span><span class="sxs-lookup"><span data-stu-id="711a2-512">Relationship</span></span> | <span data-ttu-id="711a2-513">类型</span><span class="sxs-lookup"><span data-stu-id="711a2-513">Type</span></span>   |<span data-ttu-id="711a2-514">说明</span><span class="sxs-lookup"><span data-stu-id="711a2-514">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="711a2-515">活动</span><span class="sxs-lookup"><span data-stu-id="711a2-515">activities</span></span>|<span data-ttu-id="711a2-516">[userActivity](projectrome_activity.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-516">[userActivity](projectrome_activity.md) collection</span></span>|<span data-ttu-id="711a2-517">跨设备的用户的活动。</span><span class="sxs-lookup"><span data-stu-id="711a2-517">The user's activities across devices.</span></span> <span data-ttu-id="711a2-518">只读。</span><span class="sxs-lookup"><span data-stu-id="711a2-518">Read-only.</span></span> <span data-ttu-id="711a2-519">可为空。</span><span class="sxs-lookup"><span data-stu-id="711a2-519">Nullable.</span></span>|
|<span data-ttu-id="711a2-520">日历</span><span class="sxs-lookup"><span data-stu-id="711a2-520">calendar</span></span>|[<span data-ttu-id="711a2-521">日历</span><span class="sxs-lookup"><span data-stu-id="711a2-521">Calendar</span></span>](calendar.md)|<span data-ttu-id="711a2-p148">用户的主日历。只读。</span><span class="sxs-lookup"><span data-stu-id="711a2-p148">The user's primary calendar. Read-only.</span></span>|
|<span data-ttu-id="711a2-524">calendarGroups</span><span class="sxs-lookup"><span data-stu-id="711a2-524">calendarGroups</span></span>|<span data-ttu-id="711a2-525">[CalendarGroup](calendargroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-525">[CalendarGroup](calendargroup.md) collection</span></span>|<span data-ttu-id="711a2-p149">用户的日历组。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="711a2-p149">The user's calendar groups. Read-only. Nullable.</span></span>|
|<span data-ttu-id="711a2-529">calendarView</span><span class="sxs-lookup"><span data-stu-id="711a2-529">calendarView</span></span>|<span data-ttu-id="711a2-530">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-530">[Event](event.md) collection</span></span>|<span data-ttu-id="711a2-p150">日历的日历视图。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="711a2-p150">The calendar view for the calendar. Read-only. Nullable.</span></span>|
|<span data-ttu-id="711a2-534">日历</span><span class="sxs-lookup"><span data-stu-id="711a2-534">calendars</span></span>|<span data-ttu-id="711a2-535">[日历](calendar.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-535">[Calendar](calendar.md) collection</span></span>|<span data-ttu-id="711a2-p151">用户的日历。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="711a2-p151">The user's calendars. Read-only. Nullable.</span></span>|
|<span data-ttu-id="711a2-539">contactFolders</span><span class="sxs-lookup"><span data-stu-id="711a2-539">contactFolders</span></span>|<span data-ttu-id="711a2-540">[ContactFolder](contactfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-540">[ContactFolder](contactfolder.md) collection</span></span>|<span data-ttu-id="711a2-p152">用户的联系人文件夹。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="711a2-p152">The user's contacts folders. Read-only. Nullable.</span></span>|
|<span data-ttu-id="711a2-544">联系人</span><span class="sxs-lookup"><span data-stu-id="711a2-544">contacts</span></span>|<span data-ttu-id="711a2-545">[联系人](contact.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-545">[Contact](contact.md) collection</span></span>|<span data-ttu-id="711a2-p153">用户的联系人。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="711a2-p153">The user's contacts. Read-only. Nullable.</span></span>|
|<span data-ttu-id="711a2-549">createdObjects</span><span class="sxs-lookup"><span data-stu-id="711a2-549">createdObjects</span></span>|<span data-ttu-id="711a2-550">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-550">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="711a2-p154">由用户创建的 directory 对象。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="711a2-p154">Directory objects that were created by the user. Read-only. Nullable.</span></span>|
|<span data-ttu-id="711a2-554">directReports</span><span class="sxs-lookup"><span data-stu-id="711a2-554">directReports</span></span>|<span data-ttu-id="711a2-555">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-555">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="711a2-p155">向此用户报告的用户和联系人。（其 manager 属性已设置为此用户的用户和联系人。）只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="711a2-p155">The users and contacts that report to the user. (The users and contacts that have their manager property set to this user.) Read-only. Nullable.</span></span> |
|<span data-ttu-id="711a2-559">驱动器</span><span class="sxs-lookup"><span data-stu-id="711a2-559">drive</span></span>|[<span data-ttu-id="711a2-560">驱动器</span><span class="sxs-lookup"><span data-stu-id="711a2-560">drive</span></span>](drive.md)|<span data-ttu-id="711a2-p156">用户的 OneDrive。只读。</span><span class="sxs-lookup"><span data-stu-id="711a2-p156">The user's OneDrive. Read-only.</span></span>|
|<span data-ttu-id="711a2-563">驱动器</span><span class="sxs-lookup"><span data-stu-id="711a2-563">drives</span></span>|<span data-ttu-id="711a2-564">[驱动器](drive.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-564">[drive](drive.md) collection</span></span>| <span data-ttu-id="711a2-p157">该用户的可用驱动器集合。只读。</span><span class="sxs-lookup"><span data-stu-id="711a2-p157">A collection of drives available for this user. Read-only.</span></span> |
|<span data-ttu-id="711a2-567">事件</span><span class="sxs-lookup"><span data-stu-id="711a2-567">events</span></span>|<span data-ttu-id="711a2-568">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-568">[Event](event.md) collection</span></span>|<span data-ttu-id="711a2-p158">用户的事件。默认显示“默认日历”下的事件。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="711a2-p158">The user's events. Default is to show Events under the Default Calendar. Read-only. Nullable.</span></span>|
|<span data-ttu-id="711a2-573">扩展</span><span class="sxs-lookup"><span data-stu-id="711a2-573">extensions</span></span>|<span data-ttu-id="711a2-574">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="711a2-574">[extension](extension.md) collection</span></span>|<span data-ttu-id="711a2-p159">为用户定义的开放扩展集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="711a2-p159">The collection of open extensions defined for the user. Read-only. Nullable.</span></span>|
|<span data-ttu-id="711a2-578">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="711a2-578">inferenceClassification</span></span> | [<span data-ttu-id="711a2-579">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="711a2-579">inferenceClassification</span></span>](inferenceClassification.md) | <span data-ttu-id="711a2-580">基于显式指定的用户邮件相关性分类，可以替代推导的相关性或重要性。</span><span class="sxs-lookup"><span data-stu-id="711a2-580">Relevance classification of the user's messages based on explicit designations which override inferred relevance or importance.</span></span> |
|<span data-ttu-id="711a2-581">licenseDetails</span><span class="sxs-lookup"><span data-stu-id="711a2-581">licenseDetails</span></span>|<span data-ttu-id="711a2-582">[licenseDetails](licensedetails.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-582">[licenseDetails](licensedetails.md) collection</span></span>|<span data-ttu-id="711a2-583">此用户的许可证详细信息集合。</span><span class="sxs-lookup"><span data-stu-id="711a2-583">A collection of this user's license details.</span></span> <span data-ttu-id="711a2-584">可为空。</span><span class="sxs-lookup"><span data-stu-id="711a2-584">Nullable.</span></span>|
|<span data-ttu-id="711a2-585">mailFolders</span><span class="sxs-lookup"><span data-stu-id="711a2-585">mailFolders</span></span>|<span data-ttu-id="711a2-586">[MailFolder](mailfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-586">[MailFolder](mailfolder.md) collection</span></span>| <span data-ttu-id="711a2-p161">用户的邮件文件夹。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="711a2-p161">The user's mail folders. Read-only. Nullable.</span></span>|
|<span data-ttu-id="711a2-590">管理员</span><span class="sxs-lookup"><span data-stu-id="711a2-590">manager</span></span>|[<span data-ttu-id="711a2-591">directoryObject</span><span class="sxs-lookup"><span data-stu-id="711a2-591">directoryObject</span></span>](directoryobject.md)|<span data-ttu-id="711a2-p162">是此用户的经理的用户或联系人。只读。（HTTP 方法：GET、PUT、DELETE）</span><span class="sxs-lookup"><span data-stu-id="711a2-p162">The user or contact that is this user’s manager. Read-only. (HTTP Methods: GET, PUT, DELETE.)</span></span>|
|<span data-ttu-id="711a2-595">memberOf</span><span class="sxs-lookup"><span data-stu-id="711a2-595">memberOf</span></span>|<span data-ttu-id="711a2-596">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-596">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="711a2-p163">用户所属的组和目录角色。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="711a2-p163">The groups and directory roles that the user is a member of. Read-only. Nullable.</span></span>|
|<span data-ttu-id="711a2-600">消息</span><span class="sxs-lookup"><span data-stu-id="711a2-600">messages</span></span>|<span data-ttu-id="711a2-601">[邮件](message.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-601">[Message](message.md) collection</span></span>|<span data-ttu-id="711a2-p164">邮箱或文件夹中的邮件。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="711a2-p164">The messages in a mailbox or folder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="711a2-605">onenote</span><span class="sxs-lookup"><span data-stu-id="711a2-605">onenote</span></span>|[<span data-ttu-id="711a2-606">Onenote</span><span class="sxs-lookup"><span data-stu-id="711a2-606">OneNote</span></span>](onenote.md)| <span data-ttu-id="711a2-607">只读。</span><span class="sxs-lookup"><span data-stu-id="711a2-607">Read-only.</span></span>|
|<span data-ttu-id="711a2-608">Outlook</span><span class="sxs-lookup"><span data-stu-id="711a2-608">Outlook</span></span>|[<span data-ttu-id="711a2-609">outlookUser</span><span class="sxs-lookup"><span data-stu-id="711a2-609">outlookUser</span></span>](outlookuser.md)| <span data-ttu-id="711a2-610">只读。</span><span class="sxs-lookup"><span data-stu-id="711a2-610">Read-only.</span></span>|
|<span data-ttu-id="711a2-611">ownedDevices</span><span class="sxs-lookup"><span data-stu-id="711a2-611">ownedDevices</span></span>|<span data-ttu-id="711a2-612">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-612">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="711a2-p165">用户拥有的设备。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="711a2-p165">Devices that are owned by the user. Read-only. Nullable.</span></span>|
|<span data-ttu-id="711a2-616">ownedObjects</span><span class="sxs-lookup"><span data-stu-id="711a2-616">ownedObjects</span></span>|<span data-ttu-id="711a2-617">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-617">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="711a2-p166">用户拥有的 directory 对象。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="711a2-p166">Directory objects that are owned by the user. Read-only. Nullable.</span></span>|
|<span data-ttu-id="711a2-621">人员</span><span class="sxs-lookup"><span data-stu-id="711a2-621">people</span></span>|<span data-ttu-id="711a2-622">[人员](person.md)集合</span><span class="sxs-lookup"><span data-stu-id="711a2-622">[Person](person.md) collection</span></span>| <span data-ttu-id="711a2-623">人员 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-623">People that are relevant to the user.</span></span> <span data-ttu-id="711a2-624">只读。</span><span class="sxs-lookup"><span data-stu-id="711a2-624">Read-only.</span></span> <span data-ttu-id="711a2-625">可为空。</span><span class="sxs-lookup"><span data-stu-id="711a2-625">Nullable.</span></span>
|<span data-ttu-id="711a2-626">照片</span><span class="sxs-lookup"><span data-stu-id="711a2-626">photo</span></span>|[<span data-ttu-id="711a2-627">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="711a2-627">profilePhoto</span></span>](profilephoto.md)| <span data-ttu-id="711a2-p168">用户的个人资料照片。只读。</span><span class="sxs-lookup"><span data-stu-id="711a2-p168">The user's profile photo. Read-only.</span></span>|
|<span data-ttu-id="711a2-630">计划员</span><span class="sxs-lookup"><span data-stu-id="711a2-630">planner</span></span>|[<span data-ttu-id="711a2-631">plannerUser</span><span class="sxs-lookup"><span data-stu-id="711a2-631">plannerUser</span></span>](planneruser.md)| <span data-ttu-id="711a2-632">plannerUser</span><span class="sxs-lookup"><span data-stu-id="711a2-632">Entry-point to Planner resource that might exist for a Unified Group.</span></span> <span data-ttu-id="711a2-633">只读。</span><span class="sxs-lookup"><span data-stu-id="711a2-633">Read-only.</span></span>|
|<span data-ttu-id="711a2-634">registeredDevices</span><span class="sxs-lookup"><span data-stu-id="711a2-634">registeredDevices</span></span>|<span data-ttu-id="711a2-635">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="711a2-635">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="711a2-p170">已注册的用户的设备。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="711a2-p170">Devices that are registered for the user. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="711a2-639">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="711a2-639">JSON representation</span></span>

<span data-ttu-id="711a2-640">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="711a2-640">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true,
  "optionalProperties": [
    "appRoleAssignments",
    "calendar",
    "calendarGroups",
    "calendarView",
    "calendars",
    "contactFolders",
    "contacts",
    "createdObjects",
    "directReports",
    "drive",
    "events",
    "extensions",
    "joinedGroups",
    "mailFolders",
    "manager",
    "memberOf",
    "messages",
    "oauth2PermissionGrants",
    "onenote",
    "ownedDevices",
    "ownedObjects",
    "photo",
    "registeredDevices"
  ],
  "@odata.type": "microsoft.graph.user",
  "@odata.annotations": [
    {
      "capabilities": {
        "changeTracking": true
      }
    },
    {
      "property": "calendar",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "calendarGroups",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "calendars",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "calendarView",
      "capabilities": {
        "changeTracking": true,
        "deletable": false,
        "expandable": true,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "contactFolders",
      "capabilities": {
        "changeTracking": true,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "contacts",
      "capabilities": {
        "changeTracking": true,
        "expandable": false
      }
    },
    {
      "property": "events",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "inferenceClassification",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false
      }
    },
    {
      "property": "mailFolders",
      "capabilities": {
        "changeTracking": true,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "messages",
      "capabilities": {
        "changeTracking": false,
        "expandable": false
      }
    },
    {
      "property": "people",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "updatable": false
      }
    },
    {
      "property": "photo",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false
      }
    },
    {
      "property": "photos",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "aboutMe": "string",
  "accountEnabled": true,
  "ageGroup": "string",
  "assignedLicenses": [{"@odata.type": "microsoft.graph.assignedLicense"}],
  "assignedPlans": [{"@odata.type": "microsoft.graph.assignedPlan"}],
  "birthday": "String (timestamp)",
  "businessPhones": ["string"],
  "city": "string",
  "companyName": "string",
  "consentProvidedForMinor": "string",
  "country": "string",
  "department": "string",
  "displayName": "string",
  "givenName": "string",
  "hireDate": "String (timestamp)",
  "id": "string (identifier)",
  "imAddresses": ["string"],
  "interests": ["string"],
  "jobTitle": "string",
  "legalAgeGroupClassification": "string",
  "mail": "string",
  "mailboxSettings": {"@odata.type": "microsoft.graph.mailboxSettings"},
  "mailNickname": "string",
  "mobilePhone": "string",
  "mySite": "string",
  "officeLocation": "string",
  "onPremisesImmutableId": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "passwordPolicies": "string",
  "passwordProfile": {"@odata.type": "microsoft.graph.passwordProfile"},
  "pastProjects": ["string"],
  "postalCode": "string",
  "preferredLanguage": "string",
  "preferredName": "string",
  "provisionedPlans": [{"@odata.type": "microsoft.graph.provisionedPlan"}],
  "proxyAddresses": ["string"],
  "responsibilities": ["string"],
  "schools": ["string"],
  "skills": ["string"],
  "state": "string",
  "streetAddress": "string",
  "surname": "string",
  "usageLocation": "string",
  "userPrincipalName": "string",
  "userType": "string",

  "calendar": { "@odata.type": "microsoft.graph.calendar" },
  "calendarGroups": [{ "@odata.type": "microsoft.graph.calendarGroup" }],
  "calendarView": [{ "@odata.type": "microsoft.graph.event" }],
  "calendars": [ {"@odata.type": "microsoft.graph.calendar"} ],
  "contacts": [ { "@odata.type": "microsoft.graph.contact" } ],
  "contactFolders": [ { "@odata.type": "microsoft.graph.contactFolder" } ],
  "createdObjects": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "directReports": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "drives": [ { "@odata.type": "microsoft.graph.drive" } ],
  "events": [ { "@odata.type": "microsoft.graph.event" } ],
  "inferenceClassification": { "@odata.type": "microsoft.graph.inferenceClassification" },
  "mailFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "manager": { "@odata.type": "microsoft.graph.directoryObject" },
  "memberOf": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "outlook": { "@odata.type": "microsoft.graph.outlookUser" },
  "ownedDevices": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "ownedObjects": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "photo": { "@odata.type": "microsoft.graph.profilePhoto" },
  "registeredDevices": [ { "@odata.type": "microsoft.graph.directoryObject" } ]
}

```

## <a name="see-also"></a><span data-ttu-id="711a2-641">另请参阅</span><span class="sxs-lookup"><span data-stu-id="711a2-641">See also</span></span>

- [<span data-ttu-id="711a2-642">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="711a2-642">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="711a2-643">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="711a2-643">Add custom data to users using open extensions</span></span>](../../../concepts/extensibility_open_users.md)
- [<span data-ttu-id="711a2-644">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="711a2-644">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
