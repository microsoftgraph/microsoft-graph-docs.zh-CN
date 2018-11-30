---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Video
ms.openlocfilehash: a9bf228d814526d089fb102444e6952558b07e1c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048273"
---
# <a name="video-resource-type"></a>Video 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

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

| 属性名称             | 类型   | 说明
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
<!-- {
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": ""
}-->
