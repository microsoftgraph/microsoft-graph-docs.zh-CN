---
title: participantMixerLevel 资源类型
description: 级别，以便进行音频参与者给定的混音器配置
author: VinodRavichandran
ms.openlocfilehash: 9d5a5d740fbdf250f90b28539221e8231c0bf38c
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380140"
---
# <a name="participantmixerlevel-resource-type"></a><span data-ttu-id="b6603-103">participantMixerLevel 资源类型</span><span class="sxs-lookup"><span data-stu-id="b6603-103">participantMixerLevel resource type</span></span>

> <span data-ttu-id="b6603-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b6603-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b6603-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b6603-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b6603-106">级别，以便进行音频参与者给定的混音器配置</span><span class="sxs-lookup"><span data-stu-id="b6603-106">Configuration of mixer levels for given audio participant</span></span>

## <a name="properties"></a><span data-ttu-id="b6603-107">属性</span><span class="sxs-lookup"><span data-stu-id="b6603-107">Properties</span></span>

| <span data-ttu-id="b6603-108">属性</span><span class="sxs-lookup"><span data-stu-id="b6603-108">Property</span></span>               | <span data-ttu-id="b6603-109">类型</span><span class="sxs-lookup"><span data-stu-id="b6603-109">Type</span></span>                                                      | <span data-ttu-id="b6603-110">说明</span><span class="sxs-lookup"><span data-stu-id="b6603-110">Description</span></span>                                                                                         |
| :--------------------- | :-------------------------------------------------------- | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b6603-111">放掉</span><span class="sxs-lookup"><span data-stu-id="b6603-111">ducking</span></span>                | [<span data-ttu-id="b6603-112">audioDuckingConfiguration</span><span class="sxs-lookup"><span data-stu-id="b6603-112">audioDuckingConfiguration</span></span>](audioduckingconfiguration.md) | <span data-ttu-id="b6603-113">放掉的此 partipant 其他源的 （逐步中和输出） 自定义组合的配置。</span><span class="sxs-lookup"><span data-stu-id="b6603-113">Configuration of ducking (phasing in and out) of other sources for this partipant custom mix.</span></span>       |
| <span data-ttu-id="b6603-114">exclusiveMode</span><span class="sxs-lookup"><span data-stu-id="b6603-114">exclusiveMode</span></span>          | <span data-ttu-id="b6603-115">boolean</span><span class="sxs-lookup"><span data-stu-id="b6603-115">boolean</span></span>                                                   | <span data-ttu-id="b6603-116">是否应从组合中删除源而无需显式源级别。</span><span class="sxs-lookup"><span data-stu-id="b6603-116">Whether sources without explicit source level should be removed from the mix.</span></span>                       |
| <span data-ttu-id="b6603-117">参与者</span><span class="sxs-lookup"><span data-stu-id="b6603-117">participant</span></span>            | <span data-ttu-id="b6603-118">字符串</span><span class="sxs-lookup"><span data-stu-id="b6603-118">String</span></span>                                                    | <span data-ttu-id="b6603-119">正在为其配置混音器参与者。</span><span class="sxs-lookup"><span data-stu-id="b6603-119">The participant for whom the mixer is being configured.</span></span>                                             |
| <span data-ttu-id="b6603-120">sourceLevels</span><span class="sxs-lookup"><span data-stu-id="b6603-120">sourceLevels</span></span>           | <span data-ttu-id="b6603-121">[audioSourceLevel](audiosourcelevel.md)集合</span><span class="sxs-lookup"><span data-stu-id="b6603-121">[audioSourceLevel](audiosourcelevel.md) collection</span></span>        | <span data-ttu-id="b6603-122">对于其他源的级别配置。</span><span class="sxs-lookup"><span data-stu-id="b6603-122">Level configuration for other sources.</span></span>                                                              |

## <a name="json-representation"></a><span data-ttu-id="b6603-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b6603-123">JSON representation</span></span>

<span data-ttu-id="b6603-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6603-124">The following is a JSON representation of the resource.</span></span>

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

## <a name="example---mixer-level"></a><span data-ttu-id="b6603-125">示例-混音器级别</span><span class="sxs-lookup"><span data-stu-id="b6603-125">Example - Mixer level</span></span>

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
