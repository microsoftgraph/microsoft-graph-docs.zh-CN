---
title: plannerAssignments 资源类型
description: '**PlannerAssignments**资源表示 plannerTask 资源的分配。 此类型为打开的类型。 在这种类型的每个属性名称 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 294e247346d25304a78b35e16530bf6e8791e485
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957828"
---
# <a name="plannerassignments-resource-type"></a><span data-ttu-id="5070f-105">plannerAssignments 资源类型</span><span class="sxs-lookup"><span data-stu-id="5070f-105">plannerAssignments resource type</span></span>

> <span data-ttu-id="5070f-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5070f-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5070f-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5070f-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5070f-p103">**plannerAssignments** 资源表示 [plannerTask](plannertask.md) 资源的分配。此类型是开放类型。此类型中的每个属性名称均是任务被分配到的用户对象的 ID。可以通过新建以用户 ID 命名的属性并将包含 orderHint 属性的 [plannerassignment](plannerassignment.md) 对象填充为其值来向任务分配用户。可以通过将以代理人 ID 命名的属性设置为 null 来在任务中取消分配代理人。</span><span class="sxs-lookup"><span data-stu-id="5070f-p103">The **plannerAssignments** resource represents assignments of a [plannerTask](plannertask.md) resource. This type is an open type. Each property name in this type is the ID of a user object a task is assigned to. The users can be assigned to tasks with creating new properties named with their ID, with a [plannerassignment](plannerassignment.md) object with orderHint property populated as the value. The assignees can be unassigned from the task by setting the propety named with their ID to null.</span></span>


## <a name="properties"></a><span data-ttu-id="5070f-113">属性</span><span class="sxs-lookup"><span data-stu-id="5070f-113">Properties</span></span>
<span data-ttu-id="5070f-p104">开放类型的属性可以由客户端定义。但是在这种情况下，客户必须将分配用户的 ID 作为属性名称。必须将属性设置为 **plannerAssignment** 对象才能创建或修改代理人，必须将其设置为 null 才能删除代理人。</span><span class="sxs-lookup"><span data-stu-id="5070f-p104">Properties of an Open Type can be defined by the client. In this case though, the client must provide assigned user's IDs as property names. The property must be set to a **plannerAssignment** object to create or modify assignees, and to null to remove them.</span></span>

<span data-ttu-id="5070f-117">示例：</span><span class="sxs-lookup"><span data-stu-id="5070f-117">Example:</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAssignments"
}-->

```json
{
  "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47": null,
  "4e98f8f1-bb03-4015-b8e0-19bb370949d8": { 
      "@odata.type": "microsoft.graph.plannerAssignment",
      "orderHint": "String"
    }
}
```
<span data-ttu-id="5070f-p105">该示例将从任务的代理人列表中删除 ID 为 ca2a1df2-e36b-4987-9f6b-0ea462f4eb47 的用户，并更改用户 ID 为 4e98f8f1-bb03-4015-b8e0-19bb370949d8 的代理人顺序。如果尚未将任务分配给 ID 为 4e98f8f1-bb03-4015-b8e0-19bb370949d8 的用户，则使用此值更新分配会将此任务分配给该用户。</span><span class="sxs-lookup"><span data-stu-id="5070f-p105">This example removes user with ID ca2a1df2-e36b-4987-9f6b-0ea462f4eb47 from the assignees list of the task, while changing the order of the assignee with user ID 4e98f8f1-bb03-4015-b8e0-19bb370949d8. If the task isn't already assigned to user with ID 4e98f8f1-bb03-4015-b8e0-19bb370949d8, updating the assignments with this value will assign the task to this user.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignments resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
