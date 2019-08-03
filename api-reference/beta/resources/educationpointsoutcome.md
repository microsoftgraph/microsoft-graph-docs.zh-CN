---
title: educationPointsOutcome 资源类型
description: 提供数字等级的 educationOutcome
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 12e288e49fffd3cf385111878483408b5c6610c1
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173242"
---
# <a name="educationpointsoutcome-resource-type"></a><span data-ttu-id="8c721-103">educationPointsOutcome 资源类型</span><span class="sxs-lookup"><span data-stu-id="8c721-103">educationPointsOutcome resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c721-104">提供数字等级的[educationOutcome](educationoutcome.md) 。</span><span class="sxs-lookup"><span data-stu-id="8c721-104">An [educationOutcome](educationoutcome.md) that gives a numerical grade.</span></span>

## <a name="methods"></a><span data-ttu-id="8c721-105">方法</span><span class="sxs-lookup"><span data-stu-id="8c721-105">Methods</span></span>

| <span data-ttu-id="8c721-106">方法</span><span class="sxs-lookup"><span data-stu-id="8c721-106">Method</span></span>       | <span data-ttu-id="8c721-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="8c721-107">Return Type</span></span> | <span data-ttu-id="8c721-108">说明</span><span class="sxs-lookup"><span data-stu-id="8c721-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8c721-109">更新 educationOutcome</span><span class="sxs-lookup"><span data-stu-id="8c721-109">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="8c721-110">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="8c721-110">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="8c721-111">更新 educationOutcome 对象。</span><span class="sxs-lookup"><span data-stu-id="8c721-111">Update educationOutcome object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8c721-112">属性</span><span class="sxs-lookup"><span data-stu-id="8c721-112">Properties</span></span>

| <span data-ttu-id="8c721-113">属性</span><span class="sxs-lookup"><span data-stu-id="8c721-113">Property</span></span>     | <span data-ttu-id="8c721-114">类型</span><span class="sxs-lookup"><span data-stu-id="8c721-114">Type</span></span>        | <span data-ttu-id="8c721-115">说明</span><span class="sxs-lookup"><span data-stu-id="8c721-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8c721-116">points</span><span class="sxs-lookup"><span data-stu-id="8c721-116">points</span></span>|[<span data-ttu-id="8c721-117">educationAssignmentPointsGrade</span><span class="sxs-lookup"><span data-stu-id="8c721-117">educationAssignmentPointsGrade</span></span>](educationassignmentpointsgrade.md)|<span data-ttu-id="8c721-118">教师为此工作分配提供了学生的数字等级。</span><span class="sxs-lookup"><span data-stu-id="8c721-118">The numeric grade the teacher has given the student for this assignment.</span></span>|
|<span data-ttu-id="8c721-119">publishedPoints</span><span class="sxs-lookup"><span data-stu-id="8c721-119">publishedPoints</span></span>|[<span data-ttu-id="8c721-120">educationAssignmentPointsGrade</span><span class="sxs-lookup"><span data-stu-id="8c721-120">educationAssignmentPointsGrade</span></span>](educationassignmentpointsgrade.md)|<span data-ttu-id="8c721-121">在向学生释放评分时所进行的 points 属性的副本。</span><span class="sxs-lookup"><span data-stu-id="8c721-121">A copy of the points property that is made when the grade is released to the student.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c721-122">关系</span><span class="sxs-lookup"><span data-stu-id="8c721-122">Relationships</span></span>

<span data-ttu-id="8c721-123">无</span><span class="sxs-lookup"><span data-stu-id="8c721-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c721-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8c721-124">JSON representation</span></span>

<span data-ttu-id="8c721-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c721-125">The following is a JSON representation of the resource.</span></span>

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