---
title: plannerChecklistItem 资源类型
description: '**plannerChecklistItem** 资源表示任务清单中的一个项目。 任务上的清单由 checklistItems 对象表示。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 724694c2348c250be5396f5a5be5e4f4eb2d7e04
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722319"
---
# <a name="plannerchecklistitem-resource-type"></a><span data-ttu-id="d0d3d-104">plannerChecklistItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="d0d3d-104">plannerChecklistItem resource type</span></span>

<span data-ttu-id="d0d3d-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0d3d-105">Namespace: microsoft.graph</span></span>


<span data-ttu-id="d0d3d-106">**plannerChecklistItem** 资源表示任务清单中的一个项目。</span><span class="sxs-lookup"><span data-stu-id="d0d3d-106">The **plannerChecklistItem** resource represents an item in the checklist of a task.</span></span> <span data-ttu-id="d0d3d-107">任务上的清单由 [checklistItems](plannerchecklistitems.md)对象表示。</span><span class="sxs-lookup"><span data-stu-id="d0d3d-107">The checklist on a task is represented by the [checklistItems object](plannerchecklistitems.md).</span></span>


## <a name="properties"></a><span data-ttu-id="d0d3d-108">属性</span><span class="sxs-lookup"><span data-stu-id="d0d3d-108">Properties</span></span>
| <span data-ttu-id="d0d3d-109">属性</span><span class="sxs-lookup"><span data-stu-id="d0d3d-109">Property</span></span>     | <span data-ttu-id="d0d3d-110">类型</span><span class="sxs-lookup"><span data-stu-id="d0d3d-110">Type</span></span>   |<span data-ttu-id="d0d3d-111">说明</span><span class="sxs-lookup"><span data-stu-id="d0d3d-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d0d3d-112">isChecked</span><span class="sxs-lookup"><span data-stu-id="d0d3d-112">isChecked</span></span>|<span data-ttu-id="d0d3d-113">布尔值</span><span class="sxs-lookup"><span data-stu-id="d0d3d-113">Boolean</span></span>|<span data-ttu-id="d0d3d-114">如果项目 `true` 已选中，则值为 ，否则 `false` 为 。</span><span class="sxs-lookup"><span data-stu-id="d0d3d-114">Value is `true` if the item is checked and `false` otherwise.</span></span>|
|<span data-ttu-id="d0d3d-115">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="d0d3d-115">lastModifiedBy</span></span>|[<span data-ttu-id="d0d3d-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="d0d3d-116">identitySet</span></span>](identityset.md)| <span data-ttu-id="d0d3d-117">只读。</span><span class="sxs-lookup"><span data-stu-id="d0d3d-117">Read-only.</span></span> <span data-ttu-id="d0d3d-118">上次修改的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="d0d3d-118">User ID by which this is last modified.</span></span>|
|<span data-ttu-id="d0d3d-119">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d0d3d-119">lastModifiedDateTime</span></span>|<span data-ttu-id="d0d3d-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0d3d-120">DateTimeOffset</span></span>|<span data-ttu-id="d0d3d-121">只读。</span><span class="sxs-lookup"><span data-stu-id="d0d3d-121">Read-only.</span></span> <span data-ttu-id="d0d3d-122">上次修改的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d0d3d-122">Date and time at which this is last modified.</span></span> <span data-ttu-id="d0d3d-123">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="d0d3d-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d0d3d-124">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="d0d3d-124">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="d0d3d-125">orderHint</span><span class="sxs-lookup"><span data-stu-id="d0d3d-125">orderHint</span></span>|<span data-ttu-id="d0d3d-126">String</span><span class="sxs-lookup"><span data-stu-id="d0d3d-126">String</span></span>|<span data-ttu-id="d0d3d-127">用于设置清单中项目的相对顺序。</span><span class="sxs-lookup"><span data-stu-id="d0d3d-127">Used to set the relative order of items in the checklist.</span></span> <span data-ttu-id="d0d3d-128">格式的定义[如下所述。](planner-order-hint-format.md)</span><span class="sxs-lookup"><span data-stu-id="d0d3d-128">The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="d0d3d-129">title</span><span class="sxs-lookup"><span data-stu-id="d0d3d-129">title</span></span>|<span data-ttu-id="d0d3d-130">String</span><span class="sxs-lookup"><span data-stu-id="d0d3d-130">String</span></span>|<span data-ttu-id="d0d3d-131">清单项的标题</span><span class="sxs-lookup"><span data-stu-id="d0d3d-131">Title of the checklist item</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d0d3d-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d0d3d-132">JSON representation</span></span>
<span data-ttu-id="d0d3d-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d0d3d-133">Here is a JSON representation of the resource.</span></span>

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

