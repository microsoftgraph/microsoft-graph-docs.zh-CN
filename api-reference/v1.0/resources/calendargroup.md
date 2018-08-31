# <a name="calendargroup-resource-type"></a><span data-ttu-id="1c944-101">calendarGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="1c944-101">calendarGroup resource type</span></span>

<span data-ttu-id="1c944-102">一组日历。</span><span class="sxs-lookup"><span data-stu-id="1c944-102">A group of calendars.</span></span>

## <a name="methods"></a><span data-ttu-id="1c944-103">方法</span><span class="sxs-lookup"><span data-stu-id="1c944-103">Methods</span></span>

| <span data-ttu-id="1c944-104">方法</span><span class="sxs-lookup"><span data-stu-id="1c944-104">Method</span></span>                                                      | <span data-ttu-id="1c944-105">返回类型</span><span class="sxs-lookup"><span data-stu-id="1c944-105">Return Type</span></span>                        | <span data-ttu-id="1c944-106">说明</span><span class="sxs-lookup"><span data-stu-id="1c944-106">Description</span></span>                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [<span data-ttu-id="1c944-107">列出日历组</span><span class="sxs-lookup"><span data-stu-id="1c944-107">List calendar groups</span></span>](../api/user_list_calendargroups.md)  | <span data-ttu-id="1c944-108">[日历](calendar.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1c944-108">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="1c944-109">获取用户的日历组。</span><span class="sxs-lookup"><span data-stu-id="1c944-109">Get the user's calendar groups.</span></span>                               |
| [<span data-ttu-id="1c944-110">创建日历组</span><span class="sxs-lookup"><span data-stu-id="1c944-110">Create calendar group</span></span>](../api/user_post_calendargroups.md) | [<span data-ttu-id="1c944-111">日历</span><span class="sxs-lookup"><span data-stu-id="1c944-111">Calendar</span></span>](calendar.md)            | <span data-ttu-id="1c944-112">创建新的日历组。</span><span class="sxs-lookup"><span data-stu-id="1c944-112">Create a new calendar group.</span></span>                                  |
| [<span data-ttu-id="1c944-113">创建日历组</span><span class="sxs-lookup"><span data-stu-id="1c944-113">Get calendar group</span></span>](../api/calendargroup_get.md)           | [<span data-ttu-id="1c944-114">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="1c944-114">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="1c944-115">读取 calendar 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1c944-115">Read properties and relationships of a calendar group object.</span></span> |
| [<span data-ttu-id="1c944-116">更新</span><span class="sxs-lookup"><span data-stu-id="1c944-116">Update</span></span>](../api/calendargroup_update.md)                    | [<span data-ttu-id="1c944-117">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="1c944-117">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="1c944-118">更新 calendarGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="1c944-118">Update calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="1c944-119">删除</span><span class="sxs-lookup"><span data-stu-id="1c944-119">Delete</span></span>](../api/calendargroup_delete.md)                    | <span data-ttu-id="1c944-120">无</span><span class="sxs-lookup"><span data-stu-id="1c944-120">None</span></span>                               | <span data-ttu-id="1c944-121">删除 calendarGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="1c944-121">Delete calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="1c944-122">列出日历</span><span class="sxs-lookup"><span data-stu-id="1c944-122">List calendars</span></span>](../api/calendargroup_list_calendars.md)    | <span data-ttu-id="1c944-123">[日历](calendar.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1c944-123">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="1c944-124">列出日历组中的日历。</span><span class="sxs-lookup"><span data-stu-id="1c944-124">List calendars in a calendar group.</span></span>                           |
| [<span data-ttu-id="1c944-125">创建日历</span><span class="sxs-lookup"><span data-stu-id="1c944-125">Create Calendar</span></span>](../api/calendargroup_post_calendars.md)   | [<span data-ttu-id="1c944-126">日历</span><span class="sxs-lookup"><span data-stu-id="1c944-126">Calendar</span></span>](calendar.md)            | <span data-ttu-id="1c944-127">在日历组中创建新日历。</span><span class="sxs-lookup"><span data-stu-id="1c944-127">Create a new Calendar in a calendar group.</span></span>                    |

## <a name="properties"></a><span data-ttu-id="1c944-128">属性</span><span class="sxs-lookup"><span data-stu-id="1c944-128">Properties</span></span>

| <span data-ttu-id="1c944-129">属性</span><span class="sxs-lookup"><span data-stu-id="1c944-129">Property</span></span>  | <span data-ttu-id="1c944-130">类型</span><span class="sxs-lookup"><span data-stu-id="1c944-130">Type</span></span>   | <span data-ttu-id="1c944-131">说明</span><span class="sxs-lookup"><span data-stu-id="1c944-131">Description</span></span>                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="1c944-132">名称</span><span class="sxs-lookup"><span data-stu-id="1c944-132">name</span></span>      | <span data-ttu-id="1c944-133">字符串</span><span class="sxs-lookup"><span data-stu-id="1c944-133">String</span></span> | <span data-ttu-id="1c944-134">组名称。</span><span class="sxs-lookup"><span data-stu-id="1c944-134">The group name.</span></span>                                                                                                                                                                                           |
| <span data-ttu-id="1c944-135">changeKey</span><span class="sxs-lookup"><span data-stu-id="1c944-135">changeKey</span></span> | <span data-ttu-id="1c944-136">字符串</span><span class="sxs-lookup"><span data-stu-id="1c944-136">String</span></span> | <span data-ttu-id="1c944-p101">标识日历组的版本。每次日历组更改时，ChangeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。只读。</span><span class="sxs-lookup"><span data-stu-id="1c944-p101">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span> |
| <span data-ttu-id="1c944-141">classId</span><span class="sxs-lookup"><span data-stu-id="1c944-141">classId</span></span>   | <span data-ttu-id="1c944-142">全局唯一标识符</span><span class="sxs-lookup"><span data-stu-id="1c944-142">Guid</span></span>   | <span data-ttu-id="1c944-p102">类标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="1c944-p102">The class identifier. Read-only.</span></span>                                                                                                                                                                          |
| <span data-ttu-id="1c944-145">ID</span><span class="sxs-lookup"><span data-stu-id="1c944-145">id</span></span>        | <span data-ttu-id="1c944-146">字符串</span><span class="sxs-lookup"><span data-stu-id="1c944-146">String</span></span> | <span data-ttu-id="1c944-p103">组的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="1c944-p103">The group's unique identifier. Read-only.</span></span>                                                                                                                                                                 |

## <a name="relationships"></a><span data-ttu-id="1c944-149">关系</span><span class="sxs-lookup"><span data-stu-id="1c944-149">Relationships</span></span>

| <span data-ttu-id="1c944-150">关系</span><span class="sxs-lookup"><span data-stu-id="1c944-150">Relationship</span></span> | <span data-ttu-id="1c944-151">类型</span><span class="sxs-lookup"><span data-stu-id="1c944-151">Type</span></span>                               | <span data-ttu-id="1c944-152">说明</span><span class="sxs-lookup"><span data-stu-id="1c944-152">Description</span></span>                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="1c944-153">日历</span><span class="sxs-lookup"><span data-stu-id="1c944-153">calendars</span></span>    | <span data-ttu-id="1c944-154">[日历](calendar.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1c944-154">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="1c944-p104">日历组中的日历。导航属性。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="1c944-p104">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1c944-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1c944-159">JSON representation</span></span>

<span data-ttu-id="1c944-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1c944-160">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "calendars"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.calendarGroup",
  "@odata.annotations": [
    {
      "property": "calendars",
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
