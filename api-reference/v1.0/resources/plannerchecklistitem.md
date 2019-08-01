---
title: plannerChecklistItem 资源类型
description: '**PlannerChecklistItem**资源表示任务清单中的项。 任务上的检查表由 checklistItems 对象表示。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: c1955b0c746ddb3f552428e63ca42dfebe9f5e3c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035292"
---
# <a name="plannerchecklistitem-resource-type"></a><span data-ttu-id="d535d-104">plannerChecklistItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="d535d-104">plannerChecklistItem resource type</span></span>


<span data-ttu-id="d535d-105">**PlannerChecklistItem**资源表示任务清单中的项。</span><span class="sxs-lookup"><span data-stu-id="d535d-105">The **plannerChecklistItem** resource represents an item in the checklist of a task.</span></span> <span data-ttu-id="d535d-106">任务上的检查表由[checklistItems 对象](plannerchecklistitems.md)表示。</span><span class="sxs-lookup"><span data-stu-id="d535d-106">The checklist on a task is represented by the [checklistItems object](plannerchecklistitems.md).</span></span>


## <a name="properties"></a><span data-ttu-id="d535d-107">属性</span><span class="sxs-lookup"><span data-stu-id="d535d-107">Properties</span></span>
| <span data-ttu-id="d535d-108">属性</span><span class="sxs-lookup"><span data-stu-id="d535d-108">Property</span></span>     | <span data-ttu-id="d535d-109">类型</span><span class="sxs-lookup"><span data-stu-id="d535d-109">Type</span></span>   |<span data-ttu-id="d535d-110">说明</span><span class="sxs-lookup"><span data-stu-id="d535d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d535d-111">isChecked</span><span class="sxs-lookup"><span data-stu-id="d535d-111">isChecked</span></span>|<span data-ttu-id="d535d-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="d535d-112">Boolean</span></span>|<span data-ttu-id="d535d-113">Value 是`true`选中该项时为, `false`否则为。</span><span class="sxs-lookup"><span data-stu-id="d535d-113">Value is `true` if the item is checked and `false` otherwise.</span></span>|
|<span data-ttu-id="d535d-114">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="d535d-114">lastModifiedBy</span></span>|[<span data-ttu-id="d535d-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="d535d-115">identitySet</span></span>](identityset.md)| <span data-ttu-id="d535d-116">只读。</span><span class="sxs-lookup"><span data-stu-id="d535d-116">Read-only.</span></span> <span data-ttu-id="d535d-117">上次修改此 ID 的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="d535d-117">User ID by which this is last modified.</span></span>|
|<span data-ttu-id="d535d-118">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d535d-118">lastModifiedDateTime</span></span>|<span data-ttu-id="d535d-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d535d-119">DateTimeOffset</span></span>|<span data-ttu-id="d535d-120">只读。</span><span class="sxs-lookup"><span data-stu-id="d535d-120">Read-only.</span></span> <span data-ttu-id="d535d-121">上次修改的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d535d-121">Date and time at which this is last modified.</span></span> <span data-ttu-id="d535d-122">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="d535d-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d535d-123">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d535d-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d535d-124">orderHint</span><span class="sxs-lookup"><span data-stu-id="d535d-124">orderHint</span></span>|<span data-ttu-id="d535d-125">String</span><span class="sxs-lookup"><span data-stu-id="d535d-125">String</span></span>|<span data-ttu-id="d535d-126">用于设置清单中项的相对顺序。</span><span class="sxs-lookup"><span data-stu-id="d535d-126">Used to set the relative order of items in the checklist.</span></span> <span data-ttu-id="d535d-127">格式定义如下所示。 [](planner-order-hint-format.md)</span><span class="sxs-lookup"><span data-stu-id="d535d-127">The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="d535d-128">title</span><span class="sxs-lookup"><span data-stu-id="d535d-128">title</span></span>|<span data-ttu-id="d535d-129">String</span><span class="sxs-lookup"><span data-stu-id="d535d-129">String</span></span>|<span data-ttu-id="d535d-130">检查表项的标题</span><span class="sxs-lookup"><span data-stu-id="d535d-130">Title of the checklist item</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d535d-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d535d-131">JSON representation</span></span>
<span data-ttu-id="d535d-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d535d-132">Here is a JSON representation of the resource.</span></span>

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
