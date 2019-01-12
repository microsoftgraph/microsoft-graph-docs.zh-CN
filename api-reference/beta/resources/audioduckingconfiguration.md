---
title: audioDuckingConfiguration 资源类型
description: 参数放掉的其他源 （逐步注销其他源。）
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b4132946573342976bb1f20c593454a8e18030d2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916871"
---
# <a name="audioduckingconfiguration-resource-type"></a><span data-ttu-id="5fa02-103">audioDuckingConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="5fa02-103">audioDuckingConfiguration resource type</span></span>

> <span data-ttu-id="5fa02-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5fa02-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5fa02-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5fa02-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5fa02-106">参数放掉的其他源 （逐步注销其他源。）</span><span class="sxs-lookup"><span data-stu-id="5fa02-106">Parameters for ducking of other sources (phasing in and out of other sources.)</span></span>

## <a name="properties"></a><span data-ttu-id="5fa02-107">属性</span><span class="sxs-lookup"><span data-stu-id="5fa02-107">Properties</span></span>

| <span data-ttu-id="5fa02-108">属性</span><span class="sxs-lookup"><span data-stu-id="5fa02-108">Property</span></span>      | <span data-ttu-id="5fa02-109">类型</span><span class="sxs-lookup"><span data-stu-id="5fa02-109">Type</span></span>     | <span data-ttu-id="5fa02-110">Description</span><span class="sxs-lookup"><span data-stu-id="5fa02-110">Description</span></span>                                                                     |
| :------------ | :------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="5fa02-111">lowerLevel</span><span class="sxs-lookup"><span data-stu-id="5fa02-111">lowerLevel</span></span>    | <span data-ttu-id="5fa02-112">Int64</span><span class="sxs-lookup"><span data-stu-id="5fa02-112">Int64</span></span>    | <span data-ttu-id="5fa02-113">源中时源正在 ducked %的卷。</span><span class="sxs-lookup"><span data-stu-id="5fa02-113">The volume of sources in percent when the sources are being ducked.</span></span>             |
| <span data-ttu-id="5fa02-114">rampActive</span><span class="sxs-lookup"><span data-stu-id="5fa02-114">rampActive</span></span>    | <span data-ttu-id="5fa02-115">Int64</span><span class="sxs-lookup"><span data-stu-id="5fa02-115">Int64</span></span>    | <span data-ttu-id="5fa02-116">时间 （以毫秒计） 计的 ducked 源以"淡出"。</span><span class="sxs-lookup"><span data-stu-id="5fa02-116">The amount of time (in milliseconds) it takes for ducked sources to "fade out".</span></span> |
| <span data-ttu-id="5fa02-117">rampInactive</span><span class="sxs-lookup"><span data-stu-id="5fa02-117">rampInactive</span></span>  | <span data-ttu-id="5fa02-118">Int64</span><span class="sxs-lookup"><span data-stu-id="5fa02-118">Int64</span></span>    | <span data-ttu-id="5fa02-119">时间 （以毫秒计） 计的 ducked 源"淡出"。</span><span class="sxs-lookup"><span data-stu-id="5fa02-119">The amount of time (in milliseconds) it takes for ducked sources to "fade in".</span></span>  |
| <span data-ttu-id="5fa02-120">upperLevel</span><span class="sxs-lookup"><span data-stu-id="5fa02-120">upperLevel</span></span>    | <span data-ttu-id="5fa02-121">Int64</span><span class="sxs-lookup"><span data-stu-id="5fa02-121">Int64</span></span>    | <span data-ttu-id="5fa02-122">源中时源不正在 ducked %的卷。</span><span class="sxs-lookup"><span data-stu-id="5fa02-122">The volume of sources in percent when the sources are not being ducked.</span></span>         |

> <span data-ttu-id="5fa02-123">**注意：** 提升持续时间不能超过 5000 毫秒。</span><span class="sxs-lookup"><span data-stu-id="5fa02-123">**Note:** Ramp duration cannot be more than 5,000 milliseconds.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5fa02-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5fa02-124">JSON representation</span></span>

<span data-ttu-id="5fa02-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5fa02-125">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "audioDuckingConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
