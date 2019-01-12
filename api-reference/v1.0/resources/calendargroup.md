---
title: calendarGroup 资源类型
description: 一组的用户日历。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5b75ebf253276876129859be7d37ecb6748fc0d9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949624"
---
# <a name="calendargroup-resource-type"></a><span data-ttu-id="999ef-103">calendarGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="999ef-103">calendarGroup resource type</span></span>

<span data-ttu-id="999ef-104">一组的用户日历。</span><span class="sxs-lookup"><span data-stu-id="999ef-104">A group of user calendars.</span></span>

## <a name="methods"></a><span data-ttu-id="999ef-105">方法</span><span class="sxs-lookup"><span data-stu-id="999ef-105">Methods</span></span>

| <span data-ttu-id="999ef-106">方法</span><span class="sxs-lookup"><span data-stu-id="999ef-106">Method</span></span>                                                      | <span data-ttu-id="999ef-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="999ef-107">Return Type</span></span>                        | <span data-ttu-id="999ef-108">说明</span><span class="sxs-lookup"><span data-stu-id="999ef-108">Description</span></span>                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [<span data-ttu-id="999ef-109">列出日历组</span><span class="sxs-lookup"><span data-stu-id="999ef-109">List calendar groups</span></span>](../api/user-list-calendargroups.md)  | <span data-ttu-id="999ef-110">[日历](calendar.md) 集合</span><span class="sxs-lookup"><span data-stu-id="999ef-110">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="999ef-111">获取用户的日历组。</span><span class="sxs-lookup"><span data-stu-id="999ef-111">Get the user's calendar groups.</span></span>                               |
| [<span data-ttu-id="999ef-112">创建日历组</span><span class="sxs-lookup"><span data-stu-id="999ef-112">Create calendar group</span></span>](../api/user-post-calendargroups.md) | [<span data-ttu-id="999ef-113">日历</span><span class="sxs-lookup"><span data-stu-id="999ef-113">Calendar</span></span>](calendar.md)            | <span data-ttu-id="999ef-114">创建新的日历组。</span><span class="sxs-lookup"><span data-stu-id="999ef-114">Create a new calendar group.</span></span>                                  |
| [<span data-ttu-id="999ef-115">创建日历组</span><span class="sxs-lookup"><span data-stu-id="999ef-115">Get calendar group</span></span>](../api/calendargroup-get.md)           | [<span data-ttu-id="999ef-116">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="999ef-116">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="999ef-117">读取 calendar 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="999ef-117">Read properties and relationships of a calendar group object.</span></span> |
| [<span data-ttu-id="999ef-118">更新</span><span class="sxs-lookup"><span data-stu-id="999ef-118">Update</span></span>](../api/calendargroup-update.md)                    | [<span data-ttu-id="999ef-119">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="999ef-119">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="999ef-120">更新 calendarGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="999ef-120">Update calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="999ef-121">删除</span><span class="sxs-lookup"><span data-stu-id="999ef-121">Delete</span></span>](../api/calendargroup-delete.md)                    | <span data-ttu-id="999ef-122">无</span><span class="sxs-lookup"><span data-stu-id="999ef-122">None</span></span>                               | <span data-ttu-id="999ef-123">删除 calendarGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="999ef-123">Delete calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="999ef-124">列出日历</span><span class="sxs-lookup"><span data-stu-id="999ef-124">List calendars</span></span>](../api/calendargroup-list-calendars.md)    | <span data-ttu-id="999ef-125">[日历](calendar.md) 集合</span><span class="sxs-lookup"><span data-stu-id="999ef-125">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="999ef-126">列出日历组中的日历。</span><span class="sxs-lookup"><span data-stu-id="999ef-126">List calendars in a calendar group.</span></span>                           |
| [<span data-ttu-id="999ef-127">创建日历</span><span class="sxs-lookup"><span data-stu-id="999ef-127">Create Calendar</span></span>](../api/calendargroup-post-calendars.md)   | [<span data-ttu-id="999ef-128">日历</span><span class="sxs-lookup"><span data-stu-id="999ef-128">Calendar</span></span>](calendar.md)            | <span data-ttu-id="999ef-129">在日历组中创建新日历。</span><span class="sxs-lookup"><span data-stu-id="999ef-129">Create a new Calendar in a calendar group.</span></span>                    |

## <a name="properties"></a><span data-ttu-id="999ef-130">属性</span><span class="sxs-lookup"><span data-stu-id="999ef-130">Properties</span></span>

| <span data-ttu-id="999ef-131">属性</span><span class="sxs-lookup"><span data-stu-id="999ef-131">Property</span></span>  | <span data-ttu-id="999ef-132">类型</span><span class="sxs-lookup"><span data-stu-id="999ef-132">Type</span></span>   | <span data-ttu-id="999ef-133">说明</span><span class="sxs-lookup"><span data-stu-id="999ef-133">Description</span></span>                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="999ef-134">name</span><span class="sxs-lookup"><span data-stu-id="999ef-134">name</span></span>      | <span data-ttu-id="999ef-135">String</span><span class="sxs-lookup"><span data-stu-id="999ef-135">String</span></span> | <span data-ttu-id="999ef-136">组名称。</span><span class="sxs-lookup"><span data-stu-id="999ef-136">The group name.</span></span>                                                                                                                                                                                           |
| <span data-ttu-id="999ef-137">changeKey</span><span class="sxs-lookup"><span data-stu-id="999ef-137">changeKey</span></span> | <span data-ttu-id="999ef-138">String</span><span class="sxs-lookup"><span data-stu-id="999ef-138">String</span></span> | <span data-ttu-id="999ef-p101">标识日历组的版本。每次日历组更改时，ChangeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。只读。</span><span class="sxs-lookup"><span data-stu-id="999ef-p101">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span> |
| <span data-ttu-id="999ef-143">classId</span><span class="sxs-lookup"><span data-stu-id="999ef-143">classId</span></span>   | <span data-ttu-id="999ef-144">Guid</span><span class="sxs-lookup"><span data-stu-id="999ef-144">Guid</span></span>   | <span data-ttu-id="999ef-p102">类标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="999ef-p102">The class identifier. Read-only.</span></span>                                                                                                                                                                          |
| <span data-ttu-id="999ef-147">id</span><span class="sxs-lookup"><span data-stu-id="999ef-147">id</span></span>        | <span data-ttu-id="999ef-148">String</span><span class="sxs-lookup"><span data-stu-id="999ef-148">String</span></span> | <span data-ttu-id="999ef-p103">组的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="999ef-p103">The group's unique identifier. Read-only.</span></span>                                                                                                                                                                 |

## <a name="relationships"></a><span data-ttu-id="999ef-151">Relationships</span><span class="sxs-lookup"><span data-stu-id="999ef-151">Relationships</span></span>

| <span data-ttu-id="999ef-152">关系</span><span class="sxs-lookup"><span data-stu-id="999ef-152">Relationship</span></span> | <span data-ttu-id="999ef-153">类型</span><span class="sxs-lookup"><span data-stu-id="999ef-153">Type</span></span>                               | <span data-ttu-id="999ef-154">说明</span><span class="sxs-lookup"><span data-stu-id="999ef-154">Description</span></span>                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="999ef-155">日历</span><span class="sxs-lookup"><span data-stu-id="999ef-155">calendars</span></span>    | <span data-ttu-id="999ef-156">[日历](calendar.md) 集合</span><span class="sxs-lookup"><span data-stu-id="999ef-156">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="999ef-p104">日历组中的日历。导航属性。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="999ef-p104">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="999ef-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="999ef-161">JSON representation</span></span>

<span data-ttu-id="999ef-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="999ef-162">Here is a JSON representation of the resource</span></span>

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
