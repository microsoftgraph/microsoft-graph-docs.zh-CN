---
title: plannerAssignment 资源类型
description: '**plannerAssignment** 资源表示向用户分配任务。 此类型在打开类型 plannerAssignments 中使用。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 2d42e98a2167fb69620ef7cc9d17cb57beffcd7d
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722214"
---
# <a name="plannerassignment-resource-type"></a><span data-ttu-id="6d6dc-104">plannerAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="6d6dc-104">plannerAssignment resource type</span></span>

<span data-ttu-id="6d6dc-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d6dc-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6d6dc-106">**plannerAssignment** 资源表示向用户分配任务。</span><span class="sxs-lookup"><span data-stu-id="6d6dc-106">The **plannerAssignment** resource represents the assignment of a task to a user.</span></span> <span data-ttu-id="6d6dc-107">此类型在打开类型 [plannerAssignments 中使用](plannerassignments.md)。</span><span class="sxs-lookup"><span data-stu-id="6d6dc-107">This type is used in the open type [plannerAssignments](plannerassignments.md).</span></span>


## <a name="properties"></a><span data-ttu-id="6d6dc-108">属性</span><span class="sxs-lookup"><span data-stu-id="6d6dc-108">Properties</span></span>
| <span data-ttu-id="6d6dc-109">属性</span><span class="sxs-lookup"><span data-stu-id="6d6dc-109">Property</span></span>     | <span data-ttu-id="6d6dc-110">类型</span><span class="sxs-lookup"><span data-stu-id="6d6dc-110">Type</span></span>   |<span data-ttu-id="6d6dc-111">说明</span><span class="sxs-lookup"><span data-stu-id="6d6dc-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d6dc-112">assignedBy</span><span class="sxs-lookup"><span data-stu-id="6d6dc-112">assignedBy</span></span>|[<span data-ttu-id="6d6dc-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="6d6dc-113">identitySet</span></span>](identityset.md)|<span data-ttu-id="6d6dc-114">执行任务分配的用户的标识，即分配者。</span><span class="sxs-lookup"><span data-stu-id="6d6dc-114">The identity of the user that performed the assignment of the task, i.e. the assignor.</span></span>|
|<span data-ttu-id="6d6dc-115">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="6d6dc-115">assignedDateTime</span></span>|<span data-ttu-id="6d6dc-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d6dc-116">DateTimeOffset</span></span>|<span data-ttu-id="6d6dc-117">分配任务的时间。</span><span class="sxs-lookup"><span data-stu-id="6d6dc-117">The time at which the task was assigned.</span></span> <span data-ttu-id="6d6dc-118">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="6d6dc-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6d6dc-119">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="6d6dc-119">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="6d6dc-120">orderHint</span><span class="sxs-lookup"><span data-stu-id="6d6dc-120">orderHint</span></span>|<span data-ttu-id="6d6dc-121">String</span><span class="sxs-lookup"><span data-stu-id="6d6dc-121">String</span></span>|<span data-ttu-id="6d6dc-122">用于对任务中的被分配者排序的提示。</span><span class="sxs-lookup"><span data-stu-id="6d6dc-122">Hint used to order assignees in a task.</span></span> <span data-ttu-id="6d6dc-123">格式的定义[如下所述。](planner-order-hint-format.md)</span><span class="sxs-lookup"><span data-stu-id="6d6dc-123">The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6d6dc-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6d6dc-124">JSON representation</span></span>
<span data-ttu-id="6d6dc-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d6dc-125">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

