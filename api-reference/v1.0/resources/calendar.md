---
title: 日历资源类型
description: 日历即事件容器。 可以是用户的日历，也可以是 Office 365 组的默认日历。
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 67f2fef3c77a2ade4871bbe1da1c2baa95b1e234
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229498"
---
# <a name="calendar-resource-type"></a><span data-ttu-id="d107a-104">日历资源类型</span><span class="sxs-lookup"><span data-stu-id="d107a-104">calendar resource type</span></span>

<span data-ttu-id="d107a-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d107a-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d107a-106">日历即事件容器。</span><span class="sxs-lookup"><span data-stu-id="d107a-106">A calendar which is a container for events.</span></span> <span data-ttu-id="d107a-107">可以是[用户](user.md)的日历，也可以是 Office 365 [组](group.md)的默认日历。</span><span class="sxs-lookup"><span data-stu-id="d107a-107">It can be a calendar for a [user](user.md), or the default calendar of an Office 365 [group](group.md).</span></span>

> <span data-ttu-id="d107a-108">**注意：** 与用户日历和组日历交互的方式稍有不同：</span><span class="sxs-lookup"><span data-stu-id="d107a-108">**Note:** There are a few minor differences in the way you can interact with user calendars and group calendars:</span></span>

- <span data-ttu-id="d107a-109">只能将用户日历组织到 [calendarGroup](calendargroup.md) 中。</span><span class="sxs-lookup"><span data-stu-id="d107a-109">You can organize only user calendars in a [calendarGroup](calendargroup.md).</span></span>
- <span data-ttu-id="d107a-110">Outlook 将代表组自动接受所有会议请求。</span><span class="sxs-lookup"><span data-stu-id="d107a-110">Outlook automatically accepts all meeting requests on behalf of groups.</span></span> <span data-ttu-id="d107a-111">只能[接受](../api/event-accept.md)、[暂时接受](../api/event-tentativelyaccept.md)或[拒绝](../api/event-decline.md)用户日历中的会议请求。</span><span class="sxs-lookup"><span data-stu-id="d107a-111">You can [accept](../api/event-accept.md), [tentatively accept](../api/event-tentativelyaccept.md), or [decline](../api/event-decline.md)  meeting requests for user calendars only.</span></span>
- <span data-ttu-id="d107a-112">Outlook 不支持对组事件提供提醒。</span><span class="sxs-lookup"><span data-stu-id="d107a-112">Outlook doesn't support reminders for group events.</span></span> <span data-ttu-id="d107a-113">只能[推迟](../api/event-snoozereminder.md)或[取消](../api/event-dismissreminder.md)用户日历的[提醒](reminder.md)。</span><span class="sxs-lookup"><span data-stu-id="d107a-113">You can [snooze](../api/event-snoozereminder.md) or [dismiss](../api/event-dismissreminder.md) a [reminder](reminder.md) for user calendars only.</span></span>

## <a name="methods"></a><span data-ttu-id="d107a-114">方法</span><span class="sxs-lookup"><span data-stu-id="d107a-114">Methods</span></span>

| <span data-ttu-id="d107a-115">方法</span><span class="sxs-lookup"><span data-stu-id="d107a-115">Method</span></span>       | <span data-ttu-id="d107a-116">返回类型</span><span class="sxs-lookup"><span data-stu-id="d107a-116">Return Type</span></span>  |<span data-ttu-id="d107a-117">说明</span><span class="sxs-lookup"><span data-stu-id="d107a-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d107a-118">列出日历</span><span class="sxs-lookup"><span data-stu-id="d107a-118">List calendars</span></span>](../api/user-list-calendars.md)|<span data-ttu-id="d107a-119">[日历](calendar.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d107a-119">[calendar](calendar.md) collection</span></span>|<span data-ttu-id="d107a-120">获取所有用户的日历，或者获取默认或其他特定日历组中的日历。</span><span class="sxs-lookup"><span data-stu-id="d107a-120">Get all the user's calendars, or the calendars in the default or other specific calendar group.</span></span>|
|[<span data-ttu-id="d107a-121">创建日历</span><span class="sxs-lookup"><span data-stu-id="d107a-121">Create calendar</span></span>](../api/user-post-calendars.md) |[<span data-ttu-id="d107a-122">calendar</span><span class="sxs-lookup"><span data-stu-id="d107a-122">calendar</span></span>](calendar.md)| <span data-ttu-id="d107a-123">在默认日历组或用户的指定日历组中新建日历。</span><span class="sxs-lookup"><span data-stu-id="d107a-123">Create a new calendar in the default calendar group or specified calendar group for a user.</span></span>|
|[<span data-ttu-id="d107a-124">Get calendar</span><span class="sxs-lookup"><span data-stu-id="d107a-124">Get calendar</span></span>](../api/calendar-get.md) | [<span data-ttu-id="d107a-125">calendar</span><span class="sxs-lookup"><span data-stu-id="d107a-125">calendar</span></span>](calendar.md) |<span data-ttu-id="d107a-126">获取 **calendar** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d107a-126">Get the properties and relationships of a **calendar** object.</span></span> <span data-ttu-id="d107a-127">可以是用户的日历，也可以是 Office 365 组的默认日历。</span><span class="sxs-lookup"><span data-stu-id="d107a-127">The calendar can be one for a user, or the default calendar of an Office 365 group.</span></span> |
|[<span data-ttu-id="d107a-128">Update</span><span class="sxs-lookup"><span data-stu-id="d107a-128">Update</span></span>](../api/calendar-update.md) | [<span data-ttu-id="d107a-129">calendar</span><span class="sxs-lookup"><span data-stu-id="d107a-129">calendar</span></span>](calendar.md)  |<span data-ttu-id="d107a-130">更新 **calendar** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d107a-130">Update the properties of a **calendar** object.</span></span> <span data-ttu-id="d107a-131">可以是用户的日历，也可以是 Office 365 组的默认日历。</span><span class="sxs-lookup"><span data-stu-id="d107a-131">The calendar can be one for a user, or the default calendar of an Office 365 group.</span></span> |
|[<span data-ttu-id="d107a-132">Delete</span><span class="sxs-lookup"><span data-stu-id="d107a-132">Delete</span></span>](../api/calendar-delete.md) | <span data-ttu-id="d107a-133">无</span><span class="sxs-lookup"><span data-stu-id="d107a-133">None</span></span> |<span data-ttu-id="d107a-134">删除 calendar 对象。</span><span class="sxs-lookup"><span data-stu-id="d107a-134">Delete calendar object.</span></span> |
|[<span data-ttu-id="d107a-135">列出 calendarView</span><span class="sxs-lookup"><span data-stu-id="d107a-135">List calendarView</span></span>](../api/calendar-list-calendarview.md) |<span data-ttu-id="d107a-136">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d107a-136">[event](event.md) collection</span></span>| <span data-ttu-id="d107a-137">从用户的主日历 `(../me/calendarview)` 或指定日历中，获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例。</span><span class="sxs-lookup"><span data-stu-id="d107a-137">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's primary calendar `(../me/calendarview)` or from a specified calendar.</span></span>|
|[<span data-ttu-id="d107a-138">列出事件</span><span class="sxs-lookup"><span data-stu-id="d107a-138">List events</span></span>](../api/calendar-list-events.md) |<span data-ttu-id="d107a-139">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d107a-139">[event](event.md) collection</span></span>| <span data-ttu-id="d107a-p107">检索日历中的事件列表。该列表包含单实例会议和系列主控事件。</span><span class="sxs-lookup"><span data-stu-id="d107a-p107">Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters.</span></span>|
|[<span data-ttu-id="d107a-142">创建事件</span><span class="sxs-lookup"><span data-stu-id="d107a-142">Create event</span></span>](../api/calendar-post-events.md) |[<span data-ttu-id="d107a-143">event</span><span class="sxs-lookup"><span data-stu-id="d107a-143">event</span></span>](event.md)| <span data-ttu-id="d107a-144">在默认或指定日历中创建新事件。</span><span class="sxs-lookup"><span data-stu-id="d107a-144">Create a new event in the default or specified calendar.</span></span>|
|[<span data-ttu-id="d107a-145">getSchedule</span><span class="sxs-lookup"><span data-stu-id="d107a-145">getSchedule</span></span>](../api/calendar-getschedule.md) |<span data-ttu-id="d107a-146">[scheduleInformation](scheduleinformation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d107a-146">[scheduleInformation](scheduleinformation.md) collection</span></span>|<span data-ttu-id="d107a-147">获取用户、通讯组列表或资源在指定时间段内的忙/闲状态信息。</span><span class="sxs-lookup"><span data-stu-id="d107a-147">Get the free/busy availability information for a collection of users, distributions lists, or resources, for a specified time period.</span></span> |
|[<span data-ttu-id="d107a-148">findMeetingTimes</span><span class="sxs-lookup"><span data-stu-id="d107a-148">findMeetingTimes</span></span>](../api/user-findmeetingtimes.md) |[<span data-ttu-id="d107a-149">meetingTimeSuggestionsResult</span><span class="sxs-lookup"><span data-stu-id="d107a-149">meetingTimeSuggestionsResult</span></span>](meetingtimesuggestionsresult.md) |<span data-ttu-id="d107a-150">根据组织者和与会者忙/闲状态以及时间或地点约束，建议会议时间和地点。</span><span class="sxs-lookup"><span data-stu-id="d107a-150">Suggest meeting times and locations based on organizer and attendee availability, and time or location constraints.</span></span> |
|[<span data-ttu-id="d107a-151">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="d107a-151">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="d107a-152">日历</span><span class="sxs-lookup"><span data-stu-id="d107a-152">calendar</span></span>](calendar.md)  |<span data-ttu-id="d107a-153">在新建或现有日历中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="d107a-153">Create one or more single-value extended properties in a new or existing calendar.</span></span>   |
|[<span data-ttu-id="d107a-154">获取包含单值扩展属性的日历</span><span class="sxs-lookup"><span data-stu-id="d107a-154">Get calendar with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="d107a-155">日历</span><span class="sxs-lookup"><span data-stu-id="d107a-155">calendar</span></span>](calendar.md) | <span data-ttu-id="d107a-156">通过使用 `$expand` 或 `$filter` 获取包含一个单值扩展属性的日历。</span><span class="sxs-lookup"><span data-stu-id="d107a-156">Get calendars that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="d107a-157">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="d107a-157">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="d107a-158">日历</span><span class="sxs-lookup"><span data-stu-id="d107a-158">calendar</span></span>](calendar.md) | <span data-ttu-id="d107a-159">在新建或现有的日历中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="d107a-159">Create one or more multi-value extended properties in a new or existing calendar.</span></span>  |
|[<span data-ttu-id="d107a-160">获取包含多值扩展属性的日历</span><span class="sxs-lookup"><span data-stu-id="d107a-160">Get calendar with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="d107a-161">日历</span><span class="sxs-lookup"><span data-stu-id="d107a-161">calendar</span></span>](calendar.md) | <span data-ttu-id="d107a-162">使用 `$expand` 获取包含一个多值扩展属性的日历。</span><span class="sxs-lookup"><span data-stu-id="d107a-162">Get a calendar that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="d107a-163">属性</span><span class="sxs-lookup"><span data-stu-id="d107a-163">Properties</span></span>
| <span data-ttu-id="d107a-164">属性</span><span class="sxs-lookup"><span data-stu-id="d107a-164">Property</span></span>     | <span data-ttu-id="d107a-165">类型</span><span class="sxs-lookup"><span data-stu-id="d107a-165">Type</span></span>   |<span data-ttu-id="d107a-166">Description</span><span class="sxs-lookup"><span data-stu-id="d107a-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d107a-167">allowedOnlineMeetingProviders</span><span class="sxs-lookup"><span data-stu-id="d107a-167">allowedOnlineMeetingProviders</span></span>|<span data-ttu-id="d107a-168">string 集合</span><span class="sxs-lookup"><span data-stu-id="d107a-168">string collection</span></span>| <span data-ttu-id="d107a-169">表示此日历中可用于创建联机会议的联机会议服务提供商。</span><span class="sxs-lookup"><span data-stu-id="d107a-169">Represent the online meeting service providers that can be used to create online meetings in this calendar.</span></span> <span data-ttu-id="d107a-170">可取值为：`unknown`、`skypeForBusiness`、`skypeForConsumer`、`teamsForBusiness`。</span><span class="sxs-lookup"><span data-stu-id="d107a-170">Possible values are: `unknown`, `skypeForBusiness`, `skypeForConsumer`, `teamsForBusiness`.</span></span>|
|<span data-ttu-id="d107a-171">canEdit</span><span class="sxs-lookup"><span data-stu-id="d107a-171">canEdit</span></span> |<span data-ttu-id="d107a-172">布尔</span><span class="sxs-lookup"><span data-stu-id="d107a-172">Boolean</span></span> |<span data-ttu-id="d107a-p109">如果用户可以写入日历则为 true，否则为 false。对于创建此日历的用户，此属性为 true。此属性对于共享日历并且授予写入访问权限的用户同样为 true。</span><span class="sxs-lookup"><span data-stu-id="d107a-p109">True if the user can write to the calendar, false otherwise. This property is true for the user who created the calendar. This property is also true for a user who has been shared a calendar and granted write access.</span></span> |
|<span data-ttu-id="d107a-176">canShare</span><span class="sxs-lookup"><span data-stu-id="d107a-176">canShare</span></span> |<span data-ttu-id="d107a-177">布尔</span><span class="sxs-lookup"><span data-stu-id="d107a-177">Boolean</span></span> |<span data-ttu-id="d107a-p110">如果用户有权共享日历则为 ture，否则为 false。只有创建日历的用户才可以进行共享。</span><span class="sxs-lookup"><span data-stu-id="d107a-p110">True if the user has the permission to share the calendar, false otherwise. Only the user who created the calendar can share it.</span></span> |
|<span data-ttu-id="d107a-180">canViewPrivateItems</span><span class="sxs-lookup"><span data-stu-id="d107a-180">canViewPrivateItems</span></span> |<span data-ttu-id="d107a-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="d107a-181">Boolean</span></span> |<span data-ttu-id="d107a-182">如果用户可以读取已标记为私有的日历项，则为 true，否则返回 false。</span><span class="sxs-lookup"><span data-stu-id="d107a-182">True if the user can read calendar items that have been marked private, false otherwise.</span></span> |
|<span data-ttu-id="d107a-183">changeKey</span><span class="sxs-lookup"><span data-stu-id="d107a-183">changeKey</span></span>|<span data-ttu-id="d107a-184">字符串</span><span class="sxs-lookup"><span data-stu-id="d107a-184">String</span></span>|<span data-ttu-id="d107a-p111">标识 calendar 对象的版本。每次日历更改时，changeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。只读。</span><span class="sxs-lookup"><span data-stu-id="d107a-p111">Identifies the version of the calendar object. Every time the calendar is changed, changeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span>|
|<span data-ttu-id="d107a-189">颜色</span><span class="sxs-lookup"><span data-stu-id="d107a-189">color</span></span>|<span data-ttu-id="d107a-190">calendarColor</span><span class="sxs-lookup"><span data-stu-id="d107a-190">calendarColor</span></span>|<span data-ttu-id="d107a-p112">在 UI 中指定将该日历与其他日历区分开来的颜色主题。属性值有：LightBlue=0、LightGreen=1、LightOrange=2、LightGray=3、LightYellow=4、LightTeal=5、LightPink=6、LightBrown=7、LightRed=8、MaxColor=9、Auto=-1</span><span class="sxs-lookup"><span data-stu-id="d107a-p112">Specifies the color theme to distinguish the calendar from other calendars in a UI. The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span></span>|
|<span data-ttu-id="d107a-193">defaultOnlineMeetingProvider</span><span class="sxs-lookup"><span data-stu-id="d107a-193">defaultOnlineMeetingProvider</span></span>|<span data-ttu-id="d107a-194">onlineMeetingProviderType</span><span class="sxs-lookup"><span data-stu-id="d107a-194">onlineMeetingProviderType</span></span>|<span data-ttu-id="d107a-195">从此日历发送的会议的默认联机会议提供商。</span><span class="sxs-lookup"><span data-stu-id="d107a-195">The default online meeting provider for meetings sent from this calendar.</span></span> <span data-ttu-id="d107a-196">可取值为：`unknown`、`skypeForBusiness`、`skypeForConsumer`、`teamsForBusiness`。</span><span class="sxs-lookup"><span data-stu-id="d107a-196">Possible values are: `unknown`, `skypeForBusiness`, `skypeForConsumer`, `teamsForBusiness`.</span></span>|
|<span data-ttu-id="d107a-197">id</span><span class="sxs-lookup"><span data-stu-id="d107a-197">id</span></span>|<span data-ttu-id="d107a-198">String</span><span class="sxs-lookup"><span data-stu-id="d107a-198">String</span></span>|<span data-ttu-id="d107a-p114">日历的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="d107a-p114">The calendar's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="d107a-201">isDefaultCalendar</span><span class="sxs-lookup"><span data-stu-id="d107a-201">isDefaultCalendar</span></span>|<span data-ttu-id="d107a-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="d107a-202">Boolean</span></span>|<span data-ttu-id="d107a-203">若此为默认用于新建事件的默认日志则为 True，反之为 false。</span><span class="sxs-lookup"><span data-stu-id="d107a-203">True if this is the default calendar where new events are created by default, false otherwise.</span></span>|
|<span data-ttu-id="d107a-204">isRemovable</span><span class="sxs-lookup"><span data-stu-id="d107a-204">isRemovable</span></span>|<span data-ttu-id="d107a-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="d107a-205">Boolean</span></span>| <span data-ttu-id="d107a-206">表示是否可以从用户邮箱删除此用户日志。</span><span class="sxs-lookup"><span data-stu-id="d107a-206">Indicates whether this user calendar can be deleted from the user mailbox.</span></span>|
|<span data-ttu-id="d107a-207">isTallyingResponses</span><span class="sxs-lookup"><span data-stu-id="d107a-207">isTallyingResponses</span></span>|<span data-ttu-id="d107a-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="d107a-208">Boolean</span></span>|<span data-ttu-id="d107a-209">表示此用户日历是否支持会议响应跟踪。</span><span class="sxs-lookup"><span data-stu-id="d107a-209">Indicates whether this user calendar supports tracking of meeting responses.</span></span> <span data-ttu-id="d107a-210">仅从用户的主日志发送的会议邀请支持会议响应跟踪。</span><span class="sxs-lookup"><span data-stu-id="d107a-210">Only meeting invites sent from users' primary calendars support tracking of meeting responses.</span></span>|
|<span data-ttu-id="d107a-211">name</span><span class="sxs-lookup"><span data-stu-id="d107a-211">name</span></span>|<span data-ttu-id="d107a-212">String</span><span class="sxs-lookup"><span data-stu-id="d107a-212">String</span></span>|<span data-ttu-id="d107a-213">日历名称。</span><span class="sxs-lookup"><span data-stu-id="d107a-213">The calendar name.</span></span>|
|<span data-ttu-id="d107a-214">owner</span><span class="sxs-lookup"><span data-stu-id="d107a-214">owner</span></span> |[<span data-ttu-id="d107a-215">emailAddress</span><span class="sxs-lookup"><span data-stu-id="d107a-215">emailAddress</span></span>](emailaddress.md) | <span data-ttu-id="d107a-p116">如果设置，则表示创建或添加日历的用户。对于用户创建或添加的日历，将 **owner** 属性设置为用户。对于与用户共享的日历，将 **owner** 属性设置为与此用户共享该日历的人员。</span><span class="sxs-lookup"><span data-stu-id="d107a-p116">If set, this represents the user who created or added the calendar. For a calendar that the user created or added, the **owner** property is set to the user. For a calendar shared with the user, the **owner** property is set to the person who shared that calendar with the user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d107a-219">关系</span><span class="sxs-lookup"><span data-stu-id="d107a-219">Relationships</span></span>
| <span data-ttu-id="d107a-220">关系</span><span class="sxs-lookup"><span data-stu-id="d107a-220">Relationship</span></span> | <span data-ttu-id="d107a-221">类型</span><span class="sxs-lookup"><span data-stu-id="d107a-221">Type</span></span>   |<span data-ttu-id="d107a-222">Description</span><span class="sxs-lookup"><span data-stu-id="d107a-222">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d107a-223">calendarPermissions</span><span class="sxs-lookup"><span data-stu-id="d107a-223">calendarPermissions</span></span>|<span data-ttu-id="d107a-224">[calendarPermission](calendarpermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d107a-224">[calendarPermission](calendarpermission.md) collection</span></span>| <span data-ttu-id="d107a-225">共享日历的用户的权限。</span><span class="sxs-lookup"><span data-stu-id="d107a-225">The permissions of the users with whom the calendar is shared.</span></span>|
|<span data-ttu-id="d107a-226">calendarView</span><span class="sxs-lookup"><span data-stu-id="d107a-226">calendarView</span></span>|<span data-ttu-id="d107a-227">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d107a-227">[Event](event.md) collection</span></span>|<span data-ttu-id="d107a-p117">日历的日历视图。导航属性。只读。</span><span class="sxs-lookup"><span data-stu-id="d107a-p117">The calendar view for the calendar. Navigation property. Read-only.</span></span>|
|<span data-ttu-id="d107a-231">events</span><span class="sxs-lookup"><span data-stu-id="d107a-231">events</span></span>|<span data-ttu-id="d107a-232">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d107a-232">[Event](event.md) collection</span></span>|<span data-ttu-id="d107a-p118">日历中的事件。导航属性。只读。</span><span class="sxs-lookup"><span data-stu-id="d107a-p118">The events in the calendar. Navigation property. Read-only.</span></span>|
|<span data-ttu-id="d107a-236">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="d107a-236">multiValueExtendedProperties</span></span>|<span data-ttu-id="d107a-237">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d107a-237">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="d107a-p119">为日历定义的多值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="d107a-p119">The collection of multi-value extended properties defined for the calendar. Read-only. Nullable.</span></span>|
|<span data-ttu-id="d107a-241">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="d107a-241">singleValueExtendedProperties</span></span>|<span data-ttu-id="d107a-242">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="d107a-242">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="d107a-p120">为日历定义的单值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="d107a-p120">The collection of single-value extended properties defined for the calendar. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d107a-246">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d107a-246">JSON representation</span></span>

<span data-ttu-id="d107a-247">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d107a-247">Here is a JSON representation of the resource</span></span>

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
  "isDefaultCalendar": "boolean",
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
