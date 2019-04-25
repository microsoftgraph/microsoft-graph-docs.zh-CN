---
title: 趋势资源类型
description: 将用户连接到在用户周围进行趋势分析的文档 (与用户相关) 的丰富关系。 OneDrive 文件和存储在 SharePoint 团队网站上的文件可围绕用户进行趋势。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 07fe0f50d6961f0fce6c426c7fb2431f17127bf7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551307"
---
# <a name="trending-resource-type"></a><span data-ttu-id="1163c-104">趋势资源类型</span><span class="sxs-lookup"><span data-stu-id="1163c-104">trending resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1163c-105">将用户连接到在用户周围进行趋势分析的文档 (与用户相关) 的丰富关系。</span><span class="sxs-lookup"><span data-stu-id="1163c-105">Rich relationship connecting a user to documents that are trending around the user (are relevant to the user).</span></span> <span data-ttu-id="1163c-106">OneDrive 文件和存储在 SharePoint 团队网站上的文件可围绕用户进行趋势。</span><span class="sxs-lookup"><span data-stu-id="1163c-106">OneDrive files, and files stored on SharePoint team sites can trend around the user.</span></span>

## <a name="methods"></a><span data-ttu-id="1163c-107">方法</span><span class="sxs-lookup"><span data-stu-id="1163c-107">Methods</span></span>

| <span data-ttu-id="1163c-108">方法</span><span class="sxs-lookup"><span data-stu-id="1163c-108">Method</span></span>       | <span data-ttu-id="1163c-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="1163c-109">Return Type</span></span>  |<span data-ttu-id="1163c-110">说明</span><span class="sxs-lookup"><span data-stu-id="1163c-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1163c-111">列出趋势</span><span class="sxs-lookup"><span data-stu-id="1163c-111">List trending</span></span>](../api/insights-list-trending.md) |<span data-ttu-id="1163c-112">[insights_trending](insights-trending.md)集合</span><span class="sxs-lookup"><span data-stu-id="1163c-112">[insights_trending](insights-trending.md) collection</span></span>| <span data-ttu-id="1163c-113">获取趋势文件的列表。</span><span class="sxs-lookup"><span data-stu-id="1163c-113">Get a list of trending files.</span></span>|

## <a name="properties"></a><span data-ttu-id="1163c-114">属性</span><span class="sxs-lookup"><span data-stu-id="1163c-114">Properties</span></span>

| <span data-ttu-id="1163c-115">属性</span><span class="sxs-lookup"><span data-stu-id="1163c-115">Property</span></span>      | <span data-ttu-id="1163c-116">类型</span><span class="sxs-lookup"><span data-stu-id="1163c-116">Type</span></span>                              | <span data-ttu-id="1163c-117">说明</span><span class="sxs-lookup"><span data-stu-id="1163c-117">Description</span></span>  |
| ------------- |---------------                    | -------------|
| <span data-ttu-id="1163c-118">id</span><span class="sxs-lookup"><span data-stu-id="1163c-118">id</span></span>                    | <span data-ttu-id="1163c-119">String</span><span class="sxs-lookup"><span data-stu-id="1163c-119">String</span></span>                    | <span data-ttu-id="1163c-120">关系的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1163c-120">Unique identifier of the relationship.</span></span> <span data-ttu-id="1163c-121">只读。</span><span class="sxs-lookup"><span data-stu-id="1163c-121">Read only.</span></span>        |
| <span data-ttu-id="1163c-122">weight</span><span class="sxs-lookup"><span data-stu-id="1163c-122">weight</span></span>                | <span data-ttu-id="1163c-123">双精度</span><span class="sxs-lookup"><span data-stu-id="1163c-123">Double</span></span>                    | <span data-ttu-id="1163c-124">值, 该值指示文档当前正在进行趋势计算的程度。</span><span class="sxs-lookup"><span data-stu-id="1163c-124">Value indicating how much the document is currently trending.</span></span> <span data-ttu-id="1163c-125">数字越大, 文档当前在用户周围的趋势分析越多 (相关性越好)。</span><span class="sxs-lookup"><span data-stu-id="1163c-125">The larger the number, the more the document is currently trending around the user (the more relevant it is).</span></span> <span data-ttu-id="1163c-126">返回的文档按此值进行排序。</span><span class="sxs-lookup"><span data-stu-id="1163c-126">Returned documents are sorted by this value.</span></span>  |
| <span data-ttu-id="1163c-127">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="1163c-127">resourceVisualization</span></span> | [<span data-ttu-id="1163c-128">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="1163c-128">resourceVisualization</span></span>](insights-resourcevisualization.md)    | <span data-ttu-id="1163c-129">可用于在体验中可视化文档的属性。</span><span class="sxs-lookup"><span data-stu-id="1163c-129">Properties that you can use to visualize the document in your experience.</span></span> |
| <span data-ttu-id="1163c-130">resourceReference</span><span class="sxs-lookup"><span data-stu-id="1163c-130">resourceReference</span></span>     | [<span data-ttu-id="1163c-131">resourceReference</span><span class="sxs-lookup"><span data-stu-id="1163c-131">resourceReference</span></span>](insights-resourcereference.md)        | <span data-ttu-id="1163c-132">参考趋势文档的属性, 例如文档的 url 和类型。</span><span class="sxs-lookup"><span data-stu-id="1163c-132">Reference properties of the trending document, such as the url and type of the document.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1163c-133">关系</span><span class="sxs-lookup"><span data-stu-id="1163c-133">Relationships</span></span>

| <span data-ttu-id="1163c-134">属性</span><span class="sxs-lookup"><span data-stu-id="1163c-134">Property</span></span>      | <span data-ttu-id="1163c-135">类型</span><span class="sxs-lookup"><span data-stu-id="1163c-135">Type</span></span>          | <span data-ttu-id="1163c-136">说明</span><span class="sxs-lookup"><span data-stu-id="1163c-136">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="1163c-137">资源</span><span class="sxs-lookup"><span data-stu-id="1163c-137">resource</span></span>      | <span data-ttu-id="1163c-138">实体</span><span class="sxs-lookup"><span data-stu-id="1163c-138">Entity</span></span>        | <span data-ttu-id="1163c-139">用于导航到趋势文档。</span><span class="sxs-lookup"><span data-stu-id="1163c-139">Used for navigating to the trending document.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1163c-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1163c-140">JSON representation</span></span>

<span data-ttu-id="1163c-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1163c-141">Here is a JSON representation of the resource</span></span>

```json
{
  "id": "string",
  "weight": "double",
  "resourceVisualization": [{"@odata.type": "microsoft.graph.resourceVisualization"}],
  "resourceReference": [{"@odata.type": "microsoft.graph.resourceReference"}],
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-trending.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
