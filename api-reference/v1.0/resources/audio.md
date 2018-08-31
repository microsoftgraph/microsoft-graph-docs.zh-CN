---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 音频
ms.openlocfilehash: e68b70565f0eccd7847fba2b8085661071a75ae7
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2018
ms.locfileid: "23266231"
---
# <a name="audio-facet"></a>Audio Facet

**Audio** 资源将与音频相关的属性分组到一个单一结构。

如果 [**DriveItem**](driveitem.md) 具有一个非 null **音频** facet，则该项表示一个音频文件。通过从文件中提取元数据来填充**音频**资源的属性。 

## <a name="json-representation"></a>JSON 表示形式

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.audio" } -->
```json
{
  "album": "string",
  "albumArtist": "string",
  "artist": "string",
  "bitrate": 128,
  "composers": "string",
  "copyright": "string",
  "disc": 0,
  "discCount": 0,
  "duration": 567,
  "genre": "string",
  "hasDrm": false,
  "isVariableBitrate": false,
  "title": "string",
  "track": 1,
  "trackCount": 16,
  "year": 2014
}
```

## <a name="properties"></a>属性

| 属性名称         | 类型    | 说明                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| **专辑**             | 字符串  | 此音频文件的专辑标题。                          |
| **albumArtist**       | 字符串  | 此音频文件的专辑上的艺术家。                    |
| **艺术家**            | 字符串  | 此音频文件的表演艺术家。                            |
| **比特率**           | Int64   | 比特率（以 kbps 为单位）。                                           |
| **作曲家**         | 字符串  | 此音频文件的作曲者姓名。                          |
| **版权**         | 字符串  | 此音频文件的版权信息。                            |
| **光盘**              | Int16   | 此音频文件源自的光盘编号。                    |
| **discCount**         | Int16   | 此专辑中的光盘总数。                             |
| **持续时间**          | Int64   | 此音频文件的持续时间（以毫秒为单位）                |
| **流派**             | 字符串  | 此音频文件的流派。                                        |
| **hasDrm**            | 布尔值 | 指明此文件是否受数字版权管理的保护。   |
| **isVariableBitrate** | 布尔值 | 指明此文件是否已经过可变比特率编码。            |
| **标题**             | 字符串  | 此音频文件的标题。                                         |
| **音轨**             | Int32   | 此音频文件在原始光盘上的曲目编号。    |
| **trackCount**        | Int32   | 此音频文件的原始光盘上的曲目总数。 |
| **年份**              | Int32   | 此音频文件的录制年份。                                |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a>注解

有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。

<!-- {
  "type": "#page.annotation",
  "description": "The audio facet provides information about music or audio metadata.",
  "keywords": "music,audio,metadata,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Audio"
} -->
