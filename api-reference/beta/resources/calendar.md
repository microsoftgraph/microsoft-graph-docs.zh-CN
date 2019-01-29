---
title: 日历资源类型
description: 日历即事件容器。 可以是用户的日历，也可以是 Office 365 组的默认日历。
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 832a7bc18018f4774e2c8ea8786d510c50e2580c
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574703"
---
# <a name="calendar-resource-type"></a><span data-ttu-id="9306b-104">日历资源类型</span><span class="sxs-lookup"><span data-stu-id="9306b-104">calendar resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9306b-105">日历即事件容器。</span><span class="sxs-lookup"><span data-stu-id="9306b-105">A calendar which is a container for events.</span></span> <span data-ttu-id="9306b-106">可以是[用户](user.md)的日历，也可以是 Office 365 [组](group.md)的默认日历。</span><span class="sxs-lookup"><span data-stu-id="9306b-106">It can be a calendar for a [user](user.md), or the default calendar of an Office 365 [group](group.md).</span></span>

> <span data-ttu-id="9306b-107">**注意：** 与用户日历和组日历交互的方式稍有不同：</span><span class="sxs-lookup"><span data-stu-id="9306b-107">**Note:** There are a few minor differences in the way you can interact with user calendars and group calendars:</span></span>

 - <span data-ttu-id="9306b-108">只能将用户日历组织到 [calendarGroup](calendargroup.md) 中。</span><span class="sxs-lookup"><span data-stu-id="9306b-108">You can organize only user calendars in a [calendarGroup](calendargroup.md).</span></span>
 - <span data-ttu-id="9306b-109">Outlook 将代表组自动接受所有会议请求。</span><span class="sxs-lookup"><span data-stu-id="9306b-109">Outlook automatically accepts all meeting requests on behalf of groups.</span></span> <span data-ttu-id="9306b-110">只能[接受](../api/event-accept.md)、[暂时接受](../api/event-tentativelyaccept.md)或[拒绝](../api/event-decline.md)用户日历中的会议请求。</span><span class="sxs-lookup"><span data-stu-id="9306b-110">You can [accept](../api/event-accept.md), [tentatively accept](../api/event-tentativelyaccept.md), or [decline](../api/event-decline.md)  meeting requests for user calendars only.</span></span>
  - <span data-ttu-id="9306b-111">Outlook 不支持对组事件提供提醒。</span><span class="sxs-lookup"><span data-stu-id="9306b-111">Outlook doesn't support reminders for group events.</span></span> <span data-ttu-id="9306b-112">只能[推迟](../api/event-snoozereminder.md)或[取消](../api/event-dismissreminder.md)用户日历的[提醒](reminder.md)。</span><span class="sxs-lookup"><span data-stu-id="9306b-112">You can [snooze](../api/event-snoozereminder.md) or [dismiss](../api/event-dismissreminder.md) a [reminder](reminder.md) for user calendars only.</span></span>

## <a name="methods"></a><span data-ttu-id="9306b-113">方法</span><span class="sxs-lookup"><span data-stu-id="9306b-113">Methods</span></span>

| <span data-ttu-id="9306b-114">方法</span><span class="sxs-lookup"><span data-stu-id="9306b-114">Method</span></span>       | <span data-ttu-id="9306b-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="9306b-115">Return Type</span></span>  |<span data-ttu-id="9306b-116">说明</span><span class="sxs-lookup"><span data-stu-id="9306b-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9306b-117">列出日历</span><span class="sxs-lookup"><span data-stu-id="9306b-117">List calendars</span></span>](../api/user-list-calendars.md)|<span data-ttu-id="9306b-118">[日历](calendar.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9306b-118">[calendar](calendar.md) collection</span></span>|<span data-ttu-id="9306b-119">获取所有用户的日历，或者获取默认或其他特定日历组中的日历。</span><span class="sxs-lookup"><span data-stu-id="9306b-119">Get all the user's calendars, or the calendars in the default or other specific calendar group.</span></span>|
|[<span data-ttu-id="9306b-120">创建日历</span><span class="sxs-lookup"><span data-stu-id="9306b-120">Create calendar</span></span>](../api/user-post-calendars.md) |[<span data-ttu-id="9306b-121">calendar</span><span class="sxs-lookup"><span data-stu-id="9306b-121">calendar</span></span>](calendar.md)| <span data-ttu-id="9306b-122">在默认日历组或用户的指定日历组中新建日历。</span><span class="sxs-lookup"><span data-stu-id="9306b-122">Create a new calendar in the default calendar group or specified calendar group for a user.</span></span>|
|[<span data-ttu-id="9306b-123">Get calendar</span><span class="sxs-lookup"><span data-stu-id="9306b-123">Get calendar</span></span>](../api/calendar-get.md) | [<span data-ttu-id="9306b-124">calendar</span><span class="sxs-lookup"><span data-stu-id="9306b-124">calendar</span></span>](calendar.md) |<span data-ttu-id="9306b-125">获取 **calendar** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9306b-125">Get the properties and relationships of a **calendar** object.</span></span> <span data-ttu-id="9306b-126">可以是用户的日历，也可以是 Office 365 组的默认日历。</span><span class="sxs-lookup"><span data-stu-id="9306b-126">The calendar can be one for a user, or the default calendar of an Office 365 group.</span></span> |
|[<span data-ttu-id="9306b-127">Update</span><span class="sxs-lookup"><span data-stu-id="9306b-127">Update</span></span>](../api/calendar-update.md) | [<span data-ttu-id="9306b-128">calendar</span><span class="sxs-lookup"><span data-stu-id="9306b-128">calendar</span></span>](calendar.md)  |<span data-ttu-id="9306b-129">更新 **calendar** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9306b-129">Update the properties of a **calendar** object.</span></span> <span data-ttu-id="9306b-130">可以是用户的日历，也可以是 Office 365 组的默认日历。</span><span class="sxs-lookup"><span data-stu-id="9306b-130">The calendar can be one for a user, or the default calendar of an Office 365 group.</span></span> |
|[<span data-ttu-id="9306b-131">Delete</span><span class="sxs-lookup"><span data-stu-id="9306b-131">Delete</span></span>](../api/calendar-delete.md) | <span data-ttu-id="9306b-132">无</span><span class="sxs-lookup"><span data-stu-id="9306b-132">None</span></span> |<span data-ttu-id="9306b-133">删除 calendar 对象。</span><span class="sxs-lookup"><span data-stu-id="9306b-133">Delete calendar object.</span></span> |
|[<span data-ttu-id="9306b-134">列出 calendarView</span><span class="sxs-lookup"><span data-stu-id="9306b-134">List calendarView</span></span>](../api/calendar-list-calendarview.md) |<span data-ttu-id="9306b-135">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9306b-135">[event](event.md) collection</span></span>| <span data-ttu-id="9306b-136">从用户的主日历 `(../me/calendarview)` 或指定日历中，获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例。</span><span class="sxs-lookup"><span data-stu-id="9306b-136">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's primary calendar `(../me/calendarview)` or from a specified calendar.</span></span>|
|[<span data-ttu-id="9306b-137">列出事件</span><span class="sxs-lookup"><span data-stu-id="9306b-137">List events</span></span>](../api/calendar-list-events.md) |<span data-ttu-id="9306b-138">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9306b-138">[event](event.md) collection</span></span>| <span data-ttu-id="9306b-p107">检索日历中的事件列表。该列表包含单实例会议和系列主控事件。</span><span class="sxs-lookup"><span data-stu-id="9306b-p107">Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters.</span></span>|
|[<span data-ttu-id="9306b-141">创建事件</span><span class="sxs-lookup"><span data-stu-id="9306b-141">Create event</span></span>](../api/calendar-post-events.md) |[<span data-ttu-id="9306b-142">event</span><span class="sxs-lookup"><span data-stu-id="9306b-142">event</span></span>](event.md)| <span data-ttu-id="9306b-143">在默认或指定日历中创建新事件。</span><span class="sxs-lookup"><span data-stu-id="9306b-143">Create a new Event in the default or specified calendar.</span></span>|
|[<span data-ttu-id="9306b-144">findMeetingTimes</span><span class="sxs-lookup"><span data-stu-id="9306b-144">findmeetingtimes</span></span>](../api/user-findmeetingtimes.md) |[<span data-ttu-id="9306b-145">meetingTimeSuggestionsResult</span><span class="sxs-lookup"><span data-stu-id="9306b-145">meetingTimeSuggestionsResult</span></span>](meetingtimesuggestionsresult.md) |<span data-ttu-id="9306b-146">根据组织者和与会者忙/闲状态以及时间或地点约束，建议会议时间和地点。</span><span class="sxs-lookup"><span data-stu-id="9306b-146">Suggest meeting times and locations based on organizer and attendee availability, and time or location constraints.</span></span> |
|[<span data-ttu-id="9306b-147">getSchedule（预览）</span><span class="sxs-lookup"><span data-stu-id="9306b-147">getSchedule (preview)</span></span>](../api/calendar-getschedule.md) |<span data-ttu-id="9306b-148">[scheduleInformation](scheduleinformation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9306b-148">[scheduleInformation](scheduleinformation.md) collection</span></span>|<span data-ttu-id="9306b-149">获取用户、通讯组列表或资源在指定时间段内的忙/闲状态信息。</span><span class="sxs-lookup"><span data-stu-id="9306b-149">Get the free/busy availability information for a collection of users, distributions lists, or resources, for a specified time period.</span></span> |
|[<span data-ttu-id="9306b-150">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="9306b-150">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="9306b-151">日历</span><span class="sxs-lookup"><span data-stu-id="9306b-151">calendar</span></span>](calendar.md)  |<span data-ttu-id="9306b-152">在新建或现有日历中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="9306b-152">Create one or more single-value extended properties in a new or existing calendar.</span></span>   |
|[<span data-ttu-id="9306b-153">获取包含单值扩展属性的日历</span><span class="sxs-lookup"><span data-stu-id="9306b-153">Get calendar with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="9306b-154">日历</span><span class="sxs-lookup"><span data-stu-id="9306b-154">calendar</span></span>](calendar.md) | <span data-ttu-id="9306b-155">通过使用 `$expand` 或 `$filter` 获取包含一个单值扩展属性的日历。</span><span class="sxs-lookup"><span data-stu-id="9306b-155">Get calendars that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="9306b-156">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="9306b-156">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="9306b-157">日历</span><span class="sxs-lookup"><span data-stu-id="9306b-157">calendar</span></span>](calendar.md) | <span data-ttu-id="9306b-158">在新建或现有的日历中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="9306b-158">Create one or more multi-value extended properties in a new or existing calendar.</span></span>  |
|[<span data-ttu-id="9306b-159">获取包含多值扩展属性的日历</span><span class="sxs-lookup"><span data-stu-id="9306b-159">Get calendar with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="9306b-160">日历</span><span class="sxs-lookup"><span data-stu-id="9306b-160">calendar</span></span>](calendar.md) | <span data-ttu-id="9306b-161">使用 `$expand` 获取包含一个多值扩展属性的日历。</span><span class="sxs-lookup"><span data-stu-id="9306b-161">Get a calendar that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="9306b-162">属性</span><span class="sxs-lookup"><span data-stu-id="9306b-162">Properties</span></span>
| <span data-ttu-id="9306b-163">属性</span><span class="sxs-lookup"><span data-stu-id="9306b-163">Property</span></span>     | <span data-ttu-id="9306b-164">类型</span><span class="sxs-lookup"><span data-stu-id="9306b-164">Type</span></span>   |<span data-ttu-id="9306b-165">说明</span><span class="sxs-lookup"><span data-stu-id="9306b-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9306b-166">canEdit</span><span class="sxs-lookup"><span data-stu-id="9306b-166">canEdit</span></span> |<span data-ttu-id="9306b-167">布尔</span><span class="sxs-lookup"><span data-stu-id="9306b-167">Boolean</span></span> |<span data-ttu-id="9306b-p108">如果用户可以写入日历则为 true，否则为 false。对于创建此日历的用户，此属性为 true。此属性对于共享日历并且授予写入访问权限的用户同样为 true。</span><span class="sxs-lookup"><span data-stu-id="9306b-p108">True if the user can write to the calendar, false otherwise. This property is true for the user who created the calendar. This property is also true for a user who has been shared a calendar and granted write access.</span></span> |
|<span data-ttu-id="9306b-171">canShare</span><span class="sxs-lookup"><span data-stu-id="9306b-171">canShare</span></span> |<span data-ttu-id="9306b-172">布尔</span><span class="sxs-lookup"><span data-stu-id="9306b-172">Boolean</span></span> |<span data-ttu-id="9306b-p109">如果用户有权共享日历则为 ture，否则为 false。只有创建日历的用户才可以进行共享。</span><span class="sxs-lookup"><span data-stu-id="9306b-p109">True if the user has the permission to share the calendar, false otherwise. Only the user who created the calendar can share it.</span></span> |
|<span data-ttu-id="9306b-175">canViewPrivateItems</span><span class="sxs-lookup"><span data-stu-id="9306b-175">canViewPrivateItems</span></span> |<span data-ttu-id="9306b-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="9306b-176">Boolean</span></span> |<span data-ttu-id="9306b-177">如果用户可以读取已标记为私有的日历项，则为 true，否则返回 false。</span><span class="sxs-lookup"><span data-stu-id="9306b-177">True if the user can read calendar items that have been marked private, false otherwise.</span></span> |
|<span data-ttu-id="9306b-178">changeKey</span><span class="sxs-lookup"><span data-stu-id="9306b-178">changeKey</span></span>|<span data-ttu-id="9306b-179">字符串</span><span class="sxs-lookup"><span data-stu-id="9306b-179">String</span></span>|<span data-ttu-id="9306b-p110">标识 calendar 对象的版本。每次日历更改时，changeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。只读。</span><span class="sxs-lookup"><span data-stu-id="9306b-p110">Identifies the version of the calendar object. Every time the calendar is changed, changeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span>|
|<span data-ttu-id="9306b-184">color</span><span class="sxs-lookup"><span data-stu-id="9306b-184">color</span></span>|<span data-ttu-id="9306b-185">String</span><span class="sxs-lookup"><span data-stu-id="9306b-185">String</span></span>|<span data-ttu-id="9306b-p111">在 UI 中指定将该日历与其他日历区分开来的颜色主题。属性值有：LightBlue=0、LightGreen=1、LightOrange=2、LightGray=3、LightYellow=4、LightTeal=5、LightPink=6、LightBrown=7、LightRed=8、MaxColor=9、Auto=-1</span><span class="sxs-lookup"><span data-stu-id="9306b-p111">Specifies the color theme to distinguish the calendar from other calendars in a UI. The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span></span>|
|<span data-ttu-id="9306b-188">hexColor</span><span class="sxs-lookup"><span data-stu-id="9306b-188">hexColor</span></span>|<span data-ttu-id="9306b-189">String</span><span class="sxs-lookup"><span data-stu-id="9306b-189">String</span></span>|<span data-ttu-id="9306b-190">一种表示日历的颜色。</span><span class="sxs-lookup"><span data-stu-id="9306b-190">A color representing the calendar.</span></span> <span data-ttu-id="9306b-191">该颜色由 6 位 3 字节十六进制数表示。</span><span class="sxs-lookup"><span data-stu-id="9306b-191">The color is represented by a 6-digit, 3-byte hexadecimal number.</span></span> <span data-ttu-id="9306b-192">每个字节表示颜色的红色、绿色和蓝色分量之一（位于 00 到 FF 范围内，以十六进制表示法表示）。</span><span class="sxs-lookup"><span data-stu-id="9306b-192">Each byte represents one of the red, green, and blue components of the color, in the range 00 to FF in hexadecimal notation.</span></span> |
|<span data-ttu-id="9306b-193">id</span><span class="sxs-lookup"><span data-stu-id="9306b-193">id</span></span>|<span data-ttu-id="9306b-194">String</span><span class="sxs-lookup"><span data-stu-id="9306b-194">String</span></span>|<span data-ttu-id="9306b-p113">组的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="9306b-p113">The group's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="9306b-197">isDefaultCalendar</span><span class="sxs-lookup"><span data-stu-id="9306b-197">isDefaultCalendar</span></span>|<span data-ttu-id="9306b-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="9306b-198">Boolean</span></span>|<span data-ttu-id="9306b-199">如果此日历是用户的默认日历，则值为 true，否则为 false。</span><span class="sxs-lookup"><span data-stu-id="9306b-199">True if this calendar is the user's default calendar, false otherwise.</span></span>|
|<span data-ttu-id="9306b-200">isShared</span><span class="sxs-lookup"><span data-stu-id="9306b-200">isShared</span></span> |<span data-ttu-id="9306b-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="9306b-201">Boolean</span></span> |<span data-ttu-id="9306b-202">如果用户已与其他用户共享日历，则值为 true，否则为 false。</span><span class="sxs-lookup"><span data-stu-id="9306b-202">True if the user has shared the calendar with other users, false otherwise.</span></span> <span data-ttu-id="9306b-203">由于只有创建日历的用户才能共享日历，因此同一用户的 **isShared** 和 **isSharedWithMe** 不能为 true。</span><span class="sxs-lookup"><span data-stu-id="9306b-203">Since only the user who created the calendar can share it, **isShared** and **isSharedWithMe** cannot be true for the same user.</span></span> |
|<span data-ttu-id="9306b-204">isSharedWithMe</span><span class="sxs-lookup"><span data-stu-id="9306b-204">isSharedWithMe</span></span> |<span data-ttu-id="9306b-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="9306b-205">Boolean</span></span> |<span data-ttu-id="9306b-206">如果用户已共享此日历，则值为 true，否则为 false。</span><span class="sxs-lookup"><span data-stu-id="9306b-206">True if the user has been shared this calendar, false otherwise.</span></span> <span data-ttu-id="9306b-207">对于日历所有者，此属性始终为 false。</span><span class="sxs-lookup"><span data-stu-id="9306b-207">This property is always false for a calendar owner.</span></span>  |
|<span data-ttu-id="9306b-208">name</span><span class="sxs-lookup"><span data-stu-id="9306b-208">name</span></span>|<span data-ttu-id="9306b-209">String</span><span class="sxs-lookup"><span data-stu-id="9306b-209">String</span></span>|<span data-ttu-id="9306b-210">日历名称。</span><span class="sxs-lookup"><span data-stu-id="9306b-210">The calendar name.</span></span>|
|<span data-ttu-id="9306b-211">owner</span><span class="sxs-lookup"><span data-stu-id="9306b-211">owner</span></span> |[<span data-ttu-id="9306b-212">emailAddress</span><span class="sxs-lookup"><span data-stu-id="9306b-212">emailAddress</span></span>](emailaddress.md) | <span data-ttu-id="9306b-p116">如果设置，则表示创建或添加日历的用户。对于用户创建或添加的日历，将 **owner** 属性设置为用户。对于与用户共享的日历，将 **owner** 属性设置为与此用户共享该日历的人员。</span><span class="sxs-lookup"><span data-stu-id="9306b-p116">If set, this represents the user who created or added the calendar. For a calendar that the user created or added, the **owner** property is set to the user. For a calendar shared with the user, the **owner** property is set to the person who shared that calendar with the user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9306b-216">关系</span><span class="sxs-lookup"><span data-stu-id="9306b-216">Relationships</span></span>
| <span data-ttu-id="9306b-217">关系</span><span class="sxs-lookup"><span data-stu-id="9306b-217">Relationship</span></span> | <span data-ttu-id="9306b-218">类型</span><span class="sxs-lookup"><span data-stu-id="9306b-218">Type</span></span>   |<span data-ttu-id="9306b-219">说明</span><span class="sxs-lookup"><span data-stu-id="9306b-219">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9306b-220">calendarView</span><span class="sxs-lookup"><span data-stu-id="9306b-220">calendarView</span></span>|<span data-ttu-id="9306b-221">[event](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9306b-221">[event](event.md) collection</span></span>|<span data-ttu-id="9306b-p117">日历的日历视图。导航属性。只读。</span><span class="sxs-lookup"><span data-stu-id="9306b-p117">The calendar view for the calendar. Navigation property. Read-only.</span></span>|
|<span data-ttu-id="9306b-225">events</span><span class="sxs-lookup"><span data-stu-id="9306b-225">events</span></span>|<span data-ttu-id="9306b-226">[event](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9306b-226">[event](event.md) collection</span></span>|<span data-ttu-id="9306b-p118">日历中的事件。导航属性。只读。</span><span class="sxs-lookup"><span data-stu-id="9306b-p118">The events in the calendar. Navigation property. Read-only.</span></span>|
|<span data-ttu-id="9306b-230">multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="9306b-230">multiValueLegacyExtendedProperty</span></span>| <span data-ttu-id="9306b-231">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9306b-231">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span> | <span data-ttu-id="9306b-p119">为日历定义的多值扩展属性的集合。只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="9306b-p119">The collection of multi-value extended properties defined for the calendar. Read-only. Nullable.</span></span>|
|<span data-ttu-id="9306b-235">singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="9306b-235">singleValueLegacyExtendedProperty,</span></span>| <span data-ttu-id="9306b-236">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9306b-236">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span> | <span data-ttu-id="9306b-p120">为日历定义的单值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="9306b-p120">The collection of single-value extended properties defined for the calendar. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9306b-240">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9306b-240">JSON representation</span></span>

<span data-ttu-id="9306b-241">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9306b-241">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "calendarView",
    "events",
    "multiValueLegacyExtendedProperty",
    "singleValueLegacyExtendedProperty"
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
  "canEdit": "boolean",
  "canShare": "boolean",
  "canViewPrivateItems": "boolean",
  "changeKey": "string",
  "color": "String",
  "hexColor": "String",
  "id": "string (identifier)",
  "isDefaultCalendar": "boolean",
  "isShared": "boolean",
  "isSharedWithMe": "boolean",
  "name": "string",
  "owner": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "calendar resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/calendar.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
