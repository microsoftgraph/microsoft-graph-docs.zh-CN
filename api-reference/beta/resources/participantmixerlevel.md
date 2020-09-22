---
title: participantMixerLevel 资源类型
description: 给定音频参与者的混音器级别配置
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: fdec09b80eddfc4a4ea3f87425c211ed49f22ded
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998234"
---
# <a name="participantmixerlevel-resource-type"></a><span data-ttu-id="909eb-103">participantMixerLevel 资源类型</span><span class="sxs-lookup"><span data-stu-id="909eb-103">participantMixerLevel resource type</span></span>

<span data-ttu-id="909eb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="909eb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="909eb-105">给定音频参与者的混音器级别配置</span><span class="sxs-lookup"><span data-stu-id="909eb-105">Configuration of mixer levels for given audio participant</span></span>

## <a name="properties"></a><span data-ttu-id="909eb-106">属性</span><span class="sxs-lookup"><span data-stu-id="909eb-106">Properties</span></span>

| <span data-ttu-id="909eb-107">属性</span><span class="sxs-lookup"><span data-stu-id="909eb-107">Property</span></span>               | <span data-ttu-id="909eb-108">类型</span><span class="sxs-lookup"><span data-stu-id="909eb-108">Type</span></span>                                                      | <span data-ttu-id="909eb-109">说明</span><span class="sxs-lookup"><span data-stu-id="909eb-109">Description</span></span>                                                                                         |
| :--------------------- | :-------------------------------------------------------- | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="909eb-110">ducking</span><span class="sxs-lookup"><span data-stu-id="909eb-110">ducking</span></span>                | [<span data-ttu-id="909eb-111">audioDuckingConfiguration</span><span class="sxs-lookup"><span data-stu-id="909eb-111">audioDuckingConfiguration</span></span>](audioduckingconfiguration.md) | <span data-ttu-id="909eb-112">此 partipant 自定义组合的其他源的 ducking (逐步淘汰) 配置。</span><span class="sxs-lookup"><span data-stu-id="909eb-112">Configuration of ducking (phasing in and out) of other sources for this partipant custom mix.</span></span>       |
| <span data-ttu-id="909eb-113">exclusiveMode</span><span class="sxs-lookup"><span data-stu-id="909eb-113">exclusiveMode</span></span>          | <span data-ttu-id="909eb-114">boolean</span><span class="sxs-lookup"><span data-stu-id="909eb-114">boolean</span></span>                                                   | <span data-ttu-id="909eb-115">是否应从组合中删除没有显式源级别的源。</span><span class="sxs-lookup"><span data-stu-id="909eb-115">Whether sources without explicit source level should be removed from the mix.</span></span>                       |
| <span data-ttu-id="909eb-116">参与者</span><span class="sxs-lookup"><span data-stu-id="909eb-116">participant</span></span>            | <span data-ttu-id="909eb-117">String</span><span class="sxs-lookup"><span data-stu-id="909eb-117">String</span></span>                                                    | <span data-ttu-id="909eb-118">为其配置了混合器的参与者。</span><span class="sxs-lookup"><span data-stu-id="909eb-118">The participant for whom the mixer is being configured.</span></span>                                             |
| <span data-ttu-id="909eb-119">sourceLevels</span><span class="sxs-lookup"><span data-stu-id="909eb-119">sourceLevels</span></span>           | <span data-ttu-id="909eb-120">[audioSourceLevel](audiosourcelevel.md) 集合</span><span class="sxs-lookup"><span data-stu-id="909eb-120">[audioSourceLevel](audiosourcelevel.md) collection</span></span>        | <span data-ttu-id="909eb-121">其他源的级别配置。</span><span class="sxs-lookup"><span data-stu-id="909eb-121">Level configuration for other sources.</span></span>                                                              |

## <a name="json-representation"></a><span data-ttu-id="909eb-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="909eb-122">JSON representation</span></span>

<span data-ttu-id="909eb-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="909eb-123">The following is a JSON representation of the resource.</span></span>

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

## <a name="example---mixer-level"></a><span data-ttu-id="909eb-124">示例-混音器级别</span><span class="sxs-lookup"><span data-stu-id="909eb-124">Example - Mixer level</span></span>

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


