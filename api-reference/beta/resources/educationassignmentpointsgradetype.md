---
title: educationAssignmentPointsGradeType 资源类型
description: '**Assignments.grading**属性一起使用。 这是 educationAssignmentGradeType 的一个子类。'
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 567bff38f8a20456dffffdd91775a1e32852fe20
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508893"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a><span data-ttu-id="06a33-104">educationAssignmentPointsGradeType 资源类型</span><span class="sxs-lookup"><span data-stu-id="06a33-104">educationAssignmentPointsGradeType resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06a33-105">**Assignments.grading**属性一起使用。</span><span class="sxs-lookup"><span data-stu-id="06a33-105">Used with the **assignments.grading** property.</span></span> <span data-ttu-id="06a33-106">这是[educationAssignmentGradeType](educationassignmentgradetype.md)的一个子类。</span><span class="sxs-lookup"><span data-stu-id="06a33-106">This is a subclass of [educationAssignmentGradeType](educationassignmentgradetype.md).</span></span>

<span data-ttu-id="06a33-107">这表示工作分配的分级范围，并将每个学生可以获得的点的最大数目存储在此工作项。</span><span class="sxs-lookup"><span data-stu-id="06a33-107">This indicates that the assignment is graded and stores the maximum number of points each student can achieve on this work item.</span></span> <span data-ttu-id="06a33-108">当此设置工作分配上时，每个提交将获取与之关联的每个学生的点的存储[educationAssignmentPointsGrade](educationassignmentpointsgrade.md)属性。</span><span class="sxs-lookup"><span data-stu-id="06a33-108">When this is set on an assignment, each submission will get an [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) property associated with it for the storage of each student's points.</span></span>

## <a name="properties"></a><span data-ttu-id="06a33-109">属性</span><span class="sxs-lookup"><span data-stu-id="06a33-109">Properties</span></span>
| <span data-ttu-id="06a33-110">属性</span><span class="sxs-lookup"><span data-stu-id="06a33-110">Property</span></span>     | <span data-ttu-id="06a33-111">类型</span><span class="sxs-lookup"><span data-stu-id="06a33-111">Type</span></span>   |<span data-ttu-id="06a33-112">说明</span><span class="sxs-lookup"><span data-stu-id="06a33-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06a33-113">maxPoints</span><span class="sxs-lookup"><span data-stu-id="06a33-113">maxPoints</span></span>|<span data-ttu-id="06a33-114">单精度</span><span class="sxs-lookup"><span data-stu-id="06a33-114">Single</span></span>| <span data-ttu-id="06a33-115">最大点可能的此工作分配。</span><span class="sxs-lookup"><span data-stu-id="06a33-115">Max points possible for this assignment.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="06a33-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="06a33-116">JSON representation</span></span>

<span data-ttu-id="06a33-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06a33-117">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationassignmentpointsgradetype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
