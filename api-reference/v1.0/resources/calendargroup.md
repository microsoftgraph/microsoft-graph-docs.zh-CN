---
title: calendarGroup 资源类型
description: 一组用户日历。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 230d6b0f90b8dec5ad223b7243fbc710dd720a30
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531980"
---
# <a name="calendargroup-resource-type"></a><span data-ttu-id="341aa-103">calendarGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="341aa-103">calendarGroup resource type</span></span>

<span data-ttu-id="341aa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="341aa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="341aa-105">一组用户日历。</span><span class="sxs-lookup"><span data-stu-id="341aa-105">A group of user calendars.</span></span>

## <a name="methods"></a><span data-ttu-id="341aa-106">Methods</span><span class="sxs-lookup"><span data-stu-id="341aa-106">Methods</span></span>

| <span data-ttu-id="341aa-107">方法</span><span class="sxs-lookup"><span data-stu-id="341aa-107">Method</span></span>                                                      | <span data-ttu-id="341aa-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="341aa-108">Return Type</span></span>                        | <span data-ttu-id="341aa-109">说明</span><span class="sxs-lookup"><span data-stu-id="341aa-109">Description</span></span>                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [<span data-ttu-id="341aa-110">列出日历组</span><span class="sxs-lookup"><span data-stu-id="341aa-110">List calendar groups</span></span>](../api/user-list-calendargroups.md)  | <span data-ttu-id="341aa-111">[日历](calendar.md) 集合</span><span class="sxs-lookup"><span data-stu-id="341aa-111">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="341aa-112">获取用户的日历组。</span><span class="sxs-lookup"><span data-stu-id="341aa-112">Get the user's calendar groups.</span></span>                               |
| [<span data-ttu-id="341aa-113">创建日历组</span><span class="sxs-lookup"><span data-stu-id="341aa-113">Create calendar group</span></span>](../api/user-post-calendargroups.md) | [<span data-ttu-id="341aa-114">Calendar</span><span class="sxs-lookup"><span data-stu-id="341aa-114">Calendar</span></span>](calendar.md)            | <span data-ttu-id="341aa-115">创建新的日历组。</span><span class="sxs-lookup"><span data-stu-id="341aa-115">Create a new calendar group.</span></span>                                  |
| [<span data-ttu-id="341aa-116">创建日历组</span><span class="sxs-lookup"><span data-stu-id="341aa-116">Get calendar group</span></span>](../api/calendargroup-get.md)           | [<span data-ttu-id="341aa-117">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="341aa-117">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="341aa-118">读取 calendar 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="341aa-118">Read properties and relationships of a calendar group object.</span></span> |
| [<span data-ttu-id="341aa-119">更新</span><span class="sxs-lookup"><span data-stu-id="341aa-119">Update</span></span>](../api/calendargroup-update.md)                    | [<span data-ttu-id="341aa-120">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="341aa-120">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="341aa-121">更新 calendarGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="341aa-121">Update calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="341aa-122">删除</span><span class="sxs-lookup"><span data-stu-id="341aa-122">Delete</span></span>](../api/calendargroup-delete.md)                    | <span data-ttu-id="341aa-123">无</span><span class="sxs-lookup"><span data-stu-id="341aa-123">None</span></span>                               | <span data-ttu-id="341aa-124">删除 calendarGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="341aa-124">Delete calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="341aa-125">List calendars</span><span class="sxs-lookup"><span data-stu-id="341aa-125">List calendars</span></span>](../api/calendargroup-list-calendars.md)    | <span data-ttu-id="341aa-126">[Calendar](calendar.md) collection</span><span class="sxs-lookup"><span data-stu-id="341aa-126">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="341aa-127">列出日历组中的日历。</span><span class="sxs-lookup"><span data-stu-id="341aa-127">List calendars in a calendar group.</span></span>                           |
| [<span data-ttu-id="341aa-128">创建日历</span><span class="sxs-lookup"><span data-stu-id="341aa-128">Create Calendar</span></span>](../api/calendargroup-post-calendars.md)   | [<span data-ttu-id="341aa-129">日历</span><span class="sxs-lookup"><span data-stu-id="341aa-129">Calendar</span></span>](calendar.md)            | <span data-ttu-id="341aa-130">在日历组中创建新日历。</span><span class="sxs-lookup"><span data-stu-id="341aa-130">Create a new Calendar in a calendar group.</span></span>                    |

## <a name="properties"></a><span data-ttu-id="341aa-131">属性</span><span class="sxs-lookup"><span data-stu-id="341aa-131">Properties</span></span>

| <span data-ttu-id="341aa-132">属性</span><span class="sxs-lookup"><span data-stu-id="341aa-132">Property</span></span>  | <span data-ttu-id="341aa-133">类型</span><span class="sxs-lookup"><span data-stu-id="341aa-133">Type</span></span>   | <span data-ttu-id="341aa-134">说明</span><span class="sxs-lookup"><span data-stu-id="341aa-134">Description</span></span>                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="341aa-135">name</span><span class="sxs-lookup"><span data-stu-id="341aa-135">name</span></span>      | <span data-ttu-id="341aa-136">字符串</span><span class="sxs-lookup"><span data-stu-id="341aa-136">String</span></span> | <span data-ttu-id="341aa-137">组名称。</span><span class="sxs-lookup"><span data-stu-id="341aa-137">The group name.</span></span>                                                                                                                                                                                           |
| <span data-ttu-id="341aa-138">changeKey</span><span class="sxs-lookup"><span data-stu-id="341aa-138">changeKey</span></span> | <span data-ttu-id="341aa-139">String</span><span class="sxs-lookup"><span data-stu-id="341aa-139">String</span></span> | <span data-ttu-id="341aa-p101">标识日历组的版本。每次日历组更改时，ChangeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。只读。</span><span class="sxs-lookup"><span data-stu-id="341aa-p101">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span> |
| <span data-ttu-id="341aa-144">classId</span><span class="sxs-lookup"><span data-stu-id="341aa-144">classId</span></span>   | <span data-ttu-id="341aa-145">Guid</span><span class="sxs-lookup"><span data-stu-id="341aa-145">Guid</span></span>   | <span data-ttu-id="341aa-p102">类标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="341aa-p102">The class identifier. Read-only.</span></span>                                                                                                                                                                          |
| <span data-ttu-id="341aa-148">id</span><span class="sxs-lookup"><span data-stu-id="341aa-148">id</span></span>        | <span data-ttu-id="341aa-149">String</span><span class="sxs-lookup"><span data-stu-id="341aa-149">String</span></span> | <span data-ttu-id="341aa-p103">组的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="341aa-p103">The group's unique identifier. Read-only.</span></span>                                                                                                                                                                 |

## <a name="relationships"></a><span data-ttu-id="341aa-152">关系</span><span class="sxs-lookup"><span data-stu-id="341aa-152">Relationships</span></span>

| <span data-ttu-id="341aa-153">关系</span><span class="sxs-lookup"><span data-stu-id="341aa-153">Relationship</span></span> | <span data-ttu-id="341aa-154">类型</span><span class="sxs-lookup"><span data-stu-id="341aa-154">Type</span></span>                               | <span data-ttu-id="341aa-155">说明</span><span class="sxs-lookup"><span data-stu-id="341aa-155">Description</span></span>                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="341aa-156">calendars</span><span class="sxs-lookup"><span data-stu-id="341aa-156">calendars</span></span>    | <span data-ttu-id="341aa-157">[Calendar](calendar.md) collection</span><span class="sxs-lookup"><span data-stu-id="341aa-157">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="341aa-p104">日历组中的日历。导航属性。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="341aa-p104">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="341aa-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="341aa-162">JSON representation</span></span>

<span data-ttu-id="341aa-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="341aa-163">Here is a JSON representation of the resource</span></span>

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
