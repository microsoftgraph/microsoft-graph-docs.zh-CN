---
author: MarcMroz
description: mediaSource 资源包含有关媒体源的元数据 (驱动器项) 元数据。
title: mediaSource 资源类型
localization_priority: Normal
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: 32e9fc10fe9795af0393e67b2ce2e2eef827ee7a12140c37e129180589bbe359
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54193410"
---
# <a name="mediasource-resouce-type"></a>mediaSource 资源类型

**mediaSource** 资源包含有关媒体源的元数据 (驱动器项) 元数据。

可用于 [driveItem][item-resource] 资源的媒体属性。

## <a name="properties"></a>属性

| 属性                 | 类型                       | 说明                                                                                      |
| :----------------------- | :------------------------  | :----------------------------------------------------------------------------------------------- |
| **contentCategory**      | mediaSourceContentCategory | 指示媒体内容类别的枚举值。                                     |

### <a name="mediasourcecontentcategory-values"></a>mediaSourceContentCategory 值

| 值               | 说明                                         |
|:------------------- |:----------------------------------------------------|
| meeting             | 媒体是会议。                             |
| liveStream          | 媒体是实时流。                         |
| presentation        | 媒体是演示文稿。                        |
| screenRecording     | 媒体是屏幕录制。                    |
| unknownFutureValue  | 用于将来兼容性的标记值。              |

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "contentCategory"
  ],
  "@odata.type": "microsoft.graph.mediaSource"
}-->

```json
{
  "contentCategory" : "string"
}
```

## <a name="see-also"></a>另请参阅

有关 driveItem 上 Facet 的信息，请参阅 [driveItem](driveitem.md)。

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The mediaSource facet provides information about drive item source.",
  "keywords": "mediaSource,client,media info,onedrive",
  "section": "documentation",
  "tocPath&quot;: &quot;Facets/MediaSource"
} -->
