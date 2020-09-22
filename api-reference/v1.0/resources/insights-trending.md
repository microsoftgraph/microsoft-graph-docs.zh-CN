---
title: 趋势资源类型
description: 将用户连接到围绕用户 (的趋势的文档的丰富关系与用户) 相关。 OneDrive 文件和存储在 SharePoint 团队网站上的文件可围绕用户进行趋势。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 7a9c9cf9323aa24bd50c1f817a1293088e1a4373
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054768"
---
# <a name="trending-resource-type"></a><span data-ttu-id="b0afa-104">趋势资源类型</span><span class="sxs-lookup"><span data-stu-id="b0afa-104">trending resource type</span></span>

<span data-ttu-id="b0afa-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0afa-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b0afa-106">将用户连接到围绕用户 (的趋势的文档的丰富关系与用户) 相关。</span><span class="sxs-lookup"><span data-stu-id="b0afa-106">Rich relationship connecting a user to documents that are trending around the user (are relevant to the user).</span></span> <span data-ttu-id="b0afa-107">OneDrive 文件和存储在 SharePoint 团队网站上的文件可围绕用户进行趋势。</span><span class="sxs-lookup"><span data-stu-id="b0afa-107">OneDrive files, and files stored on SharePoint team sites can trend around the user.</span></span>

## <a name="methods"></a><span data-ttu-id="b0afa-108">方法</span><span class="sxs-lookup"><span data-stu-id="b0afa-108">Methods</span></span>

| <span data-ttu-id="b0afa-109">方法</span><span class="sxs-lookup"><span data-stu-id="b0afa-109">Method</span></span>       | <span data-ttu-id="b0afa-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="b0afa-110">Return Type</span></span>  |<span data-ttu-id="b0afa-111">说明</span><span class="sxs-lookup"><span data-stu-id="b0afa-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b0afa-112">列出趋势</span><span class="sxs-lookup"><span data-stu-id="b0afa-112">List trending</span></span>](../api/insights-list-trending.md) |<span data-ttu-id="b0afa-113">[trending](insights-trending.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b0afa-113">[trending](insights-trending.md) collection</span></span>| <span data-ttu-id="b0afa-114">获取趋势文件的列表。</span><span class="sxs-lookup"><span data-stu-id="b0afa-114">Get a list of trending files.</span></span>|

## <a name="properties"></a><span data-ttu-id="b0afa-115">属性</span><span class="sxs-lookup"><span data-stu-id="b0afa-115">Properties</span></span>

| <span data-ttu-id="b0afa-116">属性</span><span class="sxs-lookup"><span data-stu-id="b0afa-116">Property</span></span>      | <span data-ttu-id="b0afa-117">类型</span><span class="sxs-lookup"><span data-stu-id="b0afa-117">Type</span></span>                              | <span data-ttu-id="b0afa-118">说明</span><span class="sxs-lookup"><span data-stu-id="b0afa-118">Description</span></span>  |
| ------------- |---------------                    | -------------|
| <span data-ttu-id="b0afa-119">id</span><span class="sxs-lookup"><span data-stu-id="b0afa-119">id</span></span>                    | <span data-ttu-id="b0afa-120">String</span><span class="sxs-lookup"><span data-stu-id="b0afa-120">String</span></span>                    | <span data-ttu-id="b0afa-121">关系的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b0afa-121">Unique identifier of the relationship.</span></span> <span data-ttu-id="b0afa-122">只读。</span><span class="sxs-lookup"><span data-stu-id="b0afa-122">Read only.</span></span>        |
| <span data-ttu-id="b0afa-123">weight</span><span class="sxs-lookup"><span data-stu-id="b0afa-123">weight</span></span>                | <span data-ttu-id="b0afa-124">双精度</span><span class="sxs-lookup"><span data-stu-id="b0afa-124">Double</span></span>                    | <span data-ttu-id="b0afa-125">值，该值指示文档当前正在进行趋势计算的程度。</span><span class="sxs-lookup"><span data-stu-id="b0afa-125">Value indicating how much the document is currently trending.</span></span> <span data-ttu-id="b0afa-126">数字越大，文档当前在用户周围的趋势 (越相关) 。</span><span class="sxs-lookup"><span data-stu-id="b0afa-126">The larger the number, the more the document is currently trending around the user (the more relevant it is).</span></span> <span data-ttu-id="b0afa-127">返回的文档按此值进行排序。</span><span class="sxs-lookup"><span data-stu-id="b0afa-127">Returned documents are sorted by this value.</span></span>  |
| <span data-ttu-id="b0afa-128">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="b0afa-128">resourceVisualization</span></span> | [<span data-ttu-id="b0afa-129">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="b0afa-129">resourceVisualization</span></span>](insights-resourcevisualization.md)    | <span data-ttu-id="b0afa-130">可用于在体验中可视化文档的属性。</span><span class="sxs-lookup"><span data-stu-id="b0afa-130">Properties that you can use to visualize the document in your experience.</span></span> |
| <span data-ttu-id="b0afa-131">resourceReference</span><span class="sxs-lookup"><span data-stu-id="b0afa-131">resourceReference</span></span>     | [<span data-ttu-id="b0afa-132">resourceReference</span><span class="sxs-lookup"><span data-stu-id="b0afa-132">resourceReference</span></span>](insights-resourcereference.md)        | <span data-ttu-id="b0afa-133">参考趋势文档的属性，例如文档的 url 和类型。</span><span class="sxs-lookup"><span data-stu-id="b0afa-133">Reference properties of the trending document, such as the url and type of the document.</span></span> |
| <span data-ttu-id="b0afa-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0afa-134">lastModifiedDateTime</span></span>  | <span data-ttu-id="b0afa-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0afa-135">DateTimeOffset</span></span>            | |
## <a name="relationships"></a><span data-ttu-id="b0afa-136">关系</span><span class="sxs-lookup"><span data-stu-id="b0afa-136">Relationships</span></span>

| <span data-ttu-id="b0afa-137">属性</span><span class="sxs-lookup"><span data-stu-id="b0afa-137">Property</span></span>      | <span data-ttu-id="b0afa-138">类型</span><span class="sxs-lookup"><span data-stu-id="b0afa-138">Type</span></span>          | <span data-ttu-id="b0afa-139">说明</span><span class="sxs-lookup"><span data-stu-id="b0afa-139">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="b0afa-140">资源</span><span class="sxs-lookup"><span data-stu-id="b0afa-140">resource</span></span>      | <span data-ttu-id="b0afa-141">属性</span><span class="sxs-lookup"><span data-stu-id="b0afa-141">entity</span></span>        | <span data-ttu-id="b0afa-142">用于导航到趋势文档。</span><span class="sxs-lookup"><span data-stu-id="b0afa-142">Used for navigating to the trending document.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b0afa-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b0afa-143">JSON representation</span></span>

<span data-ttu-id="b0afa-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b0afa-144">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [
    "resource"
  ],
  "@odata.type": "microsoft.graph.trending"
}-->

```json
{
  "id": "string",
  "weight": "double",
  "resourceVisualization": {"@odata.type": "microsoft.graph.resourceVisualization"},
  "resourceReference": {"@odata.type": "microsoft.graph.resourceReference"},
  "lastModifiedDateTime": "String (timestamp)"
}
```

