---
title: 日历资源类型
description: 日历即事件容器。 它可以是用户的日历，也可以是 Microsoft 365 组的默认日历。
localization_priority: Priority
author: harini84
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 47a63319efea2bdcdf11728bbac7d17903c6590a
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895704"
---
# <a name="calendar-resource-type"></a><span data-ttu-id="75366-104">日历资源类型</span><span class="sxs-lookup"><span data-stu-id="75366-104">calendar resource type</span></span>

<span data-ttu-id="75366-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75366-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="75366-106">日历即事件容器。</span><span class="sxs-lookup"><span data-stu-id="75366-106">A calendar which is a container for events.</span></span> <span data-ttu-id="75366-107">它可以是[用户](user.md)的日历，也可以是 Microsoft 365[组](group.md)的默认日历。</span><span class="sxs-lookup"><span data-stu-id="75366-107">It can be a calendar for a [user](user.md), or the default calendar of a Microsoft 365 [group](group.md).</span></span>

> <span data-ttu-id="75366-108">**注意：** 与用户日历和组日历交互的方式稍有不同：</span><span class="sxs-lookup"><span data-stu-id="75366-108">**Note:** There are a few minor differences in the way you can interact with user calendars and group calendars:</span></span>

- <span data-ttu-id="75366-109">只能将用户日历组织到 [calendarGroup](calendargroup.md) 中。</span><span class="sxs-lookup"><span data-stu-id="75366-109">You can organize only user calendars in a [calendarGroup](calendargroup.md).</span></span>
- <span data-ttu-id="75366-110">Outlook 将代表组自动接受所有会议请求。</span><span class="sxs-lookup"><span data-stu-id="75366-110">Outlook automatically accepts all meeting requests on behalf of groups.</span></span> <span data-ttu-id="75366-111">只能[接受](../api/event-accept.md)、[暂时接受](../api/event-tentativelyaccept.md)或[拒绝](../api/event-decline.md)用户日历中的会议请求。</span><span class="sxs-lookup"><span data-stu-id="75366-111">You can [accept](../api/event-accept.md), [tentatively accept](../api/event-tentativelyaccept.md), or [decline](../api/event-decline.md)  meeting requests for user calendars only.</span></span>
- <span data-ttu-id="75366-112">Outlook 不支持对组事件提供提醒。</span><span class="sxs-lookup"><span data-stu-id="75366-112">Outlook doesn't support reminders for group events.</span></span> <span data-ttu-id="75366-113">只能[推迟](../api/event-snoozereminder.md)或[取消](../api/event-dismissreminder.md)用户日历的[提醒](reminder.md)。</span><span class="sxs-lookup"><span data-stu-id="75366-113">You can [snooze](../api/event-snoozereminder.md) or [dismiss](../api/event-dismissreminder.md) a [reminder](reminder.md) for user calendars only.</span></span>

## <a name="methods"></a><span data-ttu-id="75366-114">方法</span><span class="sxs-lookup"><span data-stu-id="75366-114">Methods</span></span>

| <span data-ttu-id="75366-115">方法</span><span class="sxs-lookup"><span data-stu-id="75366-115">Method</span></span>       | <span data-ttu-id="75366-116">返回类型</span><span class="sxs-lookup"><span data-stu-id="75366-116">Return Type</span></span>  |<span data-ttu-id="75366-117">说明</span><span class="sxs-lookup"><span data-stu-id="75366-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="75366-118">列出日历</span><span class="sxs-lookup"><span data-stu-id="75366-118">List calendars</span></span>](../api/user-list-calendars.md)|<span data-ttu-id="75366-119">[日历](calendar.md) 集合</span><span class="sxs-lookup"><span data-stu-id="75366-119">[calendar](calendar.md) collection</span></span>|<span data-ttu-id="75366-120">获取所有用户的日历，或者获取默认或其他特定日历组中的日历。</span><span class="sxs-lookup"><span data-stu-id="75366-120">Get all the user's calendars, or the calendars in the default or other specific calendar group.</span></span>|
|[<span data-ttu-id="75366-121">创建日历</span><span class="sxs-lookup"><span data-stu-id="75366-121">Create calendar</span></span>](../api/user-post-calendars.md) |[<span data-ttu-id="75366-122">calendar</span><span class="sxs-lookup"><span data-stu-id="75366-122">calendar</span></span>](calendar.md)| <span data-ttu-id="75366-123">在默认日历组或用户的指定日历组中新建日历。</span><span class="sxs-lookup"><span data-stu-id="75366-123">Create a new calendar in the default calendar group or specified calendar group for a user.</span></span>|
|[<span data-ttu-id="75366-124">Get calendar</span><span class="sxs-lookup"><span data-stu-id="75366-124">Get calendar</span></span>](../api/calendar-get.md) | [<span data-ttu-id="75366-125">calendar</span><span class="sxs-lookup"><span data-stu-id="75366-125">calendar</span></span>](calendar.md) |<span data-ttu-id="75366-126">获取 **calendar** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="75366-126">Get the properties and relationships of a **calendar** object.</span></span> <span data-ttu-id="75366-127">日历可以是用户的一个，也可以是 Microsoft 365 组的默认日历。</span><span class="sxs-lookup"><span data-stu-id="75366-127">The calendar can be one for a user, or the default calendar of a Microsoft 365 group.</span></span> |
|[<span data-ttu-id="75366-128">Update</span><span class="sxs-lookup"><span data-stu-id="75366-128">Update</span></span>](../api/calendar-update.md) | [<span data-ttu-id="75366-129">calendar</span><span class="sxs-lookup"><span data-stu-id="75366-129">calendar</span></span>](calendar.md)  |<span data-ttu-id="75366-130">更新 **calendar** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="75366-130">Update the properties of a **calendar** object.</span></span> <span data-ttu-id="75366-131">日历可以是用户的一个，也可以是 Microsoft 365 组的默认日历。</span><span class="sxs-lookup"><span data-stu-id="75366-131">The calendar can be one for a user, or the default calendar of a Microsoft 365 group.</span></span> |
|[<span data-ttu-id="75366-132">Delete</span><span class="sxs-lookup"><span data-stu-id="75366-132">Delete</span></span>](../api/calendar-delete.md) | <span data-ttu-id="75366-133">无</span><span class="sxs-lookup"><span data-stu-id="75366-133">None</span></span> |<span data-ttu-id="75366-134">删除 calendar 对象。</span><span class="sxs-lookup"><span data-stu-id="75366-134">Delete calendar object.</span></span> |
|[<span data-ttu-id="75366-135">列出 calendarView</span><span class="sxs-lookup"><span data-stu-id="75366-135">List calendarView</span></span>](../api/calendar-list-calendarview.md) |<span data-ttu-id="75366-136">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="75366-136">[event](event.md) collection</span></span>| <span data-ttu-id="75366-137">从用户的主日历 `(../me/calendarview)` 或指定日历中，获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例。</span><span class="sxs-lookup"><span data-stu-id="75366-137">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's primary calendar `(../me/calendarview)` or from a specified calendar.</span></span>|
|[<span data-ttu-id="75366-138">列出事件</span><span class="sxs-lookup"><span data-stu-id="75366-138">List events</span></span>](../api/calendar-list-events.md) |<span data-ttu-id="75366-139">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="75366-139">[event](event.md) collection</span></span>| <span data-ttu-id="75366-p107">检索日历中的事件列表。该列表包含单实例会议和系列主控事件。</span><span class="sxs-lookup"><span data-stu-id="75366-p107">Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters.</span></span>|
|[<span data-ttu-id="75366-142">创建事件</span><span class="sxs-lookup"><span data-stu-id="75366-142">Create event</span></span>](../api/calendar-post-events.md) |[<span data-ttu-id="75366-143">event</span><span class="sxs-lookup"><span data-stu-id="75366-143">event</span></span>](event.md)| <span data-ttu-id="75366-144">在默认或指定日历中创建新事件。</span><span class="sxs-lookup"><span data-stu-id="75366-144">Create a new event in the default or specified calendar.</span></span>|
|[<span data-ttu-id="75366-145">getSchedule</span><span class="sxs-lookup"><span data-stu-id="75366-145">getSchedule</span></span>](../api/calendar-getschedule.md) |<span data-ttu-id="75366-146">[scheduleInformation](scheduleinformation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="75366-146">[scheduleInformation](scheduleinformation.md) collection</span></span>|<span data-ttu-id="75366-147">获取用户、通讯组列表或资源在指定时间段内的忙/闲状态信息。</span><span class="sxs-lookup"><span data-stu-id="75366-147">Get the free/busy availability information for a collection of users, distributions lists, or resources, for a specified time period.</span></span> |
|[<span data-ttu-id="75366-148">findMeetingTimes</span><span class="sxs-lookup"><span data-stu-id="75366-148">findMeetingTimes</span></span>](../api/user-findmeetingtimes.md) |[<span data-ttu-id="75366-149">meetingTimeSuggestionsResult</span><span class="sxs-lookup"><span data-stu-id="75366-149">meetingTimeSuggestionsResult</span></span>](meetingtimesuggestionsresult.md) |<span data-ttu-id="75366-150">根据组织者和与会者忙/闲状态以及时间或地点约束，建议会议时间和地点。</span><span class="sxs-lookup"><span data-stu-id="75366-150">Suggest meeting times and locations based on organizer and attendee availability, and time or location constraints.</span></span> |
|[<span data-ttu-id="75366-151">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="75366-151">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="75366-152">日历</span><span class="sxs-lookup"><span data-stu-id="75366-152">calendar</span></span>](calendar.md)  |<span data-ttu-id="75366-153">在新建或现有日历中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="75366-153">Create one or more single-value extended properties in a new or existing calendar.</span></span>   |
|[<span data-ttu-id="75366-154">获取包含单值扩展属性的日历</span><span class="sxs-lookup"><span data-stu-id="75366-154">Get calendar with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="75366-155">日历</span><span class="sxs-lookup"><span data-stu-id="75366-155">calendar</span></span>](calendar.md) | <span data-ttu-id="75366-156">通过使用 `$expand` 或 `$filter` 获取包含一个单值扩展属性的日历。</span><span class="sxs-lookup"><span data-stu-id="75366-156">Get calendars that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="75366-157">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="75366-157">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="75366-158">日历</span><span class="sxs-lookup"><span data-stu-id="75366-158">calendar</span></span>](calendar.md) | <span data-ttu-id="75366-159">在新建或现有的日历中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="75366-159">Create one or more multi-value extended properties in a new or existing calendar.</span></span>  |
|[<span data-ttu-id="75366-160">获取包含多值扩展属性的日历</span><span class="sxs-lookup"><span data-stu-id="75366-160">Get calendar with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="75366-161">日历</span><span class="sxs-lookup"><span data-stu-id="75366-161">calendar</span></span>](calendar.md) | <span data-ttu-id="75366-162">使用 `$expand` 获取包含一个多值扩展属性的日历。</span><span class="sxs-lookup"><span data-stu-id="75366-162">Get a calendar that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="75366-163">属性</span><span class="sxs-lookup"><span data-stu-id="75366-163">Properties</span></span>
| <span data-ttu-id="75366-164">属性</span><span class="sxs-lookup"><span data-stu-id="75366-164">Property</span></span>     | <span data-ttu-id="75366-165">类型</span><span class="sxs-lookup"><span data-stu-id="75366-165">Type</span></span>   |<span data-ttu-id="75366-166">Description</span><span class="sxs-lookup"><span data-stu-id="75366-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75366-167">allowedOnlineMeetingProviders</span><span class="sxs-lookup"><span data-stu-id="75366-167">allowedOnlineMeetingProviders</span></span>|<span data-ttu-id="75366-168">string 集合</span><span class="sxs-lookup"><span data-stu-id="75366-168">string collection</span></span>| <span data-ttu-id="75366-169">表示此日历中可用于创建联机会议的联机会议服务提供商。</span><span class="sxs-lookup"><span data-stu-id="75366-169">Represent the online meeting service providers that can be used to create online meetings in this calendar.</span></span> <span data-ttu-id="75366-170">可取值为：`unknown`、`skypeForBusiness`、`skypeForConsumer`、`teamsForBusiness`。</span><span class="sxs-lookup"><span data-stu-id="75366-170">Possible values are: `unknown`, `skypeForBusiness`, `skypeForConsumer`, `teamsForBusiness`.</span></span>|
|<span data-ttu-id="75366-171">canEdit</span><span class="sxs-lookup"><span data-stu-id="75366-171">canEdit</span></span> |<span data-ttu-id="75366-172">布尔</span><span class="sxs-lookup"><span data-stu-id="75366-172">Boolean</span></span> |<span data-ttu-id="75366-p109">如果用户可以写入日历则为 true，否则为 false。对于创建此日历的用户，此属性为 true。此属性对于共享日历并且授予写入访问权限的用户同样为 true。</span><span class="sxs-lookup"><span data-stu-id="75366-p109">True if the user can write to the calendar, false otherwise. This property is true for the user who created the calendar. This property is also true for a user who has been shared a calendar and granted write access.</span></span> |
|<span data-ttu-id="75366-176">canShare</span><span class="sxs-lookup"><span data-stu-id="75366-176">canShare</span></span> |<span data-ttu-id="75366-177">布尔</span><span class="sxs-lookup"><span data-stu-id="75366-177">Boolean</span></span> |<span data-ttu-id="75366-p110">如果用户有权共享日历则为 ture，否则为 false。只有创建日历的用户才可以进行共享。</span><span class="sxs-lookup"><span data-stu-id="75366-p110">True if the user has the permission to share the calendar, false otherwise. Only the user who created the calendar can share it.</span></span> |
|<span data-ttu-id="75366-180">canViewPrivateItems</span><span class="sxs-lookup"><span data-stu-id="75366-180">canViewPrivateItems</span></span> |<span data-ttu-id="75366-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="75366-181">Boolean</span></span> |<span data-ttu-id="75366-182">如果用户可以读取已标记为私有的日历项，则为 true，否则返回 false。</span><span class="sxs-lookup"><span data-stu-id="75366-182">True if the user can read calendar items that have been marked private, false otherwise.</span></span> |
|<span data-ttu-id="75366-183">changeKey</span><span class="sxs-lookup"><span data-stu-id="75366-183">changeKey</span></span>|<span data-ttu-id="75366-184">字符串</span><span class="sxs-lookup"><span data-stu-id="75366-184">String</span></span>|<span data-ttu-id="75366-p111">标识 calendar 对象的版本。每次日历更改时，changeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。只读。</span><span class="sxs-lookup"><span data-stu-id="75366-p111">Identifies the version of the calendar object. Every time the calendar is changed, changeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span>|
|<span data-ttu-id="75366-189">颜色</span><span class="sxs-lookup"><span data-stu-id="75366-189">color</span></span>|<span data-ttu-id="75366-190">calendarColor</span><span class="sxs-lookup"><span data-stu-id="75366-190">calendarColor</span></span>|<span data-ttu-id="75366-p112">在 UI 中指定将该日历与其他日历区分开来的颜色主题。属性值有：LightBlue=0、LightGreen=1、LightOrange=2、LightGray=3、LightYellow=4、LightTeal=5、LightPink=6、LightBrown=7、LightRed=8、MaxColor=9、Auto=-1</span><span class="sxs-lookup"><span data-stu-id="75366-p112">Specifies the color theme to distinguish the calendar from other calendars in a UI. The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span></span>|
|<span data-ttu-id="75366-193">defaultOnlineMeetingProvider</span><span class="sxs-lookup"><span data-stu-id="75366-193">defaultOnlineMeetingProvider</span></span>|<span data-ttu-id="75366-194">onlineMeetingProviderType</span><span class="sxs-lookup"><span data-stu-id="75366-194">onlineMeetingProviderType</span></span>|<span data-ttu-id="75366-195">从此日历发送的会议的默认联机会议提供商。</span><span class="sxs-lookup"><span data-stu-id="75366-195">The default online meeting provider for meetings sent from this calendar.</span></span> <span data-ttu-id="75366-196">可取值为：`unknown`、`skypeForBusiness`、`skypeForConsumer`、`teamsForBusiness`。</span><span class="sxs-lookup"><span data-stu-id="75366-196">Possible values are: `unknown`, `skypeForBusiness`, `skypeForConsumer`, `teamsForBusiness`.</span></span>|
|<span data-ttu-id="75366-197">id</span><span class="sxs-lookup"><span data-stu-id="75366-197">id</span></span>|<span data-ttu-id="75366-198">String</span><span class="sxs-lookup"><span data-stu-id="75366-198">String</span></span>|<span data-ttu-id="75366-p114">日历的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="75366-p114">The calendar's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="75366-201">isRemovable</span><span class="sxs-lookup"><span data-stu-id="75366-201">isRemovable</span></span>|<span data-ttu-id="75366-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="75366-202">Boolean</span></span>| <span data-ttu-id="75366-203">表示是否可以从用户邮箱删除此用户日志。</span><span class="sxs-lookup"><span data-stu-id="75366-203">Indicates whether this user calendar can be deleted from the user mailbox.</span></span>|
|<span data-ttu-id="75366-204">isTallyingResponses</span><span class="sxs-lookup"><span data-stu-id="75366-204">isTallyingResponses</span></span>|<span data-ttu-id="75366-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="75366-205">Boolean</span></span>|<span data-ttu-id="75366-206">表示此用户日历是否支持会议响应跟踪。</span><span class="sxs-lookup"><span data-stu-id="75366-206">Indicates whether this user calendar supports tracking of meeting responses.</span></span> <span data-ttu-id="75366-207">仅从用户的主日志发送的会议邀请支持会议响应跟踪。</span><span class="sxs-lookup"><span data-stu-id="75366-207">Only meeting invites sent from users' primary calendars support tracking of meeting responses.</span></span>|
|<span data-ttu-id="75366-208">name</span><span class="sxs-lookup"><span data-stu-id="75366-208">name</span></span>|<span data-ttu-id="75366-209">String</span><span class="sxs-lookup"><span data-stu-id="75366-209">String</span></span>|<span data-ttu-id="75366-210">日历名称。</span><span class="sxs-lookup"><span data-stu-id="75366-210">The calendar name.</span></span>|
|<span data-ttu-id="75366-211">owner</span><span class="sxs-lookup"><span data-stu-id="75366-211">owner</span></span> |[<span data-ttu-id="75366-212">emailAddress</span><span class="sxs-lookup"><span data-stu-id="75366-212">emailAddress</span></span>](emailaddress.md) | <span data-ttu-id="75366-p116">如果设置，则表示创建或添加日历的用户。对于用户创建或添加的日历，将 **owner** 属性设置为用户。对于与用户共享的日历，将 **owner** 属性设置为与此用户共享该日历的人员。</span><span class="sxs-lookup"><span data-stu-id="75366-p116">If set, this represents the user who created or added the calendar. For a calendar that the user created or added, the **owner** property is set to the user. For a calendar shared with the user, the **owner** property is set to the person who shared that calendar with the user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="75366-216">关系</span><span class="sxs-lookup"><span data-stu-id="75366-216">Relationships</span></span>
| <span data-ttu-id="75366-217">关系</span><span class="sxs-lookup"><span data-stu-id="75366-217">Relationship</span></span> | <span data-ttu-id="75366-218">类型</span><span class="sxs-lookup"><span data-stu-id="75366-218">Type</span></span>   |<span data-ttu-id="75366-219">Description</span><span class="sxs-lookup"><span data-stu-id="75366-219">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75366-220">calendarPermissions</span><span class="sxs-lookup"><span data-stu-id="75366-220">calendarPermissions</span></span>|<span data-ttu-id="75366-221">[calendarPermission](calendarpermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="75366-221">[calendarPermission](calendarpermission.md) collection</span></span>| <span data-ttu-id="75366-222">共享日历的用户的权限。</span><span class="sxs-lookup"><span data-stu-id="75366-222">The permissions of the users with whom the calendar is shared.</span></span>|
|<span data-ttu-id="75366-223">calendarView</span><span class="sxs-lookup"><span data-stu-id="75366-223">calendarView</span></span>|<span data-ttu-id="75366-224">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="75366-224">[Event](event.md) collection</span></span>|<span data-ttu-id="75366-p117">日历的日历视图。导航属性。只读。</span><span class="sxs-lookup"><span data-stu-id="75366-p117">The calendar view for the calendar. Navigation property. Read-only.</span></span>|
|<span data-ttu-id="75366-228">events</span><span class="sxs-lookup"><span data-stu-id="75366-228">events</span></span>|<span data-ttu-id="75366-229">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="75366-229">[Event](event.md) collection</span></span>|<span data-ttu-id="75366-p118">日历中的事件。导航属性。只读。</span><span class="sxs-lookup"><span data-stu-id="75366-p118">The events in the calendar. Navigation property. Read-only.</span></span>|
|<span data-ttu-id="75366-233">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="75366-233">multiValueExtendedProperties</span></span>|<span data-ttu-id="75366-234">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="75366-234">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="75366-p119">为日历定义的多值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="75366-p119">The collection of multi-value extended properties defined for the calendar. Read-only. Nullable.</span></span>|
|<span data-ttu-id="75366-238">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="75366-238">singleValueExtendedProperties</span></span>|<span data-ttu-id="75366-239">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="75366-239">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="75366-p120">为日历定义的单值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="75366-p120">The collection of single-value extended properties defined for the calendar. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="75366-243">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="75366-243">JSON representation</span></span>

<span data-ttu-id="75366-244">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="75366-244">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "calendarView",
    "events",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.calendar",
  "@odata.annotations": [
    {
      "property": "calendarView",
      "capabilities": {
        "changeTracking": true,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "events",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "navigability": "single",
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "allowedOnlineMeetingProviders": ["string"],
  "canEdit": "boolean",
  "canShare": "boolean",
  "canViewPrivateItems": "boolean",
  "changeKey": "string",
  "color": "String",
  "defaultOnlineMeetingProvider": "string",
  "id": "string (identifier)",
  "isRemovable": "boolean",
  "isTallyingResponses": "boolean",
  "name": "string",
  "owner": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "calendar resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
