---
title: timeRange 资源类型
description: 具有开始和结束时间的时间范围资源。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e9edfd06ecd65d7e08d6701d1fc885dce9067689
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519706"
---
# <a name="timerange-resource-type"></a><span data-ttu-id="fc32a-103">timeRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="fc32a-103">timeRange resource type</span></span>

<span data-ttu-id="fc32a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="fc32a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc32a-105">具有开始和结束时间的时间范围资源。</span><span class="sxs-lookup"><span data-stu-id="fc32a-105">A time range resource with a start and end time.</span></span>

## <a name="properties"></a><span data-ttu-id="fc32a-106">属性</span><span class="sxs-lookup"><span data-stu-id="fc32a-106">Properties</span></span>

| <span data-ttu-id="fc32a-107">属性</span><span class="sxs-lookup"><span data-stu-id="fc32a-107">Property</span></span>     | <span data-ttu-id="fc32a-108">类型</span><span class="sxs-lookup"><span data-stu-id="fc32a-108">Type</span></span>        | <span data-ttu-id="fc32a-109">说明</span><span class="sxs-lookup"><span data-stu-id="fc32a-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fc32a-110">endTime</span><span class="sxs-lookup"><span data-stu-id="fc32a-110">endTime</span></span>|<span data-ttu-id="fc32a-111">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="fc32a-111">TimeOfDay</span></span>|<span data-ttu-id="fc32a-112">时间范围的结束时间。</span><span class="sxs-lookup"><span data-stu-id="fc32a-112">End time for the time range.</span></span>|
|<span data-ttu-id="fc32a-113">startTime</span><span class="sxs-lookup"><span data-stu-id="fc32a-113">startTime</span></span>|<span data-ttu-id="fc32a-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="fc32a-114">TimeOfDay</span></span>|<span data-ttu-id="fc32a-115">时间范围的开始时间。</span><span class="sxs-lookup"><span data-stu-id="fc32a-115">Start time for the time range.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fc32a-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fc32a-116">JSON representation</span></span>

<span data-ttu-id="fc32a-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc32a-117">The following is a JSON representation of the resource.</span></span>

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