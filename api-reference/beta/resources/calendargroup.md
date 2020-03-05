---
title: calendarGroup 资源类型
description: 一组用户日历。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 175b3b8372214851ef62cf0740779b19fd2d4ce1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507829"
---
# <a name="calendargroup-resource-type"></a><span data-ttu-id="d8803-103">calendarGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="d8803-103">calendarGroup resource type</span></span>

<span data-ttu-id="d8803-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d8803-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8803-105">一组用户日历。</span><span class="sxs-lookup"><span data-stu-id="d8803-105">A group of user calendars.</span></span>

## <a name="methods"></a><span data-ttu-id="d8803-106">方法</span><span class="sxs-lookup"><span data-stu-id="d8803-106">Methods</span></span>

| <span data-ttu-id="d8803-107">方法</span><span class="sxs-lookup"><span data-stu-id="d8803-107">Method</span></span>                                                      | <span data-ttu-id="d8803-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="d8803-108">Return Type</span></span>                        | <span data-ttu-id="d8803-109">说明</span><span class="sxs-lookup"><span data-stu-id="d8803-109">Description</span></span>                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [<span data-ttu-id="d8803-110">列出日历组</span><span class="sxs-lookup"><span data-stu-id="d8803-110">List calendar groups</span></span>](../api/user-list-calendargroups.md)  | <span data-ttu-id="d8803-111">[日历](calendar.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d8803-111">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="d8803-112">获取用户的日历组。</span><span class="sxs-lookup"><span data-stu-id="d8803-112">Get the user's calendar groups.</span></span>                               |
| [<span data-ttu-id="d8803-113">创建日历组</span><span class="sxs-lookup"><span data-stu-id="d8803-113">Create calendar group</span></span>](../api/user-post-calendargroups.md) | [<span data-ttu-id="d8803-114">Calendar</span><span class="sxs-lookup"><span data-stu-id="d8803-114">Calendar</span></span>](calendar.md)            | <span data-ttu-id="d8803-115">创建新的日历组。</span><span class="sxs-lookup"><span data-stu-id="d8803-115">Create a new calendar group.</span></span>                                  |
| [<span data-ttu-id="d8803-116">创建日历组</span><span class="sxs-lookup"><span data-stu-id="d8803-116">Get calendar group</span></span>](../api/calendargroup-get.md)           | [<span data-ttu-id="d8803-117">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="d8803-117">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="d8803-118">读取 calendar 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d8803-118">Read properties and relationships of a calendar group object.</span></span> |
| [<span data-ttu-id="d8803-119">更新</span><span class="sxs-lookup"><span data-stu-id="d8803-119">Update</span></span>](../api/calendargroup-update.md)                    | [<span data-ttu-id="d8803-120">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="d8803-120">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="d8803-121">更新 calendarGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="d8803-121">Update calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="d8803-122">删除</span><span class="sxs-lookup"><span data-stu-id="d8803-122">Delete</span></span>](../api/calendargroup-delete.md)                    | <span data-ttu-id="d8803-123">无</span><span class="sxs-lookup"><span data-stu-id="d8803-123">None</span></span>                               | <span data-ttu-id="d8803-124">删除 calendarGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="d8803-124">Delete calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="d8803-125">List calendars</span><span class="sxs-lookup"><span data-stu-id="d8803-125">List calendars</span></span>](../api/calendargroup-list-calendars.md)    | <span data-ttu-id="d8803-126">[Calendar](calendar.md) collection</span><span class="sxs-lookup"><span data-stu-id="d8803-126">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="d8803-127">列出日历组中的日历。</span><span class="sxs-lookup"><span data-stu-id="d8803-127">List calendars in a calendar group.</span></span>                           |
| [<span data-ttu-id="d8803-128">创建日历</span><span class="sxs-lookup"><span data-stu-id="d8803-128">Create Calendar</span></span>](../api/calendargroup-post-calendars.md)   | [<span data-ttu-id="d8803-129">日历</span><span class="sxs-lookup"><span data-stu-id="d8803-129">Calendar</span></span>](calendar.md)            | <span data-ttu-id="d8803-130">在日历组中创建新日历。</span><span class="sxs-lookup"><span data-stu-id="d8803-130">Create a new Calendar in a calendar group.</span></span>                    |

## <a name="properties"></a><span data-ttu-id="d8803-131">属性</span><span class="sxs-lookup"><span data-stu-id="d8803-131">Properties</span></span>

| <span data-ttu-id="d8803-132">属性</span><span class="sxs-lookup"><span data-stu-id="d8803-132">Property</span></span>  | <span data-ttu-id="d8803-133">类型</span><span class="sxs-lookup"><span data-stu-id="d8803-133">Type</span></span>   | <span data-ttu-id="d8803-134">说明</span><span class="sxs-lookup"><span data-stu-id="d8803-134">Description</span></span>                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="d8803-135">name</span><span class="sxs-lookup"><span data-stu-id="d8803-135">name</span></span>      | <span data-ttu-id="d8803-136">字符串</span><span class="sxs-lookup"><span data-stu-id="d8803-136">String</span></span> | <span data-ttu-id="d8803-137">组名称。</span><span class="sxs-lookup"><span data-stu-id="d8803-137">The group name.</span></span>                                                                                                                                                                                           |
| <span data-ttu-id="d8803-138">changeKey</span><span class="sxs-lookup"><span data-stu-id="d8803-138">changeKey</span></span> | <span data-ttu-id="d8803-139">String</span><span class="sxs-lookup"><span data-stu-id="d8803-139">String</span></span> | <span data-ttu-id="d8803-p101">标识日历组的版本。每次日历组更改时，ChangeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。只读。</span><span class="sxs-lookup"><span data-stu-id="d8803-p101">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span> |
| <span data-ttu-id="d8803-144">classId</span><span class="sxs-lookup"><span data-stu-id="d8803-144">classId</span></span>   | <span data-ttu-id="d8803-145">Guid</span><span class="sxs-lookup"><span data-stu-id="d8803-145">Guid</span></span>   | <span data-ttu-id="d8803-p102">类标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="d8803-p102">The class identifier. Read-only.</span></span>                                                                                                                                                                          |
| <span data-ttu-id="d8803-148">id</span><span class="sxs-lookup"><span data-stu-id="d8803-148">id</span></span>        | <span data-ttu-id="d8803-149">String</span><span class="sxs-lookup"><span data-stu-id="d8803-149">String</span></span> | <span data-ttu-id="d8803-p103">组的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="d8803-p103">The group's unique identifier. Read-only.</span></span>                                                                                                                                                                 |

## <a name="relationships"></a><span data-ttu-id="d8803-152">关系</span><span class="sxs-lookup"><span data-stu-id="d8803-152">Relationships</span></span>

| <span data-ttu-id="d8803-153">关系</span><span class="sxs-lookup"><span data-stu-id="d8803-153">Relationship</span></span> | <span data-ttu-id="d8803-154">类型</span><span class="sxs-lookup"><span data-stu-id="d8803-154">Type</span></span>                               | <span data-ttu-id="d8803-155">说明</span><span class="sxs-lookup"><span data-stu-id="d8803-155">Description</span></span>                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="d8803-156">calendars</span><span class="sxs-lookup"><span data-stu-id="d8803-156">calendars</span></span>    | <span data-ttu-id="d8803-157">[Calendar](calendar.md) collection</span><span class="sxs-lookup"><span data-stu-id="d8803-157">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="d8803-p104">日历组中的日历。导航属性。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="d8803-p104">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d8803-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d8803-162">JSON representation</span></span>

<span data-ttu-id="d8803-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8803-163">Here is a JSON representation of the resource</span></span>

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
