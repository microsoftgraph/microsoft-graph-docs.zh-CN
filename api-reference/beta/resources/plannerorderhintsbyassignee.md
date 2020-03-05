---
title: plannerOrderHintsByAssignee 资源类型
description: '**PlannerOrderHintsByAssignee**是一个资源，其中包含 plannerTask 资源中的工作负责人的排序提示，以指示任务的分配对象在任务板中的显示顺序。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 3fc3e8a67e92091b5e273d45c483751c63dbbf0a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521718"
---
# <a name="plannerorderhintsbyassignee-resource-type"></a><span data-ttu-id="f63f3-103">plannerOrderHintsByAssignee 资源类型</span><span class="sxs-lookup"><span data-stu-id="f63f3-103">plannerOrderHintsByAssignee resource type</span></span>

<span data-ttu-id="f63f3-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f63f3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f63f3-105">**PlannerOrderHintsByAssignee**是一个资源，其中包含[plannerTask](plannertask.md)资源中的工作负责人的[排序提示](planner-order-hint-format.md)，以指示任务的分配对象在任务板中的显示顺序。</span><span class="sxs-lookup"><span data-stu-id="f63f3-105">The **plannerOrderHintsByAssignee** is a resource that contains [ordering hints](planner-order-hint-format.md) for assignees in a [plannerTask](plannertask.md) resource, to indicate the order of the task in Assigned To view of the Task Board.</span></span>
<span data-ttu-id="f63f3-106">此类型是开放类型。</span><span class="sxs-lookup"><span data-stu-id="f63f3-106">This type is an open type.</span></span> <span data-ttu-id="f63f3-107">这些属性是分配给该任务的用户的 id，并且值是 order 提示。</span><span class="sxs-lookup"><span data-stu-id="f63f3-107">The properties are the ids of users assigned to the task, and the values are order hints.</span></span>

## <a name="properties"></a><span data-ttu-id="f63f3-108">属性</span><span class="sxs-lookup"><span data-stu-id="f63f3-108">Properties</span></span>
<span data-ttu-id="f63f3-109">可由客户端定义打开类型的属性。</span><span class="sxs-lookup"><span data-stu-id="f63f3-109">Properties of an Open Type can be defined by the client.</span></span> <span data-ttu-id="f63f3-110">在这种情况下，客户端必须提供作为属性名称分配给该任务的用户的 id，并将有效的[order 提示](planner-order-hint-format.md)作为值。</span><span class="sxs-lookup"><span data-stu-id="f63f3-110">In this case, the client must provide ids of users assigned to the task as property names, and a valid [order hint](planner-order-hint-format.md) as the value.</span></span>
<span data-ttu-id="f63f3-111">无法从此类型中删除属性。</span><span class="sxs-lookup"><span data-stu-id="f63f3-111">Properties cannot be removed from this type.</span></span> <span data-ttu-id="f63f3-112">该服务将自动删除值，因为更新了包含的[plannerTask](plannertask.md)上的工作分配。</span><span class="sxs-lookup"><span data-stu-id="f63f3-112">The service will automatically remove values as the assignments on the containing [plannerTask](plannertask.md) are updated.</span></span>

<span data-ttu-id="f63f3-113">示例：</span><span class="sxs-lookup"><span data-stu-id="f63f3-113">Example:</span></span>

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
  "suppressions": []
}
-->
