---
author: MarcMroz
description: 媒体资源包含有关驱动器项 (或视频) 元数据。
title: 媒体资源类型
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 488201407363469ff09220c1dcce3c15f02e3b93
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236310"
---
# <a name="media-resouce-type"></a>media resouce 类型

包含有关驱动器项 (或视频) 元数据。

可用于 [driveItem][item-resource] 资源的媒体属性。


## <a name="properties"></a>属性

| 属性                 | 类型                  | 说明                                                                                                   |
| :----------------------- | :-------------------- | :------------------------------------------------------------------------------------------------------------ 
| **isTranscriptionShown** | 布尔值               | 如果文件具有脚本，则此设置控制在查看过程中是否向用户显示媒体文件的隐藏式字幕/转录。 读写。                                                    |
| **mediaSource**          | [mediaSource](mediaSource.md)         | 有关媒体源的信息。 只读。                                                             | 


## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.media"
}-->

```json
{
  "isTranscriptionShown" : true,
  "mediaSource": { "@odata.type": "microsoft.graph.mediaSource" }
}
```

## <a name="see-also"></a>另请参阅 

有关 driveItem 上 Facet 的信息，请参阅 [driveItem](driveitem.md)。

[item-resource]: ../resources/driveitem.md
[mediaSource]: mediaSource.md

<!-- {
  "type": "#page.annotation",
  "description": "The media resource type provides information about the media item.",
  "keywords": "mediaItem,client,media info,onedrive",
  "section": "documentation",
  "tocPath&quot;: &quot;Facets/Media"
} -->
