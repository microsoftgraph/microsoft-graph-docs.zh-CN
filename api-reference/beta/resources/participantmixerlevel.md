---
title: participantMixerLevel 资源类型
description: 级别，以便进行音频参与者给定的混音器配置
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 14804e02766e375568fac03cb97d2eaf76142353
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513765"
---
# <a name="participantmixerlevel-resource-type"></a><span data-ttu-id="7f094-103">participantMixerLevel 资源类型</span><span class="sxs-lookup"><span data-stu-id="7f094-103">participantMixerLevel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f094-104">级别，以便进行音频参与者给定的混音器配置</span><span class="sxs-lookup"><span data-stu-id="7f094-104">Configuration of mixer levels for given audio participant</span></span>

## <a name="properties"></a><span data-ttu-id="7f094-105">属性</span><span class="sxs-lookup"><span data-stu-id="7f094-105">Properties</span></span>

| <span data-ttu-id="7f094-106">属性</span><span class="sxs-lookup"><span data-stu-id="7f094-106">Property</span></span>               | <span data-ttu-id="7f094-107">类型</span><span class="sxs-lookup"><span data-stu-id="7f094-107">Type</span></span>                                                      | <span data-ttu-id="7f094-108">说明</span><span class="sxs-lookup"><span data-stu-id="7f094-108">Description</span></span>                                                                                         |
| :--------------------- | :-------------------------------------------------------- | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="7f094-109">放掉</span><span class="sxs-lookup"><span data-stu-id="7f094-109">ducking</span></span>                | [<span data-ttu-id="7f094-110">audioDuckingConfiguration</span><span class="sxs-lookup"><span data-stu-id="7f094-110">audioDuckingConfiguration</span></span>](audioduckingconfiguration.md) | <span data-ttu-id="7f094-111">放掉的此 partipant 其他源的 （逐步中和输出） 自定义组合的配置。</span><span class="sxs-lookup"><span data-stu-id="7f094-111">Configuration of ducking (phasing in and out) of other sources for this partipant custom mix.</span></span>       |
| <span data-ttu-id="7f094-112">exclusiveMode</span><span class="sxs-lookup"><span data-stu-id="7f094-112">exclusiveMode</span></span>          | <span data-ttu-id="7f094-113">布尔</span><span class="sxs-lookup"><span data-stu-id="7f094-113">boolean</span></span>                                                   | <span data-ttu-id="7f094-114">是否应从组合中删除源而无需显式源级别。</span><span class="sxs-lookup"><span data-stu-id="7f094-114">Whether sources without explicit source level should be removed from the mix.</span></span>                       |
| <span data-ttu-id="7f094-115">参与者</span><span class="sxs-lookup"><span data-stu-id="7f094-115">participant</span></span>            | <span data-ttu-id="7f094-116">String</span><span class="sxs-lookup"><span data-stu-id="7f094-116">String</span></span>                                                    | <span data-ttu-id="7f094-117">正在为其配置混音器参与者。</span><span class="sxs-lookup"><span data-stu-id="7f094-117">The participant for whom the mixer is being configured.</span></span>                                             |
| <span data-ttu-id="7f094-118">sourceLevels</span><span class="sxs-lookup"><span data-stu-id="7f094-118">sourceLevels</span></span>           | <span data-ttu-id="7f094-119">[audioSourceLevel](audiosourcelevel.md)集合</span><span class="sxs-lookup"><span data-stu-id="7f094-119">[audioSourceLevel](audiosourcelevel.md) collection</span></span>        | <span data-ttu-id="7f094-120">对于其他源的级别配置。</span><span class="sxs-lookup"><span data-stu-id="7f094-120">Level configuration for other sources.</span></span>                                                              |

## <a name="json-representation"></a><span data-ttu-id="7f094-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7f094-121">JSON representation</span></span>

<span data-ttu-id="7f094-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7f094-122">The following is a JSON representation of the resource.</span></span>

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

## <a name="example---mixer-level"></a><span data-ttu-id="7f094-123">示例-混音器级别</span><span class="sxs-lookup"><span data-stu-id="7f094-123">Example - Mixer level</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/participantmixerlevel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
