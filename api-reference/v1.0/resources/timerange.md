---
title: timeRange 资源类型
description: 具有开始和结束时间的时间范围资源。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 12cdae2407ea985b28afb658c7fd7517fdbb687c
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154162"
---
# <a name="timerange-resource-type"></a><span data-ttu-id="83cd5-103">timeRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="83cd5-103">timeRange resource type</span></span>

<span data-ttu-id="83cd5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83cd5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="83cd5-105">具有开始和结束时间的时间范围资源。</span><span class="sxs-lookup"><span data-stu-id="83cd5-105">A time range resource with a start and end time.</span></span>

## <a name="properties"></a><span data-ttu-id="83cd5-106">属性</span><span class="sxs-lookup"><span data-stu-id="83cd5-106">Properties</span></span>

| <span data-ttu-id="83cd5-107">属性</span><span class="sxs-lookup"><span data-stu-id="83cd5-107">Property</span></span>     | <span data-ttu-id="83cd5-108">类型</span><span class="sxs-lookup"><span data-stu-id="83cd5-108">Type</span></span>        | <span data-ttu-id="83cd5-109">Description</span><span class="sxs-lookup"><span data-stu-id="83cd5-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="83cd5-110">endTime</span><span class="sxs-lookup"><span data-stu-id="83cd5-110">endTime</span></span>|<span data-ttu-id="83cd5-111">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="83cd5-111">TimeOfDay</span></span>|<span data-ttu-id="83cd5-112">时间范围的结束时间。</span><span class="sxs-lookup"><span data-stu-id="83cd5-112">End time for the time range.</span></span>|
|<span data-ttu-id="83cd5-113">startTime</span><span class="sxs-lookup"><span data-stu-id="83cd5-113">startTime</span></span>|<span data-ttu-id="83cd5-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="83cd5-114">TimeOfDay</span></span>|<span data-ttu-id="83cd5-115">时间范围的开始时间。</span><span class="sxs-lookup"><span data-stu-id="83cd5-115">Start time for the time range.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="83cd5-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="83cd5-116">JSON representation</span></span>

<span data-ttu-id="83cd5-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83cd5-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeRange",
  "baseType": null
}-->

```json
{
  "endTime": "String (timestamp)",
  "startTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->