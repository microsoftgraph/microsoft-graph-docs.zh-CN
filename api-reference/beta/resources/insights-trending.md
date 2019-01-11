---
title: 趋势资源类型
description: 将用户连接到的文档的用户 （与用户相关) 周围趋势丰富的关系。 OneDrive 文件和文件存储在 SharePoint 工作组网站可以趋势周围用户。
author: simonhult
localization_priority: Normal
ms.openlocfilehash: dc0154d3985e5f6e1e4770bb7d10bc727a0eb0ae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862382"
---
# <a name="trending-resource-type"></a><span data-ttu-id="7befc-104">趋势资源类型</span><span class="sxs-lookup"><span data-stu-id="7befc-104">trending resource type</span></span>

> <span data-ttu-id="7befc-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7befc-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7befc-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7befc-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7befc-107">将用户连接到的文档的用户 （与用户相关) 周围趋势丰富的关系。</span><span class="sxs-lookup"><span data-stu-id="7befc-107">Rich relationship connecting a user to documents that are trending around the user (are relevant to the user).</span></span> <span data-ttu-id="7befc-108">OneDrive 文件和文件存储在 SharePoint 工作组网站可以趋势周围用户。</span><span class="sxs-lookup"><span data-stu-id="7befc-108">OneDrive files, and files stored on SharePoint team sites can trend around the user.</span></span>

## <a name="methods"></a><span data-ttu-id="7befc-109">方法</span><span class="sxs-lookup"><span data-stu-id="7befc-109">Methods</span></span>

| <span data-ttu-id="7befc-110">方法</span><span class="sxs-lookup"><span data-stu-id="7befc-110">Method</span></span>       | <span data-ttu-id="7befc-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="7befc-111">Return Type</span></span>  |<span data-ttu-id="7befc-112">说明</span><span class="sxs-lookup"><span data-stu-id="7befc-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7befc-113">列表趋势分析</span><span class="sxs-lookup"><span data-stu-id="7befc-113">List trending</span></span>](../api/insights-list-trending.md) |<span data-ttu-id="7befc-114">[insights_trending](insights-trending.md)集合</span><span class="sxs-lookup"><span data-stu-id="7befc-114">[insights_trending](insights-trending.md) collection</span></span>| <span data-ttu-id="7befc-115">获取趋势文件的列表。</span><span class="sxs-lookup"><span data-stu-id="7befc-115">Get a list of trending files.</span></span>|

## <a name="properties"></a><span data-ttu-id="7befc-116">属性</span><span class="sxs-lookup"><span data-stu-id="7befc-116">Properties</span></span>

| <span data-ttu-id="7befc-117">属性</span><span class="sxs-lookup"><span data-stu-id="7befc-117">Property</span></span>      | <span data-ttu-id="7befc-118">类型</span><span class="sxs-lookup"><span data-stu-id="7befc-118">Type</span></span>                              | <span data-ttu-id="7befc-119">说明</span><span class="sxs-lookup"><span data-stu-id="7befc-119">Description</span></span>  |
| ------------- |---------------                    | -------------|
| <span data-ttu-id="7befc-120">id</span><span class="sxs-lookup"><span data-stu-id="7befc-120">id</span></span>                    | <span data-ttu-id="7befc-121">字符串</span><span class="sxs-lookup"><span data-stu-id="7befc-121">String</span></span>                    | <span data-ttu-id="7befc-122">关系的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="7befc-122">Unique identifier of the relationship.</span></span> <span data-ttu-id="7befc-123">只读。</span><span class="sxs-lookup"><span data-stu-id="7befc-123">Read only.</span></span>        |
| <span data-ttu-id="7befc-124">weight</span><span class="sxs-lookup"><span data-stu-id="7befc-124">weight</span></span>                | <span data-ttu-id="7befc-125">Double</span><span class="sxs-lookup"><span data-stu-id="7befc-125">Double</span></span>                    | <span data-ttu-id="7befc-126">值，该值指示当前趋势多少文档。</span><span class="sxs-lookup"><span data-stu-id="7befc-126">Value indicating how much the document is currently trending.</span></span> <span data-ttu-id="7befc-127">较大的号码，更多文档当前趋势周围用户 （更多相关)。</span><span class="sxs-lookup"><span data-stu-id="7befc-127">The larger the number, the more the document is currently trending around the user (the more relevant it is).</span></span> <span data-ttu-id="7befc-128">按此值，返回的文档进行排序。</span><span class="sxs-lookup"><span data-stu-id="7befc-128">Returned documents are sorted by this value.</span></span>  |
| <span data-ttu-id="7befc-129">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="7befc-129">resourceVisualization</span></span> | [<span data-ttu-id="7befc-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="7befc-130">resourceVisualization</span></span>](insights-resourcevisualization.md)    | <span data-ttu-id="7befc-131">您可以使用可视化中您的体验的文档的属性。</span><span class="sxs-lookup"><span data-stu-id="7befc-131">Properties that you can use to visualize the document in your experience.</span></span> |
| <span data-ttu-id="7befc-132">resourceReference</span><span class="sxs-lookup"><span data-stu-id="7befc-132">resourceReference</span></span>     | [<span data-ttu-id="7befc-133">resourceReference</span><span class="sxs-lookup"><span data-stu-id="7befc-133">resourceReference</span></span>](insights-resourcereference.md)        | <span data-ttu-id="7befc-134">趋势文档，如 url 和的文档类型的引用属性。</span><span class="sxs-lookup"><span data-stu-id="7befc-134">Reference properties of the trending document, such as the url and type of the document.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7befc-135">Relationships</span><span class="sxs-lookup"><span data-stu-id="7befc-135">Relationships</span></span>

| <span data-ttu-id="7befc-136">属性</span><span class="sxs-lookup"><span data-stu-id="7befc-136">Property</span></span>      | <span data-ttu-id="7befc-137">类型</span><span class="sxs-lookup"><span data-stu-id="7befc-137">Type</span></span>          | <span data-ttu-id="7befc-138">说明</span><span class="sxs-lookup"><span data-stu-id="7befc-138">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="7befc-139">资源</span><span class="sxs-lookup"><span data-stu-id="7befc-139">resource</span></span>      | <span data-ttu-id="7befc-140">Entity</span><span class="sxs-lookup"><span data-stu-id="7befc-140">Entity</span></span>        | <span data-ttu-id="7befc-141">用于导航到趋势文档。</span><span class="sxs-lookup"><span data-stu-id="7befc-141">Used for navigating to the trending document.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7befc-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7befc-142">JSON representation</span></span>

<span data-ttu-id="7befc-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7befc-143">Here is a JSON representation of the resource</span></span>

```json
{
  "id": "string",
  "weight": "double",
  "resourceVisualization": [{"@odata.type": "microsoft.graph.resourceVisualization"}],
  "resourceReference": [{"@odata.type": "microsoft.graph.resourceReference"}],
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
