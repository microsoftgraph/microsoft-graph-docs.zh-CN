---
title: audioDuckingConfiguration 资源类型
description: 其他源的 ducking 参数（逐步淘汰 in 和其他来源。）
author: ananmishr
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 99aa202e0048b328d97453f57d249df749f7bce5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508113"
---
# <a name="audioduckingconfiguration-resource-type"></a><span data-ttu-id="00769-103">audioDuckingConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="00769-103">audioDuckingConfiguration resource type</span></span>

<span data-ttu-id="00769-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="00769-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00769-105">其他源的 ducking 参数（逐步淘汰 in 和其他来源。）</span><span class="sxs-lookup"><span data-stu-id="00769-105">Parameters for ducking of other sources (phasing in and out of other sources.)</span></span>

## <a name="properties"></a><span data-ttu-id="00769-106">属性</span><span class="sxs-lookup"><span data-stu-id="00769-106">Properties</span></span>

| <span data-ttu-id="00769-107">属性</span><span class="sxs-lookup"><span data-stu-id="00769-107">Property</span></span>      | <span data-ttu-id="00769-108">类型</span><span class="sxs-lookup"><span data-stu-id="00769-108">Type</span></span>     | <span data-ttu-id="00769-109">说明</span><span class="sxs-lookup"><span data-stu-id="00769-109">Description</span></span>                                                                     |
| :------------ | :------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="00769-110">lowerLevel</span><span class="sxs-lookup"><span data-stu-id="00769-110">lowerLevel</span></span>    | <span data-ttu-id="00769-111">Int64</span><span class="sxs-lookup"><span data-stu-id="00769-111">Int64</span></span>    | <span data-ttu-id="00769-112">源正在 ducked 时，源的数量（以百分比为单位）。</span><span class="sxs-lookup"><span data-stu-id="00769-112">The volume of sources in percent when the sources are being ducked.</span></span>             |
| <span data-ttu-id="00769-113">rampActive</span><span class="sxs-lookup"><span data-stu-id="00769-113">rampActive</span></span>    | <span data-ttu-id="00769-114">Int64</span><span class="sxs-lookup"><span data-stu-id="00769-114">Int64</span></span>    | <span data-ttu-id="00769-115">Ducked 源到 "淡出" 所需的时间量（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="00769-115">The amount of time (in milliseconds) it takes for ducked sources to "fade out".</span></span> |
| <span data-ttu-id="00769-116">rampInactive</span><span class="sxs-lookup"><span data-stu-id="00769-116">rampInactive</span></span>  | <span data-ttu-id="00769-117">Int64</span><span class="sxs-lookup"><span data-stu-id="00769-117">Int64</span></span>    | <span data-ttu-id="00769-118">Ducked 源到 "淡入" 所需的时间（以毫秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="00769-118">The amount of time (in milliseconds) it takes for ducked sources to "fade in".</span></span>  |
| <span data-ttu-id="00769-119">upperLevel</span><span class="sxs-lookup"><span data-stu-id="00769-119">upperLevel</span></span>    | <span data-ttu-id="00769-120">Int64</span><span class="sxs-lookup"><span data-stu-id="00769-120">Int64</span></span>    | <span data-ttu-id="00769-121">源未 ducked 时的源数量（以百分比为单位）。</span><span class="sxs-lookup"><span data-stu-id="00769-121">The volume of sources in percent when the sources are not being ducked.</span></span>         |

> <span data-ttu-id="00769-122">**注意：** 斜向持续时间不能超过5000毫秒。</span><span class="sxs-lookup"><span data-stu-id="00769-122">**Note:** Ramp duration cannot be more than 5,000 milliseconds.</span></span>

## <a name="json-representation"></a><span data-ttu-id="00769-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="00769-123">JSON representation</span></span>

<span data-ttu-id="00769-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00769-124">The following is a JSON representation of the resource.</span></span>

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
