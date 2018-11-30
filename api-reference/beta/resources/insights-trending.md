---
title: 趋势资源类型
description: 将用户连接到的文档的用户 （与用户相关) 周围趋势丰富的关系。 OneDrive 文件和文件存储在 SharePoint 工作组网站可以趋势周围用户。
ms.openlocfilehash: 7d240c4358047ca9ba3d6b8340fbfb7d893a6a1d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045493"
---
# <a name="trending-resource-type"></a><span data-ttu-id="cd2d4-104">趋势资源类型</span><span class="sxs-lookup"><span data-stu-id="cd2d4-104">trending resource type</span></span>

> <span data-ttu-id="cd2d4-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cd2d4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd2d4-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cd2d4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cd2d4-107">将用户连接到的文档的用户 （与用户相关) 周围趋势丰富的关系。</span><span class="sxs-lookup"><span data-stu-id="cd2d4-107">Rich relationship connecting a user to documents that are trending around the user (are relevant to the user).</span></span> <span data-ttu-id="cd2d4-108">OneDrive 文件和文件存储在 SharePoint 工作组网站可以趋势周围用户。</span><span class="sxs-lookup"><span data-stu-id="cd2d4-108">OneDrive files, and files stored on SharePoint team sites can trend around the user.</span></span>

## <a name="methods"></a><span data-ttu-id="cd2d4-109">方法</span><span class="sxs-lookup"><span data-stu-id="cd2d4-109">Methods</span></span>

| <span data-ttu-id="cd2d4-110">方法</span><span class="sxs-lookup"><span data-stu-id="cd2d4-110">Method</span></span>       | <span data-ttu-id="cd2d4-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="cd2d4-111">Return Type</span></span>  |<span data-ttu-id="cd2d4-112">说明</span><span class="sxs-lookup"><span data-stu-id="cd2d4-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cd2d4-113">列表趋势分析</span><span class="sxs-lookup"><span data-stu-id="cd2d4-113">List trending</span></span>](../api/insights-list-trending.md) |<span data-ttu-id="cd2d4-114">[insights_trending](insights-trending.md)集合</span><span class="sxs-lookup"><span data-stu-id="cd2d4-114">[insights_trending](insights-trending.md) collection</span></span>| <span data-ttu-id="cd2d4-115">获取趋势文件的列表。</span><span class="sxs-lookup"><span data-stu-id="cd2d4-115">Get a list of trending files.</span></span>|

## <a name="properties"></a><span data-ttu-id="cd2d4-116">属性</span><span class="sxs-lookup"><span data-stu-id="cd2d4-116">Properties</span></span>

| <span data-ttu-id="cd2d4-117">属性</span><span class="sxs-lookup"><span data-stu-id="cd2d4-117">Property</span></span>      | <span data-ttu-id="cd2d4-118">类型</span><span class="sxs-lookup"><span data-stu-id="cd2d4-118">Type</span></span>                              | <span data-ttu-id="cd2d4-119">说明</span><span class="sxs-lookup"><span data-stu-id="cd2d4-119">Description</span></span>  |
| ------------- |---------------                    | -------------|
| <span data-ttu-id="cd2d4-120">id</span><span class="sxs-lookup"><span data-stu-id="cd2d4-120">id</span></span>                    | <span data-ttu-id="cd2d4-121">字符串</span><span class="sxs-lookup"><span data-stu-id="cd2d4-121">String</span></span>                    | <span data-ttu-id="cd2d4-122">关系的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="cd2d4-122">Unique identifier of the relationship.</span></span> <span data-ttu-id="cd2d4-123">只读。</span><span class="sxs-lookup"><span data-stu-id="cd2d4-123">Read only.</span></span>        |
| <span data-ttu-id="cd2d4-124">weight</span><span class="sxs-lookup"><span data-stu-id="cd2d4-124">weight</span></span>                | <span data-ttu-id="cd2d4-125">双精度数</span><span class="sxs-lookup"><span data-stu-id="cd2d4-125">Double</span></span>                    | <span data-ttu-id="cd2d4-126">值，该值指示当前趋势多少文档。</span><span class="sxs-lookup"><span data-stu-id="cd2d4-126">Value indicating how much the document is currently trending.</span></span> <span data-ttu-id="cd2d4-127">较大的号码，更多文档当前趋势周围用户 （更多相关)。</span><span class="sxs-lookup"><span data-stu-id="cd2d4-127">The larger the number, the more the document is currently trending around the user (the more relevant it is).</span></span> <span data-ttu-id="cd2d4-128">按此值，返回的文档进行排序。</span><span class="sxs-lookup"><span data-stu-id="cd2d4-128">Returned documents are sorted by this value.</span></span>  |
| <span data-ttu-id="cd2d4-129">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="cd2d4-129">resourceVisualization</span></span> | [<span data-ttu-id="cd2d4-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="cd2d4-130">resourceVisualization</span></span>](insights-resourcevisualization.md)    | <span data-ttu-id="cd2d4-131">您可以使用可视化中您的体验的文档的属性。</span><span class="sxs-lookup"><span data-stu-id="cd2d4-131">Properties that you can use to visualize the document in your experience.</span></span> |
| <span data-ttu-id="cd2d4-132">resourceReference</span><span class="sxs-lookup"><span data-stu-id="cd2d4-132">resourceReference</span></span>     | [<span data-ttu-id="cd2d4-133">resourceReference</span><span class="sxs-lookup"><span data-stu-id="cd2d4-133">resourceReference</span></span>](insights-resourcereference.md)        | <span data-ttu-id="cd2d4-134">趋势文档，如 url 和的文档类型的引用属性。</span><span class="sxs-lookup"><span data-stu-id="cd2d4-134">Reference properties of the trending document, such as the url and type of the document.</span></span> |

## <a name="relationships"></a><span data-ttu-id="cd2d4-135">Relationships</span><span class="sxs-lookup"><span data-stu-id="cd2d4-135">Relationships</span></span>

| <span data-ttu-id="cd2d4-136">属性</span><span class="sxs-lookup"><span data-stu-id="cd2d4-136">Property</span></span>      | <span data-ttu-id="cd2d4-137">类型</span><span class="sxs-lookup"><span data-stu-id="cd2d4-137">Type</span></span>          | <span data-ttu-id="cd2d4-138">说明</span><span class="sxs-lookup"><span data-stu-id="cd2d4-138">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="cd2d4-139">资源</span><span class="sxs-lookup"><span data-stu-id="cd2d4-139">resource</span></span>      | <span data-ttu-id="cd2d4-140">实体</span><span class="sxs-lookup"><span data-stu-id="cd2d4-140">Entity</span></span>        | <span data-ttu-id="cd2d4-141">用于导航到趋势文档。</span><span class="sxs-lookup"><span data-stu-id="cd2d4-141">Used for navigating to the trending document.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cd2d4-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cd2d4-142">JSON representation</span></span>

<span data-ttu-id="cd2d4-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cd2d4-143">Here is a JSON representation of the resource</span></span>

```json
{
  "id": "string",
  "weight": "double",
  "resourceVisualization": [{"@odata.type": "microsoft.graph.resourceVisualization"}],
  "resourceReference": [{"@odata.type": "microsoft.graph.resourceReference"}],
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```