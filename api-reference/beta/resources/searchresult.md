---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SearchResult
localization_priority: Normal
ms.openlocfilehash: 6b7376fcfcfc15ea2ce5807a828854e5bdf9c719
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884649"
---
# <a name="searchresult-resource-type"></a><span data-ttu-id="f0b3d-102">SearchResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="f0b3d-102">SearchResult resource type</span></span>

> <span data-ttu-id="f0b3d-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f0b3d-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f0b3d-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f0b3d-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f0b3d-105">**SearchResult** 资源指示项是搜索查询的响应。</span><span class="sxs-lookup"><span data-stu-id="f0b3d-105">The **SearchResult** resource indicates than an item is the response to a search query.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f0b3d-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f0b3d-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="f0b3d-107">属性</span><span class="sxs-lookup"><span data-stu-id="f0b3d-107">Properties</span></span>

| <span data-ttu-id="f0b3d-108">属性</span><span class="sxs-lookup"><span data-stu-id="f0b3d-108">Property</span></span>            | <span data-ttu-id="f0b3d-109">类型</span><span class="sxs-lookup"><span data-stu-id="f0b3d-109">Type</span></span>   | <span data-ttu-id="f0b3d-110">说明</span><span class="sxs-lookup"><span data-stu-id="f0b3d-110">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="f0b3d-111">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="f0b3d-111">onClickTelemetryUrl</span></span> | <span data-ttu-id="f0b3d-112">字符串</span><span class="sxs-lookup"><span data-stu-id="f0b3d-112">String</span></span> | <span data-ttu-id="f0b3d-p102">可用于记录遥测信息的回调 URL。如果用户与此项交互以改善结果的质量，应用程序应在此 URL 中发出 GET。</span><span class="sxs-lookup"><span data-stu-id="f0b3d-p102">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="f0b3d-115">注解</span><span class="sxs-lookup"><span data-stu-id="f0b3d-115">Remarks</span></span> 

<span data-ttu-id="f0b3d-116">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="f0b3d-116">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The search result facet indicates an item is from a search.",
  "keywords": "search result facet",
  "section": "documentation",
  "tocPath": "Facets/SearchResult"
} -->
