---
title: calendarGroup 资源类型
description: 一组用户日历。
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 89a0a8176936654e287399c51c45e9ae55f46f23
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071617"
---
# <a name="calendargroup-resource-type"></a><span data-ttu-id="f9a6b-103">calendarGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="f9a6b-103">calendarGroup resource type</span></span>

<span data-ttu-id="f9a6b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9a6b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9a6b-105">一组用户日历。</span><span class="sxs-lookup"><span data-stu-id="f9a6b-105">A group of user calendars.</span></span>

## <a name="methods"></a><span data-ttu-id="f9a6b-106">方法</span><span class="sxs-lookup"><span data-stu-id="f9a6b-106">Methods</span></span>

| <span data-ttu-id="f9a6b-107">方法</span><span class="sxs-lookup"><span data-stu-id="f9a6b-107">Method</span></span>                                                      | <span data-ttu-id="f9a6b-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="f9a6b-108">Return Type</span></span>                        | <span data-ttu-id="f9a6b-109">说明</span><span class="sxs-lookup"><span data-stu-id="f9a6b-109">Description</span></span>                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [<span data-ttu-id="f9a6b-110">列出日历组</span><span class="sxs-lookup"><span data-stu-id="f9a6b-110">List calendar groups</span></span>](../api/user-list-calendargroups.md)  | <span data-ttu-id="f9a6b-111">[日历](calendar.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f9a6b-111">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="f9a6b-112">获取用户的日历组。</span><span class="sxs-lookup"><span data-stu-id="f9a6b-112">Get the user's calendar groups.</span></span>                               |
| [<span data-ttu-id="f9a6b-113">创建日历组</span><span class="sxs-lookup"><span data-stu-id="f9a6b-113">Create calendar group</span></span>](../api/user-post-calendargroups.md) | [<span data-ttu-id="f9a6b-114">日历</span><span class="sxs-lookup"><span data-stu-id="f9a6b-114">Calendar</span></span>](calendar.md)            | <span data-ttu-id="f9a6b-115">创建新的日历组。</span><span class="sxs-lookup"><span data-stu-id="f9a6b-115">Create a new calendar group.</span></span>                                  |
| [<span data-ttu-id="f9a6b-116">创建日历组</span><span class="sxs-lookup"><span data-stu-id="f9a6b-116">Get calendar group</span></span>](../api/calendargroup-get.md)           | [<span data-ttu-id="f9a6b-117">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="f9a6b-117">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="f9a6b-118">读取 calendar 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f9a6b-118">Read properties and relationships of a calendar group object.</span></span> |
| [<span data-ttu-id="f9a6b-119">更新</span><span class="sxs-lookup"><span data-stu-id="f9a6b-119">Update</span></span>](../api/calendargroup-update.md)                    | [<span data-ttu-id="f9a6b-120">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="f9a6b-120">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="f9a6b-121">更新 calendarGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="f9a6b-121">Update calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="f9a6b-122">删除</span><span class="sxs-lookup"><span data-stu-id="f9a6b-122">Delete</span></span>](../api/calendargroup-delete.md)                    | <span data-ttu-id="f9a6b-123">无</span><span class="sxs-lookup"><span data-stu-id="f9a6b-123">None</span></span>                               | <span data-ttu-id="f9a6b-124">删除 calendarGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="f9a6b-124">Delete calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="f9a6b-125">List calendars</span><span class="sxs-lookup"><span data-stu-id="f9a6b-125">List calendars</span></span>](../api/calendargroup-list-calendars.md)    | <span data-ttu-id="f9a6b-126">[Calendar](calendar.md) collection</span><span class="sxs-lookup"><span data-stu-id="f9a6b-126">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="f9a6b-127">列出日历组中的日历。</span><span class="sxs-lookup"><span data-stu-id="f9a6b-127">List calendars in a calendar group.</span></span>                           |
| [<span data-ttu-id="f9a6b-128">创建日历</span><span class="sxs-lookup"><span data-stu-id="f9a6b-128">Create Calendar</span></span>](../api/calendargroup-post-calendars.md)   | [<span data-ttu-id="f9a6b-129">日历</span><span class="sxs-lookup"><span data-stu-id="f9a6b-129">Calendar</span></span>](calendar.md)            | <span data-ttu-id="f9a6b-130">在日历组中创建新日历。</span><span class="sxs-lookup"><span data-stu-id="f9a6b-130">Create a new Calendar in a calendar group.</span></span>                    |

## <a name="properties"></a><span data-ttu-id="f9a6b-131">属性</span><span class="sxs-lookup"><span data-stu-id="f9a6b-131">Properties</span></span>

| <span data-ttu-id="f9a6b-132">属性</span><span class="sxs-lookup"><span data-stu-id="f9a6b-132">Property</span></span>  | <span data-ttu-id="f9a6b-133">类型</span><span class="sxs-lookup"><span data-stu-id="f9a6b-133">Type</span></span>   | <span data-ttu-id="f9a6b-134">说明</span><span class="sxs-lookup"><span data-stu-id="f9a6b-134">Description</span></span>                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="f9a6b-135">名称</span><span class="sxs-lookup"><span data-stu-id="f9a6b-135">name</span></span>      | <span data-ttu-id="f9a6b-136">String</span><span class="sxs-lookup"><span data-stu-id="f9a6b-136">String</span></span> | <span data-ttu-id="f9a6b-137">组名称。</span><span class="sxs-lookup"><span data-stu-id="f9a6b-137">The group name.</span></span>                                                                                                                                                                                           |
| <span data-ttu-id="f9a6b-138">changeKey</span><span class="sxs-lookup"><span data-stu-id="f9a6b-138">changeKey</span></span> | <span data-ttu-id="f9a6b-139">String</span><span class="sxs-lookup"><span data-stu-id="f9a6b-139">String</span></span> | <span data-ttu-id="f9a6b-p101">标识日历组的版本。每次日历组更改时，ChangeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。只读。</span><span class="sxs-lookup"><span data-stu-id="f9a6b-p101">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span> |
| <span data-ttu-id="f9a6b-144">classId</span><span class="sxs-lookup"><span data-stu-id="f9a6b-144">classId</span></span>   | <span data-ttu-id="f9a6b-145">Guid</span><span class="sxs-lookup"><span data-stu-id="f9a6b-145">Guid</span></span>   | <span data-ttu-id="f9a6b-p102">类标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="f9a6b-p102">The class identifier. Read-only.</span></span>                                                                                                                                                                          |
| <span data-ttu-id="f9a6b-148">id</span><span class="sxs-lookup"><span data-stu-id="f9a6b-148">id</span></span>        | <span data-ttu-id="f9a6b-149">String</span><span class="sxs-lookup"><span data-stu-id="f9a6b-149">String</span></span> | <span data-ttu-id="f9a6b-p103">组的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="f9a6b-p103">The group's unique identifier. Read-only.</span></span>                                                                                                                                                                 |

## <a name="relationships"></a><span data-ttu-id="f9a6b-152">关系</span><span class="sxs-lookup"><span data-stu-id="f9a6b-152">Relationships</span></span>

| <span data-ttu-id="f9a6b-153">关系</span><span class="sxs-lookup"><span data-stu-id="f9a6b-153">Relationship</span></span> | <span data-ttu-id="f9a6b-154">类型</span><span class="sxs-lookup"><span data-stu-id="f9a6b-154">Type</span></span>                               | <span data-ttu-id="f9a6b-155">说明</span><span class="sxs-lookup"><span data-stu-id="f9a6b-155">Description</span></span>                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="f9a6b-156">calendars</span><span class="sxs-lookup"><span data-stu-id="f9a6b-156">calendars</span></span>    | <span data-ttu-id="f9a6b-157">[Calendar](calendar.md) collection</span><span class="sxs-lookup"><span data-stu-id="f9a6b-157">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="f9a6b-p104">日历组中的日历。导航属性。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="f9a6b-p104">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f9a6b-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f9a6b-162">JSON representation</span></span>

<span data-ttu-id="f9a6b-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f9a6b-163">Here is a JSON representation of the resource</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "calendarGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


