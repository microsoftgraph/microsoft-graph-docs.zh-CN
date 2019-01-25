---
title: educationAssignmentPointsGrade 资源类型
description: 当工作分配设置为磅薪等级类型时，每个提交将具有此对象与**submission.grade**属性关联。 这将从 educationAssignmentGrade，创建一个子类
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 5d2a5cf6f6f886185179c6f1a61c1bb1d9d1ecfc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523734"
---
# <a name="educationassignmentpointsgrade-resource-type"></a><span data-ttu-id="ad66a-104">educationAssignmentPointsGrade 资源类型</span><span class="sxs-lookup"><span data-stu-id="ad66a-104">educationAssignmentPointsGrade resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad66a-105">当工作分配设置为磅薪等级类型时，每个提交将具有此对象与**submission.grade**属性关联。</span><span class="sxs-lookup"><span data-stu-id="ad66a-105">When an assignment is set to a points grade type, each submission will have this object associated with the **submission.grade** property.</span></span> <span data-ttu-id="ad66a-106">这将创建一个子类从[educationAssignmentGrade](educationassignmentgrade.md)，其中将 who 将数据添加到此属性。</span><span class="sxs-lookup"><span data-stu-id="ad66a-106">This creates a subclass from [educationAssignmentGrade](educationassignmentgrade.md), which will add the who data to this property.</span></span> <span data-ttu-id="ad66a-107">**Assignments.grading**属性中存储的最大点。</span><span class="sxs-lookup"><span data-stu-id="ad66a-107">The max points is stored in the **assignments.grading** property.</span></span>


## <a name="properties"></a><span data-ttu-id="ad66a-108">属性</span><span class="sxs-lookup"><span data-stu-id="ad66a-108">Properties</span></span>
| <span data-ttu-id="ad66a-109">属性</span><span class="sxs-lookup"><span data-stu-id="ad66a-109">Property</span></span>     | <span data-ttu-id="ad66a-110">类型</span><span class="sxs-lookup"><span data-stu-id="ad66a-110">Type</span></span>   |<span data-ttu-id="ad66a-111">说明</span><span class="sxs-lookup"><span data-stu-id="ad66a-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad66a-112">points</span><span class="sxs-lookup"><span data-stu-id="ad66a-112">points</span></span>|<span data-ttu-id="ad66a-113">单精度</span><span class="sxs-lookup"><span data-stu-id="ad66a-113">Single</span></span>|<span data-ttu-id="ad66a-114">教师的磅数提供此提交对象。</span><span class="sxs-lookup"><span data-stu-id="ad66a-114">Number of points a teacher is giving this submission object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ad66a-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ad66a-115">JSON representation</span></span>

<span data-ttu-id="ad66a-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ad66a-116">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationassignmentpointsgrade.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
