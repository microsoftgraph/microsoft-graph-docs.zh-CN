---
title: plannerAssignment 资源类型
description: '**plannerAssignment**资源表示将任务分配给用户。 在开放类型 plannerAssignments 中使用此类型。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 054cd42eedd27a7fe11abc2e5578a56da667e05d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541358"
---
# <a name="plannerassignment-resource-type"></a><span data-ttu-id="9e002-104">plannerAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="9e002-104">plannerAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e002-105">**plannerAssignment**资源表示将任务分配给用户。</span><span class="sxs-lookup"><span data-stu-id="9e002-105">The **plannerAssignment** resource represents the assignment of a task to a user.</span></span> <span data-ttu-id="9e002-106">在开放类型[plannerAssignments](plannerassignments.md)中使用此类型。</span><span class="sxs-lookup"><span data-stu-id="9e002-106">This type is used in the open type [plannerAssignments](plannerassignments.md).</span></span>


## <a name="properties"></a><span data-ttu-id="9e002-107">属性</span><span class="sxs-lookup"><span data-stu-id="9e002-107">Properties</span></span>
| <span data-ttu-id="9e002-108">属性</span><span class="sxs-lookup"><span data-stu-id="9e002-108">Property</span></span>     | <span data-ttu-id="9e002-109">类型</span><span class="sxs-lookup"><span data-stu-id="9e002-109">Type</span></span>   |<span data-ttu-id="9e002-110">说明</span><span class="sxs-lookup"><span data-stu-id="9e002-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e002-111">assignedBy</span><span class="sxs-lookup"><span data-stu-id="9e002-111">assignedBy</span></span>|[<span data-ttu-id="9e002-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="9e002-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="9e002-113">执行任务分配的用户的标识, 即 assignor。</span><span class="sxs-lookup"><span data-stu-id="9e002-113">The identity of the user that performed the assignment of the task, i.e. the assignor.</span></span>|
|<span data-ttu-id="9e002-114">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="9e002-114">assignedDateTime</span></span>|<span data-ttu-id="9e002-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e002-115">DateTimeOffset</span></span>|<span data-ttu-id="9e002-116">任务分配的时间。</span><span class="sxs-lookup"><span data-stu-id="9e002-116">The time at which the task was assigned.</span></span> <span data-ttu-id="9e002-117">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="9e002-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9e002-118">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9e002-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9e002-119">orderHint</span><span class="sxs-lookup"><span data-stu-id="9e002-119">orderHint</span></span>|<span data-ttu-id="9e002-120">String</span><span class="sxs-lookup"><span data-stu-id="9e002-120">String</span></span>|<span data-ttu-id="9e002-121">用于对任务中的工作负责人进行排序的提示。</span><span class="sxs-lookup"><span data-stu-id="9e002-121">Hint used to order assignees in a task.</span></span> <span data-ttu-id="9e002-122">格式定义如下所示。 [](planner-order-hint-format.md)</span><span class="sxs-lookup"><span data-stu-id="9e002-122">The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9e002-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9e002-123">JSON representation</span></span>
<span data-ttu-id="9e002-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e002-124">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerassignment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
