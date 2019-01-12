---
title: educationAssignmentPointsGradeType 资源类型
description: '**Assignments.grading**属性一起使用。 这是 educationAssignmentGradeType 的一个子类。'
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: b603ccec0ddd5be5003353a5062e51554cb61c53
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952662"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a><span data-ttu-id="28ebd-104">educationAssignmentPointsGradeType 资源类型</span><span class="sxs-lookup"><span data-stu-id="28ebd-104">educationAssignmentPointsGradeType resource type</span></span>

> <span data-ttu-id="28ebd-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="28ebd-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="28ebd-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="28ebd-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="28ebd-107">**Assignments.grading**属性一起使用。</span><span class="sxs-lookup"><span data-stu-id="28ebd-107">Used with the **assignments.grading** property.</span></span> <span data-ttu-id="28ebd-108">这是[educationAssignmentGradeType](educationassignmentgradetype.md)的一个子类。</span><span class="sxs-lookup"><span data-stu-id="28ebd-108">This is a subclass of [educationAssignmentGradeType](educationassignmentgradetype.md).</span></span>

<span data-ttu-id="28ebd-109">这表示工作分配的分级范围，并将每个学生可以获得的点的最大数目存储在此工作项。</span><span class="sxs-lookup"><span data-stu-id="28ebd-109">This indicates that the assignment is graded and stores the maximum number of points each student can achieve on this work item.</span></span> <span data-ttu-id="28ebd-110">当此设置工作分配上时，每个提交将获取与之关联的每个学生的点的存储[educationAssignmentPointsGrade](educationassignmentpointsgrade.md)属性。</span><span class="sxs-lookup"><span data-stu-id="28ebd-110">When this is set on an assignment, each submission will get an [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) property associated with it for the storage of each student's points.</span></span>

## <a name="properties"></a><span data-ttu-id="28ebd-111">属性</span><span class="sxs-lookup"><span data-stu-id="28ebd-111">Properties</span></span>
| <span data-ttu-id="28ebd-112">属性</span><span class="sxs-lookup"><span data-stu-id="28ebd-112">Property</span></span>     | <span data-ttu-id="28ebd-113">类型</span><span class="sxs-lookup"><span data-stu-id="28ebd-113">Type</span></span>   |<span data-ttu-id="28ebd-114">说明</span><span class="sxs-lookup"><span data-stu-id="28ebd-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28ebd-115">maxPoints</span><span class="sxs-lookup"><span data-stu-id="28ebd-115">maxPoints</span></span>|<span data-ttu-id="28ebd-116">Single</span><span class="sxs-lookup"><span data-stu-id="28ebd-116">Single</span></span>| <span data-ttu-id="28ebd-117">最大点可能的此工作分配。</span><span class="sxs-lookup"><span data-stu-id="28ebd-117">Max points possible for this assignment.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="28ebd-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="28ebd-118">JSON representation</span></span>

<span data-ttu-id="28ebd-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="28ebd-119">The following is a JSON representation of the resource.</span></span>

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
