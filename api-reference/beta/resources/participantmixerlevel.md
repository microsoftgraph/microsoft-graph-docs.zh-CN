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
# <a name="participantmixerlevel-resource-type"></a>participantMixerLevel 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

级别，以便进行音频参与者给定的混音器配置

## <a name="properties"></a>属性

| 属性               | 类型                                                      | 说明                                                                                         |
| :--------------------- | :-------------------------------------------------------- | :---------------------------------------------------------------------------------------------------|
| 放掉                | [audioDuckingConfiguration](audioduckingconfiguration.md) | 放掉的此 partipant 其他源的 （逐步中和输出） 自定义组合的配置。       |
| exclusiveMode          | boolean                                                   | 是否应从组合中删除源而无需显式源级别。                       |
| 参与者            | 字符串                                                    | 正在为其配置混音器参与者。                                             |
| sourceLevels           | [audioSourceLevel](audiosourcelevel.md)集合        | 对于其他源的级别配置。                                                              |

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
<!-- {
  "type": "#page.annotation",
  "description": "participantMixerLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
