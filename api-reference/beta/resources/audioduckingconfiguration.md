---
title: audioDuckingConfiguration 资源类型
description: '用于 ducking 的其他源的参数 (逐步淘汰的其他源。 ) '
author: ananmishr
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 795ad9b1740d36a365bea4d99a880c43308a01c8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024421"
---
# <a name="audioduckingconfiguration-resource-type"></a><span data-ttu-id="2a175-103">audioDuckingConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="2a175-103">audioDuckingConfiguration resource type</span></span>

<span data-ttu-id="2a175-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a175-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a175-105">用于 ducking 的其他源的参数 (逐步淘汰的其他源。 ) </span><span class="sxs-lookup"><span data-stu-id="2a175-105">Parameters for ducking of other sources (phasing in and out of other sources.)</span></span>

## <a name="properties"></a><span data-ttu-id="2a175-106">属性</span><span class="sxs-lookup"><span data-stu-id="2a175-106">Properties</span></span>

| <span data-ttu-id="2a175-107">属性</span><span class="sxs-lookup"><span data-stu-id="2a175-107">Property</span></span>      | <span data-ttu-id="2a175-108">类型</span><span class="sxs-lookup"><span data-stu-id="2a175-108">Type</span></span>     | <span data-ttu-id="2a175-109">说明</span><span class="sxs-lookup"><span data-stu-id="2a175-109">Description</span></span>                                                                     |
| :------------ | :------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="2a175-110">lowerLevel</span><span class="sxs-lookup"><span data-stu-id="2a175-110">lowerLevel</span></span>    | <span data-ttu-id="2a175-111">Int64</span><span class="sxs-lookup"><span data-stu-id="2a175-111">Int64</span></span>    | <span data-ttu-id="2a175-112">源正在 ducked 时，源的数量（以百分比为单位）。</span><span class="sxs-lookup"><span data-stu-id="2a175-112">The volume of sources in percent when the sources are being ducked.</span></span>             |
| <span data-ttu-id="2a175-113">rampActive</span><span class="sxs-lookup"><span data-stu-id="2a175-113">rampActive</span></span>    | <span data-ttu-id="2a175-114">Int64</span><span class="sxs-lookup"><span data-stu-id="2a175-114">Int64</span></span>    | <span data-ttu-id="2a175-115">Ducked 源为 "淡出" 所需的时间量（以毫秒为单位）)  (。</span><span class="sxs-lookup"><span data-stu-id="2a175-115">The amount of time (in milliseconds) it takes for ducked sources to "fade out".</span></span> |
| <span data-ttu-id="2a175-116">rampInactive</span><span class="sxs-lookup"><span data-stu-id="2a175-116">rampInactive</span></span>  | <span data-ttu-id="2a175-117">Int64</span><span class="sxs-lookup"><span data-stu-id="2a175-117">Int64</span></span>    | <span data-ttu-id="2a175-118">Ducked 源) 为 "淡入" 所需的时间量（以毫秒为单位） (。</span><span class="sxs-lookup"><span data-stu-id="2a175-118">The amount of time (in milliseconds) it takes for ducked sources to "fade in".</span></span>  |
| <span data-ttu-id="2a175-119">upperLevel</span><span class="sxs-lookup"><span data-stu-id="2a175-119">upperLevel</span></span>    | <span data-ttu-id="2a175-120">Int64</span><span class="sxs-lookup"><span data-stu-id="2a175-120">Int64</span></span>    | <span data-ttu-id="2a175-121">源未 ducked 时的源数量（以百分比为单位）。</span><span class="sxs-lookup"><span data-stu-id="2a175-121">The volume of sources in percent when the sources are not being ducked.</span></span>         |

> <span data-ttu-id="2a175-122">**注意：** 斜向持续时间不能超过5000毫秒。</span><span class="sxs-lookup"><span data-stu-id="2a175-122">**Note:** Ramp duration cannot be more than 5,000 milliseconds.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2a175-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2a175-123">JSON representation</span></span>

<span data-ttu-id="2a175-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a175-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioDuckingConfiguration"
}-->
```json
{
  "lowerLevel": 20,
  "rampActive": 1000,
  "rampInactive": 1000,
  "upperLevel": 100
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioDuckingConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


