---
title: educationAssignmentPointsGrade 资源类型
description: 当工作分配设置为磅薪等级类型时，每个提交将具有此对象与**submission.grade**属性关联。 这将从 educationAssignmentGrade，创建一个子类
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: d96b84380bc7a6d2298117b5dfeaee25d943efb2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982384"
---
# <a name="educationassignmentpointsgrade-resource-type"></a><span data-ttu-id="d138b-104">educationAssignmentPointsGrade 资源类型</span><span class="sxs-lookup"><span data-stu-id="d138b-104">educationAssignmentPointsGrade resource type</span></span>

> <span data-ttu-id="d138b-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d138b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d138b-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d138b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d138b-107">当工作分配设置为磅薪等级类型时，每个提交将具有此对象与**submission.grade**属性关联。</span><span class="sxs-lookup"><span data-stu-id="d138b-107">When an assignment is set to a points grade type, each submission will have this object associated with the **submission.grade** property.</span></span> <span data-ttu-id="d138b-108">这将创建一个子类从[educationAssignmentGrade](educationassignmentgrade.md)，其中将 who 将数据添加到此属性。</span><span class="sxs-lookup"><span data-stu-id="d138b-108">This creates a subclass from [educationAssignmentGrade](educationassignmentgrade.md), which will add the who data to this property.</span></span> <span data-ttu-id="d138b-109">**Assignments.grading**属性中存储的最大点。</span><span class="sxs-lookup"><span data-stu-id="d138b-109">The max points is stored in the **assignments.grading** property.</span></span>


## <a name="properties"></a><span data-ttu-id="d138b-110">属性</span><span class="sxs-lookup"><span data-stu-id="d138b-110">Properties</span></span>
| <span data-ttu-id="d138b-111">属性</span><span class="sxs-lookup"><span data-stu-id="d138b-111">Property</span></span>     | <span data-ttu-id="d138b-112">类型</span><span class="sxs-lookup"><span data-stu-id="d138b-112">Type</span></span>   |<span data-ttu-id="d138b-113">说明</span><span class="sxs-lookup"><span data-stu-id="d138b-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d138b-114">points</span><span class="sxs-lookup"><span data-stu-id="d138b-114">points</span></span>|<span data-ttu-id="d138b-115">Single</span><span class="sxs-lookup"><span data-stu-id="d138b-115">Single</span></span>|<span data-ttu-id="d138b-116">教师的磅数提供此提交对象。</span><span class="sxs-lookup"><span data-stu-id="d138b-116">Number of points a teacher is giving this submission object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d138b-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d138b-117">JSON representation</span></span>

<span data-ttu-id="d138b-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d138b-118">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
