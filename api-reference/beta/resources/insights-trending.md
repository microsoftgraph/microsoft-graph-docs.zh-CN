---
title: 趋势资源类型
description: 将用户连接到的文档的用户 （与用户相关) 周围趋势丰富的关系。 OneDrive 文件和文件存储在 SharePoint 工作组网站可以趋势周围用户。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 07fe0f50d6961f0fce6c426c7fb2431f17127bf7
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640369"
---
# <a name="trending-resource-type"></a><span data-ttu-id="9aaac-104">趋势资源类型</span><span class="sxs-lookup"><span data-stu-id="9aaac-104">trending resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9aaac-105">将用户连接到的文档的用户 （与用户相关) 周围趋势丰富的关系。</span><span class="sxs-lookup"><span data-stu-id="9aaac-105">Rich relationship connecting a user to documents that are trending around the user (are relevant to the user).</span></span> <span data-ttu-id="9aaac-106">OneDrive 文件和文件存储在 SharePoint 工作组网站可以趋势周围用户。</span><span class="sxs-lookup"><span data-stu-id="9aaac-106">OneDrive files, and files stored on SharePoint team sites can trend around the user.</span></span>

## <a name="methods"></a><span data-ttu-id="9aaac-107">方法</span><span class="sxs-lookup"><span data-stu-id="9aaac-107">Methods</span></span>

| <span data-ttu-id="9aaac-108">方法</span><span class="sxs-lookup"><span data-stu-id="9aaac-108">Method</span></span>       | <span data-ttu-id="9aaac-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="9aaac-109">Return Type</span></span>  |<span data-ttu-id="9aaac-110">说明</span><span class="sxs-lookup"><span data-stu-id="9aaac-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9aaac-111">列表趋势分析</span><span class="sxs-lookup"><span data-stu-id="9aaac-111">List trending</span></span>](../api/insights-list-trending.md) |<span data-ttu-id="9aaac-112">[insights_trending](insights-trending.md)集合</span><span class="sxs-lookup"><span data-stu-id="9aaac-112">[insights_trending](insights-trending.md) collection</span></span>| <span data-ttu-id="9aaac-113">获取趋势文件的列表。</span><span class="sxs-lookup"><span data-stu-id="9aaac-113">Get a list of trending files.</span></span>|

## <a name="properties"></a><span data-ttu-id="9aaac-114">属性</span><span class="sxs-lookup"><span data-stu-id="9aaac-114">Properties</span></span>

| <span data-ttu-id="9aaac-115">属性</span><span class="sxs-lookup"><span data-stu-id="9aaac-115">Property</span></span>      | <span data-ttu-id="9aaac-116">类型</span><span class="sxs-lookup"><span data-stu-id="9aaac-116">Type</span></span>                              | <span data-ttu-id="9aaac-117">说明</span><span class="sxs-lookup"><span data-stu-id="9aaac-117">Description</span></span>  |
| ------------- |---------------                    | -------------|
| <span data-ttu-id="9aaac-118">id</span><span class="sxs-lookup"><span data-stu-id="9aaac-118">id</span></span>                    | <span data-ttu-id="9aaac-119">String</span><span class="sxs-lookup"><span data-stu-id="9aaac-119">String</span></span>                    | <span data-ttu-id="9aaac-120">关系的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9aaac-120">Unique identifier of the relationship.</span></span> <span data-ttu-id="9aaac-121">只读。</span><span class="sxs-lookup"><span data-stu-id="9aaac-121">Read only.</span></span>        |
| <span data-ttu-id="9aaac-122">weight</span><span class="sxs-lookup"><span data-stu-id="9aaac-122">weight</span></span>                | <span data-ttu-id="9aaac-123">双精度</span><span class="sxs-lookup"><span data-stu-id="9aaac-123">Double</span></span>                    | <span data-ttu-id="9aaac-124">值，该值指示当前趋势多少文档。</span><span class="sxs-lookup"><span data-stu-id="9aaac-124">Value indicating how much the document is currently trending.</span></span> <span data-ttu-id="9aaac-125">较大的号码，更多文档当前趋势周围用户 （更多相关)。</span><span class="sxs-lookup"><span data-stu-id="9aaac-125">The larger the number, the more the document is currently trending around the user (the more relevant it is).</span></span> <span data-ttu-id="9aaac-126">按此值，返回的文档进行排序。</span><span class="sxs-lookup"><span data-stu-id="9aaac-126">Returned documents are sorted by this value.</span></span>  |
| <span data-ttu-id="9aaac-127">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="9aaac-127">resourceVisualization</span></span> | [<span data-ttu-id="9aaac-128">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="9aaac-128">resourceVisualization</span></span>](insights-resourcevisualization.md)    | <span data-ttu-id="9aaac-129">您可以使用可视化中您的体验的文档的属性。</span><span class="sxs-lookup"><span data-stu-id="9aaac-129">Properties that you can use to visualize the document in your experience.</span></span> |
| <span data-ttu-id="9aaac-130">resourceReference</span><span class="sxs-lookup"><span data-stu-id="9aaac-130">resourceReference</span></span>     | [<span data-ttu-id="9aaac-131">resourceReference</span><span class="sxs-lookup"><span data-stu-id="9aaac-131">resourceReference</span></span>](insights-resourcereference.md)        | <span data-ttu-id="9aaac-132">趋势文档，如 url 和的文档类型的引用属性。</span><span class="sxs-lookup"><span data-stu-id="9aaac-132">Reference properties of the trending document, such as the url and type of the document.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9aaac-133">关系</span><span class="sxs-lookup"><span data-stu-id="9aaac-133">Relationships</span></span>

| <span data-ttu-id="9aaac-134">属性</span><span class="sxs-lookup"><span data-stu-id="9aaac-134">Property</span></span>      | <span data-ttu-id="9aaac-135">类型</span><span class="sxs-lookup"><span data-stu-id="9aaac-135">Type</span></span>          | <span data-ttu-id="9aaac-136">说明</span><span class="sxs-lookup"><span data-stu-id="9aaac-136">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="9aaac-137">资源</span><span class="sxs-lookup"><span data-stu-id="9aaac-137">resource</span></span>      | <span data-ttu-id="9aaac-138">Entity</span><span class="sxs-lookup"><span data-stu-id="9aaac-138">Entity</span></span>        | <span data-ttu-id="9aaac-139">用于导航到趋势文档。</span><span class="sxs-lookup"><span data-stu-id="9aaac-139">Used for navigating to the trending document.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9aaac-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9aaac-140">JSON representation</span></span>

<span data-ttu-id="9aaac-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9aaac-141">Here is a JSON representation of the resource</span></span>

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
