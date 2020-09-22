---
title: educationAssignmentPointsGradeType 资源类型
description: 与 **工作分配. 评分** 属性一起使用。 这是 educationAssignmentGradeType 的子类。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b11ba94bba2147e2ef1d084a66cd7628371a57fa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998885"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a><span data-ttu-id="b74bc-104">educationAssignmentPointsGradeType 资源类型</span><span class="sxs-lookup"><span data-stu-id="b74bc-104">educationAssignmentPointsGradeType resource type</span></span>

<span data-ttu-id="b74bc-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b74bc-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b74bc-106">与 **工作分配. 评分** 属性一起使用。</span><span class="sxs-lookup"><span data-stu-id="b74bc-106">Used with the **assignments.grading** property.</span></span> <span data-ttu-id="b74bc-107">这是 [educationAssignmentGradeType](educationassignmentgradetype.md)的子类。</span><span class="sxs-lookup"><span data-stu-id="b74bc-107">This is a subclass of [educationAssignmentGradeType](educationassignmentgradetype.md).</span></span>

<span data-ttu-id="b74bc-108">这表示将对工作分配进行评分，并存储每个学生可在此工作项上实现的最大分数数。</span><span class="sxs-lookup"><span data-stu-id="b74bc-108">This indicates that the assignment is graded and stores the maximum number of points each student can achieve on this work item.</span></span> <span data-ttu-id="b74bc-109">在工作分配上设置此设置后，每个提交都将获取一个 [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) 属性，该属性与每个学生的点数相关联。</span><span class="sxs-lookup"><span data-stu-id="b74bc-109">When this is set on an assignment, each submission will get an [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) property associated with it for the storage of each student's points.</span></span>

## <a name="properties"></a><span data-ttu-id="b74bc-110">属性</span><span class="sxs-lookup"><span data-stu-id="b74bc-110">Properties</span></span>
| <span data-ttu-id="b74bc-111">属性</span><span class="sxs-lookup"><span data-stu-id="b74bc-111">Property</span></span>     | <span data-ttu-id="b74bc-112">类型</span><span class="sxs-lookup"><span data-stu-id="b74bc-112">Type</span></span>   |<span data-ttu-id="b74bc-113">说明</span><span class="sxs-lookup"><span data-stu-id="b74bc-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b74bc-114">maxPoints</span><span class="sxs-lookup"><span data-stu-id="b74bc-114">maxPoints</span></span>|<span data-ttu-id="b74bc-115">单一</span><span class="sxs-lookup"><span data-stu-id="b74bc-115">Single</span></span>| <span data-ttu-id="b74bc-116">此工作分配可能的最大分数。</span><span class="sxs-lookup"><span data-stu-id="b74bc-116">Max points possible for this assignment.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="b74bc-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b74bc-117">JSON representation</span></span>

<span data-ttu-id="b74bc-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b74bc-118">The following is a JSON representation of the resource.</span></span>

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


