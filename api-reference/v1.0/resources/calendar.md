---
title: 日历资源类型
description: 日历即事件容器。 可以是用户的日历，也可以是 Office 365 组的默认日历。
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 713753dc10e7576d458b5c83c994aa757085b05f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531989"
---
# <a name="calendar-resource-type"></a><span data-ttu-id="519dc-104">日历资源类型</span><span class="sxs-lookup"><span data-stu-id="519dc-104">calendar resource type</span></span>

<span data-ttu-id="519dc-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="519dc-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="519dc-106">日历即事件容器。</span><span class="sxs-lookup"><span data-stu-id="519dc-106">A calendar which is a container for events.</span></span> <span data-ttu-id="519dc-107">可以是[用户](user.md)的日历，也可以是 Office 365 [组](group.md)的默认日历。</span><span class="sxs-lookup"><span data-stu-id="519dc-107">It can be a calendar for a [user](user.md), or the default calendar of an Office 365 [group](group.md).</span></span>

> <span data-ttu-id="519dc-108">**注意：** 与用户日历和组日历交互的方式稍有不同：</span><span class="sxs-lookup"><span data-stu-id="519dc-108">**Note:** There are a few minor differences in the way you can interact with user calendars and group calendars:</span></span>

- <span data-ttu-id="519dc-109">只能将用户日历组织到 [calendarGroup](calendargroup.md) 中。</span><span class="sxs-lookup"><span data-stu-id="519dc-109">You can organize only user calendars in a [calendarGroup](calendargroup.md).</span></span>
- <span data-ttu-id="519dc-110">Outlook 将代表组自动接受所有会议请求。</span><span class="sxs-lookup"><span data-stu-id="519dc-110">Outlook automatically accepts all meeting requests on behalf of groups.</span></span> <span data-ttu-id="519dc-111">只能[接受](../api/event-accept.md)、[暂时接受](../api/event-tentativelyaccept.md)或[拒绝](../api/event-decline.md)用户日历中的会议请求。</span><span class="sxs-lookup"><span data-stu-id="519dc-111">You can [accept](../api/event-accept.md), [tentatively accept](../api/event-tentativelyaccept.md), or [decline](../api/event-decline.md)  meeting requests for user calendars only.</span></span>
- <span data-ttu-id="519dc-112">Outlook 不支持对组事件提供提醒。</span><span class="sxs-lookup"><span data-stu-id="519dc-112">Outlook doesn't support reminders for group events.</span></span> <span data-ttu-id="519dc-113">只能[推迟](../api/event-snoozereminder.md)或[取消](../api/event-dismissreminder.md)用户日历的[提醒](reminder.md)。</span><span class="sxs-lookup"><span data-stu-id="519dc-113">You can [snooze](../api/event-snoozereminder.md) or [dismiss](../api/event-dismissreminder.md) a [reminder](reminder.md) for user calendars only.</span></span>

## <a name="methods"></a><span data-ttu-id="519dc-114">方法</span><span class="sxs-lookup"><span data-stu-id="519dc-114">Methods</span></span>

| <span data-ttu-id="519dc-115">方法</span><span class="sxs-lookup"><span data-stu-id="519dc-115">Method</span></span>       | <span data-ttu-id="519dc-116">返回类型</span><span class="sxs-lookup"><span data-stu-id="519dc-116">Return Type</span></span>  |<span data-ttu-id="519dc-117">说明</span><span class="sxs-lookup"><span data-stu-id="519dc-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="519dc-118">列出日历</span><span class="sxs-lookup"><span data-stu-id="519dc-118">List calendars</span></span>](../api/user-list-calendars.md)|<span data-ttu-id="519dc-119">[日历](calendar.md) 集合</span><span class="sxs-lookup"><span data-stu-id="519dc-119">[calendar](calendar.md) collection</span></span>|<span data-ttu-id="519dc-120">获取所有用户的日历，或者获取默认或其他特定日历组中的日历。</span><span class="sxs-lookup"><span data-stu-id="519dc-120">Get all the user's calendars, or the calendars in the default or other specific calendar group.</span></span>|
|[<span data-ttu-id="519dc-121">创建日历</span><span class="sxs-lookup"><span data-stu-id="519dc-121">Create calendar</span></span>](../api/user-post-calendars.md) |[<span data-ttu-id="519dc-122">calendar</span><span class="sxs-lookup"><span data-stu-id="519dc-122">calendar</span></span>](calendar.md)| <span data-ttu-id="519dc-123">在默认日历组或用户的指定日历组中新建日历。</span><span class="sxs-lookup"><span data-stu-id="519dc-123">Create a new calendar in the default calendar group or specified calendar group for a user.</span></span>|
|[<span data-ttu-id="519dc-124">Get calendar</span><span class="sxs-lookup"><span data-stu-id="519dc-124">Get calendar</span></span>](../api/calendar-get.md) | [<span data-ttu-id="519dc-125">calendar</span><span class="sxs-lookup"><span data-stu-id="519dc-125">calendar</span></span>](calendar.md) |<span data-ttu-id="519dc-126">获取 **calendar** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="519dc-126">Get the properties and relationships of a **calendar** object.</span></span> <span data-ttu-id="519dc-127">可以是用户的日历，也可以是 Office 365 组的默认日历。</span><span class="sxs-lookup"><span data-stu-id="519dc-127">The calendar can be one for a user, or the default calendar of an Office 365 group.</span></span> |
|[<span data-ttu-id="519dc-128">Update</span><span class="sxs-lookup"><span data-stu-id="519dc-128">Update</span></span>](../api/calendar-update.md) | [<span data-ttu-id="519dc-129">calendar</span><span class="sxs-lookup"><span data-stu-id="519dc-129">calendar</span></span>](calendar.md)  |<span data-ttu-id="519dc-130">更新 **calendar** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="519dc-130">Update the properties of a **calendar** object.</span></span> <span data-ttu-id="519dc-131">可以是用户的日历，也可以是 Office 365 组的默认日历。</span><span class="sxs-lookup"><span data-stu-id="519dc-131">The calendar can be one for a user, or the default calendar of an Office 365 group.</span></span> |
|[<span data-ttu-id="519dc-132">Delete</span><span class="sxs-lookup"><span data-stu-id="519dc-132">Delete</span></span>](../api/calendar-delete.md) | <span data-ttu-id="519dc-133">无</span><span class="sxs-lookup"><span data-stu-id="519dc-133">None</span></span> |<span data-ttu-id="519dc-134">删除 calendar 对象。</span><span class="sxs-lookup"><span data-stu-id="519dc-134">Delete calendar object.</span></span> |
|[<span data-ttu-id="519dc-135">列出 calendarView</span><span class="sxs-lookup"><span data-stu-id="519dc-135">List calendarView</span></span>](../api/calendar-list-calendarview.md) |<span data-ttu-id="519dc-136">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="519dc-136">[event](event.md) collection</span></span>| <span data-ttu-id="519dc-137">从用户的主日历 `(../me/calendarview)` 或指定日历中，获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例。</span><span class="sxs-lookup"><span data-stu-id="519dc-137">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's primary calendar `(../me/calendarview)` or from a specified calendar.</span></span>|
|[<span data-ttu-id="519dc-138">列出事件</span><span class="sxs-lookup"><span data-stu-id="519dc-138">List events</span></span>](../api/calendar-list-events.md) |<span data-ttu-id="519dc-139">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="519dc-139">[event](event.md) collection</span></span>| <span data-ttu-id="519dc-p107">检索日历中的事件列表。该列表包含单实例会议和系列主控事件。</span><span class="sxs-lookup"><span data-stu-id="519dc-p107">Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters.</span></span>|
|[<span data-ttu-id="519dc-142">创建事件</span><span class="sxs-lookup"><span data-stu-id="519dc-142">Create event</span></span>](../api/calendar-post-events.md) |[<span data-ttu-id="519dc-143">event</span><span class="sxs-lookup"><span data-stu-id="519dc-143">event</span></span>](event.md)| <span data-ttu-id="519dc-144">在默认或指定日历中创建新事件。</span><span class="sxs-lookup"><span data-stu-id="519dc-144">Create a new event in the default or specified calendar.</span></span>|
|[<span data-ttu-id="519dc-145">getSchedule</span><span class="sxs-lookup"><span data-stu-id="519dc-145">getSchedule</span></span>](../api/calendar-getschedule.md) |<span data-ttu-id="519dc-146">[scheduleInformation](scheduleinformation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="519dc-146">[scheduleInformation](scheduleinformation.md) collection</span></span>|<span data-ttu-id="519dc-147">获取用户、通讯组列表或资源在指定时间段内的忙/闲状态信息。</span><span class="sxs-lookup"><span data-stu-id="519dc-147">Get the free/busy availability information for a collection of users, distributions lists, or resources, for a specified time period.</span></span> |
|[<span data-ttu-id="519dc-148">findMeetingTimes</span><span class="sxs-lookup"><span data-stu-id="519dc-148">findMeetingTimes</span></span>](../api/user-findmeetingtimes.md) |[<span data-ttu-id="519dc-149">meetingTimeSuggestionsResult</span><span class="sxs-lookup"><span data-stu-id="519dc-149">meetingTimeSuggestionsResult</span></span>](meetingtimesuggestionsresult.md) |<span data-ttu-id="519dc-150">根据组织者和与会者忙/闲状态以及时间或地点约束，建议会议时间和地点。</span><span class="sxs-lookup"><span data-stu-id="519dc-150">Suggest meeting times and locations based on organizer and attendee availability, and time or location constraints.</span></span> |
|[<span data-ttu-id="519dc-151">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="519dc-151">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="519dc-152">日历</span><span class="sxs-lookup"><span data-stu-id="519dc-152">calendar</span></span>](calendar.md)  |<span data-ttu-id="519dc-153">在新建或现有日历中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="519dc-153">Create one or more single-value extended properties in a new or existing calendar.</span></span>   |
|[<span data-ttu-id="519dc-154">获取包含单值扩展属性的日历</span><span class="sxs-lookup"><span data-stu-id="519dc-154">Get calendar with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="519dc-155">日历</span><span class="sxs-lookup"><span data-stu-id="519dc-155">calendar</span></span>](calendar.md) | <span data-ttu-id="519dc-156">通过使用 `$expand` 或 `$filter` 获取包含一个单值扩展属性的日历。</span><span class="sxs-lookup"><span data-stu-id="519dc-156">Get calendars that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="519dc-157">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="519dc-157">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="519dc-158">日历</span><span class="sxs-lookup"><span data-stu-id="519dc-158">calendar</span></span>](calendar.md) | <span data-ttu-id="519dc-159">在新建或现有的日历中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="519dc-159">Create one or more multi-value extended properties in a new or existing calendar.</span></span>  |
|[<span data-ttu-id="519dc-160">获取包含多值扩展属性的日历</span><span class="sxs-lookup"><span data-stu-id="519dc-160">Get calendar with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="519dc-161">日历</span><span class="sxs-lookup"><span data-stu-id="519dc-161">calendar</span></span>](calendar.md) | <span data-ttu-id="519dc-162">使用 `$expand` 获取包含一个多值扩展属性的日历。</span><span class="sxs-lookup"><span data-stu-id="519dc-162">Get a calendar that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="519dc-163">属性</span><span class="sxs-lookup"><span data-stu-id="519dc-163">Properties</span></span>
| <span data-ttu-id="519dc-164">属性</span><span class="sxs-lookup"><span data-stu-id="519dc-164">Property</span></span>     | <span data-ttu-id="519dc-165">类型</span><span class="sxs-lookup"><span data-stu-id="519dc-165">Type</span></span>   |<span data-ttu-id="519dc-166">说明</span><span class="sxs-lookup"><span data-stu-id="519dc-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="519dc-167">canEdit</span><span class="sxs-lookup"><span data-stu-id="519dc-167">canEdit</span></span> |<span data-ttu-id="519dc-168">布尔</span><span class="sxs-lookup"><span data-stu-id="519dc-168">Boolean</span></span> |<span data-ttu-id="519dc-p108">如果用户可以写入日历则为 true，否则为 false。对于创建此日历的用户，此属性为 true。此属性对于共享日历并且授予写入访问权限的用户同样为 true。</span><span class="sxs-lookup"><span data-stu-id="519dc-p108">True if the user can write to the calendar, false otherwise. This property is true for the user who created the calendar. This property is also true for a user who has been shared a calendar and granted write access.</span></span> |
|<span data-ttu-id="519dc-172">canShare</span><span class="sxs-lookup"><span data-stu-id="519dc-172">canShare</span></span> |<span data-ttu-id="519dc-173">布尔</span><span class="sxs-lookup"><span data-stu-id="519dc-173">Boolean</span></span> |<span data-ttu-id="519dc-p109">如果用户有权共享日历则为 ture，否则为 false。只有创建日历的用户才可以进行共享。</span><span class="sxs-lookup"><span data-stu-id="519dc-p109">True if the user has the permission to share the calendar, false otherwise. Only the user who created the calendar can share it.</span></span> |
|<span data-ttu-id="519dc-176">canViewPrivateItems</span><span class="sxs-lookup"><span data-stu-id="519dc-176">canViewPrivateItems</span></span> |<span data-ttu-id="519dc-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="519dc-177">Boolean</span></span> |<span data-ttu-id="519dc-178">如果用户可以读取已标记为私有的日历项，则为 true，否则返回 false。</span><span class="sxs-lookup"><span data-stu-id="519dc-178">True if the user can read calendar items that have been marked private, false otherwise.</span></span> |
|<span data-ttu-id="519dc-179">changeKey</span><span class="sxs-lookup"><span data-stu-id="519dc-179">changeKey</span></span>|<span data-ttu-id="519dc-180">字符串</span><span class="sxs-lookup"><span data-stu-id="519dc-180">String</span></span>|<span data-ttu-id="519dc-p110">标识 calendar 对象的版本。每次日历更改时，changeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。只读。</span><span class="sxs-lookup"><span data-stu-id="519dc-p110">Identifies the version of the calendar object. Every time the calendar is changed, changeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span>|
|<span data-ttu-id="519dc-185">颜色</span><span class="sxs-lookup"><span data-stu-id="519dc-185">color</span></span>|<span data-ttu-id="519dc-186">calendarColor</span><span class="sxs-lookup"><span data-stu-id="519dc-186">calendarColor</span></span>|<span data-ttu-id="519dc-p111">在 UI 中指定将该日历与其他日历区分开来的颜色主题。属性值有：LightBlue=0、LightGreen=1、LightOrange=2、LightGray=3、LightYellow=4、LightTeal=5、LightPink=6、LightBrown=7、LightRed=8、MaxColor=9、Auto=-1</span><span class="sxs-lookup"><span data-stu-id="519dc-p111">Specifies the color theme to distinguish the calendar from other calendars in a UI. The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span></span>|
|<span data-ttu-id="519dc-189">id</span><span class="sxs-lookup"><span data-stu-id="519dc-189">id</span></span>|<span data-ttu-id="519dc-190">String</span><span class="sxs-lookup"><span data-stu-id="519dc-190">String</span></span>|<span data-ttu-id="519dc-p112">日历的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="519dc-p112">The calendar's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="519dc-193">name</span><span class="sxs-lookup"><span data-stu-id="519dc-193">name</span></span>|<span data-ttu-id="519dc-194">String</span><span class="sxs-lookup"><span data-stu-id="519dc-194">String</span></span>|<span data-ttu-id="519dc-195">日历名称。</span><span class="sxs-lookup"><span data-stu-id="519dc-195">The calendar name.</span></span>|
|<span data-ttu-id="519dc-196">owner</span><span class="sxs-lookup"><span data-stu-id="519dc-196">owner</span></span> |[<span data-ttu-id="519dc-197">emailAddress</span><span class="sxs-lookup"><span data-stu-id="519dc-197">emailAddress</span></span>](emailaddress.md) | <span data-ttu-id="519dc-p113">如果设置，则表示创建或添加日历的用户。对于用户创建或添加的日历，将 **owner** 属性设置为用户。对于与用户共享的日历，将 **owner** 属性设置为与此用户共享该日历的人员。</span><span class="sxs-lookup"><span data-stu-id="519dc-p113">If set, this represents the user who created or added the calendar. For a calendar that the user created or added, the **owner** property is set to the user. For a calendar shared with the user, the **owner** property is set to the person who shared that calendar with the user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="519dc-201">关系</span><span class="sxs-lookup"><span data-stu-id="519dc-201">Relationships</span></span>
| <span data-ttu-id="519dc-202">关系</span><span class="sxs-lookup"><span data-stu-id="519dc-202">Relationship</span></span> | <span data-ttu-id="519dc-203">类型</span><span class="sxs-lookup"><span data-stu-id="519dc-203">Type</span></span>   |<span data-ttu-id="519dc-204">说明</span><span class="sxs-lookup"><span data-stu-id="519dc-204">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="519dc-205">calendarView</span><span class="sxs-lookup"><span data-stu-id="519dc-205">calendarView</span></span>|<span data-ttu-id="519dc-206">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="519dc-206">[Event](event.md) collection</span></span>|<span data-ttu-id="519dc-p114">日历的日历视图。导航属性。只读。</span><span class="sxs-lookup"><span data-stu-id="519dc-p114">The calendar view for the calendar. Navigation property. Read-only.</span></span>|
|<span data-ttu-id="519dc-210">events</span><span class="sxs-lookup"><span data-stu-id="519dc-210">events</span></span>|<span data-ttu-id="519dc-211">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="519dc-211">[Event](event.md) collection</span></span>|<span data-ttu-id="519dc-p115">日历中的事件。导航属性。只读。</span><span class="sxs-lookup"><span data-stu-id="519dc-p115">The events in the calendar. Navigation property. Read-only.</span></span>|
|<span data-ttu-id="519dc-215">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="519dc-215">multiValueExtendedProperties</span></span>|<span data-ttu-id="519dc-216">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="519dc-216">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="519dc-p116">为日历定义的多值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="519dc-p116">The collection of multi-value extended properties defined for the calendar. Read-only. Nullable.</span></span>|
|<span data-ttu-id="519dc-220">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="519dc-220">singleValueExtendedProperties</span></span>|<span data-ttu-id="519dc-221">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="519dc-221">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="519dc-p117">为日历定义的单值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="519dc-p117">The collection of single-value extended properties defined for the calendar. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="519dc-225">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="519dc-225">JSON representation</span></span>

<span data-ttu-id="519dc-226">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="519dc-226">Here is a JSON representation of the resource</span></span>

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
  "canEdit": "boolean",
  "canShare": "boolean",
  "canViewPrivateItems": "boolean",
  "changeKey": "string",
  "color": "String",
  "id": "string (identifier)",
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
