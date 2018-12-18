---
title: 趋势资源类型
description: 将用户连接到的文档的用户 （与用户相关) 周围趋势丰富的关系。 OneDrive 文件和文件存储在 SharePoint 工作组网站可以趋势周围用户。
author: simonhult
ms.openlocfilehash: ae3c3a876dba6c22a629cce5db8e5b4baa5fb5bf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347997"
---
# <a name="trending-resource-type"></a><span data-ttu-id="c7bdb-104">趋势资源类型</span><span class="sxs-lookup"><span data-stu-id="c7bdb-104">trending resource type</span></span>

> <span data-ttu-id="c7bdb-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c7bdb-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c7bdb-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c7bdb-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c7bdb-107">将用户连接到的文档的用户 （与用户相关) 周围趋势丰富的关系。</span><span class="sxs-lookup"><span data-stu-id="c7bdb-107">Rich relationship connecting a user to documents that are trending around the user (are relevant to the user).</span></span> <span data-ttu-id="c7bdb-108">OneDrive 文件和文件存储在 SharePoint 工作组网站可以趋势周围用户。</span><span class="sxs-lookup"><span data-stu-id="c7bdb-108">OneDrive files, and files stored on SharePoint team sites can trend around the user.</span></span>

## <a name="methods"></a><span data-ttu-id="c7bdb-109">方法</span><span class="sxs-lookup"><span data-stu-id="c7bdb-109">Methods</span></span>

| <span data-ttu-id="c7bdb-110">方法</span><span class="sxs-lookup"><span data-stu-id="c7bdb-110">Method</span></span>       | <span data-ttu-id="c7bdb-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="c7bdb-111">Return Type</span></span>  |<span data-ttu-id="c7bdb-112">说明</span><span class="sxs-lookup"><span data-stu-id="c7bdb-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c7bdb-113">列表趋势分析</span><span class="sxs-lookup"><span data-stu-id="c7bdb-113">List trending</span></span>](../api/insights-list-trending.md) |<span data-ttu-id="c7bdb-114">[insights_trending](insights-trending.md)集合</span><span class="sxs-lookup"><span data-stu-id="c7bdb-114">[insights_trending](insights-trending.md) collection</span></span>| <span data-ttu-id="c7bdb-115">获取趋势文件的列表。</span><span class="sxs-lookup"><span data-stu-id="c7bdb-115">Get a list of trending files.</span></span>|

## <a name="properties"></a><span data-ttu-id="c7bdb-116">属性</span><span class="sxs-lookup"><span data-stu-id="c7bdb-116">Properties</span></span>

| <span data-ttu-id="c7bdb-117">属性</span><span class="sxs-lookup"><span data-stu-id="c7bdb-117">Property</span></span>      | <span data-ttu-id="c7bdb-118">类型</span><span class="sxs-lookup"><span data-stu-id="c7bdb-118">Type</span></span>                              | <span data-ttu-id="c7bdb-119">说明</span><span class="sxs-lookup"><span data-stu-id="c7bdb-119">Description</span></span>  |
| ------------- |---------------                    | -------------|
| <span data-ttu-id="c7bdb-120">id</span><span class="sxs-lookup"><span data-stu-id="c7bdb-120">id</span></span>                    | <span data-ttu-id="c7bdb-121">字符串</span><span class="sxs-lookup"><span data-stu-id="c7bdb-121">String</span></span>                    | <span data-ttu-id="c7bdb-122">关系的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c7bdb-122">Unique identifier of the relationship.</span></span> <span data-ttu-id="c7bdb-123">只读。</span><span class="sxs-lookup"><span data-stu-id="c7bdb-123">Read only.</span></span>        |
| <span data-ttu-id="c7bdb-124">weight</span><span class="sxs-lookup"><span data-stu-id="c7bdb-124">weight</span></span>                | <span data-ttu-id="c7bdb-125">双精度数</span><span class="sxs-lookup"><span data-stu-id="c7bdb-125">Double</span></span>                    | <span data-ttu-id="c7bdb-126">值，该值指示当前趋势多少文档。</span><span class="sxs-lookup"><span data-stu-id="c7bdb-126">Value indicating how much the document is currently trending.</span></span> <span data-ttu-id="c7bdb-127">较大的号码，更多文档当前趋势周围用户 （更多相关)。</span><span class="sxs-lookup"><span data-stu-id="c7bdb-127">The larger the number, the more the document is currently trending around the user (the more relevant it is).</span></span> <span data-ttu-id="c7bdb-128">按此值，返回的文档进行排序。</span><span class="sxs-lookup"><span data-stu-id="c7bdb-128">Returned documents are sorted by this value.</span></span>  |
| <span data-ttu-id="c7bdb-129">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="c7bdb-129">resourceVisualization</span></span> | [<span data-ttu-id="c7bdb-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="c7bdb-130">resourceVisualization</span></span>](insights-resourcevisualization.md)    | <span data-ttu-id="c7bdb-131">您可以使用可视化中您的体验的文档的属性。</span><span class="sxs-lookup"><span data-stu-id="c7bdb-131">Properties that you can use to visualize the document in your experience.</span></span> |
| <span data-ttu-id="c7bdb-132">resourceReference</span><span class="sxs-lookup"><span data-stu-id="c7bdb-132">resourceReference</span></span>     | [<span data-ttu-id="c7bdb-133">resourceReference</span><span class="sxs-lookup"><span data-stu-id="c7bdb-133">resourceReference</span></span>](insights-resourcereference.md)        | <span data-ttu-id="c7bdb-134">趋势文档，如 url 和的文档类型的引用属性。</span><span class="sxs-lookup"><span data-stu-id="c7bdb-134">Reference properties of the trending document, such as the url and type of the document.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c7bdb-135">Relationships</span><span class="sxs-lookup"><span data-stu-id="c7bdb-135">Relationships</span></span>

| <span data-ttu-id="c7bdb-136">属性</span><span class="sxs-lookup"><span data-stu-id="c7bdb-136">Property</span></span>      | <span data-ttu-id="c7bdb-137">类型</span><span class="sxs-lookup"><span data-stu-id="c7bdb-137">Type</span></span>          | <span data-ttu-id="c7bdb-138">说明</span><span class="sxs-lookup"><span data-stu-id="c7bdb-138">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="c7bdb-139">资源</span><span class="sxs-lookup"><span data-stu-id="c7bdb-139">resource</span></span>      | <span data-ttu-id="c7bdb-140">Entity</span><span class="sxs-lookup"><span data-stu-id="c7bdb-140">Entity</span></span>        | <span data-ttu-id="c7bdb-141">用于导航到趋势文档。</span><span class="sxs-lookup"><span data-stu-id="c7bdb-141">Used for navigating to the trending document.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c7bdb-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c7bdb-142">JSON representation</span></span>

<span data-ttu-id="c7bdb-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c7bdb-143">Here is a JSON representation of the resource</span></span>

```json
{
  "id": "string",
  "weight": "double",
  "resourceVisualization": [{"@odata.type": "microsoft.graph.resourceVisualization"}],
  "resourceReference": [{"@odata.type": "microsoft.graph.resourceReference"}],
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```