---
title: searchAlteration 资源类型
description: 提供用于拼写更正的搜索更改的详细信息。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 5caab3a3fbd8f8487e6893c5f5f530cc8471bb80
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068000"
---
# <a name="searchalteration-resource-type"></a><span data-ttu-id="c3195-103">searchAlteration 资源类型</span><span class="sxs-lookup"><span data-stu-id="c3195-103">searchAlteration resource type</span></span>

<span data-ttu-id="c3195-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3195-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3195-105">提供用于拼写更正的搜索更改的详细信息。</span><span class="sxs-lookup"><span data-stu-id="c3195-105">Provides the details of search alteration for spelling correction.</span></span>

## <a name="properties"></a><span data-ttu-id="c3195-106">属性</span><span class="sxs-lookup"><span data-stu-id="c3195-106">Properties</span></span>

| <span data-ttu-id="c3195-107">属性</span><span class="sxs-lookup"><span data-stu-id="c3195-107">Property</span></span>     | <span data-ttu-id="c3195-108">类型</span><span class="sxs-lookup"><span data-stu-id="c3195-108">Type</span></span>        | <span data-ttu-id="c3195-109">说明</span><span class="sxs-lookup"><span data-stu-id="c3195-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c3195-110">alteredQueryString</span><span class="sxs-lookup"><span data-stu-id="c3195-110">alteredQueryString</span></span>|<span data-ttu-id="c3195-111">String</span><span class="sxs-lookup"><span data-stu-id="c3195-111">String</span></span>| <span data-ttu-id="c3195-112">使用拼写更正定义更改的查询字符串。</span><span class="sxs-lookup"><span data-stu-id="c3195-112">Defines the altered query string with spelling correction.</span></span>|
|<span data-ttu-id="c3195-113">alteredHighlightedQueryString</span><span class="sxs-lookup"><span data-stu-id="c3195-113">alteredHighlightedQueryString</span></span>|<span data-ttu-id="c3195-114">String</span><span class="sxs-lookup"><span data-stu-id="c3195-114">String</span></span>| <span data-ttu-id="c3195-115">使用拼写更正定义更改的突出显示查询字符串。</span><span class="sxs-lookup"><span data-stu-id="c3195-115">Defines the altered highlighted query string with spelling correction.</span></span> <span data-ttu-id="c3195-116">更正的线段周围的批注 (\ue000， \ue001) </span><span class="sxs-lookup"><span data-stu-id="c3195-116">The annotation around the corrected segment is (\ue000, \ue001)</span></span>|
|<span data-ttu-id="c3195-117">alteredQueryTokens</span><span class="sxs-lookup"><span data-stu-id="c3195-117">alteredQueryTokens</span></span>|<span data-ttu-id="c3195-118">[alteredQueryToken](alteredquerytoken.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c3195-118">[alteredQueryToken](alteredquerytoken.md) collection</span></span>| <span data-ttu-id="c3195-119">表示与原始查询有关更改的线段。</span><span class="sxs-lookup"><span data-stu-id="c3195-119">Represents changed segments with respect to original query.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c3195-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c3195-120">JSON representation</span></span>

<span data-ttu-id="c3195-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3195-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchAlteration",
  "baseType": null
}-->

```json
{
  "alteredQueryString": "String",
  "alteredHighlightedQueryString": "String",
  "alteredQueryTokens": [{"@odata.type": "microsoft.graph.alteredQueryToken"}]
}
```