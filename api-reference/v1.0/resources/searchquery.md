---
title: searchQuery 资源类型
description: searchQuery
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 3745083b404a8de6f68844af9b1767ac2319059f
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377969"
---
# <a name="searchquery-resource-type"></a><span data-ttu-id="09487-103">searchQuery 资源类型</span><span class="sxs-lookup"><span data-stu-id="09487-103">searchQuery resource type</span></span>

<span data-ttu-id="09487-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09487-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="09487-105">表示包含搜索词和可选筛选器的搜索查询。</span><span class="sxs-lookup"><span data-stu-id="09487-105">Represents a search query that contains search terms and optional filters.</span></span>

## <a name="properties"></a><span data-ttu-id="09487-106">属性</span><span class="sxs-lookup"><span data-stu-id="09487-106">Properties</span></span>

| <span data-ttu-id="09487-107">属性</span><span class="sxs-lookup"><span data-stu-id="09487-107">Property</span></span>     | <span data-ttu-id="09487-108">类型</span><span class="sxs-lookup"><span data-stu-id="09487-108">Type</span></span>        | <span data-ttu-id="09487-109">说明</span><span class="sxs-lookup"><span data-stu-id="09487-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="09487-110">queryString</span><span class="sxs-lookup"><span data-stu-id="09487-110">queryString</span></span>|<span data-ttu-id="09487-111">字符串</span><span class="sxs-lookup"><span data-stu-id="09487-111">String</span></span>|<span data-ttu-id="09487-112">包含搜索词的搜索查询。</span><span class="sxs-lookup"><span data-stu-id="09487-112">The search query containing the search terms.</span></span> <span data-ttu-id="09487-113">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="09487-113">Required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="09487-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="09487-114">JSON representation</span></span>

<span data-ttu-id="09487-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09487-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchQuery",
  "baseType": null
}-->

```json
{
  "queryString": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchQuery resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

