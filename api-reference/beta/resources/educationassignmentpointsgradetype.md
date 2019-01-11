---
title: educationAssignmentPointsGradeType 资源类型
description: '**Assignments.grading**属性一起使用。 这是 educationAssignmentGradeType 的一个子类。'
localization_priority: Normal
ms.openlocfilehash: f00014eab1dbf7bc8eb78a8898c6abba9977e8a2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860968"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a><span data-ttu-id="6a747-104">educationAssignmentPointsGradeType 资源类型</span><span class="sxs-lookup"><span data-stu-id="6a747-104">educationAssignmentPointsGradeType resource type</span></span>

> <span data-ttu-id="6a747-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6a747-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a747-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6a747-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6a747-107">**Assignments.grading**属性一起使用。</span><span class="sxs-lookup"><span data-stu-id="6a747-107">Used with the **assignments.grading** property.</span></span> <span data-ttu-id="6a747-108">这是[educationAssignmentGradeType](educationassignmentgradetype.md)的一个子类。</span><span class="sxs-lookup"><span data-stu-id="6a747-108">This is a subclass of [educationAssignmentGradeType](educationassignmentgradetype.md).</span></span>

<span data-ttu-id="6a747-109">这表示工作分配的分级范围，并将每个学生可以获得的点的最大数目存储在此工作项。</span><span class="sxs-lookup"><span data-stu-id="6a747-109">This indicates that the assignment is graded and stores the maximum number of points each student can achieve on this work item.</span></span> <span data-ttu-id="6a747-110">当此设置工作分配上时，每个提交将获取与之关联的每个学生的点的存储[educationAssignmentPointsGrade](educationassignmentpointsgrade.md)属性。</span><span class="sxs-lookup"><span data-stu-id="6a747-110">When this is set on an assignment, each submission will get an [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) property associated with it for the storage of each student's points.</span></span>

## <a name="properties"></a><span data-ttu-id="6a747-111">属性</span><span class="sxs-lookup"><span data-stu-id="6a747-111">Properties</span></span>
| <span data-ttu-id="6a747-112">属性</span><span class="sxs-lookup"><span data-stu-id="6a747-112">Property</span></span>     | <span data-ttu-id="6a747-113">类型</span><span class="sxs-lookup"><span data-stu-id="6a747-113">Type</span></span>   |<span data-ttu-id="6a747-114">Description</span><span class="sxs-lookup"><span data-stu-id="6a747-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a747-115">maxPoints</span><span class="sxs-lookup"><span data-stu-id="6a747-115">maxPoints</span></span>|<span data-ttu-id="6a747-116">Single</span><span class="sxs-lookup"><span data-stu-id="6a747-116">Single</span></span>| <span data-ttu-id="6a747-117">最大点可能的此工作分配。</span><span class="sxs-lookup"><span data-stu-id="6a747-117">Max points possible for this assignment.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="6a747-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6a747-118">JSON representation</span></span>

<span data-ttu-id="6a747-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a747-119">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGradeType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
