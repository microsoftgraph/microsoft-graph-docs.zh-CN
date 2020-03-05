---
title: educationAssignmentPointsGrade 资源类型
description: 当工作分配设置为 "点" 评分类型时，每个提交都将具有与 "**提交. 年级**" 属性相关联的此对象。 这将从 educationAssignmentGrade 中创建一个子类，
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c2ef014c3e9e2954dba5fb759fcf3f86b3681b68
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502506"
---
# <a name="educationassignmentpointsgrade-resource-type"></a><span data-ttu-id="6295a-104">educationAssignmentPointsGrade 资源类型</span><span class="sxs-lookup"><span data-stu-id="6295a-104">educationAssignmentPointsGrade resource type</span></span>

<span data-ttu-id="6295a-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="6295a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6295a-106">当工作分配设置为 "点" 评分类型时，每个提交都将具有与 "**提交. 年级**" 属性相关联的此对象。</span><span class="sxs-lookup"><span data-stu-id="6295a-106">When an assignment is set to a points grade type, each submission will have this object associated with the **submission.grade** property.</span></span> <span data-ttu-id="6295a-107">这将从[educationAssignmentGrade](educationassignmentgrade.md)创建一个子类，该子类将向此属性添加数据。</span><span class="sxs-lookup"><span data-stu-id="6295a-107">This creates a subclass from [educationAssignmentGrade](educationassignmentgrade.md), which will add the who data to this property.</span></span> <span data-ttu-id="6295a-108">最大分数存储在**工作分配. 评分**属性中。</span><span class="sxs-lookup"><span data-stu-id="6295a-108">The max points is stored in the **assignments.grading** property.</span></span>


## <a name="properties"></a><span data-ttu-id="6295a-109">属性</span><span class="sxs-lookup"><span data-stu-id="6295a-109">Properties</span></span>
| <span data-ttu-id="6295a-110">属性</span><span class="sxs-lookup"><span data-stu-id="6295a-110">Property</span></span>     | <span data-ttu-id="6295a-111">类型</span><span class="sxs-lookup"><span data-stu-id="6295a-111">Type</span></span>   |<span data-ttu-id="6295a-112">说明</span><span class="sxs-lookup"><span data-stu-id="6295a-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6295a-113">points</span><span class="sxs-lookup"><span data-stu-id="6295a-113">points</span></span>|<span data-ttu-id="6295a-114">单精度</span><span class="sxs-lookup"><span data-stu-id="6295a-114">Single</span></span>|<span data-ttu-id="6295a-115">教师向此提交对象提供的积分数。</span><span class="sxs-lookup"><span data-stu-id="6295a-115">Number of points a teacher is giving this submission object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6295a-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6295a-116">JSON representation</span></span>

<span data-ttu-id="6295a-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6295a-117">The following is a JSON representation of the resource.</span></span>

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
