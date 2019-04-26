---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: searchresult.xml
localization_priority: Normal
ms.openlocfilehash: 025d18a48105ddb5834040aba5944a9bd408cfbc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562963"
---
# <a name="searchresult-resource-type"></a><span data-ttu-id="edf83-102">SearchResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="edf83-102">SearchResult resource type</span></span>

<span data-ttu-id="edf83-103">**SearchResult** 资源指示项是搜索查询的响应。</span><span class="sxs-lookup"><span data-stu-id="edf83-103">The **SearchResult** resource indicates than an item is the response to a search query.</span></span>

## <a name="json-representation"></a><span data-ttu-id="edf83-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="edf83-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="edf83-105">属性</span><span class="sxs-lookup"><span data-stu-id="edf83-105">Properties</span></span>

| <span data-ttu-id="edf83-106">属性</span><span class="sxs-lookup"><span data-stu-id="edf83-106">Property</span></span>            | <span data-ttu-id="edf83-107">类型</span><span class="sxs-lookup"><span data-stu-id="edf83-107">Type</span></span>   | <span data-ttu-id="edf83-108">说明</span><span class="sxs-lookup"><span data-stu-id="edf83-108">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="edf83-109">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="edf83-109">onClickTelemetryUrl</span></span> | <span data-ttu-id="edf83-110">String</span><span class="sxs-lookup"><span data-stu-id="edf83-110">String</span></span> | <span data-ttu-id="edf83-p101">可用于记录遥测信息的回调 URL。如果用户与此项交互以改善结果的质量，应用程序应在此 URL 中发出 GET。</span><span class="sxs-lookup"><span data-stu-id="edf83-p101">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="edf83-113">注解</span><span class="sxs-lookup"><span data-stu-id="edf83-113">Remarks</span></span> 

<span data-ttu-id="edf83-114">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="edf83-114">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The search result facet indicates an item is from a search.",
  "keywords": "search result facet",
  "section": "documentation",
  "tocPath": "Facets/SearchResult"
} -->
