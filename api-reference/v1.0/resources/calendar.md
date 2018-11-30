---
title: 日历资源类型
description: 日历即事件容器。 可以是用户的日历，也可以是 Office 365 组的默认日历。
ms.openlocfilehash: 1c1797897c0efcd7d7196977f93b6a8c611f83f6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011003"
---
# <a name="calendar-resource-type"></a><span data-ttu-id="84354-104">日历资源类型</span><span class="sxs-lookup"><span data-stu-id="84354-104">calendar resource type</span></span>

<span data-ttu-id="84354-105">日历即事件容器。</span><span class="sxs-lookup"><span data-stu-id="84354-105">A calendar which is a container for events.</span></span> <span data-ttu-id="84354-106">可以是[用户](user.md)的日历，也可以是 Office 365 [组](group.md)的默认日历。</span><span class="sxs-lookup"><span data-stu-id="84354-106">It can be a calendar for a [user](user.md), or the default calendar of an Office 365 [group](group.md).</span></span>

> <span data-ttu-id="84354-107">**注意：** 有几个您可以与用户日历和日历组进行交互的方式不同：</span><span class="sxs-lookup"><span data-stu-id="84354-107">**Note:** There are a few minor differences in the way you can interact with user calendars and group calendars:</span></span>

 - <span data-ttu-id="84354-108">您可以组织只有用户日历中[calendarGroup](calendargroup.md)。</span><span class="sxs-lookup"><span data-stu-id="84354-108">You can organize only user calendars in a [calendarGroup](calendargroup.md).</span></span>
 - <span data-ttu-id="84354-109">Outlook 自动接受代表组的所有会议请求。</span><span class="sxs-lookup"><span data-stu-id="84354-109">Outlook automatically accepts all meeting requests on behalf of groups.</span></span> <span data-ttu-id="84354-110">您可以为用户日历仅[接受](../api/event-accept.md)、[暂时接受](../api/event-tentativelyaccept.md)或[拒绝](../api/event-decline.md)会议请求。</span><span class="sxs-lookup"><span data-stu-id="84354-110">You can [accept](../api/event-accept.md), [tentatively accept](../api/event-tentativelyaccept.md), or [decline](../api/event-decline.md)  meeting requests for user calendars only.</span></span>
  - <span data-ttu-id="84354-111">Outlook 不支持为组事件的提醒。</span><span class="sxs-lookup"><span data-stu-id="84354-111">Outlook doesn't support reminders for group events.</span></span> <span data-ttu-id="84354-112">您可以为仅用户日历[snooze](../api/event-snoozereminder.md)或[消除](../api/event-dismissreminder.md)的[提醒](reminder.md)。</span><span class="sxs-lookup"><span data-stu-id="84354-112">You can [snooze](../api/event-snoozereminder.md) or [dismiss](../api/event-dismissreminder.md) a [reminder](reminder.md) for user calendars only.</span></span>

## <a name="methods"></a><span data-ttu-id="84354-113">方法</span><span class="sxs-lookup"><span data-stu-id="84354-113">Methods</span></span>

| <span data-ttu-id="84354-114">方法</span><span class="sxs-lookup"><span data-stu-id="84354-114">Method</span></span>       | <span data-ttu-id="84354-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="84354-115">Return Type</span></span>  |<span data-ttu-id="84354-116">说明</span><span class="sxs-lookup"><span data-stu-id="84354-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="84354-117">列出日历</span><span class="sxs-lookup"><span data-stu-id="84354-117">List calendars</span></span>](../api/user-list-calendars.md)|<span data-ttu-id="84354-118">[日历](calendar.md) 集合</span><span class="sxs-lookup"><span data-stu-id="84354-118">[calendar](calendar.md) collection</span></span>|<span data-ttu-id="84354-119">获取所有用户的日历，或者获取默认或其他特定日历组中的日历。</span><span class="sxs-lookup"><span data-stu-id="84354-119">Get all the user's calendars, or the calendars in the default or other specific calendar group.</span></span>|
|[<span data-ttu-id="84354-120">创建日历</span><span class="sxs-lookup"><span data-stu-id="84354-120">Create calendar</span></span>](../api/user-post-calendars.md) |[<span data-ttu-id="84354-121">calendar</span><span class="sxs-lookup"><span data-stu-id="84354-121">calendar</span></span>](calendar.md)| <span data-ttu-id="84354-122">在默认日历组或用户的指定日历组中新建日历。</span><span class="sxs-lookup"><span data-stu-id="84354-122">Create a new calendar in the default calendar group or specified calendar group for a user.</span></span>|
|[<span data-ttu-id="84354-123">Get calendar</span><span class="sxs-lookup"><span data-stu-id="84354-123">Get calendar</span></span>](../api/calendar-get.md) | [<span data-ttu-id="84354-124">calendar</span><span class="sxs-lookup"><span data-stu-id="84354-124">calendar</span></span>](calendar.md) |<span data-ttu-id="84354-125">获取 **calendar** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="84354-125">Get the properties and relationships of a **calendar** object.</span></span> <span data-ttu-id="84354-126">可以是用户的日历，也可以是 Office 365 组的默认日历。</span><span class="sxs-lookup"><span data-stu-id="84354-126">The calendar can be one for a user, or the default calendar of an Office 365 group.</span></span> |
|[<span data-ttu-id="84354-127">Update</span><span class="sxs-lookup"><span data-stu-id="84354-127">Update</span></span>](../api/calendar-update.md) | [<span data-ttu-id="84354-128">calendar</span><span class="sxs-lookup"><span data-stu-id="84354-128">calendar</span></span>](calendar.md)  |<span data-ttu-id="84354-129">更新 **calendar** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="84354-129">Update the properties of a **calendar** object.</span></span> <span data-ttu-id="84354-130">可以是用户的日历，也可以是 Office 365 组的默认日历。</span><span class="sxs-lookup"><span data-stu-id="84354-130">The calendar can be one for a user, or the default calendar of an Office 365 group.</span></span> |
|[<span data-ttu-id="84354-131">Delete</span><span class="sxs-lookup"><span data-stu-id="84354-131">Delete</span></span>](../api/calendar-delete.md) | <span data-ttu-id="84354-132">无</span><span class="sxs-lookup"><span data-stu-id="84354-132">None</span></span> |<span data-ttu-id="84354-133">删除 calendar 对象。</span><span class="sxs-lookup"><span data-stu-id="84354-133">Delete calendar object.</span></span> |
|[<span data-ttu-id="84354-134">列出 calendarView</span><span class="sxs-lookup"><span data-stu-id="84354-134">List calendarView</span></span>](../api/calendar-list-calendarview.md) |<span data-ttu-id="84354-135">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="84354-135">[event](event.md) collection</span></span>| <span data-ttu-id="84354-136">从用户的主日历 `(../me/calendarview)` 或指定日历中，获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例。</span><span class="sxs-lookup"><span data-stu-id="84354-136">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's primary calendar `(../me/calendarview)` or from a specified calendar.</span></span>|
|[<span data-ttu-id="84354-137">列出事件</span><span class="sxs-lookup"><span data-stu-id="84354-137">List events</span></span>](../api/calendar-list-events.md) |<span data-ttu-id="84354-138">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="84354-138">[event](event.md) collection</span></span>| <span data-ttu-id="84354-p107">检索日历中的事件列表。该列表包含单个实例会议和系列主控形状。</span><span class="sxs-lookup"><span data-stu-id="84354-p107">Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters.</span></span>|
|[<span data-ttu-id="84354-141">创建事件</span><span class="sxs-lookup"><span data-stu-id="84354-141">Create event</span></span>](../api/calendar-post-events.md) |[<span data-ttu-id="84354-142">事件</span><span class="sxs-lookup"><span data-stu-id="84354-142">event</span></span>](event.md)| <span data-ttu-id="84354-143">创建默认或指定的日历中的新事件。</span><span class="sxs-lookup"><span data-stu-id="84354-143">Create a new event in the default or specified calendar.</span></span>|
|[<span data-ttu-id="84354-144">findMeetingTimes</span><span class="sxs-lookup"><span data-stu-id="84354-144">findMeetingTimes</span></span>](../api/user-findmeetingtimes.md) |[<span data-ttu-id="84354-145">meetingTimeSuggestionsResult</span><span class="sxs-lookup"><span data-stu-id="84354-145">meetingTimeSuggestionsResult</span></span>](meetingtimesuggestionsresult.md) |<span data-ttu-id="84354-146">建议的会议时间内和基于组织者和与会者可用性和时间或位置的约束位置。</span><span class="sxs-lookup"><span data-stu-id="84354-146">Suggest meeting times and locations based on organizer and attendee availability, and time or location constraints.</span></span> |
|[<span data-ttu-id="84354-147">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="84354-147">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="84354-148">日历</span><span class="sxs-lookup"><span data-stu-id="84354-148">calendar</span></span>](calendar.md)  |<span data-ttu-id="84354-149">在新建或现有日历中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="84354-149">Create one or more single-value extended properties in a new or existing calendar.</span></span>   |
|[<span data-ttu-id="84354-150">获取包含单值扩展属性的日历</span><span class="sxs-lookup"><span data-stu-id="84354-150">Get calendar with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="84354-151">日历</span><span class="sxs-lookup"><span data-stu-id="84354-151">calendar</span></span>](calendar.md) | <span data-ttu-id="84354-152">通过使用 `$expand` 或 `$filter` 获取包含一个单值扩展属性的日历。</span><span class="sxs-lookup"><span data-stu-id="84354-152">Get calendars that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="84354-153">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="84354-153">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="84354-154">日历</span><span class="sxs-lookup"><span data-stu-id="84354-154">calendar</span></span>](calendar.md) | <span data-ttu-id="84354-155">在新建或现有的日历中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="84354-155">Create one or more multi-value extended properties in a new or existing calendar.</span></span>  |
|[<span data-ttu-id="84354-156">获取包含多值扩展属性的日历</span><span class="sxs-lookup"><span data-stu-id="84354-156">Get calendar with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="84354-157">日历</span><span class="sxs-lookup"><span data-stu-id="84354-157">calendar</span></span>](calendar.md) | <span data-ttu-id="84354-158">使用 `$expand` 获取包含一个多值扩展属性的日历。</span><span class="sxs-lookup"><span data-stu-id="84354-158">Get a calendar that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="84354-159">属性</span><span class="sxs-lookup"><span data-stu-id="84354-159">Properties</span></span>
| <span data-ttu-id="84354-160">属性</span><span class="sxs-lookup"><span data-stu-id="84354-160">Property</span></span>     | <span data-ttu-id="84354-161">类型</span><span class="sxs-lookup"><span data-stu-id="84354-161">Type</span></span>   |<span data-ttu-id="84354-162">说明</span><span class="sxs-lookup"><span data-stu-id="84354-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="84354-163">canEdit</span><span class="sxs-lookup"><span data-stu-id="84354-163">canEdit</span></span> |<span data-ttu-id="84354-164">布尔</span><span class="sxs-lookup"><span data-stu-id="84354-164">Boolean</span></span> |<span data-ttu-id="84354-p108">如果用户可以写入日历则为 true，否则为 false。对于创建此日历的用户，此属性为 true。此属性对于共享日历并且授予写入访问权限的用户同样为 true。</span><span class="sxs-lookup"><span data-stu-id="84354-p108">True if the user can write to the calendar, false otherwise. This property is true for the user who created the calendar. This property is also true for a user who has been shared a calendar and granted write access.</span></span> |
|<span data-ttu-id="84354-168">canShare</span><span class="sxs-lookup"><span data-stu-id="84354-168">canShare</span></span> |<span data-ttu-id="84354-169">布尔</span><span class="sxs-lookup"><span data-stu-id="84354-169">Boolean</span></span> |<span data-ttu-id="84354-p109">如果用户有权共享日历则为 ture，否则为 false。只有创建日历的用户才可以进行共享。</span><span class="sxs-lookup"><span data-stu-id="84354-p109">True if the user has the permission to share the calendar, false otherwise. Only the user who created the calendar can share it.</span></span> |
|<span data-ttu-id="84354-172">canViewPrivateItems</span><span class="sxs-lookup"><span data-stu-id="84354-172">canViewPrivateItems</span></span> |<span data-ttu-id="84354-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="84354-173">Boolean</span></span> |<span data-ttu-id="84354-174">如果用户可以读取已标记为私有的日历项，则为 true，否则返回 false。</span><span class="sxs-lookup"><span data-stu-id="84354-174">True if the user can read calendar items that have been marked private, false otherwise.</span></span> |
|<span data-ttu-id="84354-175">changeKey</span><span class="sxs-lookup"><span data-stu-id="84354-175">changeKey</span></span>|<span data-ttu-id="84354-176">字符串</span><span class="sxs-lookup"><span data-stu-id="84354-176">String</span></span>|<span data-ttu-id="84354-p110">标识 calendar 对象的版本。每次日历更改时，changeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。只读。</span><span class="sxs-lookup"><span data-stu-id="84354-p110">Identifies the version of the calendar object. Every time the calendar is changed, changeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span>|
|<span data-ttu-id="84354-181">color</span><span class="sxs-lookup"><span data-stu-id="84354-181">color</span></span>|<span data-ttu-id="84354-182">calendarColor</span><span class="sxs-lookup"><span data-stu-id="84354-182">calendarColor</span></span>|<span data-ttu-id="84354-p111">在 UI 中指定将该日历与其他日历区分开来的颜色主题。属性值有：LightBlue=0、LightGreen=1、LightOrange=2、LightGray=3、LightYellow=4、LightTeal=5、LightPink=6、LightBrown=7、LightRed=8、MaxColor=9、Auto=-1</span><span class="sxs-lookup"><span data-stu-id="84354-p111">Specifies the color theme to distinguish the calendar from other calendars in a UI. The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span></span>|
|<span data-ttu-id="84354-185">id</span><span class="sxs-lookup"><span data-stu-id="84354-185">id</span></span>|<span data-ttu-id="84354-186">String</span><span class="sxs-lookup"><span data-stu-id="84354-186">String</span></span>|<span data-ttu-id="84354-p112">组的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="84354-p112">The group's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="84354-189">name</span><span class="sxs-lookup"><span data-stu-id="84354-189">name</span></span>|<span data-ttu-id="84354-190">String</span><span class="sxs-lookup"><span data-stu-id="84354-190">String</span></span>|<span data-ttu-id="84354-191">日历名称。</span><span class="sxs-lookup"><span data-stu-id="84354-191">The calendar name.</span></span>|
|<span data-ttu-id="84354-192">owner</span><span class="sxs-lookup"><span data-stu-id="84354-192">owner</span></span> |[<span data-ttu-id="84354-193">emailAddress</span><span class="sxs-lookup"><span data-stu-id="84354-193">emailAddress</span></span>](emailaddress.md) | <span data-ttu-id="84354-p113">如果设置，则表示创建或添加日历的用户。对于用户创建或添加的日历，将 **owner** 属性设置为用户。对于与用户共享的日历，将 **owner** 属性设置为与此用户共享该日历的人员。</span><span class="sxs-lookup"><span data-stu-id="84354-p113">If set, this represents the user who created or added the calendar. For a calendar that the user created or added, the **owner** property is set to the user. For a calendar shared with the user, the **owner** property is set to the person who shared that calendar with the user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="84354-197">关系</span><span class="sxs-lookup"><span data-stu-id="84354-197">Relationships</span></span>
| <span data-ttu-id="84354-198">关系</span><span class="sxs-lookup"><span data-stu-id="84354-198">Relationship</span></span> | <span data-ttu-id="84354-199">类型</span><span class="sxs-lookup"><span data-stu-id="84354-199">Type</span></span>   |<span data-ttu-id="84354-200">说明</span><span class="sxs-lookup"><span data-stu-id="84354-200">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="84354-201">calendarView</span><span class="sxs-lookup"><span data-stu-id="84354-201">calendarView</span></span>|<span data-ttu-id="84354-202">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="84354-202">[Event](event.md) collection</span></span>|<span data-ttu-id="84354-p114">日历的日历视图。导航属性。只读。</span><span class="sxs-lookup"><span data-stu-id="84354-p114">The calendar view for the calendar. Navigation property. Read-only.</span></span>|
|<span data-ttu-id="84354-206">events</span><span class="sxs-lookup"><span data-stu-id="84354-206">events</span></span>|<span data-ttu-id="84354-207">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="84354-207">[Event](event.md) collection</span></span>|<span data-ttu-id="84354-p115">日历中的事件。导航属性。只读。</span><span class="sxs-lookup"><span data-stu-id="84354-p115">The events in the calendar. Navigation property. Read-only.</span></span>|
|<span data-ttu-id="84354-211">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="84354-211">multiValueExtendedProperties</span></span>|<span data-ttu-id="84354-212">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="84354-212">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="84354-p116">为日历定义的多值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="84354-p116">The collection of multi-value extended properties defined for the calendar. Read-only. Nullable.</span></span>|
|<span data-ttu-id="84354-216">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="84354-216">singleValueExtendedProperties</span></span>|<span data-ttu-id="84354-217">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="84354-217">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="84354-p117">为日历定义的单值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="84354-p117">The collection of single-value extended properties defined for the calendar. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="84354-221">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="84354-221">JSON representation</span></span>

<span data-ttu-id="84354-222">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84354-222">Here is a JSON representation of the resource</span></span>

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
