---
title: searchAlterationOptions 资源类型
description: 提供用于拼写更正的搜索更改选项。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: dc17698715b4ea6e894ae13f1999e78ab361cc5e
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068001"
---
# <a name="searchalterationoptions-resource-type"></a><span data-ttu-id="0c156-103">searchAlterationOptions 资源类型</span><span class="sxs-lookup"><span data-stu-id="0c156-103">searchAlterationOptions resource type</span></span>

<span data-ttu-id="0c156-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c156-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c156-105">提供用于拼写更正的搜索更改选项。</span><span class="sxs-lookup"><span data-stu-id="0c156-105">Provides the search alteration options for spelling correction.</span></span>

## <a name="properties"></a><span data-ttu-id="0c156-106">属性</span><span class="sxs-lookup"><span data-stu-id="0c156-106">Properties</span></span>

| <span data-ttu-id="0c156-107">属性</span><span class="sxs-lookup"><span data-stu-id="0c156-107">Property</span></span>     | <span data-ttu-id="0c156-108">类型</span><span class="sxs-lookup"><span data-stu-id="0c156-108">Type</span></span>        | <span data-ttu-id="0c156-109">说明</span><span class="sxs-lookup"><span data-stu-id="0c156-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0c156-110">enableSuggestion</span><span class="sxs-lookup"><span data-stu-id="0c156-110">enableSuggestion</span></span>|<span data-ttu-id="0c156-111">布尔值</span><span class="sxs-lookup"><span data-stu-id="0c156-111">Boolean</span></span>|<span data-ttu-id="0c156-112">指示是否启用拼写建议。</span><span class="sxs-lookup"><span data-stu-id="0c156-112">Indicates whether spelling suggestions are enabled.</span></span> <span data-ttu-id="0c156-113">如果启用，用户将获取原始搜索查询的搜索结果，并建议查询中拼写错误的响应的 **queryAlterationResponse** 属性中的 [](/graph/api/resources/searchresponse?view=graph-rest-beta&preserve-view=true)拼写更正。</span><span class="sxs-lookup"><span data-stu-id="0c156-113">If enabled, user will get the search results for original search query and suggesting spelling correction in **queryAlterationResponse** property of the [response](/graph/api/resources/searchresponse?view=graph-rest-beta&preserve-view=true) for typos in query.</span></span> <span data-ttu-id="0c156-114">可选。</span><span class="sxs-lookup"><span data-stu-id="0c156-114">Optional.</span></span>|
|<span data-ttu-id="0c156-115">enableModification</span><span class="sxs-lookup"><span data-stu-id="0c156-115">enableModification</span></span>|<span data-ttu-id="0c156-116">布尔值</span><span class="sxs-lookup"><span data-stu-id="0c156-116">Boolean</span></span>|<span data-ttu-id="0c156-117">指示是否启用拼写修改。</span><span class="sxs-lookup"><span data-stu-id="0c156-117">Indicates whether spelling modifications are enabled.</span></span> <span data-ttu-id="0c156-118">如果启用，则当原始查询没有拼写错误的结果时，用户将获取更正后的查询的搜索结果，并获取响应 的 **queryAlterationResponse** 属性中的拼写修改 [信息](/graph/api/resources/searchresponse?view=graph-rest-beta&preserve-view=true)。</span><span class="sxs-lookup"><span data-stu-id="0c156-118">If enabled, user will get the search results for corrected query **when there are no results** for the original query with typos and get the spelling modification information in **queryAlterationResponse** property of the [response](/graph/api/resources/searchresponse?view=graph-rest-beta&preserve-view=true).</span></span> <span data-ttu-id="0c156-119">可选。</span><span class="sxs-lookup"><span data-stu-id="0c156-119">Optional.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0c156-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0c156-120">JSON representation</span></span>

<span data-ttu-id="0c156-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0c156-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchAlterationOptions",
  "baseType": null
}-->

```json
{
  "enableSuggestion": true,
  "enableModification": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchAlterationOptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
