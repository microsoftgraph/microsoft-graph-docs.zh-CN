---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 视频
localization_priority: Normal
ms.openlocfilehash: 1e780c8392316be1f7fcc59f3818085dc462da29
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454021"
---
# <a name="video-resource-type"></a>Video 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**视频**资源将与视频相关的数据项分组到一个单一结构。

如果 [**DriveItem**](driveitem.md) 具有一个非 null **视频**方面，则该项表示一个视频文件。通过从文件中提取元数据对**视频**资源的属性进行填充。

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

| 属性名称             | 类型   | 描述
|:--------------------------|:-------|:----------------------------------------
| **audioBitsPerSample**    | Int32  | 每个样本的音频位数。
| **audioChannels**         | Int32  | 音频频道数。
| **audioFormat**           | string | 音频格式名称（AAC、MP3 等）。
| **audioSamplesPerSecond** | Int32  | 每秒音频采样数。
| **bitrate**               | Int32  | 视频比特率（以位/秒为单位）。
| **duration**              | Int64  | 文件时长（以毫秒为单位）。
| **fourCC**                | string | 视频格式的“四个字符代码”名称。
| **framerate**             | double | 视频的帧速率。
| **height**                | Int32  | 视频高度（以像素为单位）。
| **width**                 | Int32  | 视频的宽度，以像素为单位。

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a>注解

有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。





<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/video.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
