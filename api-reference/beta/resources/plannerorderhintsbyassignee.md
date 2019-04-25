---
title: plannerOrderHintsByAssignee 资源类型
description: '**plannerOrderHintsByAssignee**是一个资源, 其中包含 plannerTask 资源中的工作负责人的排序提示, 以指示任务的分配对象在任务板中的显示顺序。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 27ef2c796c636e39ed6408c373cf0ac66c5572dd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575924"
---
# <a name="plannerorderhintsbyassignee-resource-type"></a><span data-ttu-id="dcba1-103">plannerOrderHintsByAssignee 资源类型</span><span class="sxs-lookup"><span data-stu-id="dcba1-103">plannerOrderHintsByAssignee resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dcba1-104">**plannerOrderHintsByAssignee**是一个资源, 其中包含[plannerTask](plannertask.md)资源中的工作负责人的[排序提示](planner-order-hint-format.md), 以指示任务的分配对象在任务板中的显示顺序。</span><span class="sxs-lookup"><span data-stu-id="dcba1-104">The **plannerOrderHintsByAssignee** is a resource that contains [ordering hints](planner-order-hint-format.md) for assignees in a [plannerTask](plannertask.md) resource, to indicate the order of the task in Assigned To view of the Task Board.</span></span>
<span data-ttu-id="dcba1-105">此类型是开放类型。</span><span class="sxs-lookup"><span data-stu-id="dcba1-105">This type is an open type.</span></span> <span data-ttu-id="dcba1-106">这些属性是分配给该任务的用户的 id, 并且值是 order 提示。</span><span class="sxs-lookup"><span data-stu-id="dcba1-106">The properties are the ids of users assigned to the task, and the values are order hints.</span></span>

## <a name="properties"></a><span data-ttu-id="dcba1-107">属性</span><span class="sxs-lookup"><span data-stu-id="dcba1-107">Properties</span></span>
<span data-ttu-id="dcba1-108">可由客户端定义打开类型的属性。</span><span class="sxs-lookup"><span data-stu-id="dcba1-108">Properties of an Open Type can be defined by the client.</span></span> <span data-ttu-id="dcba1-109">在这种情况下, 客户端必须提供作为属性名称分配给该任务的用户的 id, 并将有效的[order 提示](planner-order-hint-format.md)作为值。</span><span class="sxs-lookup"><span data-stu-id="dcba1-109">In this case, the client must provide ids of users assigned to the task as property names, and a valid [order hint](planner-order-hint-format.md) as the value.</span></span>
<span data-ttu-id="dcba1-110">无法从此类型中删除属性。</span><span class="sxs-lookup"><span data-stu-id="dcba1-110">Properties cannot be removed from this type.</span></span> <span data-ttu-id="dcba1-111">该服务将自动删除值, 因为更新了包含的[plannerTask](plannertask.md)上的工作分配。</span><span class="sxs-lookup"><span data-stu-id="dcba1-111">The service will automatically remove values as the assignments on the containing [plannerTask](plannertask.md) are updated.</span></span>

<span data-ttu-id="dcba1-112">示例：</span><span class="sxs-lookup"><span data-stu-id="dcba1-112">Example:</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"
}-->

```json
{
  "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47": "String",
  "4e98f8f1-bb03-4015-b8e0-19bb370949d8": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerOrderHintsByAssignee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerorderhintsbyassignee.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
