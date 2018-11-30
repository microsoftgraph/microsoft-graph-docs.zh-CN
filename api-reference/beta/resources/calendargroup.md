---
title: calendarGroup 资源类型
description: 一组的用户日历。
ms.openlocfilehash: 4ff927e4bcf8bcd54f3cfe6756895d59e43e44b4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041583"
---
# <a name="calendargroup-resource-type"></a><span data-ttu-id="48ad3-103">calendarGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="48ad3-103">calendarGroup resource type</span></span>

> <span data-ttu-id="48ad3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="48ad3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="48ad3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="48ad3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="48ad3-106">一组的用户日历。</span><span class="sxs-lookup"><span data-stu-id="48ad3-106">A group of user calendars.</span></span>

## <a name="methods"></a><span data-ttu-id="48ad3-107">方法</span><span class="sxs-lookup"><span data-stu-id="48ad3-107">Methods</span></span>

| <span data-ttu-id="48ad3-108">方法</span><span class="sxs-lookup"><span data-stu-id="48ad3-108">Method</span></span>                                                      | <span data-ttu-id="48ad3-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="48ad3-109">Return Type</span></span>                        | <span data-ttu-id="48ad3-110">说明</span><span class="sxs-lookup"><span data-stu-id="48ad3-110">Description</span></span>                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [<span data-ttu-id="48ad3-111">列出日历组</span><span class="sxs-lookup"><span data-stu-id="48ad3-111">List calendar groups</span></span>](../api/user-list-calendargroups.md)  | <span data-ttu-id="48ad3-112">[日历](calendar.md) 集合</span><span class="sxs-lookup"><span data-stu-id="48ad3-112">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="48ad3-113">获取用户的日历组。</span><span class="sxs-lookup"><span data-stu-id="48ad3-113">Get the user's calendar groups.</span></span>                               |
| [<span data-ttu-id="48ad3-114">创建日历组</span><span class="sxs-lookup"><span data-stu-id="48ad3-114">Create calendar group</span></span>](../api/user-post-calendargroups.md) | [<span data-ttu-id="48ad3-115">日历</span><span class="sxs-lookup"><span data-stu-id="48ad3-115">Calendar</span></span>](calendar.md)            | <span data-ttu-id="48ad3-116">创建新的日历组。</span><span class="sxs-lookup"><span data-stu-id="48ad3-116">Create a new calendar group.</span></span>                                  |
| [<span data-ttu-id="48ad3-117">创建日历组</span><span class="sxs-lookup"><span data-stu-id="48ad3-117">Get calendar group</span></span>](../api/calendargroup-get.md)           | [<span data-ttu-id="48ad3-118">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="48ad3-118">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="48ad3-119">读取 calendar 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="48ad3-119">Read properties and relationships of a calendar group object.</span></span> |
| [<span data-ttu-id="48ad3-120">更新</span><span class="sxs-lookup"><span data-stu-id="48ad3-120">Update</span></span>](../api/calendargroup-update.md)                    | [<span data-ttu-id="48ad3-121">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="48ad3-121">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="48ad3-122">更新 calendarGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="48ad3-122">Update calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="48ad3-123">删除</span><span class="sxs-lookup"><span data-stu-id="48ad3-123">Delete</span></span>](../api/calendargroup-delete.md)                    | <span data-ttu-id="48ad3-124">无</span><span class="sxs-lookup"><span data-stu-id="48ad3-124">None</span></span>                               | <span data-ttu-id="48ad3-125">删除 calendarGroup 对象。</span><span class="sxs-lookup"><span data-stu-id="48ad3-125">Delete calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="48ad3-126">列出日历</span><span class="sxs-lookup"><span data-stu-id="48ad3-126">List calendars</span></span>](../api/calendargroup-list-calendars.md)    | <span data-ttu-id="48ad3-127">[日历](calendar.md) 集合</span><span class="sxs-lookup"><span data-stu-id="48ad3-127">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="48ad3-128">列出日历组中的日历。</span><span class="sxs-lookup"><span data-stu-id="48ad3-128">List calendars in a calendar group.</span></span>                           |
| [<span data-ttu-id="48ad3-129">创建日历</span><span class="sxs-lookup"><span data-stu-id="48ad3-129">Create Calendar</span></span>](../api/calendargroup-post-calendars.md)   | [<span data-ttu-id="48ad3-130">日历</span><span class="sxs-lookup"><span data-stu-id="48ad3-130">Calendar</span></span>](calendar.md)            | <span data-ttu-id="48ad3-131">在日历组中创建新日历。</span><span class="sxs-lookup"><span data-stu-id="48ad3-131">Create a new Calendar in a calendar group.</span></span>                    |

## <a name="properties"></a><span data-ttu-id="48ad3-132">属性</span><span class="sxs-lookup"><span data-stu-id="48ad3-132">Properties</span></span>

| <span data-ttu-id="48ad3-133">属性</span><span class="sxs-lookup"><span data-stu-id="48ad3-133">Property</span></span>  | <span data-ttu-id="48ad3-134">类型</span><span class="sxs-lookup"><span data-stu-id="48ad3-134">Type</span></span>   | <span data-ttu-id="48ad3-135">说明</span><span class="sxs-lookup"><span data-stu-id="48ad3-135">Description</span></span>                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="48ad3-136">name</span><span class="sxs-lookup"><span data-stu-id="48ad3-136">name</span></span>      | <span data-ttu-id="48ad3-137">String</span><span class="sxs-lookup"><span data-stu-id="48ad3-137">String</span></span> | <span data-ttu-id="48ad3-138">组名称。</span><span class="sxs-lookup"><span data-stu-id="48ad3-138">The group name.</span></span>                                                                                                                                                                                           |
| <span data-ttu-id="48ad3-139">changeKey</span><span class="sxs-lookup"><span data-stu-id="48ad3-139">changeKey</span></span> | <span data-ttu-id="48ad3-140">String</span><span class="sxs-lookup"><span data-stu-id="48ad3-140">String</span></span> | <span data-ttu-id="48ad3-p102">标识日历组的版本。每次日历组更改时，ChangeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。只读。</span><span class="sxs-lookup"><span data-stu-id="48ad3-p102">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span> |
| <span data-ttu-id="48ad3-145">classId</span><span class="sxs-lookup"><span data-stu-id="48ad3-145">classId</span></span>   | <span data-ttu-id="48ad3-146">Guid</span><span class="sxs-lookup"><span data-stu-id="48ad3-146">Guid</span></span>   | <span data-ttu-id="48ad3-p103">类标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="48ad3-p103">The class identifier. Read-only.</span></span>                                                                                                                                                                          |
| <span data-ttu-id="48ad3-149">id</span><span class="sxs-lookup"><span data-stu-id="48ad3-149">id</span></span>        | <span data-ttu-id="48ad3-150">String</span><span class="sxs-lookup"><span data-stu-id="48ad3-150">String</span></span> | <span data-ttu-id="48ad3-p104">组的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="48ad3-p104">The group's unique identifier. Read-only.</span></span>                                                                                                                                                                 |

## <a name="relationships"></a><span data-ttu-id="48ad3-153">Relationships</span><span class="sxs-lookup"><span data-stu-id="48ad3-153">Relationships</span></span>

| <span data-ttu-id="48ad3-154">关系</span><span class="sxs-lookup"><span data-stu-id="48ad3-154">Relationship</span></span> | <span data-ttu-id="48ad3-155">类型</span><span class="sxs-lookup"><span data-stu-id="48ad3-155">Type</span></span>                               | <span data-ttu-id="48ad3-156">说明</span><span class="sxs-lookup"><span data-stu-id="48ad3-156">Description</span></span>                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="48ad3-157">日历</span><span class="sxs-lookup"><span data-stu-id="48ad3-157">calendars</span></span>    | <span data-ttu-id="48ad3-158">[日历](calendar.md) 集合</span><span class="sxs-lookup"><span data-stu-id="48ad3-158">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="48ad3-p105">日历组中的日历。导航属性。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="48ad3-p105">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="48ad3-163">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="48ad3-163">JSON representation</span></span>

<span data-ttu-id="48ad3-164">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="48ad3-164">Here is a JSON representation of the resource</span></span>

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
