# <a name="calendar-resource-type"></a><span data-ttu-id="b4a6d-101">日历资源类型</span><span class="sxs-lookup"><span data-stu-id="b4a6d-101">calendar resource type</span></span>

<span data-ttu-id="b4a6d-102">日历即事件容器。</span><span class="sxs-lookup"><span data-stu-id="b4a6d-102">A calendar which is a container for events.</span></span> <span data-ttu-id="b4a6d-103">可以是[用户](user.md)的日历，也可以是 Office 365 [组](group.md)的默认日历。</span><span class="sxs-lookup"><span data-stu-id="b4a6d-103">It can be a calendar for a [user](user.md), or the default calendar of an Office 365 [group](group.md).</span></span>

> <span data-ttu-id="b4a6d-104">**注意：** 可以与用户日历和群组日历进行交互的方式有一些细微差异：</span><span class="sxs-lookup"><span data-stu-id="b4a6d-104">**Note:** There are a few minor differences in the way you can interact with user calendars and group calendars:</span></span>

 - <span data-ttu-id="b4a6d-105">你可以仅整理 [calendarGroup](calendargroup.md) 中的用户日历。</span><span class="sxs-lookup"><span data-stu-id="b4a6d-105">You can organize only user calendars in a [calendarGroup](calendargroup.md).</span></span>
 - <span data-ttu-id="b4a6d-106">Outlook 可代表组自动接受所有会议请求。</span><span class="sxs-lookup"><span data-stu-id="b4a6d-106">Outlook automatically accepts all meeting requests on behalf of groups.</span></span> <span data-ttu-id="b4a6d-107">你可以仅为用户日历[接受](../api/event_accept.md)、[暂时接受](../api/event_tentativelyaccept.md)或[拒绝](../api/event_decline.md)会议请求。</span><span class="sxs-lookup"><span data-stu-id="b4a6d-107">You can [accept](../api/event_accept.md), [tentatively accept](../api/event_tentativelyaccept.md), or [decline](../api/event_decline.md)  meeting requests for user calendars only.</span></span>
  - <span data-ttu-id="b4a6d-108">Outlook 不支持为群组事件的提醒。</span><span class="sxs-lookup"><span data-stu-id="b4a6d-108">Outlook doesn't support reminders for group events.</span></span> <span data-ttu-id="b4a6d-109">你可以仅[暂停](../api/event_snoozereminder.md)或[消除](../api/event_dismissreminder.md)用户日历的[提醒](reminder.md)。</span><span class="sxs-lookup"><span data-stu-id="b4a6d-109">You can [snooze](../api/event_snoozereminder.md) or [dismiss](../api/event_dismissreminder.md) a [reminder](reminder.md) for user calendars only.</span></span>

## <a name="methods"></a><span data-ttu-id="b4a6d-110">方法</span><span class="sxs-lookup"><span data-stu-id="b4a6d-110">Methods</span></span>

| <span data-ttu-id="b4a6d-111">方法</span><span class="sxs-lookup"><span data-stu-id="b4a6d-111">Method</span></span>       | <span data-ttu-id="b4a6d-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="b4a6d-112">Return Type</span></span>  |<span data-ttu-id="b4a6d-113">说明</span><span class="sxs-lookup"><span data-stu-id="b4a6d-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b4a6d-114">列出日历</span><span class="sxs-lookup"><span data-stu-id="b4a6d-114">List calendars</span></span>](../api/user_list_calendars.md)|<span data-ttu-id="b4a6d-115">[日历](calendar.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b4a6d-115">[calendar](calendar.md) collection</span></span>|<span data-ttu-id="b4a6d-116">获取所有用户的日历，或者获取默认或其他特定日历组中的日历。</span><span class="sxs-lookup"><span data-stu-id="b4a6d-116">Get all the user's calendars, or the calendars in the default or other specific calendar group.</span></span>|
|[<span data-ttu-id="b4a6d-117">创建日历</span><span class="sxs-lookup"><span data-stu-id="b4a6d-117">Create calendar</span></span>](../api/user_post_calendars.md) |[<span data-ttu-id="b4a6d-118">日历</span><span class="sxs-lookup"><span data-stu-id="b4a6d-118">calendar</span></span>](calendar.md)| <span data-ttu-id="b4a6d-119">在默认日历组或用户的指定日历组中新建日历。</span><span class="sxs-lookup"><span data-stu-id="b4a6d-119">Create a new calendar in the default calendar group or specified calendar group for a user.</span></span>|
|[<span data-ttu-id="b4a6d-120">获取日历</span><span class="sxs-lookup"><span data-stu-id="b4a6d-120">Get calendar</span></span>](../api/calendar_get.md) | [<span data-ttu-id="b4a6d-121">日历</span><span class="sxs-lookup"><span data-stu-id="b4a6d-121">calendar</span></span>](calendar.md) |<span data-ttu-id="b4a6d-122">获取 **calendar** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b4a6d-122">Get the properties and relationships of a **calendar** object.</span></span> <span data-ttu-id="b4a6d-123">可以是用户的日历，也可以是 Office 365 组的默认日历。</span><span class="sxs-lookup"><span data-stu-id="b4a6d-123">The calendar can be one for a user, or the default calendar of an Office 365 group.</span></span> |
|[<span data-ttu-id="b4a6d-124">更新</span><span class="sxs-lookup"><span data-stu-id="b4a6d-124">Update</span></span>](../api/calendar_update.md) | [<span data-ttu-id="b4a6d-125">日历</span><span class="sxs-lookup"><span data-stu-id="b4a6d-125">calendar</span></span>](calendar.md)  |<span data-ttu-id="b4a6d-126">更新 **calendar** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b4a6d-126">Update the properties of a **calendar** object.</span></span> <span data-ttu-id="b4a6d-127">可以是用户的日历，也可以是 Office 365 组的默认日历。</span><span class="sxs-lookup"><span data-stu-id="b4a6d-127">The calendar can be one for a user, or the default calendar of an Office 365 group.</span></span> |
|[<span data-ttu-id="b4a6d-128">删除</span><span class="sxs-lookup"><span data-stu-id="b4a6d-128">Delete</span></span>](../api/calendar_delete.md) | <span data-ttu-id="b4a6d-129">无</span><span class="sxs-lookup"><span data-stu-id="b4a6d-129">None</span></span> |<span data-ttu-id="b4a6d-130">删除 calendar 对象。</span><span class="sxs-lookup"><span data-stu-id="b4a6d-130">Delete calendar object.</span></span> |
|[<span data-ttu-id="b4a6d-131">列出 calendarView</span><span class="sxs-lookup"><span data-stu-id="b4a6d-131">List calendarView</span></span>](../api/calendar_list_calendarview.md) |<span data-ttu-id="b4a6d-132">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b4a6d-132">[event](event.md) collection</span></span>| <span data-ttu-id="b4a6d-133">从用户的主日历 `(../me/calendarview)` 或指定日历中，获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例。</span><span class="sxs-lookup"><span data-stu-id="b4a6d-133">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's primary calendar `(../me/calendarview)` or from a specified calendar.</span></span>|
|[<span data-ttu-id="b4a6d-134">列出事件</span><span class="sxs-lookup"><span data-stu-id="b4a6d-134">List events</span></span>](../api/calendar_list_events.md) |<span data-ttu-id="b4a6d-135">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b4a6d-135">[event](event.md) collection</span></span>| <span data-ttu-id="b4a6d-p106">检索日历中的事件列表。该列表包含单个实例会议和系列主控形状。</span><span class="sxs-lookup"><span data-stu-id="b4a6d-p106">Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters.</span></span>|
|[<span data-ttu-id="b4a6d-138">创建事件</span><span class="sxs-lookup"><span data-stu-id="b4a6d-138">Create Event</span></span>](../api/calendar_post_events.md) |[<span data-ttu-id="b4a6d-139">事件</span><span class="sxs-lookup"><span data-stu-id="b4a6d-139">event</span></span>](event.md)| <span data-ttu-id="b4a6d-140">在默认或指定日历中创建新事件。</span><span class="sxs-lookup"><span data-stu-id="b4a6d-140">Create a new Event in the default or specified calendar.</span></span>|
|[<span data-ttu-id="b4a6d-141">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="b4a6d-141">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[<span data-ttu-id="b4a6d-142">日历</span><span class="sxs-lookup"><span data-stu-id="b4a6d-142">calendar</span></span>](calendar.md)  |<span data-ttu-id="b4a6d-143">在新建或现有日历中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="b4a6d-143">Create one or more single-value extended properties in a new or existing calendar.</span></span>   |
|[<span data-ttu-id="b4a6d-144">获取包含单值扩展属性的日历</span><span class="sxs-lookup"><span data-stu-id="b4a6d-144">Get calendar with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="b4a6d-145">日历</span><span class="sxs-lookup"><span data-stu-id="b4a6d-145">calendar</span></span>](calendar.md) | <span data-ttu-id="b4a6d-146">通过使用 `$expand` 或 `$filter` 获取包含一个单值扩展属性的日历。</span><span class="sxs-lookup"><span data-stu-id="b4a6d-146">Get calendars that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="b4a6d-147">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="b4a6d-147">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [<span data-ttu-id="b4a6d-148">日历</span><span class="sxs-lookup"><span data-stu-id="b4a6d-148">calendar</span></span>](calendar.md) | <span data-ttu-id="b4a6d-149">在新建或现有的日历中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="b4a6d-149">Create one or more multi-value extended properties in a new or existing calendar.</span></span>  |
|[<span data-ttu-id="b4a6d-150">获取包含多值扩展属性的日历</span><span class="sxs-lookup"><span data-stu-id="b4a6d-150">Get calendar with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="b4a6d-151">日历</span><span class="sxs-lookup"><span data-stu-id="b4a6d-151">calendar</span></span>](calendar.md) | <span data-ttu-id="b4a6d-152">使用 `$expand` 获取包含一个多值扩展属性的日历。</span><span class="sxs-lookup"><span data-stu-id="b4a6d-152">Get a calendar that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="b4a6d-153">属性</span><span class="sxs-lookup"><span data-stu-id="b4a6d-153">Properties</span></span>
| <span data-ttu-id="b4a6d-154">属性</span><span class="sxs-lookup"><span data-stu-id="b4a6d-154">Property</span></span>     | <span data-ttu-id="b4a6d-155">类型</span><span class="sxs-lookup"><span data-stu-id="b4a6d-155">Type</span></span>   |<span data-ttu-id="b4a6d-156">说明</span><span class="sxs-lookup"><span data-stu-id="b4a6d-156">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b4a6d-157">canEdit</span><span class="sxs-lookup"><span data-stu-id="b4a6d-157">canEdit</span></span> |<span data-ttu-id="b4a6d-158">布尔值</span><span class="sxs-lookup"><span data-stu-id="b4a6d-158">Boolean</span></span> |<span data-ttu-id="b4a6d-p107">如果用户可以写入日历则为 true，否则为 false。对于创建此日历的用户，此属性为 true。此属性对于共享日历并且授予写入访问权限的用户同样为 true。</span><span class="sxs-lookup"><span data-stu-id="b4a6d-p107">True if the user can write to the calendar, false otherwise. This property is true for the user who created the calendar. This property is also true for a user who has been shared a calendar and granted write access.</span></span> |
|<span data-ttu-id="b4a6d-162">canShare</span><span class="sxs-lookup"><span data-stu-id="b4a6d-162">canShare</span></span> |<span data-ttu-id="b4a6d-163">布尔值</span><span class="sxs-lookup"><span data-stu-id="b4a6d-163">Boolean</span></span> |<span data-ttu-id="b4a6d-p108">如果用户有权共享日历则为 ture，否则为 false。只有创建日历的用户才可以进行共享。</span><span class="sxs-lookup"><span data-stu-id="b4a6d-p108">True if the user has the permission to share the calendar, false otherwise. Only the user who created the calendar can share it.</span></span> |
|<span data-ttu-id="b4a6d-166">canViewPrivateItems</span><span class="sxs-lookup"><span data-stu-id="b4a6d-166">canViewPrivateItems</span></span> |<span data-ttu-id="b4a6d-167">布尔值</span><span class="sxs-lookup"><span data-stu-id="b4a6d-167">Boolean</span></span> |<span data-ttu-id="b4a6d-168">如果用户可以读取已标记为私有的日历项，则为 true，否则返回 false。</span><span class="sxs-lookup"><span data-stu-id="b4a6d-168">True if the user can read calendar items that have been marked private, false otherwise.</span></span> |
|<span data-ttu-id="b4a6d-169">changeKey</span><span class="sxs-lookup"><span data-stu-id="b4a6d-169">changeKey</span></span>|<span data-ttu-id="b4a6d-170">字符串</span><span class="sxs-lookup"><span data-stu-id="b4a6d-170">String</span></span>|<span data-ttu-id="b4a6d-p109">标识 calendar 对象的版本。每次日历更改时，changeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。只读。</span><span class="sxs-lookup"><span data-stu-id="b4a6d-p109">Identifies the version of the calendar object. Every time the calendar is changed, changeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span>|
|<span data-ttu-id="b4a6d-175">颜色</span><span class="sxs-lookup"><span data-stu-id="b4a6d-175">color</span></span>|<span data-ttu-id="b4a6d-176">calendarColor</span><span class="sxs-lookup"><span data-stu-id="b4a6d-176">CalendarColor</span></span>|<span data-ttu-id="b4a6d-p110">在 UI 中指定将该日历与其他日历区分开来的颜色主题。属性值有：LightBlue=0、LightGreen=1、LightOrange=2、LightGray=3、LightYellow=4、LightTeal=5、LightPink=6、LightBrown=7、LightRed=8、MaxColor=9、Auto=-1</span><span class="sxs-lookup"><span data-stu-id="b4a6d-p110">Specifies the color theme to distinguish the calendar from other calendars in a UI. The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span></span>|
|<span data-ttu-id="b4a6d-179">ID</span><span class="sxs-lookup"><span data-stu-id="b4a6d-179">id</span></span>|<span data-ttu-id="b4a6d-180">字符串</span><span class="sxs-lookup"><span data-stu-id="b4a6d-180">String</span></span>|<span data-ttu-id="b4a6d-p111">组的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="b4a6d-p111">The group's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="b4a6d-183">名称</span><span class="sxs-lookup"><span data-stu-id="b4a6d-183">name</span></span>|<span data-ttu-id="b4a6d-184">字符串</span><span class="sxs-lookup"><span data-stu-id="b4a6d-184">String</span></span>|<span data-ttu-id="b4a6d-185">日历名称。</span><span class="sxs-lookup"><span data-stu-id="b4a6d-185">The calendar name.</span></span>|
|<span data-ttu-id="b4a6d-186">负责人</span><span class="sxs-lookup"><span data-stu-id="b4a6d-186">owner</span></span> |[<span data-ttu-id="b4a6d-187">emailAddress</span><span class="sxs-lookup"><span data-stu-id="b4a6d-187">emailAddress</span></span>](emailaddress.md) | <span data-ttu-id="b4a6d-p112">如果设置，则表示创建或添加日历的用户。对于用户创建或添加的日历，将 **owner** 属性设置为用户。对于与用户共享的日历，将 **owner** 属性设置为与此用户共享该日历的人员。</span><span class="sxs-lookup"><span data-stu-id="b4a6d-p112">If set, this represents the user who created or added the calendar. For a calendar that the user created or added, the **owner** property is set to the user. For a calendar shared with the user, the **owner** property is set to the person who shared that calendar with the user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b4a6d-191">关系</span><span class="sxs-lookup"><span data-stu-id="b4a6d-191">Relationships</span></span>
| <span data-ttu-id="b4a6d-192">关系</span><span class="sxs-lookup"><span data-stu-id="b4a6d-192">Relationship</span></span> | <span data-ttu-id="b4a6d-193">类型</span><span class="sxs-lookup"><span data-stu-id="b4a6d-193">Type</span></span>   |<span data-ttu-id="b4a6d-194">说明</span><span class="sxs-lookup"><span data-stu-id="b4a6d-194">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b4a6d-195">calendarView</span><span class="sxs-lookup"><span data-stu-id="b4a6d-195">calendarView</span></span>|<span data-ttu-id="b4a6d-196">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b4a6d-196">[Event](event.md) collection</span></span>|<span data-ttu-id="b4a6d-p113">日历的日历视图。导航属性。只读。</span><span class="sxs-lookup"><span data-stu-id="b4a6d-p113">The calendar view for the calendar. Navigation property. Read-only.</span></span>|
|<span data-ttu-id="b4a6d-200">事件</span><span class="sxs-lookup"><span data-stu-id="b4a6d-200">events</span></span>|<span data-ttu-id="b4a6d-201">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b4a6d-201">[Event](event.md) collection</span></span>|<span data-ttu-id="b4a6d-p114">日历中的事件。导航属性。只读。</span><span class="sxs-lookup"><span data-stu-id="b4a6d-p114">The events in the calendar. Navigation property. Read-only.</span></span>|
|<span data-ttu-id="b4a6d-205">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="b4a6d-205">multiValueExtendedProperties</span></span>|<span data-ttu-id="b4a6d-206">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b4a6d-206">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="b4a6d-p115">为日历定义的多值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="b4a6d-p115">The collection of multi-value extended properties defined for the calendar. Read-only. Nullable.</span></span>|
|<span data-ttu-id="b4a6d-210">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="b4a6d-210">singleValueExtendedProperties</span></span>|<span data-ttu-id="b4a6d-211">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b4a6d-211">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="b4a6d-p116">为日历定义的单值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="b4a6d-p116">The collection of single-value extended properties defined for the calendar. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b4a6d-215">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b4a6d-215">JSON representation</span></span>

<span data-ttu-id="b4a6d-216">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b4a6d-216">Here is a JSON representation of the resource</span></span>

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
