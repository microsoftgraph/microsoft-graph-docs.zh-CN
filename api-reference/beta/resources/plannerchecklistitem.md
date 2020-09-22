---
title: plannerChecklistItem 资源类型
description: '**PlannerChecklistItem**资源表示任务清单中的项。 任务上的检查表由 checklistItems 对象表示。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 3c60b2727af2fccfdac8e8f9e60e055b0471c861
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046802"
---
# <a name="plannerchecklistitem-resource-type"></a><span data-ttu-id="ab067-104">plannerChecklistItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="ab067-104">plannerChecklistItem resource type</span></span>

<span data-ttu-id="ab067-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab067-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab067-106">**PlannerChecklistItem**资源表示任务清单中的项。</span><span class="sxs-lookup"><span data-stu-id="ab067-106">The **plannerChecklistItem** resource represents an item in the checklist of a task.</span></span> <span data-ttu-id="ab067-107">任务上的检查表由 [checklistItems 对象](plannerchecklistitems.md)表示。</span><span class="sxs-lookup"><span data-stu-id="ab067-107">The checklist on a task is represented by the [checklistItems object](plannerchecklistitems.md).</span></span>


## <a name="properties"></a><span data-ttu-id="ab067-108">属性</span><span class="sxs-lookup"><span data-stu-id="ab067-108">Properties</span></span>
| <span data-ttu-id="ab067-109">属性</span><span class="sxs-lookup"><span data-stu-id="ab067-109">Property</span></span>     | <span data-ttu-id="ab067-110">类型</span><span class="sxs-lookup"><span data-stu-id="ab067-110">Type</span></span>   |<span data-ttu-id="ab067-111">说明</span><span class="sxs-lookup"><span data-stu-id="ab067-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ab067-112">isChecked</span><span class="sxs-lookup"><span data-stu-id="ab067-112">isChecked</span></span>|<span data-ttu-id="ab067-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab067-113">Boolean</span></span>|<span data-ttu-id="ab067-114">Value 是 `true` 选中该项时为， `false` 否则为。</span><span class="sxs-lookup"><span data-stu-id="ab067-114">Value is `true` if the item is checked and `false` otherwise.</span></span>|
|<span data-ttu-id="ab067-115">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="ab067-115">lastModifiedBy</span></span>|[<span data-ttu-id="ab067-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="ab067-116">identitySet</span></span>](identityset.md)| <span data-ttu-id="ab067-117">只读。</span><span class="sxs-lookup"><span data-stu-id="ab067-117">Read-only.</span></span> <span data-ttu-id="ab067-118">上次修改此 ID 的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="ab067-118">User ID by which this is last modified.</span></span>|
|<span data-ttu-id="ab067-119">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ab067-119">lastModifiedDateTime</span></span>|<span data-ttu-id="ab067-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab067-120">DateTimeOffset</span></span>|<span data-ttu-id="ab067-121">只读。</span><span class="sxs-lookup"><span data-stu-id="ab067-121">Read-only.</span></span> <span data-ttu-id="ab067-122">上次修改的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ab067-122">Date and time at which this is last modified.</span></span> <span data-ttu-id="ab067-123">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="ab067-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ab067-124">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ab067-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ab067-125">orderHint</span><span class="sxs-lookup"><span data-stu-id="ab067-125">orderHint</span></span>|<span data-ttu-id="ab067-126">String</span><span class="sxs-lookup"><span data-stu-id="ab067-126">String</span></span>|<span data-ttu-id="ab067-127">用于设置清单中项的相对顺序。</span><span class="sxs-lookup"><span data-stu-id="ab067-127">Used to set the relative order of items in the checklist.</span></span> <span data-ttu-id="ab067-128">格式[定义如下所示。](planner-order-hint-format.md)</span><span class="sxs-lookup"><span data-stu-id="ab067-128">The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="ab067-129">title</span><span class="sxs-lookup"><span data-stu-id="ab067-129">title</span></span>|<span data-ttu-id="ab067-130">String</span><span class="sxs-lookup"><span data-stu-id="ab067-130">String</span></span>|<span data-ttu-id="ab067-131">检查表项的标题</span><span class="sxs-lookup"><span data-stu-id="ab067-131">Title of the checklist item</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ab067-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ab067-132">JSON representation</span></span>
<span data-ttu-id="ab067-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ab067-133">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerChecklistItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


