---
title: educationAssignmentPointsGrade 资源类型
description: 当作业设置为分数类型时，每个提交都将具有与此对象关联的 **submission.grade** 属性。
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b624bd0e82336e4e416641240e072c8b4ac6392d
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912310"
---
# <a name="educationassignmentpointsgrade-resource-type"></a><span data-ttu-id="76068-103">educationAssignmentPointsGrade 资源类型</span><span class="sxs-lookup"><span data-stu-id="76068-103">educationAssignmentPointsGrade resource type</span></span>

<span data-ttu-id="76068-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76068-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="76068-105">当作业设置为分数类型时，每个提交都将具有与此对象关联的 **submission.grade** 属性。</span><span class="sxs-lookup"><span data-stu-id="76068-105">When an assignment is set to a points grade type, each submission will have this object associated with the **submission.grade** property.</span></span> <span data-ttu-id="76068-106">这将从 [educationAssignmentGrade](educationassignmentgrade.md)创建一个子类，它将向此属性添加 who 数据。</span><span class="sxs-lookup"><span data-stu-id="76068-106">This creates a subclass from [educationAssignmentGrade](educationassignmentgrade.md), which will add the who data to this property.</span></span> <span data-ttu-id="76068-107">最大点数存储在 **assignments.assignments** 属性中。</span><span class="sxs-lookup"><span data-stu-id="76068-107">The max points is stored in the **assignments.grading** property.</span></span>


## <a name="properties"></a><span data-ttu-id="76068-108">属性</span><span class="sxs-lookup"><span data-stu-id="76068-108">Properties</span></span>
| <span data-ttu-id="76068-109">属性</span><span class="sxs-lookup"><span data-stu-id="76068-109">Property</span></span>     | <span data-ttu-id="76068-110">类型</span><span class="sxs-lookup"><span data-stu-id="76068-110">Type</span></span>   |<span data-ttu-id="76068-111">说明</span><span class="sxs-lookup"><span data-stu-id="76068-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="76068-112">points</span><span class="sxs-lookup"><span data-stu-id="76068-112">points</span></span>|<span data-ttu-id="76068-113">单一</span><span class="sxs-lookup"><span data-stu-id="76068-113">Single</span></span>|<span data-ttu-id="76068-114">教师提供此提交对象的点数。</span><span class="sxs-lookup"><span data-stu-id="76068-114">Number of points a teacher is giving this submission object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="76068-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="76068-115">JSON representation</span></span>

<span data-ttu-id="76068-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="76068-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentPointsGrade"
}-->

```json
{
  "points": "Double"
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


