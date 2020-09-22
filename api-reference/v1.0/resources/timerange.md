---
title: timeRange 资源类型
description: 具有开始和结束时间的时间范围资源。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 64f018cb0c554ae36c9ec0b8ec0bfa655b7499f4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090758"
---
# <a name="timerange-resource-type"></a><span data-ttu-id="5bcc6-103">timeRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="5bcc6-103">timeRange resource type</span></span>

<span data-ttu-id="5bcc6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bcc6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5bcc6-105">具有开始和结束时间的时间范围资源。</span><span class="sxs-lookup"><span data-stu-id="5bcc6-105">A time range resource with a start and end time.</span></span>

## <a name="properties"></a><span data-ttu-id="5bcc6-106">属性</span><span class="sxs-lookup"><span data-stu-id="5bcc6-106">Properties</span></span>

| <span data-ttu-id="5bcc6-107">属性</span><span class="sxs-lookup"><span data-stu-id="5bcc6-107">Property</span></span>     | <span data-ttu-id="5bcc6-108">类型</span><span class="sxs-lookup"><span data-stu-id="5bcc6-108">Type</span></span>        | <span data-ttu-id="5bcc6-109">说明</span><span class="sxs-lookup"><span data-stu-id="5bcc6-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5bcc6-110">endTime</span><span class="sxs-lookup"><span data-stu-id="5bcc6-110">endTime</span></span>|<span data-ttu-id="5bcc6-111">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="5bcc6-111">TimeOfDay</span></span>|<span data-ttu-id="5bcc6-112">时间范围的结束时间。</span><span class="sxs-lookup"><span data-stu-id="5bcc6-112">End time for the time range.</span></span>|
|<span data-ttu-id="5bcc6-113">startTime</span><span class="sxs-lookup"><span data-stu-id="5bcc6-113">startTime</span></span>|<span data-ttu-id="5bcc6-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="5bcc6-114">TimeOfDay</span></span>|<span data-ttu-id="5bcc6-115">时间范围的开始时间。</span><span class="sxs-lookup"><span data-stu-id="5bcc6-115">Start time for the time range.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5bcc6-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5bcc6-116">JSON representation</span></span>

<span data-ttu-id="5bcc6-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5bcc6-117">The following is a JSON representation of the resource.</span></span>

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
