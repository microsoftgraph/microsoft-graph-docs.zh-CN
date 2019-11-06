---
title: participantMixerLevel 资源类型
description: 给定音频参与者的混音器级别配置
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: cc305274d619a3686d4d391516947f1d06b92745
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006583"
---
# <a name="participantmixerlevel-resource-type"></a>participantMixerLevel 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

给定音频参与者的混音器级别配置

## <a name="properties"></a>属性

| 属性               | 类型                                                      | 说明                                                                                         |
| :--------------------- | :-------------------------------------------------------- | :---------------------------------------------------------------------------------------------------|
| ducking                | [audioDuckingConfiguration](audioduckingconfiguration.md) | 此 partipant 自定义组合的其他源的 ducking （逐步淘汰 in 和 out）配置。       |
| exclusiveMode          | boolean                                                   | 是否应从组合中删除没有显式源级别的源。                       |
| 参与者            | String                                                    | 为其配置了混合器的参与者。                                             |
| sourceLevels           | [audioSourceLevel](audiosourcelevel.md)集合        | 其他源的级别配置。                                                              |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

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

## <a name="example---mixer-level"></a>示例-混音器级别

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
