---
author: ananmishr
ms.date: 09/10/2017
title: 音频
ms.localizationpriority: medium
ms.prod: microsoft-teams
description: Audio 资源将与音频相关的属性分组到一个单一结构。
doc_type: resourcePageType
ms.openlocfilehash: 54423143955f8e9626ec7097a3ea4c0c7e5867c8
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61789969"
---
# <a name="audio-facet"></a>Audio Facet

命名空间：microsoft.graph

**Audio** 资源将与音频相关的属性分组到一个单一结构。

如果 [**DriveItem**](driveitem.md) 具有一个非 null **音频** facet，则该项表示一个音频文件。通过从文件中提取元数据来填充 **音频** 资源的属性。 

**音频** 资源仅在个人OneDrive受支持。

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
| **album**             | string  | 此音频文件的专辑标题。                          |
| **albumArtist**       | string  | 此音频文件的专辑上的艺术家。                    |
| **artist**            | string  | 此音频文件的表演艺术家。                            |
| **bitrate**           | Int64   | 比特率（以 kbps 为单位）。                                           |
| **composers**         | string  | 此音频文件的作曲者姓名。                          |
| **copyright**         | string  | 此音频文件的版权信息。                            |
| **disc**              | Int16   | 此音频文件源自的光盘编号。                    |
| **discCount**         | Int16   | 此专辑中的光盘总数。                             |
| **duration**          | Int64   | 此音频文件的持续时间（以毫秒为单位）                |
| **genre**             | string  | 此音频文件的流派。                                        |
| **hasDrm**            | boolean | 指明此文件是否受数字版权管理的保护。   |
| **isVariableBitrate** | boolean | 指明此文件是否已经过可变比特率编码。            |
| **title**             | string  | 此音频文件的标题。                                         |
| **track**             | Int32   | 此音频文件在原始光盘上的曲目编号。    |
| **trackCount**        | Int32   | 此音频文件的原始光盘上的曲目总数。 |
| **year**              | Int32   | 此音频文件的录制年份。                                |

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

