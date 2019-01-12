---
title: calendarGroup 资源类型
description: 一组的用户日历。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 10a840fd9ae9835eb5ca6a96b88719605f89245b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985289"
---
# <a name="calendargroup-resource-type"></a><span data-ttu-id="277f4-103">calendarGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="277f4-103">calendarGroup resource type</span></span>

> <span data-ttu-id="277f4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="277f4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="277f4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="277f4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="277f4-106">一组的用户日历。</span><span class="sxs-lookup"><span data-stu-id="277f4-106">A group of user calendars.</span></span>

## <a name="methods"></a><span data-ttu-id="277f4-107">方法</span><span class="sxs-lookup"><span data-stu-id="277f4-107">Methods</span></span>

| <span data-ttu-id="277f4-108">方法</span><span class="sxs-lookup"><span data-stu-id="277f4-108">Method</span></span>                                                      | <span data-ttu-id="277f4-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="277f4-109">Return Type</span></span>                        | <span data-ttu-id="277f4-110">说明</span><span class="sxs-lookup"><span data-stu-id="277f4-110">Description</span></span>                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [<span data-ttu-id="277f4-111">列出日历组</span><span class="sxs-lookup"><span data-stu-id="277f4-111">List calendar groups</span></span>](../api/user-list-calendargroups.md)  | <span data-ttu-id="277f4-112">[日历](calendar.md) 集合</span><span class="sxs-lookup"><span data-stu-id="277f4-112">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="277f4-113">获取用户的日历组。</span><span class="sxs-lookup"><span data-stu-id="277f4-113">Get the user's calendar groups.</span></span>                               |
| [<span data-ttu-id="277f4-114">创建日历组</span><span class="sxs-lookup"><span data-stu-id="277f4-114">Create calendar group</span></span>](../api/user-post-calendargroups.md) | [<span data-ttu-id="277f4-115">日历</span><span class="sxs-lookup"><span data-stu-id="277f4-115">Calendar</span></span>](calendar.md)            | <span data-ttu-id="277f4-116">创建新的日历组。</span><span class="sxs-lookup"><span data-stu-id="277f4-116">Create a new calendar group.</span></span>                                  |
| [<span data-ttu-id="277f4-117">创建日历组</span><span class="sxs-lookup"><span data-stu-id="277f4-117">Get calendar group</span></span>](../api/calendargroup-get.md)           | [<span data-ttu-id="277f4-118">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="277f4-118">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="277f4-119">读取 calendar 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="277f4-119">Read properties and relationships of a calendar group object.</span></span> |
| [<span data-ttu-id="277f4-120">更新</span><span class="sxs-lookup"><span data-stu-id="277f4-120">Update</span></span>](../api/calendargroup-update.md)                    | [<span data-ttu-id="277f4-121">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="277f4-121">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="277f4-122">更新 calendarGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="277f4-122">Update calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="277f4-123">删除</span><span class="sxs-lookup"><span data-stu-id="277f4-123">Delete</span></span>](../api/calendargroup-delete.md)                    | <span data-ttu-id="277f4-124">无</span><span class="sxs-lookup"><span data-stu-id="277f4-124">None</span></span>                               | <span data-ttu-id="277f4-125">删除 calendarGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="277f4-125">Delete calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="277f4-126">列出日历</span><span class="sxs-lookup"><span data-stu-id="277f4-126">List calendars</span></span>](../api/calendargroup-list-calendars.md)    | <span data-ttu-id="277f4-127">[日历](calendar.md) 集合</span><span class="sxs-lookup"><span data-stu-id="277f4-127">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="277f4-128">列出日历组中的日历。</span><span class="sxs-lookup"><span data-stu-id="277f4-128">List calendars in a calendar group.</span></span>                           |
| [<span data-ttu-id="277f4-129">创建日历</span><span class="sxs-lookup"><span data-stu-id="277f4-129">Create Calendar</span></span>](../api/calendargroup-post-calendars.md)   | [<span data-ttu-id="277f4-130">日历</span><span class="sxs-lookup"><span data-stu-id="277f4-130">Calendar</span></span>](calendar.md)            | <span data-ttu-id="277f4-131">在日历组中创建新日历。</span><span class="sxs-lookup"><span data-stu-id="277f4-131">Create a new Calendar in a calendar group.</span></span>                    |

## <a name="properties"></a><span data-ttu-id="277f4-132">属性</span><span class="sxs-lookup"><span data-stu-id="277f4-132">Properties</span></span>

| <span data-ttu-id="277f4-133">属性</span><span class="sxs-lookup"><span data-stu-id="277f4-133">Property</span></span>  | <span data-ttu-id="277f4-134">类型</span><span class="sxs-lookup"><span data-stu-id="277f4-134">Type</span></span>   | <span data-ttu-id="277f4-135">说明</span><span class="sxs-lookup"><span data-stu-id="277f4-135">Description</span></span>                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="277f4-136">name</span><span class="sxs-lookup"><span data-stu-id="277f4-136">name</span></span>      | <span data-ttu-id="277f4-137">String</span><span class="sxs-lookup"><span data-stu-id="277f4-137">String</span></span> | <span data-ttu-id="277f4-138">组名称。</span><span class="sxs-lookup"><span data-stu-id="277f4-138">The group name.</span></span>                                                                                                                                                                                           |
| <span data-ttu-id="277f4-139">changeKey</span><span class="sxs-lookup"><span data-stu-id="277f4-139">changeKey</span></span> | <span data-ttu-id="277f4-140">String</span><span class="sxs-lookup"><span data-stu-id="277f4-140">String</span></span> | <span data-ttu-id="277f4-p102">标识日历组的版本。每次日历组更改时，ChangeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。只读。</span><span class="sxs-lookup"><span data-stu-id="277f4-p102">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span> |
| <span data-ttu-id="277f4-145">classId</span><span class="sxs-lookup"><span data-stu-id="277f4-145">classId</span></span>   | <span data-ttu-id="277f4-146">Guid</span><span class="sxs-lookup"><span data-stu-id="277f4-146">Guid</span></span>   | <span data-ttu-id="277f4-p103">类标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="277f4-p103">The class identifier. Read-only.</span></span>                                                                                                                                                                          |
| <span data-ttu-id="277f4-149">id</span><span class="sxs-lookup"><span data-stu-id="277f4-149">id</span></span>        | <span data-ttu-id="277f4-150">String</span><span class="sxs-lookup"><span data-stu-id="277f4-150">String</span></span> | <span data-ttu-id="277f4-p104">组的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="277f4-p104">The group's unique identifier. Read-only.</span></span>                                                                                                                                                                 |

## <a name="relationships"></a><span data-ttu-id="277f4-153">Relationships</span><span class="sxs-lookup"><span data-stu-id="277f4-153">Relationships</span></span>

| <span data-ttu-id="277f4-154">关系</span><span class="sxs-lookup"><span data-stu-id="277f4-154">Relationship</span></span> | <span data-ttu-id="277f4-155">类型</span><span class="sxs-lookup"><span data-stu-id="277f4-155">Type</span></span>                               | <span data-ttu-id="277f4-156">说明</span><span class="sxs-lookup"><span data-stu-id="277f4-156">Description</span></span>                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="277f4-157">日历</span><span class="sxs-lookup"><span data-stu-id="277f4-157">calendars</span></span>    | <span data-ttu-id="277f4-158">[日历](calendar.md) 集合</span><span class="sxs-lookup"><span data-stu-id="277f4-158">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="277f4-p105">日历组中的日历。导航属性。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="277f4-p105">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="277f4-163">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="277f4-163">JSON representation</span></span>

<span data-ttu-id="277f4-164">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="277f4-164">Here is a JSON representation of the resource</span></span>

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
