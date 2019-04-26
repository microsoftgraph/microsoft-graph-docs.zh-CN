---
title: participantMixerLevel 资源类型
description: 给定音频参与者的混音器级别配置
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 00beb746a29ae06de838f00b699a97e01f2f1941
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344926"
---
# <a name="participantmixerlevel-resource-type"></a><span data-ttu-id="6993a-103">participantMixerLevel 资源类型</span><span class="sxs-lookup"><span data-stu-id="6993a-103">participantMixerLevel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6993a-104">给定音频参与者的混音器级别配置</span><span class="sxs-lookup"><span data-stu-id="6993a-104">Configuration of mixer levels for given audio participant</span></span>

## <a name="properties"></a><span data-ttu-id="6993a-105">属性</span><span class="sxs-lookup"><span data-stu-id="6993a-105">Properties</span></span>

| <span data-ttu-id="6993a-106">属性</span><span class="sxs-lookup"><span data-stu-id="6993a-106">Property</span></span>               | <span data-ttu-id="6993a-107">类型</span><span class="sxs-lookup"><span data-stu-id="6993a-107">Type</span></span>                                                      | <span data-ttu-id="6993a-108">说明</span><span class="sxs-lookup"><span data-stu-id="6993a-108">Description</span></span>                                                                                         |
| :--------------------- | :-------------------------------------------------------- | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="6993a-109">ducking</span><span class="sxs-lookup"><span data-stu-id="6993a-109">ducking</span></span>                | [<span data-ttu-id="6993a-110">audioDuckingConfiguration</span><span class="sxs-lookup"><span data-stu-id="6993a-110">audioDuckingConfiguration</span></span>](audioduckingconfiguration.md) | <span data-ttu-id="6993a-111">此 partipant 自定义组合的其他源的 ducking (逐步淘汰 in 和 out) 配置。</span><span class="sxs-lookup"><span data-stu-id="6993a-111">Configuration of ducking (phasing in and out) of other sources for this partipant custom mix.</span></span>       |
| <span data-ttu-id="6993a-112">exclusiveMode</span><span class="sxs-lookup"><span data-stu-id="6993a-112">exclusiveMode</span></span>          | <span data-ttu-id="6993a-113">boolean</span><span class="sxs-lookup"><span data-stu-id="6993a-113">boolean</span></span>                                                   | <span data-ttu-id="6993a-114">是否应从组合中删除没有显式源级别的源。</span><span class="sxs-lookup"><span data-stu-id="6993a-114">Whether sources without explicit source level should be removed from the mix.</span></span>                       |
| <span data-ttu-id="6993a-115">参与者</span><span class="sxs-lookup"><span data-stu-id="6993a-115">participant</span></span>            | <span data-ttu-id="6993a-116">String</span><span class="sxs-lookup"><span data-stu-id="6993a-116">String</span></span>                                                    | <span data-ttu-id="6993a-117">为其配置了混合器的参与者。</span><span class="sxs-lookup"><span data-stu-id="6993a-117">The participant for whom the mixer is being configured.</span></span>                                             |
| <span data-ttu-id="6993a-118">sourceLevels</span><span class="sxs-lookup"><span data-stu-id="6993a-118">sourceLevels</span></span>           | <span data-ttu-id="6993a-119">[audioSourceLevel](audiosourcelevel.md)集合</span><span class="sxs-lookup"><span data-stu-id="6993a-119">[audioSourceLevel](audiosourcelevel.md) collection</span></span>        | <span data-ttu-id="6993a-120">其他源的级别配置。</span><span class="sxs-lookup"><span data-stu-id="6993a-120">Level configuration for other sources.</span></span>                                                              |

## <a name="json-representation"></a><span data-ttu-id="6993a-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6993a-121">JSON representation</span></span>

<span data-ttu-id="6993a-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6993a-122">The following is a JSON representation of the resource.</span></span>

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

## <a name="example---mixer-level"></a><span data-ttu-id="6993a-123">示例-混音器级别</span><span class="sxs-lookup"><span data-stu-id="6993a-123">Example - Mixer level</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "participantMixerLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
