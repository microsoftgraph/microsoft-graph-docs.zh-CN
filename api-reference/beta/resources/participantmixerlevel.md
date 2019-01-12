---
title: participantMixerLevel 资源类型
description: 级别，以便进行音频参与者给定的混音器配置
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9bf0788b1f7822311882cfa2133083d81deff16b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977784"
---
# <a name="participantmixerlevel-resource-type"></a><span data-ttu-id="c00f6-103">participantMixerLevel 资源类型</span><span class="sxs-lookup"><span data-stu-id="c00f6-103">participantMixerLevel resource type</span></span>

> <span data-ttu-id="c00f6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c00f6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c00f6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c00f6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c00f6-106">级别，以便进行音频参与者给定的混音器配置</span><span class="sxs-lookup"><span data-stu-id="c00f6-106">Configuration of mixer levels for given audio participant</span></span>

## <a name="properties"></a><span data-ttu-id="c00f6-107">属性</span><span class="sxs-lookup"><span data-stu-id="c00f6-107">Properties</span></span>

| <span data-ttu-id="c00f6-108">属性</span><span class="sxs-lookup"><span data-stu-id="c00f6-108">Property</span></span>               | <span data-ttu-id="c00f6-109">类型</span><span class="sxs-lookup"><span data-stu-id="c00f6-109">Type</span></span>                                                      | <span data-ttu-id="c00f6-110">Description</span><span class="sxs-lookup"><span data-stu-id="c00f6-110">Description</span></span>                                                                                         |
| :--------------------- | :-------------------------------------------------------- | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c00f6-111">放掉</span><span class="sxs-lookup"><span data-stu-id="c00f6-111">ducking</span></span>                | [<span data-ttu-id="c00f6-112">audioDuckingConfiguration</span><span class="sxs-lookup"><span data-stu-id="c00f6-112">audioDuckingConfiguration</span></span>](audioduckingconfiguration.md) | <span data-ttu-id="c00f6-113">放掉的此 partipant 其他源的 （逐步中和输出） 自定义组合的配置。</span><span class="sxs-lookup"><span data-stu-id="c00f6-113">Configuration of ducking (phasing in and out) of other sources for this partipant custom mix.</span></span>       |
| <span data-ttu-id="c00f6-114">exclusiveMode</span><span class="sxs-lookup"><span data-stu-id="c00f6-114">exclusiveMode</span></span>          | <span data-ttu-id="c00f6-115">boolean</span><span class="sxs-lookup"><span data-stu-id="c00f6-115">boolean</span></span>                                                   | <span data-ttu-id="c00f6-116">是否应从组合中删除源而无需显式源级别。</span><span class="sxs-lookup"><span data-stu-id="c00f6-116">Whether sources without explicit source level should be removed from the mix.</span></span>                       |
| <span data-ttu-id="c00f6-117">参与者</span><span class="sxs-lookup"><span data-stu-id="c00f6-117">participant</span></span>            | <span data-ttu-id="c00f6-118">字符串</span><span class="sxs-lookup"><span data-stu-id="c00f6-118">String</span></span>                                                    | <span data-ttu-id="c00f6-119">正在为其配置混音器参与者。</span><span class="sxs-lookup"><span data-stu-id="c00f6-119">The participant for whom the mixer is being configured.</span></span>                                             |
| <span data-ttu-id="c00f6-120">sourceLevels</span><span class="sxs-lookup"><span data-stu-id="c00f6-120">sourceLevels</span></span>           | <span data-ttu-id="c00f6-121">[audioSourceLevel](audiosourcelevel.md)集合</span><span class="sxs-lookup"><span data-stu-id="c00f6-121">[audioSourceLevel](audiosourcelevel.md) collection</span></span>        | <span data-ttu-id="c00f6-122">对于其他源的级别配置。</span><span class="sxs-lookup"><span data-stu-id="c00f6-122">Level configuration for other sources.</span></span>                                                              |

## <a name="json-representation"></a><span data-ttu-id="c00f6-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c00f6-123">JSON representation</span></span>

<span data-ttu-id="c00f6-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c00f6-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.participantMixerLevel"
}-->
```json
{
  "ducking": { "@odata.type": "#microsoft.graph.audioDuckingConfiguration" },
  "exclusiveMode": true,
  "participant": "String",
  "sourceLevels": [ { "@odata.type": "#microsoft.graph.audioSourceLevel" } ]
}
```

## <a name="example---mixer-level"></a><span data-ttu-id="c00f6-125">示例-混音器级别</span><span class="sxs-lookup"><span data-stu-id="c00f6-125">Example - Mixer level</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.participantMixerLevel"
}-->
```json
{
  "ducking": {
    "@odata.type": "#microsoft.graph.audioDuckingParameters",
    "rampActive": 1000,
    "rampInactive": 1000,
    "lowerLevel": 20,
    "upperLevel": 100
  },
  "exclusiveMode": true,
  "participant": "123456W77E24E4D85F80597083CB830",
  "sourceLevels": [
    {
      "@odata.type": "#microsoft.graph.audioSourceLevel",
      "duckOthers": false,
      "level": 100,
      "participant": "8A34A46B3D174ADC8DCEDC4E7D572698"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "participantMixerLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
