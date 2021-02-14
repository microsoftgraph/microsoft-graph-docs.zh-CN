---
author: JeremyKelley
ms.date: 09/10/2017
title: SearchResult
localization_priority: Normal
description: SearchResult 资源指示项是搜索查询的响应。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: aac8ee9c4dea8ba7744e5c86d865b4d2f75a37d8
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240099"
---
# <a name="searchresult-resource-type"></a><span data-ttu-id="b3fa8-103">SearchResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="b3fa8-103">SearchResult resource type</span></span>

<span data-ttu-id="b3fa8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3fa8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b3fa8-105">**SearchResult** 资源指示项是搜索查询的响应。</span><span class="sxs-lookup"><span data-stu-id="b3fa8-105">The **SearchResult** resource indicates than an item is the response to a search query.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3fa8-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b3fa8-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "onClickTelemtryUrl" ],
  "@odata.type": "microsoft.graph.searchResult"
}-->

```json
{
  "onClickTelemetryUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="b3fa8-107">属性</span><span class="sxs-lookup"><span data-stu-id="b3fa8-107">Properties</span></span>

| <span data-ttu-id="b3fa8-108">属性</span><span class="sxs-lookup"><span data-stu-id="b3fa8-108">Property</span></span>            | <span data-ttu-id="b3fa8-109">类型</span><span class="sxs-lookup"><span data-stu-id="b3fa8-109">Type</span></span>   | <span data-ttu-id="b3fa8-110">说明</span><span class="sxs-lookup"><span data-stu-id="b3fa8-110">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="b3fa8-111">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="b3fa8-111">onClickTelemetryUrl</span></span> | <span data-ttu-id="b3fa8-112">String</span><span class="sxs-lookup"><span data-stu-id="b3fa8-112">String</span></span> | <span data-ttu-id="b3fa8-p101">可用于记录遥测信息的回调 URL。如果用户与此项交互以改善结果的质量，应用程序应在此 URL 中发出 GET。</span><span class="sxs-lookup"><span data-stu-id="b3fa8-p101">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="b3fa8-115">注解</span><span class="sxs-lookup"><span data-stu-id="b3fa8-115">Remarks</span></span> 

<span data-ttu-id="b3fa8-116">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="b3fa8-116">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The search result facet indicates an item is from a search.",
  "keywords": "search result facet",
  "section": "documentation",
  "tocPath": "Facets/SearchResult"
} -->

