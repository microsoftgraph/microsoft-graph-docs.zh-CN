---
title: plannerAssignment 资源类型
description: '**PlannerAssignment**资源表示将任务分配给用户。 在开放类型 plannerAssignments 中使用此类型。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 492809e15132294a32834fcbbd90de696e8e219f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971508"
---
# <a name="plannerassignment-resource-type"></a><span data-ttu-id="e096f-104">plannerAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="e096f-104">plannerAssignment resource type</span></span>

<span data-ttu-id="e096f-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e096f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e096f-106">**PlannerAssignment**资源表示将任务分配给用户。</span><span class="sxs-lookup"><span data-stu-id="e096f-106">The **plannerAssignment** resource represents the assignment of a task to a user.</span></span> <span data-ttu-id="e096f-107">在开放类型 [plannerAssignments](plannerassignments.md)中使用此类型。</span><span class="sxs-lookup"><span data-stu-id="e096f-107">This type is used in the open type [plannerAssignments](plannerassignments.md).</span></span>


## <a name="properties"></a><span data-ttu-id="e096f-108">属性</span><span class="sxs-lookup"><span data-stu-id="e096f-108">Properties</span></span>
| <span data-ttu-id="e096f-109">属性</span><span class="sxs-lookup"><span data-stu-id="e096f-109">Property</span></span>     | <span data-ttu-id="e096f-110">类型</span><span class="sxs-lookup"><span data-stu-id="e096f-110">Type</span></span>   |<span data-ttu-id="e096f-111">说明</span><span class="sxs-lookup"><span data-stu-id="e096f-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e096f-112">assignedBy</span><span class="sxs-lookup"><span data-stu-id="e096f-112">assignedBy</span></span>|[<span data-ttu-id="e096f-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="e096f-113">identitySet</span></span>](identityset.md)|<span data-ttu-id="e096f-114">执行任务分配的用户的标识，即 assignor。</span><span class="sxs-lookup"><span data-stu-id="e096f-114">The identity of the user that performed the assignment of the task, i.e. the assignor.</span></span>|
|<span data-ttu-id="e096f-115">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="e096f-115">assignedDateTime</span></span>|<span data-ttu-id="e096f-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e096f-116">DateTimeOffset</span></span>|<span data-ttu-id="e096f-117">任务分配的时间。</span><span class="sxs-lookup"><span data-stu-id="e096f-117">The time at which the task was assigned.</span></span> <span data-ttu-id="e096f-118">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="e096f-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e096f-119">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e096f-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e096f-120">orderHint</span><span class="sxs-lookup"><span data-stu-id="e096f-120">orderHint</span></span>|<span data-ttu-id="e096f-121">String</span><span class="sxs-lookup"><span data-stu-id="e096f-121">String</span></span>|<span data-ttu-id="e096f-122">用于对任务中的工作负责人进行排序的提示。</span><span class="sxs-lookup"><span data-stu-id="e096f-122">Hint used to order assignees in a task.</span></span> <span data-ttu-id="e096f-123">格式[定义如下所示。](planner-order-hint-format.md)</span><span class="sxs-lookup"><span data-stu-id="e096f-123">The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e096f-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e096f-124">JSON representation</span></span>
<span data-ttu-id="e096f-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e096f-125">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAssignment"
}-->

```json
{
  "assignedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "assignedDateTime": "String (timestamp)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


