---
author: MarcMroz
description: driveItemSource 包含有关创建驱动器项的源应用程序的元数据。
title: driveItemSource 资源类型
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: eada8fa22672a80d712ef78be5cc3d44ac354216
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59047455"
---
# <a name="driveitemsource-resource-type"></a>driveItemSource 资源类型

包含有关驱动器项源的元数据。

可用于 [driveItem][item-resource] 资源的 source 属性。

## <a name="properties"></a>属性

| 属性                 | 类型                       | 说明                                                                                      |
| :----------------------- | :------------------------  | :----------------------------------------------------------------------------------------------- |
| **application**          | driveItemSourceApplication | 指示创建文件的源应用程序的枚举值。              |
| **externalId**           | 字符串                     | 源中的驱动器项的外部标识符。                                      |

### <a name="driveitemsourceapplication-values"></a>driveItemSourceApplication 值

| 值               | 说明                                       |
|:--------------------|:--------------------------------------------------|
| teams               | 应用程序已Teams。                         |
| yammer              | 应用程序已Yammer。                        |
| sharePoint          | 应用程序已SharePoint。                    |
| oneDrive            | 应用程序已OneDrive。                      |
| stream              | 应用程序为 Stream。                        |
| powerPoint          | 应用程序已PowerPoint                     |
| 办公室              | 应用程序已Office                         |
| unknownFutureValue  | 用于将来兼容性的标记值。            |

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "application",
    "externalId",
  ],
  "@odata.type": "microsoft.graph.driveItemSource"
}-->

```json
{
  "application": "string",
  "externalId" : "string"
}
```

## <a name="see-also"></a>另请参阅

有关 driveItem 上 Facet 的信息，请参阅 [driveItem](driveitem.md)。

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The driveItemSource facet provides information about drive item source.",
  "keywords": "driveItemSoruce,client,media info,onedrive",
  "section": "documentation",
  "tocPath&quot;: &quot;Facets/driveItemSource"
} -->
