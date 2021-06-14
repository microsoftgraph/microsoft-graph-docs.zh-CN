---
title: educationAssignmentPointsGradeType 资源类型
description: 与 **assignments.assignments** 属性一同使用的资源类型。 这是 educationAssignmentGradeType 的子类。
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ca5a6ba0dd6674d55b4659fbdb1e2c288a65eb12
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912329"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a><span data-ttu-id="19473-104">educationAssignmentPointsGradeType 资源类型</span><span class="sxs-lookup"><span data-stu-id="19473-104">educationAssignmentPointsGradeType resource type</span></span>

<span data-ttu-id="19473-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19473-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="19473-106">与 **assignments.assignments** 属性一同使用的资源类型。</span><span class="sxs-lookup"><span data-stu-id="19473-106">Resource type that is used with the **assignments.grading** property.</span></span> <span data-ttu-id="19473-107">这是 [educationAssignmentGradeType 的子类](educationassignmentgradetype.md)。</span><span class="sxs-lookup"><span data-stu-id="19473-107">This is a subclass of [educationAssignmentGradeType](educationassignmentgradetype.md).</span></span>

<span data-ttu-id="19473-108">这表示作业已评分，并存储每个学生可在此工作项上实现的最大点数。</span><span class="sxs-lookup"><span data-stu-id="19473-108">This indicates that the assignment is graded and stores the maximum number of points each student can achieve on this work item.</span></span> <span data-ttu-id="19473-109">在作业中设置此选项时，每个提交都将获得一个 [与其关联的 educationAssignmentPointsGrade](educationassignmentpointsgrade.md) 属性，用于存储每个学生的分数。</span><span class="sxs-lookup"><span data-stu-id="19473-109">When this is set on an assignment, each submission will get an [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) property associated with it for the storage of each student's points.</span></span>

## <a name="properties"></a><span data-ttu-id="19473-110">属性</span><span class="sxs-lookup"><span data-stu-id="19473-110">Properties</span></span>
| <span data-ttu-id="19473-111">属性</span><span class="sxs-lookup"><span data-stu-id="19473-111">Property</span></span>     | <span data-ttu-id="19473-112">类型</span><span class="sxs-lookup"><span data-stu-id="19473-112">Type</span></span>   |<span data-ttu-id="19473-113">说明</span><span class="sxs-lookup"><span data-stu-id="19473-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19473-114">maxPoints</span><span class="sxs-lookup"><span data-stu-id="19473-114">maxPoints</span></span>|<span data-ttu-id="19473-115">单一</span><span class="sxs-lookup"><span data-stu-id="19473-115">Single</span></span>| <span data-ttu-id="19473-116">此工作分配可能的最大点数。</span><span class="sxs-lookup"><span data-stu-id="19473-116">Max points possible for this assignment.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="19473-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="19473-117">JSON representation</span></span>

<span data-ttu-id="19473-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="19473-118">The following is a JSON representation of the resource.</span></span>

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


