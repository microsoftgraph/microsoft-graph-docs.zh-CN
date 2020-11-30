---
title: searchHit 资源类型
description: SearchHit 实体的说明
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: bad671657e46068263d3386eb0bb04026cfaa28e
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377968"
---
# <a name="searchhit-resource-type"></a><span data-ttu-id="b7313-103">searchHit 资源类型</span><span class="sxs-lookup"><span data-stu-id="b7313-103">searchHit resource type</span></span>

<span data-ttu-id="b7313-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7313-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b7313-105">代表搜索结果列表中的单个结果。</span><span class="sxs-lookup"><span data-stu-id="b7313-105">Represents a single result within the list of search results.</span></span>

## <a name="properties"></a><span data-ttu-id="b7313-106">属性</span><span class="sxs-lookup"><span data-stu-id="b7313-106">Properties</span></span>

| <span data-ttu-id="b7313-107">属性</span><span class="sxs-lookup"><span data-stu-id="b7313-107">Property</span></span>     | <span data-ttu-id="b7313-108">类型</span><span class="sxs-lookup"><span data-stu-id="b7313-108">Type</span></span>        | <span data-ttu-id="b7313-109">说明</span><span class="sxs-lookup"><span data-stu-id="b7313-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b7313-110">hitId</span><span class="sxs-lookup"><span data-stu-id="b7313-110">hitId</span></span>|<span data-ttu-id="b7313-111">字符串</span><span class="sxs-lookup"><span data-stu-id="b7313-111">String</span></span>|<span data-ttu-id="b7313-112">项的内部标识符。</span><span class="sxs-lookup"><span data-stu-id="b7313-112">The internal identifier for the item.</span></span>|
|<span data-ttu-id="b7313-113">排名</span><span class="sxs-lookup"><span data-stu-id="b7313-113">rank</span></span>|<span data-ttu-id="b7313-114">Int32</span><span class="sxs-lookup"><span data-stu-id="b7313-114">Int32</span></span>|<span data-ttu-id="b7313-115">结果的排名或顺序。</span><span class="sxs-lookup"><span data-stu-id="b7313-115">The rank or the order of the result.</span></span>|
|<span data-ttu-id="b7313-116">contentSource</span><span class="sxs-lookup"><span data-stu-id="b7313-116">contentSource</span></span>|<span data-ttu-id="b7313-117">字符串</span><span class="sxs-lookup"><span data-stu-id="b7313-117">String</span></span>|<span data-ttu-id="b7313-118">**ExternalItem** 所属的内容源的名称。</span><span class="sxs-lookup"><span data-stu-id="b7313-118">The name of the content source which the **externalItem** is part of .</span></span>|
|<span data-ttu-id="b7313-119">摘要</span><span class="sxs-lookup"><span data-stu-id="b7313-119">summary</span></span>|<span data-ttu-id="b7313-120">字符串</span><span class="sxs-lookup"><span data-stu-id="b7313-120">String</span></span>|<span data-ttu-id="b7313-121">如果摘要可用，则为结果摘要。</span><span class="sxs-lookup"><span data-stu-id="b7313-121">A summary of the result, if a summary is available.</span></span>|
|<span data-ttu-id="b7313-122">resource</span><span class="sxs-lookup"><span data-stu-id="b7313-122">resource</span></span>|[<span data-ttu-id="b7313-123">实体</span><span class="sxs-lookup"><span data-stu-id="b7313-123">entity</span></span>](entity.md)|<span data-ttu-id="b7313-124">搜索结果的基本 Microsoft Graph 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b7313-124">The underlying Microsoft Graph representation of the search result.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b7313-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b7313-125">JSON representation</span></span>

<span data-ttu-id="b7313-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b7313-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchHit",
  "baseType": null
}-->

```json
{
  "hitId": "String",
  "rank": 1,
  "summary": "String",
  "contentSource": "String",
  "resource": { "@odata.type": "microsoft.graph.entity" }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchHit resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

