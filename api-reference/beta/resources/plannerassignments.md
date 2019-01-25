---
title: plannerAssignments 资源类型
description: '**PlannerAssignments**资源表示 plannerTask 资源的分配。 此类型为打开的类型。 在这种类型的每个属性名称 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 2c379c786e3b94395aa3de7bc382e184db0fcc24
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507766"
---
# <a name="plannerassignments-resource-type"></a><span data-ttu-id="d2f54-105">plannerAssignments 资源类型</span><span class="sxs-lookup"><span data-stu-id="d2f54-105">plannerAssignments resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2f54-p102">**plannerAssignments** 资源表示 [plannerTask](plannertask.md) 资源的分配。此类型是开放类型。此类型中的每个属性名称均是任务被分配到的用户对象的 ID。可以通过新建以用户 ID 命名的属性并将包含 orderHint 属性的 [plannerassignment](plannerassignment.md) 对象填充为其值来向任务分配用户。可以通过将以代理人 ID 命名的属性设置为 null 来在任务中取消分配代理人。</span><span class="sxs-lookup"><span data-stu-id="d2f54-p102">The **plannerAssignments** resource represents assignments of a [plannerTask](plannertask.md) resource. This type is an open type. Each property name in this type is the ID of a user object a task is assigned to. The users can be assigned to tasks with creating new properties named with their ID, with a [plannerassignment](plannerassignment.md) object with orderHint property populated as the value. The assignees can be unassigned from the task by setting the propety named with their ID to null.</span></span>


## <a name="properties"></a><span data-ttu-id="d2f54-111">属性</span><span class="sxs-lookup"><span data-stu-id="d2f54-111">Properties</span></span>
<span data-ttu-id="d2f54-p103">开放类型的属性可以由客户端定义。但是在这种情况下，客户必须将分配用户的 ID 作为属性名称。必须将属性设置为 **plannerAssignment** 对象才能创建或修改代理人，必须将其设置为 null 才能删除代理人。</span><span class="sxs-lookup"><span data-stu-id="d2f54-p103">Properties of an Open Type can be defined by the client. In this case though, the client must provide assigned user's IDs as property names. The property must be set to a **plannerAssignment** object to create or modify assignees, and to null to remove them.</span></span>

<span data-ttu-id="d2f54-115">示例：</span><span class="sxs-lookup"><span data-stu-id="d2f54-115">Example:</span></span>

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
<span data-ttu-id="d2f54-p104">该示例将从任务的代理人列表中删除 ID 为 ca2a1df2-e36b-4987-9f6b-0ea462f4eb47 的用户，并更改用户 ID 为 4e98f8f1-bb03-4015-b8e0-19bb370949d8 的代理人顺序。如果尚未将任务分配给 ID 为 4e98f8f1-bb03-4015-b8e0-19bb370949d8 的用户，则使用此值更新分配会将此任务分配给该用户。</span><span class="sxs-lookup"><span data-stu-id="d2f54-p104">This example removes user with ID ca2a1df2-e36b-4987-9f6b-0ea462f4eb47 from the assignees list of the task, while changing the order of the assignee with user ID 4e98f8f1-bb03-4015-b8e0-19bb370949d8. If the task isn't already assigned to user with ID 4e98f8f1-bb03-4015-b8e0-19bb370949d8, updating the assignments with this value will assign the task to this user.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerAssignments resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerassignments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
