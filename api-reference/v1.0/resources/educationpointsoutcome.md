---
title: educationPointsOutcome 资源类型
description: 提供数字成绩的 educationOutcome。
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2fdef09c65203c8fc17786f0e663db326057323d
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912275"
---
# <a name="educationpointsoutcome-resource-type"></a><span data-ttu-id="24bd1-103">educationPointsOutcome 资源类型</span><span class="sxs-lookup"><span data-stu-id="24bd1-103">educationPointsOutcome resource type</span></span>

<span data-ttu-id="24bd1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24bd1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="24bd1-105">提供[数字成绩的 educationOutcome。](educationoutcome.md)</span><span class="sxs-lookup"><span data-stu-id="24bd1-105">An [educationOutcome](educationoutcome.md) that gives a numerical grade.</span></span>

## <a name="methods"></a><span data-ttu-id="24bd1-106">方法</span><span class="sxs-lookup"><span data-stu-id="24bd1-106">Methods</span></span>

| <span data-ttu-id="24bd1-107">方法</span><span class="sxs-lookup"><span data-stu-id="24bd1-107">Method</span></span>       | <span data-ttu-id="24bd1-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="24bd1-108">Return Type</span></span> | <span data-ttu-id="24bd1-109">说明</span><span class="sxs-lookup"><span data-stu-id="24bd1-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="24bd1-110">更新 educationOutcome</span><span class="sxs-lookup"><span data-stu-id="24bd1-110">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="24bd1-111">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="24bd1-111">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="24bd1-112">更新 educationOutcome 对象。</span><span class="sxs-lookup"><span data-stu-id="24bd1-112">Update educationOutcome object.</span></span> |

## <a name="properties"></a><span data-ttu-id="24bd1-113">属性</span><span class="sxs-lookup"><span data-stu-id="24bd1-113">Properties</span></span>

| <span data-ttu-id="24bd1-114">属性</span><span class="sxs-lookup"><span data-stu-id="24bd1-114">Property</span></span>     | <span data-ttu-id="24bd1-115">类型</span><span class="sxs-lookup"><span data-stu-id="24bd1-115">Type</span></span>        | <span data-ttu-id="24bd1-116">说明</span><span class="sxs-lookup"><span data-stu-id="24bd1-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="24bd1-117">points</span><span class="sxs-lookup"><span data-stu-id="24bd1-117">points</span></span>|[<span data-ttu-id="24bd1-118">educationAssignmentPointsGrade</span><span class="sxs-lookup"><span data-stu-id="24bd1-118">educationAssignmentPointsGrade</span></span>](educationassignmentpointsgrade.md)|<span data-ttu-id="24bd1-119">教师为此作业为学生提供的数字等级。</span><span class="sxs-lookup"><span data-stu-id="24bd1-119">The numeric grade the teacher has given the student for this assignment.</span></span>|
|<span data-ttu-id="24bd1-120">publishedPoints</span><span class="sxs-lookup"><span data-stu-id="24bd1-120">publishedPoints</span></span>|[<span data-ttu-id="24bd1-121">educationAssignmentPointsGrade</span><span class="sxs-lookup"><span data-stu-id="24bd1-121">educationAssignmentPointsGrade</span></span>](educationassignmentpointsgrade.md)|<span data-ttu-id="24bd1-122">在将成绩释放给学生时所创建数据点属性的副本。</span><span class="sxs-lookup"><span data-stu-id="24bd1-122">A copy of the points property that is made when the grade is released to the student.</span></span>|

## <a name="relationships"></a><span data-ttu-id="24bd1-123">关系</span><span class="sxs-lookup"><span data-stu-id="24bd1-123">Relationships</span></span>

<span data-ttu-id="24bd1-124">无</span><span class="sxs-lookup"><span data-stu-id="24bd1-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="24bd1-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="24bd1-125">JSON representation</span></span>

<span data-ttu-id="24bd1-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="24bd1-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPointsOutcome",
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

