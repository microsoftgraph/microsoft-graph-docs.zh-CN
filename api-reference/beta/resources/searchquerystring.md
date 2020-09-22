---
title: searchQueryString 资源类型
description: searchQueryString
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 70c029ccb7751287b090015467549169dde4bae9
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193252"
---
# <a name="searchquerystring-resource-type-deprecated"></a><span data-ttu-id="d2433-103">searchQueryString 资源类型 (弃用) </span><span class="sxs-lookup"><span data-stu-id="d2433-103">searchQueryString resource type (deprecated)</span></span>

<span data-ttu-id="d2433-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2433-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]
<span data-ttu-id="d2433-105">查询的搜索词。</span><span class="sxs-lookup"><span data-stu-id="d2433-105">The search terms for the query.</span></span>

## <a name="properties"></a><span data-ttu-id="d2433-106">属性</span><span class="sxs-lookup"><span data-stu-id="d2433-106">Properties</span></span>

| <span data-ttu-id="d2433-107">属性</span><span class="sxs-lookup"><span data-stu-id="d2433-107">Property</span></span>     | <span data-ttu-id="d2433-108">类型</span><span class="sxs-lookup"><span data-stu-id="d2433-108">Type</span></span>        | <span data-ttu-id="d2433-109">描述</span><span class="sxs-lookup"><span data-stu-id="d2433-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d2433-110">查询</span><span class="sxs-lookup"><span data-stu-id="d2433-110">query</span></span>|<span data-ttu-id="d2433-111">字符串</span><span class="sxs-lookup"><span data-stu-id="d2433-111">String</span></span>|<span data-ttu-id="d2433-112">包含请求的实际搜索词。</span><span class="sxs-lookup"><span data-stu-id="d2433-112">Contains the actual search terms of the request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d2433-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d2433-113">JSON representation</span></span>

<span data-ttu-id="d2433-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2433-114">The following is a JSON representation of the resource.</span></span>

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

