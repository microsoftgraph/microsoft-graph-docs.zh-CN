---
title: searchQueryString 资源类型
description: searchQueryString
localization_priority: Normal
author: nmoreau
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b273d9ec15b949019b780dd5ce9f1a6184191763
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520904"
---
# <a name="searchquerystring-resource-type"></a><span data-ttu-id="5658b-103">searchQueryString 资源类型</span><span class="sxs-lookup"><span data-stu-id="5658b-103">searchQueryString resource type</span></span>

<span data-ttu-id="5658b-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="5658b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5658b-105">查询的搜索词。</span><span class="sxs-lookup"><span data-stu-id="5658b-105">The search terms for the query.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="5658b-106">属性</span><span class="sxs-lookup"><span data-stu-id="5658b-106">Properties</span></span>

| <span data-ttu-id="5658b-107">属性</span><span class="sxs-lookup"><span data-stu-id="5658b-107">Property</span></span>     | <span data-ttu-id="5658b-108">类型</span><span class="sxs-lookup"><span data-stu-id="5658b-108">Type</span></span>        | <span data-ttu-id="5658b-109">说明</span><span class="sxs-lookup"><span data-stu-id="5658b-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5658b-110">查询</span><span class="sxs-lookup"><span data-stu-id="5658b-110">query</span></span>|<span data-ttu-id="5658b-111">String</span><span class="sxs-lookup"><span data-stu-id="5658b-111">String</span></span>|<span data-ttu-id="5658b-112">包含请求的实际搜索词。</span><span class="sxs-lookup"><span data-stu-id="5658b-112">Contains the actual search terms of the request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5658b-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5658b-113">JSON representation</span></span>

<span data-ttu-id="5658b-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5658b-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchQueryString",
  "baseType": null
}-->

```json
{
  "query": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchQueryString resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->