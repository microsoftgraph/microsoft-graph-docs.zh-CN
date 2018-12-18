---
title: calendarGroup 资源类型
description: 一组的用户日历。
author: angelgolfer-ms
ms.openlocfilehash: fda8a3006631f45d49e83363d61f7b0363675ed1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334368"
---
# <a name="calendargroup-resource-type"></a><span data-ttu-id="e6caa-103">calendarGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="e6caa-103">calendarGroup resource type</span></span>

> <span data-ttu-id="e6caa-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e6caa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e6caa-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e6caa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e6caa-106">一组的用户日历。</span><span class="sxs-lookup"><span data-stu-id="e6caa-106">A group of user calendars.</span></span>

## <a name="methods"></a><span data-ttu-id="e6caa-107">方法</span><span class="sxs-lookup"><span data-stu-id="e6caa-107">Methods</span></span>

| <span data-ttu-id="e6caa-108">方法</span><span class="sxs-lookup"><span data-stu-id="e6caa-108">Method</span></span>                                                      | <span data-ttu-id="e6caa-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e6caa-109">Return Type</span></span>                        | <span data-ttu-id="e6caa-110">说明</span><span class="sxs-lookup"><span data-stu-id="e6caa-110">Description</span></span>                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [<span data-ttu-id="e6caa-111">列出日历组</span><span class="sxs-lookup"><span data-stu-id="e6caa-111">List calendar groups</span></span>](../api/user-list-calendargroups.md)  | <span data-ttu-id="e6caa-112">[日历](calendar.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e6caa-112">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="e6caa-113">获取用户的日历组。</span><span class="sxs-lookup"><span data-stu-id="e6caa-113">Get the user's calendar groups.</span></span>                               |
| [<span data-ttu-id="e6caa-114">创建日历组</span><span class="sxs-lookup"><span data-stu-id="e6caa-114">Create calendar group</span></span>](../api/user-post-calendargroups.md) | [<span data-ttu-id="e6caa-115">日历</span><span class="sxs-lookup"><span data-stu-id="e6caa-115">Calendar</span></span>](calendar.md)            | <span data-ttu-id="e6caa-116">创建新的日历组。</span><span class="sxs-lookup"><span data-stu-id="e6caa-116">Create a new calendar group.</span></span>                                  |
| [<span data-ttu-id="e6caa-117">创建日历组</span><span class="sxs-lookup"><span data-stu-id="e6caa-117">Get calendar group</span></span>](../api/calendargroup-get.md)           | [<span data-ttu-id="e6caa-118">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="e6caa-118">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="e6caa-119">读取 calendar 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e6caa-119">Read properties and relationships of a calendar group object.</span></span> |
| [<span data-ttu-id="e6caa-120">更新</span><span class="sxs-lookup"><span data-stu-id="e6caa-120">Update</span></span>](../api/calendargroup-update.md)                    | [<span data-ttu-id="e6caa-121">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="e6caa-121">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="e6caa-122">更新 calendarGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="e6caa-122">Update calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="e6caa-123">删除</span><span class="sxs-lookup"><span data-stu-id="e6caa-123">Delete</span></span>](../api/calendargroup-delete.md)                    | <span data-ttu-id="e6caa-124">无</span><span class="sxs-lookup"><span data-stu-id="e6caa-124">None</span></span>                               | <span data-ttu-id="e6caa-125">删除 calendarGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="e6caa-125">Delete calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="e6caa-126">列出日历</span><span class="sxs-lookup"><span data-stu-id="e6caa-126">List calendars</span></span>](../api/calendargroup-list-calendars.md)    | <span data-ttu-id="e6caa-127">[日历](calendar.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e6caa-127">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="e6caa-128">列出日历组中的日历。</span><span class="sxs-lookup"><span data-stu-id="e6caa-128">List calendars in a calendar group.</span></span>                           |
| [<span data-ttu-id="e6caa-129">创建日历</span><span class="sxs-lookup"><span data-stu-id="e6caa-129">Create Calendar</span></span>](../api/calendargroup-post-calendars.md)   | [<span data-ttu-id="e6caa-130">日历</span><span class="sxs-lookup"><span data-stu-id="e6caa-130">Calendar</span></span>](calendar.md)            | <span data-ttu-id="e6caa-131">在日历组中创建新日历。</span><span class="sxs-lookup"><span data-stu-id="e6caa-131">Create a new Calendar in a calendar group.</span></span>                    |

## <a name="properties"></a><span data-ttu-id="e6caa-132">属性</span><span class="sxs-lookup"><span data-stu-id="e6caa-132">Properties</span></span>

| <span data-ttu-id="e6caa-133">属性</span><span class="sxs-lookup"><span data-stu-id="e6caa-133">Property</span></span>  | <span data-ttu-id="e6caa-134">类型</span><span class="sxs-lookup"><span data-stu-id="e6caa-134">Type</span></span>   | <span data-ttu-id="e6caa-135">说明</span><span class="sxs-lookup"><span data-stu-id="e6caa-135">Description</span></span>                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="e6caa-136">name</span><span class="sxs-lookup"><span data-stu-id="e6caa-136">name</span></span>      | <span data-ttu-id="e6caa-137">String</span><span class="sxs-lookup"><span data-stu-id="e6caa-137">String</span></span> | <span data-ttu-id="e6caa-138">组名称。</span><span class="sxs-lookup"><span data-stu-id="e6caa-138">The group name.</span></span>                                                                                                                                                                                           |
| <span data-ttu-id="e6caa-139">changeKey</span><span class="sxs-lookup"><span data-stu-id="e6caa-139">changeKey</span></span> | <span data-ttu-id="e6caa-140">String</span><span class="sxs-lookup"><span data-stu-id="e6caa-140">String</span></span> | <span data-ttu-id="e6caa-p102">标识日历组的版本。每次日历组更改时，ChangeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。只读。</span><span class="sxs-lookup"><span data-stu-id="e6caa-p102">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span> |
| <span data-ttu-id="e6caa-145">classId</span><span class="sxs-lookup"><span data-stu-id="e6caa-145">classId</span></span>   | <span data-ttu-id="e6caa-146">Guid</span><span class="sxs-lookup"><span data-stu-id="e6caa-146">Guid</span></span>   | <span data-ttu-id="e6caa-p103">类标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="e6caa-p103">The class identifier. Read-only.</span></span>                                                                                                                                                                          |
| <span data-ttu-id="e6caa-149">id</span><span class="sxs-lookup"><span data-stu-id="e6caa-149">id</span></span>        | <span data-ttu-id="e6caa-150">String</span><span class="sxs-lookup"><span data-stu-id="e6caa-150">String</span></span> | <span data-ttu-id="e6caa-p104">组的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="e6caa-p104">The group's unique identifier. Read-only.</span></span>                                                                                                                                                                 |

## <a name="relationships"></a><span data-ttu-id="e6caa-153">Relationships</span><span class="sxs-lookup"><span data-stu-id="e6caa-153">Relationships</span></span>

| <span data-ttu-id="e6caa-154">关系</span><span class="sxs-lookup"><span data-stu-id="e6caa-154">Relationship</span></span> | <span data-ttu-id="e6caa-155">类型</span><span class="sxs-lookup"><span data-stu-id="e6caa-155">Type</span></span>                               | <span data-ttu-id="e6caa-156">说明</span><span class="sxs-lookup"><span data-stu-id="e6caa-156">Description</span></span>                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="e6caa-157">日历</span><span class="sxs-lookup"><span data-stu-id="e6caa-157">calendars</span></span>    | <span data-ttu-id="e6caa-158">[日历](calendar.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e6caa-158">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="e6caa-p105">日历组中的日历。导航属性。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="e6caa-p105">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e6caa-163">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e6caa-163">JSON representation</span></span>

<span data-ttu-id="e6caa-164">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6caa-164">Here is a JSON representation of the resource</span></span>

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
