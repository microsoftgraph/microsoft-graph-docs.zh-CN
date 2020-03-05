---
title: educationAssignmentPointsGradeType 资源类型
description: 与**工作分配. 评分**属性一起使用。 这是 educationAssignmentGradeType 的子类。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2e233faa1ab550c5f970018b6d4bf6879ba99c8f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502471"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a><span data-ttu-id="1c902-104">educationAssignmentPointsGradeType 资源类型</span><span class="sxs-lookup"><span data-stu-id="1c902-104">educationAssignmentPointsGradeType resource type</span></span>

<span data-ttu-id="1c902-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="1c902-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c902-106">与**工作分配. 评分**属性一起使用。</span><span class="sxs-lookup"><span data-stu-id="1c902-106">Used with the **assignments.grading** property.</span></span> <span data-ttu-id="1c902-107">这是[educationAssignmentGradeType](educationassignmentgradetype.md)的子类。</span><span class="sxs-lookup"><span data-stu-id="1c902-107">This is a subclass of [educationAssignmentGradeType](educationassignmentgradetype.md).</span></span>

<span data-ttu-id="1c902-108">这表示将对工作分配进行评分，并存储每个学生可在此工作项上实现的最大分数数。</span><span class="sxs-lookup"><span data-stu-id="1c902-108">This indicates that the assignment is graded and stores the maximum number of points each student can achieve on this work item.</span></span> <span data-ttu-id="1c902-109">在工作分配上设置此设置后，每个提交都将获取一个[educationAssignmentPointsGrade](educationassignmentpointsgrade.md)属性，该属性与每个学生的点数相关联。</span><span class="sxs-lookup"><span data-stu-id="1c902-109">When this is set on an assignment, each submission will get an [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) property associated with it for the storage of each student's points.</span></span>

## <a name="properties"></a><span data-ttu-id="1c902-110">属性</span><span class="sxs-lookup"><span data-stu-id="1c902-110">Properties</span></span>
| <span data-ttu-id="1c902-111">属性</span><span class="sxs-lookup"><span data-stu-id="1c902-111">Property</span></span>     | <span data-ttu-id="1c902-112">类型</span><span class="sxs-lookup"><span data-stu-id="1c902-112">Type</span></span>   |<span data-ttu-id="1c902-113">说明</span><span class="sxs-lookup"><span data-stu-id="1c902-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1c902-114">maxPoints</span><span class="sxs-lookup"><span data-stu-id="1c902-114">maxPoints</span></span>|<span data-ttu-id="1c902-115">单精度</span><span class="sxs-lookup"><span data-stu-id="1c902-115">Single</span></span>| <span data-ttu-id="1c902-116">此工作分配可能的最大分数。</span><span class="sxs-lookup"><span data-stu-id="1c902-116">Max points possible for this assignment.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="1c902-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1c902-117">JSON representation</span></span>

<span data-ttu-id="1c902-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1c902-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentPointsGradeType"
}-->

```json
{
  "maxPoints": "Double"
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
