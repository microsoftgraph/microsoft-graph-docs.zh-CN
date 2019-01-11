---
title: plannerChecklistItem 资源类型
description: '**PlannerChecklistItem**资源表示任务的清单中的项。 由 checklistItems 对象代表对任务的清单。'
localization_priority: Normal
ms.openlocfilehash: 116d85ecfad403409933ea485c71dd0f1ebeae9b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866477"
---
# <a name="plannerchecklistitem-resource-type"></a><span data-ttu-id="45593-104">plannerChecklistItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="45593-104">plannerChecklistItem resource type</span></span>

> <span data-ttu-id="45593-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="45593-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="45593-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="45593-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="45593-p103">**plannerChecklistItem** 资源表示任务的检查表中的项目。任务上的检查表由 [checklistItems 对象](plannerchecklistitems.md)表示。</span><span class="sxs-lookup"><span data-stu-id="45593-p103">The **plannerChecklistItem** resource represents an item in the checklist of a task. The checklist on a task is represented by the [checklistItems object](plannerchecklistitems.md).</span></span>


## <a name="properties"></a><span data-ttu-id="45593-109">属性</span><span class="sxs-lookup"><span data-stu-id="45593-109">Properties</span></span>
| <span data-ttu-id="45593-110">属性</span><span class="sxs-lookup"><span data-stu-id="45593-110">Property</span></span>     | <span data-ttu-id="45593-111">类型</span><span class="sxs-lookup"><span data-stu-id="45593-111">Type</span></span>   |<span data-ttu-id="45593-112">说明</span><span class="sxs-lookup"><span data-stu-id="45593-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="45593-113">isChecked</span><span class="sxs-lookup"><span data-stu-id="45593-113">isChecked</span></span>|<span data-ttu-id="45593-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="45593-114">Boolean</span></span>|<span data-ttu-id="45593-115">如果已检查此项目，值则为 `true`，否则为 `false`。</span><span class="sxs-lookup"><span data-stu-id="45593-115">Value is `true` if the item is checked and `false` otherwise.</span></span>|
|<span data-ttu-id="45593-116">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="45593-116">lastModifiedBy</span></span>|[<span data-ttu-id="45593-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="45593-117">identitySet</span></span>](identityset.md)| <span data-ttu-id="45593-p104">只读。上一次修改它的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="45593-p104">Read-only. User ID by which this is last modified.</span></span>|
|<span data-ttu-id="45593-120">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="45593-120">lastModifiedDateTime</span></span>|<span data-ttu-id="45593-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45593-121">DateTimeOffset</span></span>|<span data-ttu-id="45593-p105">只读。上一次修改它的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="45593-p105">Read-only. Date and time at which this is last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="45593-126">orderHint</span><span class="sxs-lookup"><span data-stu-id="45593-126">orderHint</span></span>|<span data-ttu-id="45593-127">String</span><span class="sxs-lookup"><span data-stu-id="45593-127">String</span></span>|<span data-ttu-id="45593-p106">用于设置检查表中的项目的相对顺序。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="45593-p106">Used to set the relative order of items in the checklist. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="45593-130">title</span><span class="sxs-lookup"><span data-stu-id="45593-130">title</span></span>|<span data-ttu-id="45593-131">String</span><span class="sxs-lookup"><span data-stu-id="45593-131">String</span></span>|<span data-ttu-id="45593-132">检查表项目的标题</span><span class="sxs-lookup"><span data-stu-id="45593-132">Title of the checklist item</span></span>|

## <a name="json-representation"></a><span data-ttu-id="45593-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="45593-133">JSON representation</span></span>
<span data-ttu-id="45593-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="45593-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerChecklistItem"
}-->

```json
{
  "isChecked": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "orderHint": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerChecklistItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
