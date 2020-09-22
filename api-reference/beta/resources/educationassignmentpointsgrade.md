---
title: educationAssignmentPointsGrade 资源类型
description: 当工作分配设置为 "点" 评分类型时，每个提交都将具有与 " **提交. 年级** " 属性相关联的此对象。 这将从 educationAssignmentGrade 中创建一个子类，
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: bcce2fc6445c465defb2d795f3bfab9545838643
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013713"
---
# <a name="educationassignmentpointsgrade-resource-type"></a><span data-ttu-id="9e3cd-104">educationAssignmentPointsGrade 资源类型</span><span class="sxs-lookup"><span data-stu-id="9e3cd-104">educationAssignmentPointsGrade resource type</span></span>

<span data-ttu-id="9e3cd-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e3cd-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e3cd-106">当工作分配设置为 "点" 评分类型时，每个提交都将具有与 " **提交. 年级** " 属性相关联的此对象。</span><span class="sxs-lookup"><span data-stu-id="9e3cd-106">When an assignment is set to a points grade type, each submission will have this object associated with the **submission.grade** property.</span></span> <span data-ttu-id="9e3cd-107">这将从 [educationAssignmentGrade](educationassignmentgrade.md)创建一个子类，该子类将向此属性添加数据。</span><span class="sxs-lookup"><span data-stu-id="9e3cd-107">This creates a subclass from [educationAssignmentGrade](educationassignmentgrade.md), which will add the who data to this property.</span></span> <span data-ttu-id="9e3cd-108">最大分数存储在 **工作分配. 评分** 属性中。</span><span class="sxs-lookup"><span data-stu-id="9e3cd-108">The max points is stored in the **assignments.grading** property.</span></span>


## <a name="properties"></a><span data-ttu-id="9e3cd-109">属性</span><span class="sxs-lookup"><span data-stu-id="9e3cd-109">Properties</span></span>
| <span data-ttu-id="9e3cd-110">属性</span><span class="sxs-lookup"><span data-stu-id="9e3cd-110">Property</span></span>     | <span data-ttu-id="9e3cd-111">类型</span><span class="sxs-lookup"><span data-stu-id="9e3cd-111">Type</span></span>   |<span data-ttu-id="9e3cd-112">说明</span><span class="sxs-lookup"><span data-stu-id="9e3cd-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e3cd-113">points</span><span class="sxs-lookup"><span data-stu-id="9e3cd-113">points</span></span>|<span data-ttu-id="9e3cd-114">单一</span><span class="sxs-lookup"><span data-stu-id="9e3cd-114">Single</span></span>|<span data-ttu-id="9e3cd-115">教师向此提交对象提供的积分数。</span><span class="sxs-lookup"><span data-stu-id="9e3cd-115">Number of points a teacher is giving this submission object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9e3cd-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9e3cd-116">JSON representation</span></span>

<span data-ttu-id="9e3cd-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e3cd-117">The following is a JSON representation of the resource.</span></span>

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


