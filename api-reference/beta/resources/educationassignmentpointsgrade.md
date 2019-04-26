---
title: educationAssignmentPointsGrade 资源类型
description: 当工作分配设置为 "点" 评分类型时, 每个提交都将具有与 "**提交. 年级**" 属性相关联的此对象。 这将从 educationAssignmentGrade 中创建一个子类,
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 166f6b5ce377441641cf12232c2194dff1184765
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340576"
---
# <a name="educationassignmentpointsgrade-resource-type"></a><span data-ttu-id="6c6ed-104">educationAssignmentPointsGrade 资源类型</span><span class="sxs-lookup"><span data-stu-id="6c6ed-104">educationAssignmentPointsGrade resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c6ed-105">当工作分配设置为 "点" 评分类型时, 每个提交都将具有与 "**提交. 年级**" 属性相关联的此对象。</span><span class="sxs-lookup"><span data-stu-id="6c6ed-105">When an assignment is set to a points grade type, each submission will have this object associated with the **submission.grade** property.</span></span> <span data-ttu-id="6c6ed-106">这将从[educationAssignmentGrade](educationassignmentgrade.md)创建一个子类, 该子类将向此属性添加数据。</span><span class="sxs-lookup"><span data-stu-id="6c6ed-106">This creates a subclass from [educationAssignmentGrade](educationassignmentgrade.md), which will add the who data to this property.</span></span> <span data-ttu-id="6c6ed-107">最大分数存储在**工作分配. 评分**属性中。</span><span class="sxs-lookup"><span data-stu-id="6c6ed-107">The max points is stored in the **assignments.grading** property.</span></span>


## <a name="properties"></a><span data-ttu-id="6c6ed-108">属性</span><span class="sxs-lookup"><span data-stu-id="6c6ed-108">Properties</span></span>
| <span data-ttu-id="6c6ed-109">属性</span><span class="sxs-lookup"><span data-stu-id="6c6ed-109">Property</span></span>     | <span data-ttu-id="6c6ed-110">类型</span><span class="sxs-lookup"><span data-stu-id="6c6ed-110">Type</span></span>   |<span data-ttu-id="6c6ed-111">说明</span><span class="sxs-lookup"><span data-stu-id="6c6ed-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c6ed-112">points</span><span class="sxs-lookup"><span data-stu-id="6c6ed-112">points</span></span>|<span data-ttu-id="6c6ed-113">单精度</span><span class="sxs-lookup"><span data-stu-id="6c6ed-113">Single</span></span>|<span data-ttu-id="6c6ed-114">教师向此提交对象提供的积分数。</span><span class="sxs-lookup"><span data-stu-id="6c6ed-114">Number of points a teacher is giving this submission object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6c6ed-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6c6ed-115">JSON representation</span></span>

<span data-ttu-id="6c6ed-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c6ed-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentPointsGrade"
}-->

```json
{
  "points": "Single"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
