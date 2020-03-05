---
title: participantMixerLevel 资源类型
description: 给定音频参与者的混音器级别配置
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 31e4ec08014907480cfe7bafaa21b061ec1434b6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522023"
---
# <a name="participantmixerlevel-resource-type"></a><span data-ttu-id="8d34c-103">participantMixerLevel 资源类型</span><span class="sxs-lookup"><span data-stu-id="8d34c-103">participantMixerLevel resource type</span></span>

<span data-ttu-id="8d34c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="8d34c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d34c-105">给定音频参与者的混音器级别配置</span><span class="sxs-lookup"><span data-stu-id="8d34c-105">Configuration of mixer levels for given audio participant</span></span>

## <a name="properties"></a><span data-ttu-id="8d34c-106">属性</span><span class="sxs-lookup"><span data-stu-id="8d34c-106">Properties</span></span>

| <span data-ttu-id="8d34c-107">属性</span><span class="sxs-lookup"><span data-stu-id="8d34c-107">Property</span></span>               | <span data-ttu-id="8d34c-108">类型</span><span class="sxs-lookup"><span data-stu-id="8d34c-108">Type</span></span>                                                      | <span data-ttu-id="8d34c-109">说明</span><span class="sxs-lookup"><span data-stu-id="8d34c-109">Description</span></span>                                                                                         |
| :--------------------- | :-------------------------------------------------------- | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="8d34c-110">ducking</span><span class="sxs-lookup"><span data-stu-id="8d34c-110">ducking</span></span>                | [<span data-ttu-id="8d34c-111">audioDuckingConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d34c-111">audioDuckingConfiguration</span></span>](audioduckingconfiguration.md) | <span data-ttu-id="8d34c-112">此 partipant 自定义组合的其他源的 ducking （逐步淘汰 in 和 out）配置。</span><span class="sxs-lookup"><span data-stu-id="8d34c-112">Configuration of ducking (phasing in and out) of other sources for this partipant custom mix.</span></span>       |
| <span data-ttu-id="8d34c-113">exclusiveMode</span><span class="sxs-lookup"><span data-stu-id="8d34c-113">exclusiveMode</span></span>          | <span data-ttu-id="8d34c-114">boolean</span><span class="sxs-lookup"><span data-stu-id="8d34c-114">boolean</span></span>                                                   | <span data-ttu-id="8d34c-115">是否应从组合中删除没有显式源级别的源。</span><span class="sxs-lookup"><span data-stu-id="8d34c-115">Whether sources without explicit source level should be removed from the mix.</span></span>                       |
| <span data-ttu-id="8d34c-116">参与者</span><span class="sxs-lookup"><span data-stu-id="8d34c-116">participant</span></span>            | <span data-ttu-id="8d34c-117">String</span><span class="sxs-lookup"><span data-stu-id="8d34c-117">String</span></span>                                                    | <span data-ttu-id="8d34c-118">为其配置了混合器的参与者。</span><span class="sxs-lookup"><span data-stu-id="8d34c-118">The participant for whom the mixer is being configured.</span></span>                                             |
| <span data-ttu-id="8d34c-119">sourceLevels</span><span class="sxs-lookup"><span data-stu-id="8d34c-119">sourceLevels</span></span>           | <span data-ttu-id="8d34c-120">[audioSourceLevel](audiosourcelevel.md)集合</span><span class="sxs-lookup"><span data-stu-id="8d34c-120">[audioSourceLevel](audiosourcelevel.md) collection</span></span>        | <span data-ttu-id="8d34c-121">其他源的级别配置。</span><span class="sxs-lookup"><span data-stu-id="8d34c-121">Level configuration for other sources.</span></span>                                                              |

## <a name="json-representation"></a><span data-ttu-id="8d34c-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8d34c-122">JSON representation</span></span>

<span data-ttu-id="8d34c-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8d34c-123">The following is a JSON representation of the resource.</span></span>

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

## <a name="example---mixer-level"></a><span data-ttu-id="8d34c-124">示例-混音器级别</span><span class="sxs-lookup"><span data-stu-id="8d34c-124">Example - Mixer level</span></span>

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
