---
title: educationAssignmentPointsGradeType 资源类型
description: 与**工作分配. 评分**属性一起使用。 这是 educationAssignmentGradeType 的子类。
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 61e6e425730685d4447875cdb074526e7ebc0a17
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334428"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a><span data-ttu-id="c10c6-104">educationAssignmentPointsGradeType 资源类型</span><span class="sxs-lookup"><span data-stu-id="c10c6-104">educationAssignmentPointsGradeType resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c10c6-105">与**工作分配. 评分**属性一起使用。</span><span class="sxs-lookup"><span data-stu-id="c10c6-105">Used with the **assignments.grading** property.</span></span> <span data-ttu-id="c10c6-106">这是[educationAssignmentGradeType](educationassignmentgradetype.md)的子类。</span><span class="sxs-lookup"><span data-stu-id="c10c6-106">This is a subclass of [educationAssignmentGradeType](educationassignmentgradetype.md).</span></span>

<span data-ttu-id="c10c6-107">这表示将对工作分配进行评分, 并存储每个学生可在此工作项上实现的最大分数数。</span><span class="sxs-lookup"><span data-stu-id="c10c6-107">This indicates that the assignment is graded and stores the maximum number of points each student can achieve on this work item.</span></span> <span data-ttu-id="c10c6-108">在工作分配上设置此设置后, 每个提交都将获取一个[educationAssignmentPointsGrade](educationassignmentpointsgrade.md)属性, 该属性与每个学生的点数相关联。</span><span class="sxs-lookup"><span data-stu-id="c10c6-108">When this is set on an assignment, each submission will get an [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) property associated with it for the storage of each student's points.</span></span>

## <a name="properties"></a><span data-ttu-id="c10c6-109">属性</span><span class="sxs-lookup"><span data-stu-id="c10c6-109">Properties</span></span>
| <span data-ttu-id="c10c6-110">属性</span><span class="sxs-lookup"><span data-stu-id="c10c6-110">Property</span></span>     | <span data-ttu-id="c10c6-111">类型</span><span class="sxs-lookup"><span data-stu-id="c10c6-111">Type</span></span>   |<span data-ttu-id="c10c6-112">说明</span><span class="sxs-lookup"><span data-stu-id="c10c6-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c10c6-113">maxPoints</span><span class="sxs-lookup"><span data-stu-id="c10c6-113">maxPoints</span></span>|<span data-ttu-id="c10c6-114">单精度</span><span class="sxs-lookup"><span data-stu-id="c10c6-114">Single</span></span>| <span data-ttu-id="c10c6-115">此工作分配可能的最大分数。</span><span class="sxs-lookup"><span data-stu-id="c10c6-115">Max points possible for this assignment.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="c10c6-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c10c6-116">JSON representation</span></span>

<span data-ttu-id="c10c6-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c10c6-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentPointsGradeType"
}-->

```json
{
  "maxPoints": "Single"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGradeType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
