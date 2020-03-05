---
title: 趋势资源类型
description: 将用户连接到在用户周围进行趋势分析的文档（与用户相关）的丰富关系。 OneDrive 文件和存储在 SharePoint 团队网站上的文件可围绕用户进行趋势。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 5c6fe9f81b9474ca8d1a4c2aeeb3fcc449499c82
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42495534"
---
# <a name="trending-resource-type"></a><span data-ttu-id="0c961-104">趋势资源类型</span><span class="sxs-lookup"><span data-stu-id="0c961-104">trending resource type</span></span>

<span data-ttu-id="0c961-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="0c961-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c961-106">将用户连接到在用户周围进行趋势分析的文档（与用户相关）的丰富关系。</span><span class="sxs-lookup"><span data-stu-id="0c961-106">Rich relationship connecting a user to documents that are trending around the user (are relevant to the user).</span></span> <span data-ttu-id="0c961-107">OneDrive 文件和存储在 SharePoint 团队网站上的文件可围绕用户进行趋势。</span><span class="sxs-lookup"><span data-stu-id="0c961-107">OneDrive files, and files stored on SharePoint team sites can trend around the user.</span></span>

## <a name="methods"></a><span data-ttu-id="0c961-108">方法</span><span class="sxs-lookup"><span data-stu-id="0c961-108">Methods</span></span>

| <span data-ttu-id="0c961-109">方法</span><span class="sxs-lookup"><span data-stu-id="0c961-109">Method</span></span>       | <span data-ttu-id="0c961-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="0c961-110">Return Type</span></span>  |<span data-ttu-id="0c961-111">说明</span><span class="sxs-lookup"><span data-stu-id="0c961-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0c961-112">列出趋势</span><span class="sxs-lookup"><span data-stu-id="0c961-112">List trending</span></span>](../api/insights-list-trending.md) |<span data-ttu-id="0c961-113">[trending](insights-trending.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0c961-113">[trending](insights-trending.md) collection</span></span>| <span data-ttu-id="0c961-114">获取趋势文件的列表。</span><span class="sxs-lookup"><span data-stu-id="0c961-114">Get a list of trending files.</span></span>|

## <a name="properties"></a><span data-ttu-id="0c961-115">属性</span><span class="sxs-lookup"><span data-stu-id="0c961-115">Properties</span></span>

| <span data-ttu-id="0c961-116">属性</span><span class="sxs-lookup"><span data-stu-id="0c961-116">Property</span></span>      | <span data-ttu-id="0c961-117">类型</span><span class="sxs-lookup"><span data-stu-id="0c961-117">Type</span></span>                              | <span data-ttu-id="0c961-118">说明</span><span class="sxs-lookup"><span data-stu-id="0c961-118">Description</span></span>  |
| ------------- |---------------                    | -------------|
| <span data-ttu-id="0c961-119">id</span><span class="sxs-lookup"><span data-stu-id="0c961-119">id</span></span>                    | <span data-ttu-id="0c961-120">String</span><span class="sxs-lookup"><span data-stu-id="0c961-120">String</span></span>                    | <span data-ttu-id="0c961-121">关系的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0c961-121">Unique identifier of the relationship.</span></span> <span data-ttu-id="0c961-122">只读。</span><span class="sxs-lookup"><span data-stu-id="0c961-122">Read only.</span></span>        |
| <span data-ttu-id="0c961-123">weight</span><span class="sxs-lookup"><span data-stu-id="0c961-123">weight</span></span>                | <span data-ttu-id="0c961-124">双精度</span><span class="sxs-lookup"><span data-stu-id="0c961-124">Double</span></span>                    | <span data-ttu-id="0c961-125">值，该值指示文档当前正在进行趋势计算的程度。</span><span class="sxs-lookup"><span data-stu-id="0c961-125">Value indicating how much the document is currently trending.</span></span> <span data-ttu-id="0c961-126">数字越大，文档当前在用户周围的趋势分析越多（相关性越好）。</span><span class="sxs-lookup"><span data-stu-id="0c961-126">The larger the number, the more the document is currently trending around the user (the more relevant it is).</span></span> <span data-ttu-id="0c961-127">返回的文档按此值进行排序。</span><span class="sxs-lookup"><span data-stu-id="0c961-127">Returned documents are sorted by this value.</span></span>  |
| <span data-ttu-id="0c961-128">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="0c961-128">resourceVisualization</span></span> | [<span data-ttu-id="0c961-129">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="0c961-129">resourceVisualization</span></span>](insights-resourcevisualization.md)    | <span data-ttu-id="0c961-130">可用于在体验中可视化文档的属性。</span><span class="sxs-lookup"><span data-stu-id="0c961-130">Properties that you can use to visualize the document in your experience.</span></span> |
| <span data-ttu-id="0c961-131">resourceReference</span><span class="sxs-lookup"><span data-stu-id="0c961-131">resourceReference</span></span>     | [<span data-ttu-id="0c961-132">resourceReference</span><span class="sxs-lookup"><span data-stu-id="0c961-132">resourceReference</span></span>](insights-resourcereference.md)        | <span data-ttu-id="0c961-133">参考趋势文档的属性，例如文档的 url 和类型。</span><span class="sxs-lookup"><span data-stu-id="0c961-133">Reference properties of the trending document, such as the url and type of the document.</span></span> |
| <span data-ttu-id="0c961-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0c961-134">lastModifiedDateTime</span></span>  | <span data-ttu-id="0c961-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c961-135">DateTimeOffset</span></span>            | |
## <a name="relationships"></a><span data-ttu-id="0c961-136">关系</span><span class="sxs-lookup"><span data-stu-id="0c961-136">Relationships</span></span>

| <span data-ttu-id="0c961-137">属性</span><span class="sxs-lookup"><span data-stu-id="0c961-137">Property</span></span>      | <span data-ttu-id="0c961-138">类型</span><span class="sxs-lookup"><span data-stu-id="0c961-138">Type</span></span>          | <span data-ttu-id="0c961-139">说明</span><span class="sxs-lookup"><span data-stu-id="0c961-139">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="0c961-140">资源</span><span class="sxs-lookup"><span data-stu-id="0c961-140">resource</span></span>      | <span data-ttu-id="0c961-141">属性</span><span class="sxs-lookup"><span data-stu-id="0c961-141">entity</span></span>        | <span data-ttu-id="0c961-142">用于导航到趋势文档。</span><span class="sxs-lookup"><span data-stu-id="0c961-142">Used for navigating to the trending document.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0c961-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0c961-143">JSON representation</span></span>

<span data-ttu-id="0c961-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0c961-144">Here is a JSON representation of the resource</span></span>

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
