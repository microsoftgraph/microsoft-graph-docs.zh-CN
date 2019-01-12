---
title: plannerAssignment 资源类型
description: '**PlannerAssignment**资源代表分配给用户的任务。 开放类型 plannerAssignments 中使用此类型。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 5eaeb00abf7446db1085a7c0d0916b0a7b5b2434
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963960"
---
# <a name="plannerassignment-resource-type"></a><span data-ttu-id="9b719-104">plannerAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="9b719-104">plannerAssignment resource type</span></span>

> <span data-ttu-id="9b719-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9b719-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b719-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9b719-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9b719-p103">**plannerAssignment** 资源表示针对用户的任务分配。该类型用于开放类型 [plannerAssignments](plannerassignments.md)。</span><span class="sxs-lookup"><span data-stu-id="9b719-p103">The **plannerAssignment** resource represents the assignment of a task to a user. This type is used in the open type [plannerAssignments](plannerassignments.md).</span></span>


## <a name="properties"></a><span data-ttu-id="9b719-109">属性</span><span class="sxs-lookup"><span data-stu-id="9b719-109">Properties</span></span>
| <span data-ttu-id="9b719-110">属性</span><span class="sxs-lookup"><span data-stu-id="9b719-110">Property</span></span>     | <span data-ttu-id="9b719-111">类型</span><span class="sxs-lookup"><span data-stu-id="9b719-111">Type</span></span>   |<span data-ttu-id="9b719-112">说明</span><span class="sxs-lookup"><span data-stu-id="9b719-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9b719-113">assignedBy</span><span class="sxs-lookup"><span data-stu-id="9b719-113">assignedBy</span></span>|[<span data-ttu-id="9b719-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="9b719-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="9b719-115">执行任务分配的用户身份，即委派者。</span><span class="sxs-lookup"><span data-stu-id="9b719-115">The identity of the user that performed the assignment of the task, i.e. the assignor.</span></span>|
|<span data-ttu-id="9b719-116">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="9b719-116">assignedDateTime</span></span>|<span data-ttu-id="9b719-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b719-117">DateTimeOffset</span></span>|<span data-ttu-id="9b719-p104">分配任务的时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9b719-p104">The time at which the task was assigned. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9b719-121">orderHint</span><span class="sxs-lookup"><span data-stu-id="9b719-121">orderHint</span></span>|<span data-ttu-id="9b719-122">String</span><span class="sxs-lookup"><span data-stu-id="9b719-122">String</span></span>|<span data-ttu-id="9b719-p105">用于对任务中的代理人进行排序的提示。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="9b719-p105">Hint used to order assignees in a task. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9b719-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9b719-125">JSON representation</span></span>
<span data-ttu-id="9b719-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9b719-126">Here is a JSON representation of the resource.</span></span>

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
