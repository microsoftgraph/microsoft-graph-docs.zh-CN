---
title: searchResultSet 资源类型
description: searchResultSet 的说明
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: ee5ac6d892b6562ca5c1053b474135f1dd745ba5
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210204"
---
# <a name="searchresultset-resource-type"></a><span data-ttu-id="2778f-103">searchResultSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="2778f-103">searchResultSet resource type</span></span>

<span data-ttu-id="2778f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2778f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2778f-105">表示来自搜索查询的结果，以及用于查询的术语。</span><span class="sxs-lookup"><span data-stu-id="2778f-105">Represents results from a search query, and the terms used for the query.</span></span> 

## <a name="properties"></a><span data-ttu-id="2778f-106">属性</span><span class="sxs-lookup"><span data-stu-id="2778f-106">Properties</span></span>

| <span data-ttu-id="2778f-107">属性</span><span class="sxs-lookup"><span data-stu-id="2778f-107">Property</span></span>     | <span data-ttu-id="2778f-108">类型</span><span class="sxs-lookup"><span data-stu-id="2778f-108">Type</span></span>        | <span data-ttu-id="2778f-109">说明</span><span class="sxs-lookup"><span data-stu-id="2778f-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2778f-110">hitsContainers</span><span class="sxs-lookup"><span data-stu-id="2778f-110">hitsContainers</span></span>|<span data-ttu-id="2778f-111">[searchHitsContainer](searchhitscontainer.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2778f-111">[searchHitsContainer](searchhitscontainer.md) collection</span></span>|<span data-ttu-id="2778f-112">搜索结果的集合。</span><span class="sxs-lookup"><span data-stu-id="2778f-112">A collection of search results.</span></span>|
|<span data-ttu-id="2778f-113">searchTerms</span><span class="sxs-lookup"><span data-stu-id="2778f-113">searchTerms</span></span>|<span data-ttu-id="2778f-114">String collection</span><span class="sxs-lookup"><span data-stu-id="2778f-114">String collection</span></span>|<span data-ttu-id="2778f-115">包含初始搜索查询中发送的搜索词。</span><span class="sxs-lookup"><span data-stu-id="2778f-115">Contains the search terms sent in the initial search query.</span></span>|
|<span data-ttu-id="2778f-116">resultTemplates</span><span class="sxs-lookup"><span data-stu-id="2778f-116">resultTemplates</span></span>|<span data-ttu-id="2778f-117">[resultTemplate](resultTemplate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2778f-117">[resultTemplate](resultTemplate.md) collection</span></span>|<span data-ttu-id="2778f-118">resultTemplateIds 和关联值的字典，其中包括结果模板的名称和 JSON 架构。</span><span class="sxs-lookup"><span data-stu-id="2778f-118">A dictionary of resultTemplateIds and associated values, which include the name and JSON schema of the result templates.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2778f-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2778f-119">JSON representation</span></span>

<span data-ttu-id="2778f-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2778f-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchResultSet",
  "baseType": null
}-->

```json
{
  "hitsContainers": [{"@odata.type": "microsoft.graph.searchHitsContainer"}],
  "searchTerms": ["String"],
  "resultTemplates": [{"@odata.type":"microsoft.graph.resultTemplateDictionary"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchResultSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

