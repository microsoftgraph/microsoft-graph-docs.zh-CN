---
author: JeremyKelley
title: 视频资源类型
ms.localizationpriority: medium
description: 视频资源将与视频相关的数据项分组到单个结构中。
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 81a2ccd6250261c87b5af84cc0bef0ace4342702
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65897823"
---
# <a name="video-resource-type"></a>视频资源类型

命名空间：microsoft.graph

**视频** 资源将与视频相关的数据项分组到单个结构中。

如果 [**driveItem**](driveitem.md) 具有非 null **视频** 方面，则该项表示视频文件。
通过从文件中提取元数据来填充 **视频** 资源的属性。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.video"
}-->

```json
{
  "audioBitsPerSample": 16,
  "audioChannels": 1,
  "audioFormat": "AAC",
  "audioSamplesPerSecond": 44100,
  "bitrate": 39101896,
  "duration": 8053,
  "fourCC": "H264",
  "frameRate": 239.877,
  "height": 1280,
  "width": 720
}
```

## <a name="properties"></a>属性

| 属性名称             | 类型   | 说明
|:--------------------------|:-------|:----------------------------------------
| **audioBitsPerSample**    | Int32  | 每个样本的音频位数。
| **audioChannels**         | Int32  | 音频频道数。
| **audioFormat**           | string | 音频格式名称（AAC、MP3 等）。
| **audioSamplesPerSecond** | Int32  | 每秒音频采样数。
| **bitrate**               | Int32  | 视频比特率（以位/秒为单位）。
| **duration**              | Int64  | 文件时长（以毫秒为单位）。
| **fourCC**                | string | 视频格式的“四个字符代码”名称。
| **frameRate**             | double | 视频的帧速率。
| **height**                | Int32  | 视频高度（以像素为单位）。
| **width**                 | Int32  | 视频的宽度，以像素为单位。

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a>注解

有关 driveItem 上的分面的详细信息，请参阅 [driveItem](driveitem.md)。

<!-- {
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": "Facets/Video"
} -->

