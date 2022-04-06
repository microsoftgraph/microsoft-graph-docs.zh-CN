---
author: JeremyKelley
description: FolderView 资源提供或设置关于文件夹的用户体验建议。
ms.date: 09/10/2017
title: FolderView
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: f5097377c8180e0bc9e226cb2a2dd071bcb53eec
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723368"
---
# <a name="folderview-resource-type"></a>FolderView 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**FolderView** 资源提供或设置关于文件夹的用户体验建议。

可从 [driveItem][item-resource] 资源的 [folder][folder-facet] 属性获得它。

## <a name="json-representation"></a>JSON 表示形式

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "viewType": "default | icons | details | thumbnails",
  "sortOrder": "string"
}
```

## <a name="properties"></a>属性

| 属性      | 类型   | 说明                                                                                                      |
| :------------ | :----- | :--------------------------------------------------------------------------------------------------------------- |
| **sortBy**    | string | 文件夹应采用的排序方法。                                                                 |
| **sortOrder** | string | 如果为 true，表明应按降序排列项。 否则，应按升序排列项。 |
| **viewType**  | string | 应用于表示文件夹的视图类型。                                                    |

可以使用 _sortBy_ 属性控制遵循 **viewType** Facet 的应用中项的排序顺序。

### <a name="sortby-values"></a>sortBy 值

以下值是针对 **sortBy** 属性进行定义。

| 值                    | 说明                                                                                                                                           |
| ------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
| `default`                | 应用的默认排序顺序。                                                                                                            |
| `name`                   | 应按项的 **name** 属性排列项。                                                                                       |
| `type`                   | 应按项类型排列项。                                                                                                         |
| `size`                   | 应按项的 **size** 属性排列项。                                                                                       |
| `takenOrCreatedDateTime` | 应按 **Photo** Facet 的 **takenDateTime** 属性排列项。 如果此属性不可用，应按 **createdDateTime** 属性排列项。 |
| `lastModifiedDateTime`   | 应按项的 **lastModifiedDateTime** 属性排列项。                                                                       |
| `sequence`               | 这些项按照用户指定的自定义序列排列。                                                                                                 |

### <a name="sortorder-values"></a>sortOrder 值

以下值是针对 **sortOrder** 属性进行定义。

| 值        | 说明                                   |
| ------------ | --------------------------------------------- |
| `ascending`  | 应按升序排列项。  |
| `descending` | 应按降序排列项。 |

### <a name="viewtype-values"></a>viewType 值

以下值是针对 **viewType** 属性进行定义。

| 值        | 说明                                                                   |
| ------------ | ----------------------------------------------------------------------------- |
| `default`    | 应用的默认视图类型。                                    |
| `icons`      | 使用图标表示 driveItem 的视图。                               |
| `details`    | 使用多个列提供每一项的其他详细信息的视图。 |
| `thumbnails` | 使用 driveItem 的大缩略图表示项的视图。      |

[item-resource]: driveitem.md
[folder-facet]: folder.md

<!-- uuid: f9e446fd-190b-4692-a605-bb60e78f1f19
2017-05-03 02:34:40 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "folderView resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
