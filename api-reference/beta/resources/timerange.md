---
title: timeRange 资源类型
description: 具有开始和结束时间的时间范围资源。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0e91f08e9f421a348f5ec7c2ebf5e2f23d4e9377
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952312"
---
# <a name="timerange-resource-type"></a><span data-ttu-id="7f66c-103">timeRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="7f66c-103">timeRange resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f66c-104">具有开始和结束时间的时间范围资源。</span><span class="sxs-lookup"><span data-stu-id="7f66c-104">A time range resource with a start and end time.</span></span>

## <a name="properties"></a><span data-ttu-id="7f66c-105">属性</span><span class="sxs-lookup"><span data-stu-id="7f66c-105">Properties</span></span>

| <span data-ttu-id="7f66c-106">属性</span><span class="sxs-lookup"><span data-stu-id="7f66c-106">Property</span></span>     | <span data-ttu-id="7f66c-107">类型</span><span class="sxs-lookup"><span data-stu-id="7f66c-107">Type</span></span>        | <span data-ttu-id="7f66c-108">Description</span><span class="sxs-lookup"><span data-stu-id="7f66c-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7f66c-109">endTime</span><span class="sxs-lookup"><span data-stu-id="7f66c-109">endTime</span></span>|<span data-ttu-id="7f66c-110">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="7f66c-110">TimeOfDay</span></span>|<span data-ttu-id="7f66c-111">时间范围的结束时间。</span><span class="sxs-lookup"><span data-stu-id="7f66c-111">End time for the time range.</span></span>|
|<span data-ttu-id="7f66c-112">startTime</span><span class="sxs-lookup"><span data-stu-id="7f66c-112">startTime</span></span>|<span data-ttu-id="7f66c-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="7f66c-113">TimeOfDay</span></span>|<span data-ttu-id="7f66c-114">时间范围的开始时间。</span><span class="sxs-lookup"><span data-stu-id="7f66c-114">Start time for the time range.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7f66c-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7f66c-115">JSON representation</span></span>

<span data-ttu-id="7f66c-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7f66c-116">The following is a JSON representation of the resource.</span></span>

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