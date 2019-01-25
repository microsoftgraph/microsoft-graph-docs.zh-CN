---
title: plannerGroup 资源类型
description: '**plannerGroup** 资源提供组的 Planner 资源的访问权限。它不包含任何可用属性。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 84bb20d0b13f9a99db2f8c59b20e0c9c7c87f93f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513779"
---
# <a name="plannergroup-resource-type"></a><span data-ttu-id="3c4d2-104">plannerGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="3c4d2-104">plannerGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c4d2-p102">**plannerGroup** 资源提供[组](group.md)的 Planner 资源的访问权限。它不包含任何可用属性。</span><span class="sxs-lookup"><span data-stu-id="3c4d2-p102">The **plannerGroup** resource provides access to Planner resources for a [group](group.md). It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="3c4d2-107">方法</span><span class="sxs-lookup"><span data-stu-id="3c4d2-107">Methods</span></span>

| <span data-ttu-id="3c4d2-108">方法</span><span class="sxs-lookup"><span data-stu-id="3c4d2-108">Method</span></span>           | <span data-ttu-id="3c4d2-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="3c4d2-109">Return Type</span></span>    |<span data-ttu-id="3c4d2-110">说明</span><span class="sxs-lookup"><span data-stu-id="3c4d2-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3c4d2-111">List plans</span><span class="sxs-lookup"><span data-stu-id="3c4d2-111">List plans</span></span>](../api/plannergroup-list-plans.md) |<span data-ttu-id="3c4d2-112">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3c4d2-112">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="3c4d2-113">获取 **plannerPlan** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3c4d2-113">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="3c4d2-114">属性</span><span class="sxs-lookup"><span data-stu-id="3c4d2-114">Properties</span></span>
| <span data-ttu-id="3c4d2-115">属性</span><span class="sxs-lookup"><span data-stu-id="3c4d2-115">Property</span></span>     | <span data-ttu-id="3c4d2-116">类型</span><span class="sxs-lookup"><span data-stu-id="3c4d2-116">Type</span></span>   |<span data-ttu-id="3c4d2-117">说明</span><span class="sxs-lookup"><span data-stu-id="3c4d2-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c4d2-118">id</span><span class="sxs-lookup"><span data-stu-id="3c4d2-118">id</span></span>|<span data-ttu-id="3c4d2-119">String</span><span class="sxs-lookup"><span data-stu-id="3c4d2-119">String</span></span>| <span data-ttu-id="3c4d2-p103">只读。**plannerGroup** 的标识符</span><span class="sxs-lookup"><span data-stu-id="3c4d2-p103">Read-only. Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c4d2-122">关系</span><span class="sxs-lookup"><span data-stu-id="3c4d2-122">Relationships</span></span>
| <span data-ttu-id="3c4d2-123">关系</span><span class="sxs-lookup"><span data-stu-id="3c4d2-123">Relationship</span></span> | <span data-ttu-id="3c4d2-124">类型</span><span class="sxs-lookup"><span data-stu-id="3c4d2-124">Type</span></span>   |<span data-ttu-id="3c4d2-125">说明</span><span class="sxs-lookup"><span data-stu-id="3c4d2-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c4d2-126">plans</span><span class="sxs-lookup"><span data-stu-id="3c4d2-126">plans</span></span>|<span data-ttu-id="3c4d2-127">[plannerPlan](plannerplan.md) collection</span><span class="sxs-lookup"><span data-stu-id="3c4d2-127">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="3c4d2-p104">只读。可为 NULL。返回组拥有的 [plannerPlans](plannerplan.md)。</span><span class="sxs-lookup"><span data-stu-id="3c4d2-p104">Read-only. Nullable. Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3c4d2-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3c4d2-131">JSON representation</span></span>
<span data-ttu-id="3c4d2-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c4d2-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerGroup"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannergroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
