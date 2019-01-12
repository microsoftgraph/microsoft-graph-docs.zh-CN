---
title: 用户资源类型
description: 表示 Azure AD 用户帐户。继承自 directoryObject。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1845bdbc349712141c5e356acaaafb8ba1c49aba
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964457"
---
# <a name="user-resource-type"></a><span data-ttu-id="82122-104">用户资源类型</span><span class="sxs-lookup"><span data-stu-id="82122-104">user resource type</span></span>

<span data-ttu-id="82122-p102">表示 Azure AD 用户帐户。继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="82122-p102">Represents an Azure AD user account. Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="82122-107">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="82122-107">This resource supports:</span></span>

- <span data-ttu-id="82122-108">将您自己的数据添加到自定义属性，作为[扩展](/graph/extensibility-overview)。</span><span class="sxs-lookup"><span data-stu-id="82122-108">Adding your own data to custom properties as [extensions](/graph/extensibility-overview).</span></span>
- <span data-ttu-id="82122-109">订阅[更改通知](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="82122-109">Subscribing to [change notifications](/graph/webhooks).</span></span>
- <span data-ttu-id="82122-110">通过提供 [delta](../api/user-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="82122-110">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/user-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="82122-111">方法</span><span class="sxs-lookup"><span data-stu-id="82122-111">Methods</span></span>

| <span data-ttu-id="82122-112">方法</span><span class="sxs-lookup"><span data-stu-id="82122-112">Method</span></span>       | <span data-ttu-id="82122-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="82122-113">Return Type</span></span>  |<span data-ttu-id="82122-114">说明</span><span class="sxs-lookup"><span data-stu-id="82122-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="82122-115">List users</span><span class="sxs-lookup"><span data-stu-id="82122-115">List users</span></span>](../api/user-list.md) |<span data-ttu-id="82122-116">[user](user.md) 集合</span><span class="sxs-lookup"><span data-stu-id="82122-116">[user](user.md) collection</span></span>| <span data-ttu-id="82122-117">获取用户对象列表。</span><span class="sxs-lookup"><span data-stu-id="82122-117">Get a list of user objects.</span></span>|
|[<span data-ttu-id="82122-118">Create user</span><span class="sxs-lookup"><span data-stu-id="82122-118">Create user</span></span>](../api/user-post-users.md) |[<span data-ttu-id="82122-119">user</span><span class="sxs-lookup"><span data-stu-id="82122-119">user</span></span>](user.md)| <span data-ttu-id="82122-120">新建用户对象。</span><span class="sxs-lookup"><span data-stu-id="82122-120">Create a new user object.</span></span>|
|[<span data-ttu-id="82122-121">Get user</span><span class="sxs-lookup"><span data-stu-id="82122-121">Get user</span></span>](../api/user-get.md) | [<span data-ttu-id="82122-122">user</span><span class="sxs-lookup"><span data-stu-id="82122-122">user</span></span>](user.md) |<span data-ttu-id="82122-123">读取 user 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="82122-123">Read properties and relationships of user object.</span></span>|
|[<span data-ttu-id="82122-124">Update user</span><span class="sxs-lookup"><span data-stu-id="82122-124">Update user</span></span>](../api/user-update.md) | [<span data-ttu-id="82122-125">user</span><span class="sxs-lookup"><span data-stu-id="82122-125">user</span></span>](user.md) |<span data-ttu-id="82122-126">更新 user 对象。</span><span class="sxs-lookup"><span data-stu-id="82122-126">Update user object.</span></span> |
|[<span data-ttu-id="82122-127">Delete user</span><span class="sxs-lookup"><span data-stu-id="82122-127">Delete user</span></span>](../api/user-delete.md) | <span data-ttu-id="82122-128">无</span><span class="sxs-lookup"><span data-stu-id="82122-128">None</span></span> |<span data-ttu-id="82122-129">删除 user 对象。</span><span class="sxs-lookup"><span data-stu-id="82122-129">Delete user object.</span></span> |
|[<span data-ttu-id="82122-130">List messages</span><span class="sxs-lookup"><span data-stu-id="82122-130">List messages</span></span>](../api/user-list-messages.md) |<span data-ttu-id="82122-131">[Message](message.md) collection</span><span class="sxs-lookup"><span data-stu-id="82122-131">[Message](message.md) collection</span></span>| <span data-ttu-id="82122-132">获取已登录用户的邮箱中的所有邮件。</span><span class="sxs-lookup"><span data-stu-id="82122-132">Get all the messages in the signed-in user's mailbox.</span></span>|
|[<span data-ttu-id="82122-133">Create Message</span><span class="sxs-lookup"><span data-stu-id="82122-133">Create Message</span></span>](../api/user-post-messages.md) |[<span data-ttu-id="82122-134">Message</span><span class="sxs-lookup"><span data-stu-id="82122-134">Message</span></span>](message.md)| <span data-ttu-id="82122-135">通过发布到邮件集合新建邮件。</span><span class="sxs-lookup"><span data-stu-id="82122-135">Create a new Message by posting to the messages collection.</span></span>|
|[<span data-ttu-id="82122-136">List mailFolders</span><span class="sxs-lookup"><span data-stu-id="82122-136">List mailFolders</span></span>](../api/user-list-mailfolders.md) |<span data-ttu-id="82122-137">[MailFolder](mailfolder.md) collection</span><span class="sxs-lookup"><span data-stu-id="82122-137">[MailFolder](mailfolder.md) collection</span></span>| <span data-ttu-id="82122-138">在已登录用户的根文件夹下获取邮件文件夹集合。</span><span class="sxs-lookup"><span data-stu-id="82122-138">Get the mail folder collection under the root folder of the signed-in user.</span></span> |
|[<span data-ttu-id="82122-139">Create mailFolder</span><span class="sxs-lookup"><span data-stu-id="82122-139">Create mailFolder</span></span>](../api/user-post-mailfolders.md) |[<span data-ttu-id="82122-140">MailFolder</span><span class="sxs-lookup"><span data-stu-id="82122-140">MailFolder</span></span>](mailfolder.md)| <span data-ttu-id="82122-141">通过发布到 mailFolders 集合创建新 MailFolder。</span><span class="sxs-lookup"><span data-stu-id="82122-141">Create a new MailFolder by posting to the mailFolders collection.</span></span>|
|[<span data-ttu-id="82122-142">sendMail</span><span class="sxs-lookup"><span data-stu-id="82122-142">sendMail</span></span>](../api/user-sendmail.md)|<span data-ttu-id="82122-143">None</span><span class="sxs-lookup"><span data-stu-id="82122-143">None</span></span>|<span data-ttu-id="82122-144">发送请求正文中指定的邮件。</span><span class="sxs-lookup"><span data-stu-id="82122-144">Send the message specified in the request body.</span></span>|
|[<span data-ttu-id="82122-145">List events</span><span class="sxs-lookup"><span data-stu-id="82122-145">List events</span></span>](../api/user-list-events.md) |<span data-ttu-id="82122-146">[Event](event.md) collection</span><span class="sxs-lookup"><span data-stu-id="82122-146">[Event](event.md) collection</span></span>| <span data-ttu-id="82122-p103">获取用户邮箱中的 event 对象列表。该列表包含单个实例会议和系列主控形状。</span><span class="sxs-lookup"><span data-stu-id="82122-p103">Get a list of event objects in the user's mailbox. The list contains single instance meetings and series masters.</span></span>|
|[<span data-ttu-id="82122-149">创建事件</span><span class="sxs-lookup"><span data-stu-id="82122-149">Create event</span></span>](../api/user-post-events.md) |[<span data-ttu-id="82122-150">Event</span><span class="sxs-lookup"><span data-stu-id="82122-150">Event</span></span>](event.md)| <span data-ttu-id="82122-151">通过发布到事件集合创建新事件。</span><span class="sxs-lookup"><span data-stu-id="82122-151">Create a new Event by posting to the events collection.</span></span>|
|[<span data-ttu-id="82122-152">List calendars</span><span class="sxs-lookup"><span data-stu-id="82122-152">List calendars</span></span>](../api/user-list-calendars.md) |<span data-ttu-id="82122-153">[Calendar](calendar.md) collection</span><span class="sxs-lookup"><span data-stu-id="82122-153">[Calendar](calendar.md) collection</span></span>| <span data-ttu-id="82122-154">获取 Calendar 对象集合。</span><span class="sxs-lookup"><span data-stu-id="82122-154">Get a Calendar object collection.</span></span>|
|[<span data-ttu-id="82122-155">Create calendar</span><span class="sxs-lookup"><span data-stu-id="82122-155">Create calendar</span></span>](../api/user-post-calendars.md) |[<span data-ttu-id="82122-156">Calendar</span><span class="sxs-lookup"><span data-stu-id="82122-156">Calendar</span></span>](calendar.md)| <span data-ttu-id="82122-157">通过发布到日历集合创建新日历。</span><span class="sxs-lookup"><span data-stu-id="82122-157">Create a new Calendar by posting to the calendars collection.</span></span>|
|[<span data-ttu-id="82122-158">List calendarGroups</span><span class="sxs-lookup"><span data-stu-id="82122-158">List calendarGroups</span></span>](../api/user-list-calendargroups.md) |<span data-ttu-id="82122-159">[CalendarGroup](calendargroup.md) collection</span><span class="sxs-lookup"><span data-stu-id="82122-159">[CalendarGroup](calendargroup.md) collection</span></span>| <span data-ttu-id="82122-160">获取 CalendarGroup 对象集合。</span><span class="sxs-lookup"><span data-stu-id="82122-160">Get a CalendarGroup object collection.</span></span>|
|[<span data-ttu-id="82122-161">Create calendarGroup</span><span class="sxs-lookup"><span data-stu-id="82122-161">Create calendarGroup</span></span>](../api/user-post-calendargroups.md) |[<span data-ttu-id="82122-162">CalendarGroup</span><span class="sxs-lookup"><span data-stu-id="82122-162">CalendarGroup</span></span>](calendargroup.md)| <span data-ttu-id="82122-163">通过发布到 calendarGroups 集合新建 CalendarGroup。</span><span class="sxs-lookup"><span data-stu-id="82122-163">Create a new CalendarGroup by posting to the calendarGroups collection.</span></span>|
|[<span data-ttu-id="82122-164">List calendarView</span><span class="sxs-lookup"><span data-stu-id="82122-164">List calendarView</span></span>](../api/user-list-calendarview.md) |<span data-ttu-id="82122-165">[Event](event.md) collection</span><span class="sxs-lookup"><span data-stu-id="82122-165">[Event](event.md) collection</span></span>| <span data-ttu-id="82122-166">获取 Event 对象集合。</span><span class="sxs-lookup"><span data-stu-id="82122-166">Get a Event object collection.</span></span>|
|[<span data-ttu-id="82122-167">List contacts</span><span class="sxs-lookup"><span data-stu-id="82122-167">List contacts</span></span>](../api/user-list-contacts.md) |<span data-ttu-id="82122-168">[Contact](contact.md) collection</span><span class="sxs-lookup"><span data-stu-id="82122-168">[Contact](contact.md) collection</span></span>| <span data-ttu-id="82122-169">从已登录用户的默认联系人文件夹中获取联系人集合。</span><span class="sxs-lookup"><span data-stu-id="82122-169">Get a contact collection from the default Contacts folder of the signed-in user.</span></span>|
|[<span data-ttu-id="82122-170">Create Contact</span><span class="sxs-lookup"><span data-stu-id="82122-170">Create Contact</span></span>](../api/user-post-contacts.md) |[<span data-ttu-id="82122-171">Contact</span><span class="sxs-lookup"><span data-stu-id="82122-171">Contact</span></span>](contact.md)| <span data-ttu-id="82122-172">通过发布到联系人集合新建联系人。</span><span class="sxs-lookup"><span data-stu-id="82122-172">Create a new Contact by posting to the contacts collection.</span></span>|
|[<span data-ttu-id="82122-173">List contactFolders</span><span class="sxs-lookup"><span data-stu-id="82122-173">List contactFolders</span></span>](../api/user-list-contactfolders.md) |<span data-ttu-id="82122-174">[ContactFolder](contactfolder.md) collection</span><span class="sxs-lookup"><span data-stu-id="82122-174">[ContactFolder](contactfolder.md) collection</span></span>| <span data-ttu-id="82122-175">获取已登录用户的默认联系人文件夹中的联系人文件夹集合。</span><span class="sxs-lookup"><span data-stu-id="82122-175">Get the contact folder collection in the default Contacts folder of the signed-in user.</span></span>|
|[<span data-ttu-id="82122-176">Create ContactFolder</span><span class="sxs-lookup"><span data-stu-id="82122-176">Create ContactFolder</span></span>](../api/user-post-contactfolders.md) |[<span data-ttu-id="82122-177">ContactFolder</span><span class="sxs-lookup"><span data-stu-id="82122-177">ContactFolder</span></span>](contactfolder.md)| <span data-ttu-id="82122-178">通过发布到 contactFolders 集合创建新 ContactFolder。</span><span class="sxs-lookup"><span data-stu-id="82122-178">Create a new ContactFolder by posting to the contactFolders collection.</span></span>|
|[<span data-ttu-id="82122-179">List directReports</span><span class="sxs-lookup"><span data-stu-id="82122-179">List directReports</span></span>](../api/user-list-directreports.md) |<span data-ttu-id="82122-180">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="82122-180">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="82122-181">从 directReports 导航属性中获取向此用户报告的用户和联系人。</span><span class="sxs-lookup"><span data-stu-id="82122-181">Get the users and contacts that report to the user from the directReports navigation property.</span></span>|
|[<span data-ttu-id="82122-182">List manager</span><span class="sxs-lookup"><span data-stu-id="82122-182">List manager</span></span>](../api/user-list-manager.md) |[<span data-ttu-id="82122-183">directoryObject</span><span class="sxs-lookup"><span data-stu-id="82122-183">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="82122-184">从 manager 导航属性中获取是此用户的经理的用户或联系人。</span><span class="sxs-lookup"><span data-stu-id="82122-184">Get the user or contact that is this user's manager from the manager navigation property.</span></span>|
|[<span data-ttu-id="82122-185">List memberOf</span><span class="sxs-lookup"><span data-stu-id="82122-185">List memberOf</span></span>](../api/user-list-memberof.md) |<span data-ttu-id="82122-186">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="82122-186">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="82122-187">从 memberOf 导航属性中获取此用户是其直接成员的组和目录角色。</span><span class="sxs-lookup"><span data-stu-id="82122-187">Get the groups and directory roles that the user is a direct member of from the memberOf navigation property.</span></span>|
|[<span data-ttu-id="82122-188">List ownedDevices</span><span class="sxs-lookup"><span data-stu-id="82122-188">List ownedDevices</span></span>](../api/user-list-owneddevices.md) |<span data-ttu-id="82122-189">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="82122-189">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="82122-190">从 ownedDevices 导航属性中获取此用户所拥有的设备。</span><span class="sxs-lookup"><span data-stu-id="82122-190">Get the devices that are owned by the user from the ownedDevices navigation property.</span></span>|
|[<span data-ttu-id="82122-191">List ownedObjects</span><span class="sxs-lookup"><span data-stu-id="82122-191">List ownedObjects</span></span>](../api/user-list-ownedobjects.md) |<span data-ttu-id="82122-192">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="82122-192">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="82122-193">从 ownedObjects 导航属性中获取此用户所拥有的目录对象。</span><span class="sxs-lookup"><span data-stu-id="82122-193">Get the directory objects that are owned by the user from the ownedObjects navigation property.</span></span>|
|[<span data-ttu-id="82122-194">List registeredDevices</span><span class="sxs-lookup"><span data-stu-id="82122-194">List registeredDevices</span></span>](../api/user-list-registereddevices.md) |<span data-ttu-id="82122-195">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="82122-195">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="82122-196">从 registeredDevices 导航属性中获取为此用户注册的设备。</span><span class="sxs-lookup"><span data-stu-id="82122-196">Get the devices that are retistered for the user from the registeredDevices navigation property.</span></span>|
|[<span data-ttu-id="82122-197">List createdObjects</span><span class="sxs-lookup"><span data-stu-id="82122-197">List createdObjects</span></span>](../api/user-list-createdobjects.md) |<span data-ttu-id="82122-198">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="82122-198">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="82122-199">从 createdObjects 导航属性中获取此用户创建的目录对象。</span><span class="sxs-lookup"><span data-stu-id="82122-199">Get the directory objects created by the user from the createdObjects navigation property.</span></span>|
|[<span data-ttu-id="82122-200">assignLicense</span><span class="sxs-lookup"><span data-stu-id="82122-200">assignLicense</span></span>](../api/user-assignlicense.md)|[<span data-ttu-id="82122-201">用户</span><span class="sxs-lookup"><span data-stu-id="82122-201">user</span></span>](user.md)|<span data-ttu-id="82122-p104">为用户添加或删除订阅。还可以启用和禁用与订阅相关的特定计划。</span><span class="sxs-lookup"><span data-stu-id="82122-p104">Add or remove subscriptions for the user. You can also enable and disable specific plans associated with a subscription.</span></span>|
|[<span data-ttu-id="82122-204">List licenseDetails</span><span class="sxs-lookup"><span data-stu-id="82122-204">List licenseDetails</span></span>](../api/user-list-licensedetails.md) |<span data-ttu-id="82122-205">[licenseDetails](licensedetails.md) 集合</span><span class="sxs-lookup"><span data-stu-id="82122-205">[licenseDetails](licensedetails.md) collection</span></span>| <span data-ttu-id="82122-206">获取 licenseDetails 对象集合。</span><span class="sxs-lookup"><span data-stu-id="82122-206">Get a licenseDetails object collection.</span></span>|
|[<span data-ttu-id="82122-207">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="82122-207">checkMemberGroups</span></span>](../api/user-checkmembergroups.md)|<span data-ttu-id="82122-208">String collection</span><span class="sxs-lookup"><span data-stu-id="82122-208">String collection</span></span>|<span data-ttu-id="82122-p105">检查组列表中的成员身份。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="82122-p105">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="82122-211">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="82122-211">getMemberGroups</span></span>](../api/user-getmembergroups.md)|<span data-ttu-id="82122-212">String collection</span><span class="sxs-lookup"><span data-stu-id="82122-212">String collection</span></span>|<span data-ttu-id="82122-p106">返回用户是其成员的所有组。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="82122-p106">Return all the groups that the user is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="82122-215">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="82122-215">getMemberObjects</span></span>](../api/user-getmemberobjects.md)|<span data-ttu-id="82122-216">String collection</span><span class="sxs-lookup"><span data-stu-id="82122-216">String collection</span></span>| <span data-ttu-id="82122-p107">返回用户所属的所有组和目录角色。检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="82122-p107">Return all of the groups and directory roles that the user is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="82122-219">reminderView</span><span class="sxs-lookup"><span data-stu-id="82122-219">reminderView</span></span>](../api/user-reminderview.md)|<span data-ttu-id="82122-220">[Reminder](reminder.md) collection</span><span class="sxs-lookup"><span data-stu-id="82122-220">[Reminder](reminder.md) collection</span></span>|<span data-ttu-id="82122-221">返回指定开始时间和结束时间范围内的日历提醒列表。</span><span class="sxs-lookup"><span data-stu-id="82122-221">Return a list of calendar reminders within the start and end times specified.</span></span>|
|[<span data-ttu-id="82122-222">delta</span><span class="sxs-lookup"><span data-stu-id="82122-222">delta</span></span>](../api/user-delta.md)|<span data-ttu-id="82122-223">用户集合</span><span class="sxs-lookup"><span data-stu-id="82122-223">user collection</span></span>| <span data-ttu-id="82122-224">获取用户的增量更改。</span><span class="sxs-lookup"><span data-stu-id="82122-224">Get incremental changes for users.</span></span> |
|<span data-ttu-id="82122-225">**开放扩展**</span><span class="sxs-lookup"><span data-stu-id="82122-225">**Open extensions**</span></span>| | |
|[<span data-ttu-id="82122-226">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="82122-226">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="82122-227">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="82122-227">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="82122-228">创建开放扩展，并将自定义属性添加到新资源或现有资源。</span><span class="sxs-lookup"><span data-stu-id="82122-228">Create an open extension and add custom properties to a new or existing resource.</span></span>|
|[<span data-ttu-id="82122-229">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="82122-229">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="82122-230">[openTypeExtension](opentypeextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="82122-230">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="82122-231">获取扩展名称标识的开放扩展。</span><span class="sxs-lookup"><span data-stu-id="82122-231">Get an open extension identified by the extension name.</span></span>|
|<span data-ttu-id="82122-232">**架构扩展**</span><span class="sxs-lookup"><span data-stu-id="82122-232">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="82122-233">添加架构扩展值</span><span class="sxs-lookup"><span data-stu-id="82122-233">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="82122-234">创建架构扩展定义，然后使用它向资源添加自定义键入数据。</span><span class="sxs-lookup"><span data-stu-id="82122-234">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|

## <a name="properties"></a><span data-ttu-id="82122-235">属性</span><span class="sxs-lookup"><span data-stu-id="82122-235">Properties</span></span>

| <span data-ttu-id="82122-236">属性</span><span class="sxs-lookup"><span data-stu-id="82122-236">Property</span></span>       | <span data-ttu-id="82122-237">类型</span><span class="sxs-lookup"><span data-stu-id="82122-237">Type</span></span>    |<span data-ttu-id="82122-238">说明</span><span class="sxs-lookup"><span data-stu-id="82122-238">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="82122-239">aboutMe</span><span class="sxs-lookup"><span data-stu-id="82122-239">aboutMe</span></span>|<span data-ttu-id="82122-240">String</span><span class="sxs-lookup"><span data-stu-id="82122-240">String</span></span>|<span data-ttu-id="82122-241">任意形式的文本输入字段，用于介绍用户自身。</span><span class="sxs-lookup"><span data-stu-id="82122-241">A freeform text entry field for the user to describe themselves.</span></span>|
|<span data-ttu-id="82122-242">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="82122-242">accountEnabled</span></span>|<span data-ttu-id="82122-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="82122-243">Boolean</span></span>| <span data-ttu-id="82122-p108">启用帐户时为 **true**，否则为 **false**。创建用户时此属性是必需的。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="82122-p108">**true** if the account is enabled; otherwise, **false**. This property is required when a user is created. Supports $filter.</span></span>    |
|<span data-ttu-id="82122-247">ageGroup</span><span class="sxs-lookup"><span data-stu-id="82122-247">ageGroup</span></span>|<span data-ttu-id="82122-248">字符串</span><span class="sxs-lookup"><span data-stu-id="82122-248">String</span></span>|<span data-ttu-id="82122-249">设置用户的年龄组。</span><span class="sxs-lookup"><span data-stu-id="82122-249">Sets the age group of the user.</span></span> <span data-ttu-id="82122-250">允许值： `null`， `minor`，`notAdult`和`adult`。</span><span class="sxs-lookup"><span data-stu-id="82122-250">Allowed values: `null`, `minor`, `notAdult` and `adult`.</span></span> <span data-ttu-id="82122-251">请参阅[法律期限组属性定义](#legal-age-group-property-definitions)有关详细信息。</span><span class="sxs-lookup"><span data-stu-id="82122-251">Refer to the [legal age group property definitions](#legal-age-group-property-definitions) for further information.</span></span> |
|<span data-ttu-id="82122-252">assignedLicenses</span><span class="sxs-lookup"><span data-stu-id="82122-252">assignedLicenses</span></span>|<span data-ttu-id="82122-253">[assignedLicense](assignedlicense.md) collection</span><span class="sxs-lookup"><span data-stu-id="82122-253">[assignedLicense](assignedlicense.md) collection</span></span>|<span data-ttu-id="82122-p110">分配给该用户的许可证。不可为 null。</span><span class="sxs-lookup"><span data-stu-id="82122-p110">The licenses that are assigned to the user. Not nullable.</span></span>            |
|<span data-ttu-id="82122-256">assignedPlans</span><span class="sxs-lookup"><span data-stu-id="82122-256">assignedPlans</span></span>|<span data-ttu-id="82122-257">[assignedPlan](assignedplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="82122-257">[assignedPlan](assignedplan.md) collection</span></span>|<span data-ttu-id="82122-p111">分配给该用户的计划。只读。不可为 null。</span><span class="sxs-lookup"><span data-stu-id="82122-p111">The plans that are assigned to the user. Read-only. Not nullable.</span></span> |
|<span data-ttu-id="82122-261">birthday</span><span class="sxs-lookup"><span data-stu-id="82122-261">birthday</span></span>|<span data-ttu-id="82122-262">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82122-262">DateTimeOffset</span></span>|<span data-ttu-id="82122-p112">用户的生日。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="82122-p112">The birthday of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="82122-266">businessPhones</span><span class="sxs-lookup"><span data-stu-id="82122-266">businessPhones</span></span>|<span data-ttu-id="82122-267">String collection</span><span class="sxs-lookup"><span data-stu-id="82122-267">String collection</span></span>|<span data-ttu-id="82122-p113">用户的电话号码。注意：虽然这是字符串集合，但是只能为该属性设置一个号码。</span><span class="sxs-lookup"><span data-stu-id="82122-p113">The telephone numbers for the user. NOTE: Although this is a string collection, only one number can be set for this property.</span></span>|
|<span data-ttu-id="82122-270">城市</span><span class="sxs-lookup"><span data-stu-id="82122-270">city</span></span>|<span data-ttu-id="82122-271">字符串</span><span class="sxs-lookup"><span data-stu-id="82122-271">String</span></span>|<span data-ttu-id="82122-p114">用户所在的城市。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="82122-p114">The city in which the user is located. Supports $filter.</span></span>|
|<span data-ttu-id="82122-274">companyName</span><span class="sxs-lookup"><span data-stu-id="82122-274">companyName</span></span> | <span data-ttu-id="82122-275">String</span><span class="sxs-lookup"><span data-stu-id="82122-275">String</span></span> | <span data-ttu-id="82122-276">与用户关联的公司名称。</span><span class="sxs-lookup"><span data-stu-id="82122-276">The company name which the user is associated.</span></span> <span data-ttu-id="82122-277">只读。</span><span class="sxs-lookup"><span data-stu-id="82122-277">Read-only.</span></span> |
|<span data-ttu-id="82122-278">consentProvidedForMinor</span><span class="sxs-lookup"><span data-stu-id="82122-278">consentProvidedForMinor</span></span>|<span data-ttu-id="82122-279">字符串</span><span class="sxs-lookup"><span data-stu-id="82122-279">String</span></span>|<span data-ttu-id="82122-280">设置是否已为未成年人获得许可。</span><span class="sxs-lookup"><span data-stu-id="82122-280">Sets whether consent has been obtained for minors.</span></span> <span data-ttu-id="82122-281">允许值： `null`， `granted`，`denied`和`notRequired`。</span><span class="sxs-lookup"><span data-stu-id="82122-281">Allowed values: `null`, `granted`, `denied` and `notRequired`.</span></span> <span data-ttu-id="82122-282">请参阅[法律期限组属性定义](#legal-age-group-property-definitions)有关详细信息。</span><span class="sxs-lookup"><span data-stu-id="82122-282">Refer to the [legal age group property definitions](#legal-age-group-property-definitions) for further information.</span></span>|
|<span data-ttu-id="82122-283">country</span><span class="sxs-lookup"><span data-stu-id="82122-283">country</span></span>|<span data-ttu-id="82122-284">String</span><span class="sxs-lookup"><span data-stu-id="82122-284">String</span></span>|<span data-ttu-id="82122-p117">用户所在的国家/地区；例如，“美国”或“英国”。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="82122-p117">The country/region in which the user is located; for example, “US” or “UK”. Supports $filter.</span></span>|
|<span data-ttu-id="82122-287">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="82122-287">createdDateTime</span></span> | <span data-ttu-id="82122-288">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82122-288">DateTimeOffset</span></span> |<span data-ttu-id="82122-289">用户对象的创建的日期。</span><span class="sxs-lookup"><span data-stu-id="82122-289">The created date of the user object.</span></span> |
|<span data-ttu-id="82122-290">department</span><span class="sxs-lookup"><span data-stu-id="82122-290">department</span></span>|<span data-ttu-id="82122-291">字符串</span><span class="sxs-lookup"><span data-stu-id="82122-291">String</span></span>|<span data-ttu-id="82122-p118">用户工作部门的名称。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="82122-p118">The name for the department in which the user works. Supports $filter.</span></span>|
|<span data-ttu-id="82122-294">displayName</span><span class="sxs-lookup"><span data-stu-id="82122-294">displayName</span></span>|<span data-ttu-id="82122-295">字符串</span><span class="sxs-lookup"><span data-stu-id="82122-295">String</span></span>|<span data-ttu-id="82122-p119">用户通讯簿中显示的名称。这通常是用户名字、中间名首字母和姓氏的组合。此属性在创建用户时是必需的，并且在更新过程中不能清除。支持 $filter 和 $orderby。</span><span class="sxs-lookup"><span data-stu-id="82122-p119">The name displayed in the address book for the user. This is usually the combination of the user's first name, middle initial and last name. This property is required when a user is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="82122-300">givenName</span><span class="sxs-lookup"><span data-stu-id="82122-300">givenName</span></span>|<span data-ttu-id="82122-301">字符串</span><span class="sxs-lookup"><span data-stu-id="82122-301">String</span></span>|<span data-ttu-id="82122-p120">用户的名。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="82122-p120">The given name (first name) of the user. Supports $filter.</span></span>|
|<span data-ttu-id="82122-304">hireDate</span><span class="sxs-lookup"><span data-stu-id="82122-304">hireDate</span></span>|<span data-ttu-id="82122-305">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82122-305">DateTimeOffset</span></span>|<span data-ttu-id="82122-p121">用户的雇佣日期。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="82122-p121">The hire date of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="82122-309">id</span><span class="sxs-lookup"><span data-stu-id="82122-309">id</span></span>|<span data-ttu-id="82122-310">String</span><span class="sxs-lookup"><span data-stu-id="82122-310">String</span></span>|<span data-ttu-id="82122-p122">用户的唯一标识符。继承自 [directoryObject](directoryobject.md)。键。不可为 null。只读。</span><span class="sxs-lookup"><span data-stu-id="82122-p122">The unique identifier for the user. Inherited from [directoryObject](directoryobject.md). Key. Not nullable. Read-only.</span></span>|
|<span data-ttu-id="82122-316">imAddresses</span><span class="sxs-lookup"><span data-stu-id="82122-316">imAddresses</span></span>|<span data-ttu-id="82122-317">String collection</span><span class="sxs-lookup"><span data-stu-id="82122-317">String collection</span></span>|<span data-ttu-id="82122-p123">用户的即时消息 IP 语音 (VOIP) 会话初始协议 (SIP) 地址。只读。</span><span class="sxs-lookup"><span data-stu-id="82122-p123">The instant message voice over IP (VOIP) session initiation protocol (SIP) addresses for the user. Read-only.</span></span>|
|<span data-ttu-id="82122-320">interests</span><span class="sxs-lookup"><span data-stu-id="82122-320">interests</span></span>|<span data-ttu-id="82122-321">String collection</span><span class="sxs-lookup"><span data-stu-id="82122-321">String collection</span></span>|<span data-ttu-id="82122-322">用户介绍自身兴趣的列表。</span><span class="sxs-lookup"><span data-stu-id="82122-322">A list for the user to describe their interests.</span></span>|
|<span data-ttu-id="82122-323">jobTitle</span><span class="sxs-lookup"><span data-stu-id="82122-323">jobTitle</span></span>|<span data-ttu-id="82122-324">字符串</span><span class="sxs-lookup"><span data-stu-id="82122-324">String</span></span>|<span data-ttu-id="82122-p124">用户的职务。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="82122-p124">The user’s job title. Supports $filter.</span></span>|
|<span data-ttu-id="82122-327">legalAgeGroupClassification</span><span class="sxs-lookup"><span data-stu-id="82122-327">legalAgeGroupClassification</span></span>|<span data-ttu-id="82122-328">String</span><span class="sxs-lookup"><span data-stu-id="82122-328">String</span></span>| <span data-ttu-id="82122-329">企业应用程序用于确定的用户的法律年龄组。</span><span class="sxs-lookup"><span data-stu-id="82122-329">Used by enterprise applications to determine the legal age group of the user.</span></span> <span data-ttu-id="82122-330">此属性是只读的计算基于`ageGroup`和`consentProvidedForMinor`属性。</span><span class="sxs-lookup"><span data-stu-id="82122-330">This property is read-only and calculated based on `ageGroup` and `consentProvidedForMinor` properties.</span></span> <span data-ttu-id="82122-331">允许值： `null`， `minorWithOutParentalConsent`， `minorWithParentalConsent`， `minorNoParentalConsentRequired`，`notAdult`和`adult`。</span><span class="sxs-lookup"><span data-stu-id="82122-331">Allowed values: `null`, `minorWithOutParentalConsent`, `minorWithParentalConsent`, `minorNoParentalConsentRequired`, `notAdult` and `adult`.</span></span> <span data-ttu-id="82122-332">引用[法律期限组属性定义](#legal-age-group-property-definitions)有关详细信息。）</span><span class="sxs-lookup"><span data-stu-id="82122-332">Refer to the [legal age group property definitions](#legal-age-group-property-definitions) for further information.)</span></span>|
|<span data-ttu-id="82122-333">mail</span><span class="sxs-lookup"><span data-stu-id="82122-333">mail</span></span>|<span data-ttu-id="82122-334">字符串</span><span class="sxs-lookup"><span data-stu-id="82122-334">String</span></span>|<span data-ttu-id="82122-p126">用户的 SMTP 地址，例如，“jeff@contoso.onmicrosoft.com”。只读。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="82122-p126">The SMTP address for the user, for example, "jeff@contoso.onmicrosoft.com". Read-Only. Supports $filter.</span></span>|
|<span data-ttu-id="82122-338">mailboxSettings</span><span class="sxs-lookup"><span data-stu-id="82122-338">mailboxSettings</span></span>|[<span data-ttu-id="82122-339">mailboxSettings</span><span class="sxs-lookup"><span data-stu-id="82122-339">mailboxSettings</span></span>](mailboxsettings.md)|<span data-ttu-id="82122-p127">已登录用户的主邮箱的设置。可以[获取](../api/user-get-mailboxsettings.md)或[更新](../api/user-update-mailboxsettings.md)用于向传入邮件发送自动答复、区域设置和时区的设置。</span><span class="sxs-lookup"><span data-stu-id="82122-p127">Settings for the primary mailbox of the signed-in user. You can [get](../api/user-get-mailboxsettings.md) or [update](../api/user-update-mailboxsettings.md) settings for sending automatic replies to incoming messages, locale and time zone.</span></span>|
|<span data-ttu-id="82122-342">mailNickname</span><span class="sxs-lookup"><span data-stu-id="82122-342">mailNickname</span></span>|<span data-ttu-id="82122-343">字符串</span><span class="sxs-lookup"><span data-stu-id="82122-343">String</span></span>|<span data-ttu-id="82122-p128">用户的邮件别名。创建用户时必须指定此属性。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="82122-p128">The mail alias for the user. This property must be specified when a user is created. Supports $filter.</span></span>|
|<span data-ttu-id="82122-347">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="82122-347">mobilePhone</span></span>|<span data-ttu-id="82122-348">String</span><span class="sxs-lookup"><span data-stu-id="82122-348">String</span></span>|<span data-ttu-id="82122-349">用户的主要移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="82122-349">The primary cellular telephone number for the user.</span></span>|
|<span data-ttu-id="82122-350">mySite</span><span class="sxs-lookup"><span data-stu-id="82122-350">mySite</span></span>|<span data-ttu-id="82122-351">String</span><span class="sxs-lookup"><span data-stu-id="82122-351">String</span></span>|<span data-ttu-id="82122-352">用户个人网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="82122-352">The URL for the user's personal site.</span></span>|
|<span data-ttu-id="82122-353">officeLocation</span><span class="sxs-lookup"><span data-stu-id="82122-353">officeLocation</span></span>|<span data-ttu-id="82122-354">String</span><span class="sxs-lookup"><span data-stu-id="82122-354">String</span></span>|<span data-ttu-id="82122-355">用户公司地点的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="82122-355">The office location in the user's place of business.</span></span>|
|<span data-ttu-id="82122-356">onPremisesDomainName</span><span class="sxs-lookup"><span data-stu-id="82122-356">onPremisesDomainName</span></span>|<span data-ttu-id="82122-357">字符串</span><span class="sxs-lookup"><span data-stu-id="82122-357">String</span></span>| <span data-ttu-id="82122-358">包含本地`domainFQDN`，也称为 dnsDomainName 从内部部署目录同步。</span><span class="sxs-lookup"><span data-stu-id="82122-358">Contains the on-premises `domainFQDN`, also called dnsDomainName synchronized from the on-premises directory.</span></span> <span data-ttu-id="82122-359">正在同步到 Azure Active Directory Azure AD 连接通过其内部部署目录的客户仅填充属性。</span><span class="sxs-lookup"><span data-stu-id="82122-359">The property is only populated for customers who are synchronizing their on-premises directory to Azure Active Directory via Azure AD Connect.</span></span> <span data-ttu-id="82122-360">只读。</span><span class="sxs-lookup"><span data-stu-id="82122-360">Read-only.</span></span> |
|<span data-ttu-id="82122-361">onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="82122-361">onPremisesExtensionAttributes</span></span>|[<span data-ttu-id="82122-362">OnPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="82122-362">OnPremisesExtensionAttributes</span></span>](onpremisesextensionattributes.md)|<span data-ttu-id="82122-363">包含用户的 extensionAttributes 1-15。</span><span class="sxs-lookup"><span data-stu-id="82122-363">Contains extensionAttributes 1-15 for the user.</span></span> <span data-ttu-id="82122-364">请注意，单个扩展属性既不可选，也不可筛选。</span><span class="sxs-lookup"><span data-stu-id="82122-364">Note that the individual extension attributes are neither selectable nor filterable.</span></span> <span data-ttu-id="82122-365">为`onPremisesSyncEnabled`用户，此组属性是主要的内部部署和是只读的。</span><span class="sxs-lookup"><span data-stu-id="82122-365">For an `onPremisesSyncEnabled` user, this set of properties is mastered on-premises and is read-only.</span></span> <span data-ttu-id="82122-366">仅限云用户 (其中`onPremisesSyncEnabled`为 false)，这些属性的创建过程中可以设置或更新。</span><span class="sxs-lookup"><span data-stu-id="82122-366">For a cloud-only user (where `onPremisesSyncEnabled` is false), these properties may be set during creation or update.</span></span> |
|<span data-ttu-id="82122-367">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="82122-367">onPremisesImmutableId</span></span>|<span data-ttu-id="82122-368">字符串</span><span class="sxs-lookup"><span data-stu-id="82122-368">String</span></span>|<span data-ttu-id="82122-369">此属性用于将内部部署 Active Directory 用户帐户对其 Azure AD 用户对象相关联。</span><span class="sxs-lookup"><span data-stu-id="82122-369">This property is used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span> <span data-ttu-id="82122-370">在此图中创建新的用户帐户，如果您使用的联盟的域用户的**userPrincipalName** (UPN) 属性时，必须指定此属性。</span><span class="sxs-lookup"><span data-stu-id="82122-370">This property must be specified when creating a new user account in the Graph if you are using a federated domain for the user’s **userPrincipalName** (UPN) property.</span></span> <span data-ttu-id="82122-371">**重要：\*\*\*\*$** 和**\_** 指定此属性时，不能使用字符。</span><span class="sxs-lookup"><span data-stu-id="82122-371">**Important:** The **$** and **\_** characters cannot be used when specifying this property.</span></span> <span data-ttu-id="82122-372">支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="82122-372">Supports $filter.</span></span>                            |
|<span data-ttu-id="82122-373">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="82122-373">onPremisesLastSyncDateTime</span></span>|<span data-ttu-id="82122-374">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82122-374">DateTimeOffset</span></span>|<span data-ttu-id="82122-p132">表示上一次对象与本地目录同步的时间；例如：“2013-02-16T03:04:54Z”。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。</span><span class="sxs-lookup"><span data-stu-id="82122-p132">Indicates the last time at which the object was synced with the on-premises directory; for example: "2013-02-16T03:04:54Z". The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="82122-379">onPremisesProvisioningErrors</span><span class="sxs-lookup"><span data-stu-id="82122-379">onPremisesProvisioningErrors</span></span>|<span data-ttu-id="82122-380">[onPremisesProvisioningError](onpremisesprovisioningerror.md)集合</span><span class="sxs-lookup"><span data-stu-id="82122-380">[onPremisesProvisioningError](onpremisesprovisioningerror.md) collection</span></span>| <span data-ttu-id="82122-381">设置过程中使用 Microsoft 同步产品时错误。</span><span class="sxs-lookup"><span data-stu-id="82122-381">Errors when using Microsoft synchronization product during provisioning.</span></span> |
|<span data-ttu-id="82122-382">onPremisesSamAccountName</span><span class="sxs-lookup"><span data-stu-id="82122-382">onPremisesSamAccountName</span></span>|<span data-ttu-id="82122-383">字符串</span><span class="sxs-lookup"><span data-stu-id="82122-383">String</span></span>| <span data-ttu-id="82122-384">包含本地`samAccountName`从内部部署目录同步。</span><span class="sxs-lookup"><span data-stu-id="82122-384">Contains the on-premises `samAccountName` synchronized from the on-premises directory.</span></span> <span data-ttu-id="82122-385">正在同步到 Azure Active Directory Azure AD 连接通过其内部部署目录的客户仅填充属性。</span><span class="sxs-lookup"><span data-stu-id="82122-385">The property is only populated for customers who are synchronizing their on-premises directory to Azure Active Directory via Azure AD Connect.</span></span> <span data-ttu-id="82122-386">只读。</span><span class="sxs-lookup"><span data-stu-id="82122-386">Read-only.</span></span> |
|<span data-ttu-id="82122-387">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="82122-387">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="82122-388">字符串</span><span class="sxs-lookup"><span data-stu-id="82122-388">String</span></span>|<span data-ttu-id="82122-p134">包含从本地同步到云的用户的本地安全标识符 (SID)。只读。</span><span class="sxs-lookup"><span data-stu-id="82122-p134">Contains the on-premises security identifier (SID) for the user that was synchronized from on-premises to the cloud. Read-only.</span></span>|
|<span data-ttu-id="82122-391">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="82122-391">onPremisesSyncEnabled</span></span>|<span data-ttu-id="82122-392">Boolean</span><span class="sxs-lookup"><span data-stu-id="82122-392">Boolean</span></span>| <span data-ttu-id="82122-p135">如果此对象从本地目录同步，则为 **true**；如果此对象最初从本地目录同步，但以后不再同步，则为 **false**；如果此对象从未从本地目录同步，则为 **null**（默认值）。只读</span><span class="sxs-lookup"><span data-stu-id="82122-p135">**true** if this object is synced from an on-premises directory; **false** if this object was originally synced from an on-premises directory but is no longer synced; **null** if this object has never been synced from an on-premises directory (default). Read-only</span></span> |
|<span data-ttu-id="82122-395">onPremisesUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="82122-395">onPremisesUserPrincipalName</span></span>|<span data-ttu-id="82122-396">字符串</span><span class="sxs-lookup"><span data-stu-id="82122-396">String</span></span>| <span data-ttu-id="82122-397">包含本地`userPrincipalName`从内部部署目录同步。</span><span class="sxs-lookup"><span data-stu-id="82122-397">Contains the on-premises `userPrincipalName` synchronized from the on-premises directory.</span></span> <span data-ttu-id="82122-398">正在同步到 Azure Active Directory Azure AD 连接通过其内部部署目录的客户仅填充属性。</span><span class="sxs-lookup"><span data-stu-id="82122-398">The property is only populated for customers who are synchronizing their on-premises directory to Azure Active Directory via Azure AD Connect.</span></span> <span data-ttu-id="82122-399">只读。</span><span class="sxs-lookup"><span data-stu-id="82122-399">Read-only.</span></span> |
|<span data-ttu-id="82122-400">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="82122-400">passwordPolicies</span></span>|<span data-ttu-id="82122-401">字符串</span><span class="sxs-lookup"><span data-stu-id="82122-401">String</span></span>|<span data-ttu-id="82122-p137">指定用户的密码策略。此值是一个枚举，具有一个可能值“DisableStrongPassword”，允许指定比默认策略弱的密码。还可以指定“DisablePasswordExpiration”。可以同时指定这两个策略；例如：“DisablePasswordExpiration、DisableStrongPassword”。</span><span class="sxs-lookup"><span data-stu-id="82122-p137">Specifies password policies for the user. This value is an enumeration with one possible value being “DisableStrongPassword”, which allows weaker passwords than the default policy to be specified. “DisablePasswordExpiration” can also be specified. The two may be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".</span></span>|
|<span data-ttu-id="82122-406">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="82122-406">passwordProfile</span></span>|[<span data-ttu-id="82122-407">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="82122-407">PasswordProfile</span></span>](passwordprofile.md)|<span data-ttu-id="82122-p138">指定用户的密码配置文件。配置文件包含用户的密码。创建用户时此属性是必需的。配置文件中的密码必须满足 **passwordPolicies** 属性指定的最低要求。默认情况下，必须使用强密码。</span><span class="sxs-lookup"><span data-stu-id="82122-p138">Specifies the password profile for the user. The profile contains the user’s password. This property is required when a user is created. The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property. By default, a strong password is required.</span></span>|
|<span data-ttu-id="82122-413">pastProjects</span><span class="sxs-lookup"><span data-stu-id="82122-413">pastProjects</span></span>|<span data-ttu-id="82122-414">String collection</span><span class="sxs-lookup"><span data-stu-id="82122-414">String collection</span></span>|<span data-ttu-id="82122-415">供用户枚举其过去项目的列表。</span><span class="sxs-lookup"><span data-stu-id="82122-415">A list for the user to enumerate their past projects.</span></span>|
|<span data-ttu-id="82122-416">postalCode</span><span class="sxs-lookup"><span data-stu-id="82122-416">postalCode</span></span>|<span data-ttu-id="82122-417">字符串</span><span class="sxs-lookup"><span data-stu-id="82122-417">String</span></span>|<span data-ttu-id="82122-p139">用户邮政地址的邮政编码。邮政编码特定于用户所在的国家/地区。在美国，此属性包含邮政编码。</span><span class="sxs-lookup"><span data-stu-id="82122-p139">The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.</span></span>|
|<span data-ttu-id="82122-421">preferredDataLocation</span><span class="sxs-lookup"><span data-stu-id="82122-421">preferredDataLocation</span></span>|<span data-ttu-id="82122-422">字符串</span><span class="sxs-lookup"><span data-stu-id="82122-422">String</span></span>|<span data-ttu-id="82122-423">用户首选的数据位置。</span><span class="sxs-lookup"><span data-stu-id="82122-423">The preferred data location for the user.</span></span> <span data-ttu-id="82122-424">有关详细信息，请参阅[OneDrive 联机多地理](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction)。</span><span class="sxs-lookup"><span data-stu-id="82122-424">For more information, see [OneDrive Online Multi-Geo](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction).</span></span>|
|<span data-ttu-id="82122-425">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="82122-425">preferredLanguage</span></span>|<span data-ttu-id="82122-426">字符串</span><span class="sxs-lookup"><span data-stu-id="82122-426">String</span></span>|<span data-ttu-id="82122-p141">用户的首选语言。应遵循 ISO 639-1 代码；例如“EN-US”。</span><span class="sxs-lookup"><span data-stu-id="82122-p141">The preferred language for the user. Should follow ISO 639-1 Code; for example "en-US".</span></span>|
|<span data-ttu-id="82122-429">preferredName</span><span class="sxs-lookup"><span data-stu-id="82122-429">preferredName</span></span>|<span data-ttu-id="82122-430">String</span><span class="sxs-lookup"><span data-stu-id="82122-430">String</span></span>|<span data-ttu-id="82122-431">用户的首选名称。</span><span class="sxs-lookup"><span data-stu-id="82122-431">The preferred name for the user.</span></span>|
|<span data-ttu-id="82122-432">provisionedPlans</span><span class="sxs-lookup"><span data-stu-id="82122-432">provisionedPlans</span></span>|<span data-ttu-id="82122-433">[ProvisionedPlan](provisionedplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="82122-433">[ProvisionedPlan](provisionedplan.md) collection</span></span>|<span data-ttu-id="82122-p142">为用户设置的计划。只读。不可为 null。</span><span class="sxs-lookup"><span data-stu-id="82122-p142">The plans that are provisioned for the user. Read-only. Not nullable.</span></span> |
|<span data-ttu-id="82122-437">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="82122-437">proxyAddresses</span></span>|<span data-ttu-id="82122-438">String collection</span><span class="sxs-lookup"><span data-stu-id="82122-438">String collection</span></span>|<span data-ttu-id="82122-p143">例如：`["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` 需要多值属性筛选器表达式的 **any** 运算符。只读，不可为 Null。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="82122-p143">For example: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` The **any** operator is required for filter expressions on multi-valued properties. Read-only, Not nullable. Supports $filter.</span></span>          |
|<span data-ttu-id="82122-442">responsibilities</span><span class="sxs-lookup"><span data-stu-id="82122-442">responsibilities</span></span>|<span data-ttu-id="82122-443">String collection</span><span class="sxs-lookup"><span data-stu-id="82122-443">String collection</span></span>|<span data-ttu-id="82122-444">供用户枚举其职责的列表。</span><span class="sxs-lookup"><span data-stu-id="82122-444">A list for the user to enumerate their responsibilities.</span></span>|
|<span data-ttu-id="82122-445">schools</span><span class="sxs-lookup"><span data-stu-id="82122-445">schools</span></span>|<span data-ttu-id="82122-446">String collection</span><span class="sxs-lookup"><span data-stu-id="82122-446">String collection</span></span>|<span data-ttu-id="82122-447">供用户枚举其学习过的学校列表。</span><span class="sxs-lookup"><span data-stu-id="82122-447">A list for the user to enumerate the schools they have attended.</span></span>|
|<span data-ttu-id="82122-448">skills</span><span class="sxs-lookup"><span data-stu-id="82122-448">skills</span></span>|<span data-ttu-id="82122-449">String collection</span><span class="sxs-lookup"><span data-stu-id="82122-449">String collection</span></span>|<span data-ttu-id="82122-450">供用户枚举其技能的列表。</span><span class="sxs-lookup"><span data-stu-id="82122-450">A list for the user to enumerate their skills.</span></span>|
|<span data-ttu-id="82122-451">state</span><span class="sxs-lookup"><span data-stu-id="82122-451">state</span></span>|<span data-ttu-id="82122-452">字符串</span><span class="sxs-lookup"><span data-stu-id="82122-452">String</span></span>|<span data-ttu-id="82122-p144">用户地址中的省/市/自治区或省。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="82122-p144">The state or province in the user's address. Supports $filter.</span></span>|
|<span data-ttu-id="82122-455">streetAddress</span><span class="sxs-lookup"><span data-stu-id="82122-455">streetAddress</span></span>|<span data-ttu-id="82122-456">String</span><span class="sxs-lookup"><span data-stu-id="82122-456">String</span></span>|<span data-ttu-id="82122-457">用户公司地点的街道地址。</span><span class="sxs-lookup"><span data-stu-id="82122-457">The street address of the user's place of business.</span></span>|
|<span data-ttu-id="82122-458">surname</span><span class="sxs-lookup"><span data-stu-id="82122-458">surname</span></span>|<span data-ttu-id="82122-459">字符串</span><span class="sxs-lookup"><span data-stu-id="82122-459">String</span></span>|<span data-ttu-id="82122-p145">用户的姓氏。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="82122-p145">The user's surname (family name or last name). Supports $filter.</span></span>|
|<span data-ttu-id="82122-462">usageLocation</span><span class="sxs-lookup"><span data-stu-id="82122-462">usageLocation</span></span>|<span data-ttu-id="82122-463">字符串</span><span class="sxs-lookup"><span data-stu-id="82122-463">String</span></span>|<span data-ttu-id="82122-p146">两个字母的国家/地区代码（ISO 标准 3166）。为检查服务在国家/地区的可用性，这对根据法律要求将分配许可证的用户而言是必需的。示例包括：“US”、“JP”和“GB”。不可为 null。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="82122-p146">A two letter country code (ISO standard 3166). Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries.  Examples include: "US", "JP", and "GB". Not nullable. Supports $filter.</span></span>|
|<span data-ttu-id="82122-469">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="82122-469">userPrincipalName</span></span>|<span data-ttu-id="82122-470">String</span><span class="sxs-lookup"><span data-stu-id="82122-470">String</span></span>|<span data-ttu-id="82122-p147">用户的用户主体名称 (UPN)。UPN 是用户基于 Internet 标准 RFC 822 的 Internet 式登录名。按照惯例，此名称应映射到用户的电子邮件名称。常规格式是 alias@domain，其中，domain 必须位于租户的已验证域集合中。创建用户时此属性是必需的。可从 [组织](organization.md) 的 **verifiedDomains** 属性访问租户的已验证域。支持 $filter 和 $orderby。</span><span class="sxs-lookup"><span data-stu-id="82122-p147">The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains. This property is required when a user is created. The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](organization.md). Supports $filter and $orderby.</span></span>
|<span data-ttu-id="82122-478">userType</span><span class="sxs-lookup"><span data-stu-id="82122-478">userType</span></span>|<span data-ttu-id="82122-479">字符串</span><span class="sxs-lookup"><span data-stu-id="82122-479">String</span></span>|<span data-ttu-id="82122-p148">可用于对目录中的用户类型分类的字符串值，例如“成员”和“访客”。支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="82122-p148">A string value that can be used to classify user types in your directory, such as “Member” and “Guest”. Supports $filter.</span></span>          |

### <a name="legal-age-group-property-definitions"></a><span data-ttu-id="82122-482">法律期限组属性定义</span><span class="sxs-lookup"><span data-stu-id="82122-482">Legal age group property definitions</span></span>

<span data-ttu-id="82122-483">本节介绍如何三个 age 组属性 (`legalAgeGroupClassification`，`ageGroup`和`consentProvidedForMinor`) 的 Azure AD 管理员和企业应用程序开发人员用于满足期限相关法规。</span><span class="sxs-lookup"><span data-stu-id="82122-483">This section explains how the three age group properties (`legalAgeGroupClassification`, `ageGroup` and `consentProvidedForMinor`) are used by Azure AD administrators and enterprise application developers to meet age-related regulations.</span></span>

<span data-ttu-id="82122-484">例如： Cameron 是管理员在英国 Holyport 小学的目录。</span><span class="sxs-lookup"><span data-stu-id="82122-484">For example: Cameron is administrator of a directory for an elementary school in Holyport in the United Kingdom.</span></span> <span data-ttu-id="82122-485">学校本年度开头他使用许可书面工作征得次要的父级基于 United Kingdom 的年龄相关法规。</span><span class="sxs-lookup"><span data-stu-id="82122-485">At the beginning of the school year he uses the admissions paperwork to obtain consent from the minor's parents based on the age-related regulations of the United Kingdom.</span></span> <span data-ttu-id="82122-486">从父获得许可允许 Holyport 学校和 Microsoft 应用程序使用次要的帐户。</span><span class="sxs-lookup"><span data-stu-id="82122-486">The consent obtained from the parent allows the minor's account to be used by Holyport school and Microsoft apps.</span></span> <span data-ttu-id="82122-487">Cameron 然后创建所有帐户，并设置为"次要"ageGroup 和 consentProvidedForMinor 到"授予"。</span><span class="sxs-lookup"><span data-stu-id="82122-487">Cameron then creates all the accounts and sets ageGroup to "minor" and consentProvidedForMinor to "granted".</span></span> <span data-ttu-id="82122-488">使用学生的应用程序就可以禁止不合适进行评级的功能。</span><span class="sxs-lookup"><span data-stu-id="82122-488">Applications used by his students are then able to suppress features that are not suitable for minors.</span></span>

#### <a name="legal-age-group-classification"></a><span data-ttu-id="82122-489">法律期限组分类</span><span class="sxs-lookup"><span data-stu-id="82122-489">Legal age group classification</span></span>

<span data-ttu-id="82122-490">企业应用程序开发人员使用此只读属性以确保正确处理根据其法律年龄组的用户。</span><span class="sxs-lookup"><span data-stu-id="82122-490">This read-only property is used by enterprise application developers to ensure the correct handling of a user based on their legal age group.</span></span> <span data-ttu-id="82122-491">计算基于用户的`ageGroup`和`consentProvidedForMinor`属性。</span><span class="sxs-lookup"><span data-stu-id="82122-491">It is calculated based on the user's `ageGroup` and `consentProvidedForMinor` properties.</span></span>

| <span data-ttu-id="82122-492">值</span><span class="sxs-lookup"><span data-stu-id="82122-492">Value</span></span>    | #  |<span data-ttu-id="82122-493">说明</span><span class="sxs-lookup"><span data-stu-id="82122-493">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="82122-494">null</span><span class="sxs-lookup"><span data-stu-id="82122-494">null</span></span>|<span data-ttu-id="82122-495">0</span><span class="sxs-lookup"><span data-stu-id="82122-495">0</span></span>|<span data-ttu-id="82122-496">默认值，不`ageGroup`已经为用户设置。</span><span class="sxs-lookup"><span data-stu-id="82122-496">Default value, no `ageGroup` has been set for the user.</span></span>|
|<span data-ttu-id="82122-497">minorWithoutParentalConsent</span><span class="sxs-lookup"><span data-stu-id="82122-497">minorWithoutParentalConsent</span></span> |<span data-ttu-id="82122-498">1</span><span class="sxs-lookup"><span data-stu-id="82122-498">1</span></span>|<span data-ttu-id="82122-499">（留作将来使用）</span><span class="sxs-lookup"><span data-stu-id="82122-499">(Reserved for future use)</span></span>|
|<span data-ttu-id="82122-500">minorWithParentalConsent</span><span class="sxs-lookup"><span data-stu-id="82122-500">minorWithParentalConsent</span></span>|<span data-ttu-id="82122-501">2</span><span class="sxs-lookup"><span data-stu-id="82122-501">2</span></span>| <span data-ttu-id="82122-502">用户被视为基于其所在国家/地区的年龄相关规章次要或区域和管理员的帐户已从父或监护人获取适当许可。</span><span class="sxs-lookup"><span data-stu-id="82122-502">The user is considered a minor based on the age-related regulations of their country or region and the administrator of the account has obtained appropriate consent from a parent or guardian.</span></span>|
|<span data-ttu-id="82122-503">成人</span><span class="sxs-lookup"><span data-stu-id="82122-503">adult</span></span>|<span data-ttu-id="82122-504">3</span><span class="sxs-lookup"><span data-stu-id="82122-504">3</span></span>|<span data-ttu-id="82122-505">用户视为成人基于其国家或地区的年龄相关法规。</span><span class="sxs-lookup"><span data-stu-id="82122-505">The user considered an adult based on the age-related regulations of their country or region.</span></span>|
|<span data-ttu-id="82122-506">notAdult</span><span class="sxs-lookup"><span data-stu-id="82122-506">notAdult</span></span>|<span data-ttu-id="82122-507">4</span><span class="sxs-lookup"><span data-stu-id="82122-507">4</span></span>|<span data-ttu-id="82122-508">是用户距离的国家或地区具有其他期限相关法规 （如美国、 英国、 欧盟或韩国），并且用户的年龄之间次要和成人期限 （作为规定根据的国家或地区）。</span><span class="sxs-lookup"><span data-stu-id="82122-508">The user is from a country or region that has additional age-related regulations (such as the United States, United Kingdom, European Union or South Korea), and the user's age is between a minor and an adult age (as stipulated based on country or region).</span></span> <span data-ttu-id="82122-509">通常，这意味着青少年都会被视为`notAdult`监管国家/地区。</span><span class="sxs-lookup"><span data-stu-id="82122-509">Generally, this means that teenagers are considered as `notAdult` in regulated countries.</span></span>|
|<span data-ttu-id="82122-510">minorNoParentalConsentRequired</span><span class="sxs-lookup"><span data-stu-id="82122-510">minorNoParentalConsentRequired</span></span>|<span data-ttu-id="82122-511">5</span><span class="sxs-lookup"><span data-stu-id="82122-511">5</span></span>|<span data-ttu-id="82122-512">用户是次要，但从的国家或地区已没有与时间有关的法规。</span><span class="sxs-lookup"><span data-stu-id="82122-512">The user is a minor but is from a country or region that has no age-related regulations.</span></span>|

#### <a name="age-group-and-minor-consent"></a><span data-ttu-id="82122-513">年龄组和次要同意</span><span class="sxs-lookup"><span data-stu-id="82122-513">Age group and minor consent</span></span>

<span data-ttu-id="82122-514">年龄组和次要同意属性是 Azure AD 管理员用来帮助确保正确基于调控用户的国家或地区的年龄相关的管理法规规则处理帐户使用的可选属性。</span><span class="sxs-lookup"><span data-stu-id="82122-514">The age group and minor consent properties are optional properties used by Azure AD administrators to help ensure the use of an account is handled correctly based on the age-related regulatory rules governing the user's country or region.</span></span>

#### <a name="agegroup-property"></a><span data-ttu-id="82122-515">ageGroup 属性</span><span class="sxs-lookup"><span data-stu-id="82122-515">ageGroup property</span></span>

| <span data-ttu-id="82122-516">值</span><span class="sxs-lookup"><span data-stu-id="82122-516">Value</span></span>    | #  |<span data-ttu-id="82122-517">说明</span><span class="sxs-lookup"><span data-stu-id="82122-517">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="82122-518">null</span><span class="sxs-lookup"><span data-stu-id="82122-518">null</span></span>|<span data-ttu-id="82122-519">0</span><span class="sxs-lookup"><span data-stu-id="82122-519">0</span></span>|<span data-ttu-id="82122-520">默认值，不`ageGroup`已经为用户设置。</span><span class="sxs-lookup"><span data-stu-id="82122-520">Default value, no `ageGroup` has been set for the user.</span></span>|
|<span data-ttu-id="82122-521">次要</span><span class="sxs-lookup"><span data-stu-id="82122-521">minor</span></span>|<span data-ttu-id="82122-522">1</span><span class="sxs-lookup"><span data-stu-id="82122-522">1</span></span>|<span data-ttu-id="82122-523">用户是考虑次要。</span><span class="sxs-lookup"><span data-stu-id="82122-523">The user is consider a minor.</span></span>|
|<span data-ttu-id="82122-524">notAdult</span><span class="sxs-lookup"><span data-stu-id="82122-524">notAdult</span></span>|<span data-ttu-id="82122-525">2</span><span class="sxs-lookup"><span data-stu-id="82122-525">2</span></span>|<span data-ttu-id="82122-526">用户是从具有法定法规美国、 英国、 欧盟或韩国的国家/地区） 并且用户的年龄孩子期限 （根据国家/地区） 的上限超过和成人年龄小于下限 （作为规定根据的国家或地区）.</span><span class="sxs-lookup"><span data-stu-id="82122-526">The user is from a country that has statutory regulations  United States, United Kingdom, European Union or South Korea) and user’s age is more than the upper limit of kid age (as per country) and less than lower limit of adult age (as stipulated based on country or region).</span></span> <span data-ttu-id="82122-527">基本上，因此视为青少年`notAdult`监管国家/地区。</span><span class="sxs-lookup"><span data-stu-id="82122-527">So basically, teenagers are considered as `notAdult` in regulated countries.</span></span>|
|<span data-ttu-id="82122-528">成人</span><span class="sxs-lookup"><span data-stu-id="82122-528">adult</span></span>|<span data-ttu-id="82122-529">3</span><span class="sxs-lookup"><span data-stu-id="82122-529">3</span></span>|<span data-ttu-id="82122-530">用户应该为成人内容处理。</span><span class="sxs-lookup"><span data-stu-id="82122-530">The user should be a treated as an adult.</span></span>|

#### <a name="consentprovidedforminor-property"></a><span data-ttu-id="82122-531">consentProvidedForMinor 属性</span><span class="sxs-lookup"><span data-stu-id="82122-531">consentProvidedForMinor property</span></span>

| <span data-ttu-id="82122-532">值</span><span class="sxs-lookup"><span data-stu-id="82122-532">Value</span></span>    | #  |<span data-ttu-id="82122-533">说明</span><span class="sxs-lookup"><span data-stu-id="82122-533">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="82122-534">null</span><span class="sxs-lookup"><span data-stu-id="82122-534">null</span></span>|<span data-ttu-id="82122-535">0</span><span class="sxs-lookup"><span data-stu-id="82122-535">0</span></span>|<span data-ttu-id="82122-536">默认值，不`consentProvidedForMinor`已经为用户设置。</span><span class="sxs-lookup"><span data-stu-id="82122-536">Default value, no `consentProvidedForMinor` has been set for the user.</span></span>|
|<span data-ttu-id="82122-537">授予</span><span class="sxs-lookup"><span data-stu-id="82122-537">granted</span></span>|<span data-ttu-id="82122-538">1</span><span class="sxs-lookup"><span data-stu-id="82122-538">1</span></span>|<span data-ttu-id="82122-539">已为用户都具有帐户获得许可。</span><span class="sxs-lookup"><span data-stu-id="82122-539">Consent has been obtained for the user to have an account.</span></span>|
|<span data-ttu-id="82122-540">denied</span><span class="sxs-lookup"><span data-stu-id="82122-540">denied</span></span>|<span data-ttu-id="82122-541">2</span><span class="sxs-lookup"><span data-stu-id="82122-541">2</span></span>|<span data-ttu-id="82122-542">用户具有帐户未获得许可。</span><span class="sxs-lookup"><span data-stu-id="82122-542">Consent has not been obtained for the user to have an account.</span></span>|
|<span data-ttu-id="82122-543">notRequired</span><span class="sxs-lookup"><span data-stu-id="82122-543">notRequired</span></span>|<span data-ttu-id="82122-544">3</span><span class="sxs-lookup"><span data-stu-id="82122-544">3</span></span>|<span data-ttu-id="82122-545">用户从不需要同意位置。</span><span class="sxs-lookup"><span data-stu-id="82122-545">The user is from a location that does not require consent.</span></span>|
 
## <a name="relationships"></a><span data-ttu-id="82122-546">Relationships</span><span class="sxs-lookup"><span data-stu-id="82122-546">Relationships</span></span>

| <span data-ttu-id="82122-547">关系</span><span class="sxs-lookup"><span data-stu-id="82122-547">Relationship</span></span> | <span data-ttu-id="82122-548">类型</span><span class="sxs-lookup"><span data-stu-id="82122-548">Type</span></span>   |<span data-ttu-id="82122-549">说明</span><span class="sxs-lookup"><span data-stu-id="82122-549">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="82122-550">activities</span><span class="sxs-lookup"><span data-stu-id="82122-550">activities</span></span>|<span data-ttu-id="82122-551">[userActivity](projectrome-activity.md)集合</span><span class="sxs-lookup"><span data-stu-id="82122-551">[userActivity](projectrome-activity.md) collection</span></span>|<span data-ttu-id="82122-552">跨设备的用户的活动。</span><span class="sxs-lookup"><span data-stu-id="82122-552">The user's activities across devices.</span></span> <span data-ttu-id="82122-553">只读。</span><span class="sxs-lookup"><span data-stu-id="82122-553">Read-only.</span></span> <span data-ttu-id="82122-554">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="82122-554">Nullable.</span></span>|
|<span data-ttu-id="82122-555">calendar</span><span class="sxs-lookup"><span data-stu-id="82122-555">calendar</span></span>|[<span data-ttu-id="82122-556">Calendar</span><span class="sxs-lookup"><span data-stu-id="82122-556">Calendar</span></span>](calendar.md)|<span data-ttu-id="82122-p154">用户的主日历。只读。</span><span class="sxs-lookup"><span data-stu-id="82122-p154">The user's primary calendar. Read-only.</span></span>|
|<span data-ttu-id="82122-559">calendarGroups</span><span class="sxs-lookup"><span data-stu-id="82122-559">calendarGroups</span></span>|<span data-ttu-id="82122-560">[CalendarGroup](calendargroup.md) collection</span><span class="sxs-lookup"><span data-stu-id="82122-560">[CalendarGroup](calendargroup.md) collection</span></span>|<span data-ttu-id="82122-p155">用户的日历组。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="82122-p155">The user's calendar groups. Read-only. Nullable.</span></span>|
|<span data-ttu-id="82122-564">calendarView</span><span class="sxs-lookup"><span data-stu-id="82122-564">calendarView</span></span>|<span data-ttu-id="82122-565">[Event](event.md) collection</span><span class="sxs-lookup"><span data-stu-id="82122-565">[Event](event.md) collection</span></span>|<span data-ttu-id="82122-p156">日历的日历视图。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="82122-p156">The calendar view for the calendar. Read-only. Nullable.</span></span>|
|<span data-ttu-id="82122-569">calendars</span><span class="sxs-lookup"><span data-stu-id="82122-569">calendars</span></span>|<span data-ttu-id="82122-570">[日历](calendar.md) 集合</span><span class="sxs-lookup"><span data-stu-id="82122-570">[Calendar](calendar.md) collection</span></span>|<span data-ttu-id="82122-p157">用户的日历。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="82122-p157">The user's calendars. Read-only. Nullable.</span></span>|
|<span data-ttu-id="82122-574">contactFolders</span><span class="sxs-lookup"><span data-stu-id="82122-574">contactFolders</span></span>|<span data-ttu-id="82122-575">[ContactFolder](contactfolder.md) collection</span><span class="sxs-lookup"><span data-stu-id="82122-575">[ContactFolder](contactfolder.md) collection</span></span>|<span data-ttu-id="82122-p158">用户的联系人文件夹。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="82122-p158">The user's contacts folders. Read-only. Nullable.</span></span>|
|<span data-ttu-id="82122-579">contacts</span><span class="sxs-lookup"><span data-stu-id="82122-579">contacts</span></span>|<span data-ttu-id="82122-580">[Contact](contact.md) collection</span><span class="sxs-lookup"><span data-stu-id="82122-580">[Contact](contact.md) collection</span></span>|<span data-ttu-id="82122-p159">用户的联系人。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="82122-p159">The user's contacts. Read-only. Nullable.</span></span>|
|<span data-ttu-id="82122-584">createdObjects</span><span class="sxs-lookup"><span data-stu-id="82122-584">createdObjects</span></span>|<span data-ttu-id="82122-585">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="82122-585">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="82122-p160">由用户创建的 directory 对象。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="82122-p160">Directory objects that were created by the user. Read-only. Nullable.</span></span>|
|<span data-ttu-id="82122-589">directReports</span><span class="sxs-lookup"><span data-stu-id="82122-589">directReports</span></span>|<span data-ttu-id="82122-590">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="82122-590">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="82122-p161">向此用户报告的用户和联系人。（其 manager 属性已设置为此用户的用户和联系人。）只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="82122-p161">The users and contacts that report to the user. (The users and contacts that have their manager property set to this user.) Read-only. Nullable.</span></span> |
|<span data-ttu-id="82122-594">drive</span><span class="sxs-lookup"><span data-stu-id="82122-594">drive</span></span>|[<span data-ttu-id="82122-595">驱动器</span><span class="sxs-lookup"><span data-stu-id="82122-595">drive</span></span>](drive.md)|<span data-ttu-id="82122-p162">用户的 OneDrive。只读。</span><span class="sxs-lookup"><span data-stu-id="82122-p162">The user's OneDrive. Read-only.</span></span>|
|<span data-ttu-id="82122-598">驱动器</span><span class="sxs-lookup"><span data-stu-id="82122-598">drives</span></span>|<span data-ttu-id="82122-599">[驱动器](drive.md) 集合</span><span class="sxs-lookup"><span data-stu-id="82122-599">[drive](drive.md) collection</span></span>| <span data-ttu-id="82122-p163">该用户的可用驱动器集合。只读。</span><span class="sxs-lookup"><span data-stu-id="82122-p163">A collection of drives available for this user. Read-only.</span></span> |
|<span data-ttu-id="82122-602">events</span><span class="sxs-lookup"><span data-stu-id="82122-602">events</span></span>|<span data-ttu-id="82122-603">[Event](event.md) collection</span><span class="sxs-lookup"><span data-stu-id="82122-603">[Event](event.md) collection</span></span>|<span data-ttu-id="82122-p164">用户的事件。默认显示“默认日历”下的事件。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="82122-p164">The user's events. Default is to show Events under the Default Calendar. Read-only. Nullable.</span></span>|
|<span data-ttu-id="82122-608">extensions</span><span class="sxs-lookup"><span data-stu-id="82122-608">extensions</span></span>|<span data-ttu-id="82122-609">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="82122-609">[extension](extension.md) collection</span></span>|<span data-ttu-id="82122-p165">为用户定义的开放扩展集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="82122-p165">The collection of open extensions defined for the user. Read-only. Nullable.</span></span>|
|<span data-ttu-id="82122-613">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="82122-613">inferenceClassification</span></span> | [<span data-ttu-id="82122-614">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="82122-614">inferenceClassification</span></span>](inferenceclassification.md) | <span data-ttu-id="82122-615">基于显式指定的用户邮件的相关性分类，可以替代推断的相关性或重要性。</span><span class="sxs-lookup"><span data-stu-id="82122-615">Relevance classification of the user's messages based on explicit designations which override inferred relevance or importance.</span></span> |
|<span data-ttu-id="82122-616">licenseDetails</span><span class="sxs-lookup"><span data-stu-id="82122-616">licenseDetails</span></span>|<span data-ttu-id="82122-617">[LicenseDetails](licensedetails.md)集合</span><span class="sxs-lookup"><span data-stu-id="82122-617">[LicenseDetails](licensedetails.md) collection</span></span>|<span data-ttu-id="82122-618">此用户的许可证详细信息的集合。</span><span class="sxs-lookup"><span data-stu-id="82122-618">A collection of this user's license details.</span></span> <span data-ttu-id="82122-619">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="82122-619">Nullable.</span></span>|
|<span data-ttu-id="82122-620">mailFolders</span><span class="sxs-lookup"><span data-stu-id="82122-620">mailFolders</span></span>|<span data-ttu-id="82122-621">[MailFolder](mailfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="82122-621">[MailFolder](mailfolder.md) collection</span></span>| <span data-ttu-id="82122-p167">用户的邮件文件夹。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="82122-p167">The user's mail folders. Read-only. Nullable.</span></span>|
|<span data-ttu-id="82122-625">manager</span><span class="sxs-lookup"><span data-stu-id="82122-625">manager</span></span>|[<span data-ttu-id="82122-626">directoryObject</span><span class="sxs-lookup"><span data-stu-id="82122-626">directoryObject</span></span>](directoryobject.md)|<span data-ttu-id="82122-p168">是此用户的经理的用户或联系人。只读。（HTTP 方法：GET、PUT、DELETE）</span><span class="sxs-lookup"><span data-stu-id="82122-p168">The user or contact that is this user’s manager. Read-only. (HTTP Methods: GET, PUT, DELETE.)</span></span>|
|<span data-ttu-id="82122-630">memberOf</span><span class="sxs-lookup"><span data-stu-id="82122-630">memberOf</span></span>|<span data-ttu-id="82122-631">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="82122-631">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="82122-p169">用户所属的组和目录角色。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="82122-p169">The groups and directory roles that the user is a member of. Read-only. Nullable.</span></span>|
|<span data-ttu-id="82122-635">messages</span><span class="sxs-lookup"><span data-stu-id="82122-635">messages</span></span>|<span data-ttu-id="82122-636">[邮件](message.md) 集合</span><span class="sxs-lookup"><span data-stu-id="82122-636">[Message](message.md) collection</span></span>|<span data-ttu-id="82122-p170">邮箱或文件夹中的邮件。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="82122-p170">The messages in a mailbox or folder. Read-only. Nullable.</span></span>|
|<span data-ttu-id="82122-640">onenote</span><span class="sxs-lookup"><span data-stu-id="82122-640">onenote</span></span>|[<span data-ttu-id="82122-641">Onenote</span><span class="sxs-lookup"><span data-stu-id="82122-641">Onenote</span></span>](onenote.md)| <span data-ttu-id="82122-642">只读。</span><span class="sxs-lookup"><span data-stu-id="82122-642">Read-only.</span></span>|
|<span data-ttu-id="82122-643">outlook</span><span class="sxs-lookup"><span data-stu-id="82122-643">outlook</span></span>|[<span data-ttu-id="82122-644">OutlookUser</span><span class="sxs-lookup"><span data-stu-id="82122-644">OutlookUser</span></span>](outlookuser.md)| <span data-ttu-id="82122-645">只读。</span><span class="sxs-lookup"><span data-stu-id="82122-645">Read-only.</span></span>|
|<span data-ttu-id="82122-646">ownedDevices</span><span class="sxs-lookup"><span data-stu-id="82122-646">ownedDevices</span></span>|<span data-ttu-id="82122-647">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="82122-647">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="82122-p171">用户拥有的设备。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="82122-p171">Devices that are owned by the user. Read-only. Nullable.</span></span>|
|<span data-ttu-id="82122-651">ownedObjects</span><span class="sxs-lookup"><span data-stu-id="82122-651">ownedObjects</span></span>|<span data-ttu-id="82122-652">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="82122-652">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="82122-p172">用户拥有的 directory 对象。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="82122-p172">Directory objects that are owned by the user. Read-only. Nullable.</span></span>|
|<span data-ttu-id="82122-656">人脉</span><span class="sxs-lookup"><span data-stu-id="82122-656">people</span></span>|<span data-ttu-id="82122-657">[人员](person.md)集合</span><span class="sxs-lookup"><span data-stu-id="82122-657">[person](person.md) collection</span></span>| <span data-ttu-id="82122-658">与用户相关的人员。</span><span class="sxs-lookup"><span data-stu-id="82122-658">People that are relevant to the user.</span></span> <span data-ttu-id="82122-659">只读。</span><span class="sxs-lookup"><span data-stu-id="82122-659">Read-only.</span></span> <span data-ttu-id="82122-660">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="82122-660">Nullable.</span></span>
|<span data-ttu-id="82122-661">photo</span><span class="sxs-lookup"><span data-stu-id="82122-661">photo</span></span>|[<span data-ttu-id="82122-662">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="82122-662">profilePhoto</span></span>](profilephoto.md)| <span data-ttu-id="82122-p174">用户的个人资料照片。只读。</span><span class="sxs-lookup"><span data-stu-id="82122-p174">The user's profile photo. Read-only.</span></span>|
|<span data-ttu-id="82122-665">planner</span><span class="sxs-lookup"><span data-stu-id="82122-665">planner</span></span>|[<span data-ttu-id="82122-666">plannerUser</span><span class="sxs-lookup"><span data-stu-id="82122-666">plannerUser</span></span>](planneruser.md)| <span data-ttu-id="82122-667">计划工具资源可能存在的用户的入口点。</span><span class="sxs-lookup"><span data-stu-id="82122-667">Entry-point to the Planner resource that might exist for a user.</span></span> <span data-ttu-id="82122-668">只读。</span><span class="sxs-lookup"><span data-stu-id="82122-668">Read-only.</span></span>|
|<span data-ttu-id="82122-669">registeredDevices</span><span class="sxs-lookup"><span data-stu-id="82122-669">registeredDevices</span></span>|<span data-ttu-id="82122-670">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="82122-670">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="82122-p176">已注册的用户的设备。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="82122-p176">Devices that are registered for the user. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="82122-674">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="82122-674">JSON representation</span></span>

<span data-ttu-id="82122-675">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="82122-675">Here is a JSON representation of the resource</span></span>

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
  "onPremisesDomainName": "string",
  "onPremisesExtensionAttributes": {"@odata.type": "microsoft.graph.onPremisesExtensionAttributes"},
  "onPremisesImmutableId": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSamAccountName": "string",
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "onPremisesUserPrincipalName": "string",
  "passwordPolicies": "string",
  "passwordProfile": {"@odata.type": "microsoft.graph.passwordProfile"},
  "pastProjects": ["string"],
  "postalCode": "string",
  "preferredDataLocation": "string",
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

## <a name="see-also"></a><span data-ttu-id="82122-676">另请参阅</span><span class="sxs-lookup"><span data-stu-id="82122-676">See also</span></span>

- [<span data-ttu-id="82122-677">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="82122-677">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="82122-678">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="82122-678">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="82122-679">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="82122-679">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user resource",
  "keywords": "",
  "suppressions" : [
     "Warning: /api-reference/v1.0/resources/user.md/microsoft.graph.user:
      Property 'createdDateTime' found in markdown table but not in resource definition."
  ],
  "section": "documentation",
  "tocPath": ""
}-->
