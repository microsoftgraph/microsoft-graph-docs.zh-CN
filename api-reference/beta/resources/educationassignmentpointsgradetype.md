---
title: educationAssignmentPointsGradeType 资源类型
description: 与**工作分配. 评分**属性一起使用。 这是 educationAssignmentGradeType 的子类。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 18661c6d0eb0269f429fe22203b59b4f6862f21c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972801"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a><span data-ttu-id="a7870-104">educationAssignmentPointsGradeType 资源类型</span><span class="sxs-lookup"><span data-stu-id="a7870-104">educationAssignmentPointsGradeType resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7870-105">与**工作分配. 评分**属性一起使用。</span><span class="sxs-lookup"><span data-stu-id="a7870-105">Used with the **assignments.grading** property.</span></span> <span data-ttu-id="a7870-106">这是[educationAssignmentGradeType](educationassignmentgradetype.md)的子类。</span><span class="sxs-lookup"><span data-stu-id="a7870-106">This is a subclass of [educationAssignmentGradeType](educationassignmentgradetype.md).</span></span>

<span data-ttu-id="a7870-107">这表示将对工作分配进行评分, 并存储每个学生可在此工作项上实现的最大分数数。</span><span class="sxs-lookup"><span data-stu-id="a7870-107">This indicates that the assignment is graded and stores the maximum number of points each student can achieve on this work item.</span></span> <span data-ttu-id="a7870-108">在工作分配上设置此设置后, 每个提交都将获取一个[educationAssignmentPointsGrade](educationassignmentpointsgrade.md)属性, 该属性与每个学生的点数相关联。</span><span class="sxs-lookup"><span data-stu-id="a7870-108">When this is set on an assignment, each submission will get an [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) property associated with it for the storage of each student's points.</span></span>

## <a name="properties"></a><span data-ttu-id="a7870-109">属性</span><span class="sxs-lookup"><span data-stu-id="a7870-109">Properties</span></span>
| <span data-ttu-id="a7870-110">属性</span><span class="sxs-lookup"><span data-stu-id="a7870-110">Property</span></span>     | <span data-ttu-id="a7870-111">类型</span><span class="sxs-lookup"><span data-stu-id="a7870-111">Type</span></span>   |<span data-ttu-id="a7870-112">说明</span><span class="sxs-lookup"><span data-stu-id="a7870-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a7870-113">maxPoints</span><span class="sxs-lookup"><span data-stu-id="a7870-113">maxPoints</span></span>|<span data-ttu-id="a7870-114">单精度</span><span class="sxs-lookup"><span data-stu-id="a7870-114">Single</span></span>| <span data-ttu-id="a7870-115">此工作分配可能的最大分数。</span><span class="sxs-lookup"><span data-stu-id="a7870-115">Max points possible for this assignment.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="a7870-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a7870-116">JSON representation</span></span>

<span data-ttu-id="a7870-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a7870-117">The following is a JSON representation of the resource.</span></span>

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
