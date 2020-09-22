---
title: educationPointsOutcome 资源类型
description: 提供数字等级的 educationOutcome
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: eb8c95fa7d13f57cca2c2fe19d7b992e6e2cab98
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049742"
---
# <a name="educationpointsoutcome-resource-type"></a><span data-ttu-id="24c1d-103">educationPointsOutcome 资源类型</span><span class="sxs-lookup"><span data-stu-id="24c1d-103">educationPointsOutcome resource type</span></span>

<span data-ttu-id="24c1d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24c1d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24c1d-105">提供数字等级的 [educationOutcome](educationoutcome.md) 。</span><span class="sxs-lookup"><span data-stu-id="24c1d-105">An [educationOutcome](educationoutcome.md) that gives a numerical grade.</span></span>

## <a name="methods"></a><span data-ttu-id="24c1d-106">方法</span><span class="sxs-lookup"><span data-stu-id="24c1d-106">Methods</span></span>

| <span data-ttu-id="24c1d-107">方法</span><span class="sxs-lookup"><span data-stu-id="24c1d-107">Method</span></span>       | <span data-ttu-id="24c1d-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="24c1d-108">Return Type</span></span> | <span data-ttu-id="24c1d-109">说明</span><span class="sxs-lookup"><span data-stu-id="24c1d-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="24c1d-110">更新 educationOutcome</span><span class="sxs-lookup"><span data-stu-id="24c1d-110">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="24c1d-111">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="24c1d-111">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="24c1d-112">更新 educationOutcome 对象。</span><span class="sxs-lookup"><span data-stu-id="24c1d-112">Update educationOutcome object.</span></span> |

## <a name="properties"></a><span data-ttu-id="24c1d-113">属性</span><span class="sxs-lookup"><span data-stu-id="24c1d-113">Properties</span></span>

| <span data-ttu-id="24c1d-114">属性</span><span class="sxs-lookup"><span data-stu-id="24c1d-114">Property</span></span>     | <span data-ttu-id="24c1d-115">类型</span><span class="sxs-lookup"><span data-stu-id="24c1d-115">Type</span></span>        | <span data-ttu-id="24c1d-116">说明</span><span class="sxs-lookup"><span data-stu-id="24c1d-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="24c1d-117">points</span><span class="sxs-lookup"><span data-stu-id="24c1d-117">points</span></span>|[<span data-ttu-id="24c1d-118">educationAssignmentPointsGrade</span><span class="sxs-lookup"><span data-stu-id="24c1d-118">educationAssignmentPointsGrade</span></span>](educationassignmentpointsgrade.md)|<span data-ttu-id="24c1d-119">教师为此工作分配提供了学生的数字等级。</span><span class="sxs-lookup"><span data-stu-id="24c1d-119">The numeric grade the teacher has given the student for this assignment.</span></span>|
|<span data-ttu-id="24c1d-120">publishedPoints</span><span class="sxs-lookup"><span data-stu-id="24c1d-120">publishedPoints</span></span>|[<span data-ttu-id="24c1d-121">educationAssignmentPointsGrade</span><span class="sxs-lookup"><span data-stu-id="24c1d-121">educationAssignmentPointsGrade</span></span>](educationassignmentpointsgrade.md)|<span data-ttu-id="24c1d-122">在向学生释放评分时所进行的 points 属性的副本。</span><span class="sxs-lookup"><span data-stu-id="24c1d-122">A copy of the points property that is made when the grade is released to the student.</span></span>|

## <a name="relationships"></a><span data-ttu-id="24c1d-123">关系</span><span class="sxs-lookup"><span data-stu-id="24c1d-123">Relationships</span></span>

<span data-ttu-id="24c1d-124">无</span><span class="sxs-lookup"><span data-stu-id="24c1d-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="24c1d-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="24c1d-125">JSON representation</span></span>

<span data-ttu-id="24c1d-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="24c1d-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPointsOutcome",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "points": {"@odata.type": "microsoft.graph.educationAssignmentPointsGrade"},
  "publishedPoints": {"@odata.type": "microsoft.graph.educationAssignmentPointsGrade"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationPointsOutcome resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

