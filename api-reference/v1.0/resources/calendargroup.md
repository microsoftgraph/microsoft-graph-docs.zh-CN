# <a name="calendargroup-resource-type"></a><span data-ttu-id="b53b3-101">calendarGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="b53b3-101">calendarGroup resource type</span></span>

<span data-ttu-id="b53b3-102">一组日历。</span><span class="sxs-lookup"><span data-stu-id="b53b3-102">A group of calendars.</span></span>

<span data-ttu-id="b53b3-p101">**注意** Outlook.com 仅支持可通过 /me/calendars 快捷方式访问的默认日历组。无法删除该日历组。</span><span class="sxs-lookup"><span data-stu-id="b53b3-p101">**Note** Outlook.com supports only the default calendar group which is accessible by the ../me/calendars shortcut. You cannot delete that calendar group.</span></span>

## <a name="methods"></a><span data-ttu-id="b53b3-105">方法</span><span class="sxs-lookup"><span data-stu-id="b53b3-105">Methods</span></span>

| <span data-ttu-id="b53b3-106">方法</span><span class="sxs-lookup"><span data-stu-id="b53b3-106">Method</span></span>       | <span data-ttu-id="b53b3-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="b53b3-107">Return Type</span></span>  |<span data-ttu-id="b53b3-108">说明</span><span class="sxs-lookup"><span data-stu-id="b53b3-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b53b3-109">列出日历组</span><span class="sxs-lookup"><span data-stu-id="b53b3-109">List calendar groups</span></span>](../api/user_list_calendargroups.md) |<span data-ttu-id="b53b3-110">[日历](calendar.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b53b3-110">[Calendar](calendar.md) collection</span></span>| <span data-ttu-id="b53b3-111">获取用户的日历组。</span><span class="sxs-lookup"><span data-stu-id="b53b3-111">Get the user's calendar groups.</span></span>|
|[<span data-ttu-id="b53b3-112">创建日历组</span><span class="sxs-lookup"><span data-stu-id="b53b3-112">Create calendar group</span></span>](../api/user_post_calendargroups.md) |[<span data-ttu-id="b53b3-113">日历</span><span class="sxs-lookup"><span data-stu-id="b53b3-113">Calendar</span></span>](calendar.md)| <span data-ttu-id="b53b3-114">创建新的日历组。</span><span class="sxs-lookup"><span data-stu-id="b53b3-114">Create a new calendar group.</span></span>|
|[<span data-ttu-id="b53b3-115">创建日历组</span><span class="sxs-lookup"><span data-stu-id="b53b3-115">Get calendar group</span></span>](../api/calendargroup_get.md) | [<span data-ttu-id="b53b3-116">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="b53b3-116">calendarGroup</span></span>](calendargroup.md) |<span data-ttu-id="b53b3-117">读取 calendar 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b53b3-117">Read properties and relationships of a calendar group object.</span></span>|
|[<span data-ttu-id="b53b3-118">更新</span><span class="sxs-lookup"><span data-stu-id="b53b3-118">Update</span></span>](../api/calendargroup_update.md) | [<span data-ttu-id="b53b3-119">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="b53b3-119">calendarGroup</span></span>](calendargroup.md) |<span data-ttu-id="b53b3-120">更新 calendarGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="b53b3-120">Update calendarGroup object.</span></span> |
|[<span data-ttu-id="b53b3-121">删除</span><span class="sxs-lookup"><span data-stu-id="b53b3-121">Delete</span></span>](../api/calendargroup_delete.md) | <span data-ttu-id="b53b3-122">无</span><span class="sxs-lookup"><span data-stu-id="b53b3-122">None</span></span> |<span data-ttu-id="b53b3-123">删除 calendarGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="b53b3-123">Delete calendarGroup object.</span></span> |
|[<span data-ttu-id="b53b3-124">列出日历</span><span class="sxs-lookup"><span data-stu-id="b53b3-124">List calendars</span></span>](../api/calendargroup_list_calendars.md) |<span data-ttu-id="b53b3-125">[日历](calendar.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b53b3-125">[Calendar](calendar.md) collection</span></span>| <span data-ttu-id="b53b3-126">列出日历组中的日历。</span><span class="sxs-lookup"><span data-stu-id="b53b3-126">List calendars in a calendar group.</span></span>|
|[<span data-ttu-id="b53b3-127">创建日历</span><span class="sxs-lookup"><span data-stu-id="b53b3-127">Create Calendar</span></span>](../api/calendargroup_post_calendars.md) |[<span data-ttu-id="b53b3-128">日历</span><span class="sxs-lookup"><span data-stu-id="b53b3-128">Calendar</span></span>](calendar.md)| <span data-ttu-id="b53b3-129">在日历组中创建新日历。</span><span class="sxs-lookup"><span data-stu-id="b53b3-129">Create a new Calendar in a calendar group.</span></span>|

## <a name="properties"></a><span data-ttu-id="b53b3-130">属性</span><span class="sxs-lookup"><span data-stu-id="b53b3-130">Properties</span></span>
| <span data-ttu-id="b53b3-131">属性</span><span class="sxs-lookup"><span data-stu-id="b53b3-131">Property</span></span>     | <span data-ttu-id="b53b3-132">类型</span><span class="sxs-lookup"><span data-stu-id="b53b3-132">Type</span></span>   |<span data-ttu-id="b53b3-133">说明</span><span class="sxs-lookup"><span data-stu-id="b53b3-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b53b3-134">名称</span><span class="sxs-lookup"><span data-stu-id="b53b3-134">name</span></span>|<span data-ttu-id="b53b3-135">String</span><span class="sxs-lookup"><span data-stu-id="b53b3-135">String</span></span>|<span data-ttu-id="b53b3-136">组名称。</span><span class="sxs-lookup"><span data-stu-id="b53b3-136">The group name.</span></span>|
|<span data-ttu-id="b53b3-137">changeKey</span><span class="sxs-lookup"><span data-stu-id="b53b3-137">changeKey</span></span>|<span data-ttu-id="b53b3-138">String</span><span class="sxs-lookup"><span data-stu-id="b53b3-138">String</span></span>|<span data-ttu-id="b53b3-p102">标识日历组的版本。每次日历组更改时，ChangeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。只读。</span><span class="sxs-lookup"><span data-stu-id="b53b3-p102">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span>|
|<span data-ttu-id="b53b3-143">classId</span><span class="sxs-lookup"><span data-stu-id="b53b3-143">classId</span></span>|<span data-ttu-id="b53b3-144">Guid</span><span class="sxs-lookup"><span data-stu-id="b53b3-144">Guid</span></span>|<span data-ttu-id="b53b3-p103">类标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="b53b3-p103">The class identifier. Read-only.</span></span>|
|<span data-ttu-id="b53b3-147">id</span><span class="sxs-lookup"><span data-stu-id="b53b3-147">id</span></span>|<span data-ttu-id="b53b3-148">String</span><span class="sxs-lookup"><span data-stu-id="b53b3-148">String</span></span>|<span data-ttu-id="b53b3-p104">组的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="b53b3-p104">The group's unique identifier. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b53b3-151">关系</span><span class="sxs-lookup"><span data-stu-id="b53b3-151">Relationships</span></span>
| <span data-ttu-id="b53b3-152">关系</span><span class="sxs-lookup"><span data-stu-id="b53b3-152">Relationship</span></span> | <span data-ttu-id="b53b3-153">类型</span><span class="sxs-lookup"><span data-stu-id="b53b3-153">Type</span></span>   |<span data-ttu-id="b53b3-154">说明</span><span class="sxs-lookup"><span data-stu-id="b53b3-154">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b53b3-155">日历</span><span class="sxs-lookup"><span data-stu-id="b53b3-155">calendars</span></span>|<span data-ttu-id="b53b3-156">[日历](calendar.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b53b3-156">[Calendar](calendar.md) collection</span></span>|<span data-ttu-id="b53b3-p105">日历组中的日历。导航属性。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="b53b3-p105">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b53b3-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b53b3-161">JSON representation</span></span>

<span data-ttu-id="b53b3-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b53b3-162">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "calendars"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.calendarGroup"
}-->

```json
{
  "changeKey": "string",
  "classId": "guid",
  "id": "string (identifier)",
  "name": "string"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "calendarGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
