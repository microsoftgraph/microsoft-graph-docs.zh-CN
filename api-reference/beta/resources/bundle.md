---
author: JeremyKelley
ms.author: jeremyke
title: 捆绑资源类型
description: 描述作为其他 Driveitem 的逻辑分组的 driveItem 的 Facet
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: ae03674970c8861c7d1c158e62662d9691e74789
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507864"
---
# <a name="bundle-resource-type"></a>捆绑资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

捆绑包是一次用于一次性共享多个文件的文件的逻辑分组。 它由包含`bundle` Facet 的[driveItem][]实体表示，并且可以像其他任何其他 driveItem 一样进行共享。

DriveItem `bundle`上的 facet [][]将项目标识为捆绑包，并将捆绑包中的信息分组到一个单一结构中。 它仅包含在从**捆绑包**终结点返回的[driveItem][]资源中。

请注意， `bundle`资源类型本身并不是自己的实体，并且只是[driveItem][]上的一个 facet。 驱动器`bundles`上的集合[][]的类型为[driveItem][]，而不`bundle`是。

## <a name="methods"></a>方法

|                        方法             |         返回类型      | 说明        |
| :---------------------------------------- | :----------------------- | :------------------|
| [列出捆绑包][bundle-list]               | [driveItem][] 集合 | 列出驱动器中的所有捆绑包 |
| [获取捆绑包][bundle-get]                  | [driveItem][]            | 获取捆绑包元数据 |
| [创建捆绑包][bundle-create]            | [driveItem][]            | 创建新的捆绑包 |
| [添加项目][bundle-add-item]               | 无                     | 将[driveItem][]添加到现有捆绑包 |
| [删除项][bundle-remove-item]         | 无                     | 从现有捆绑包中删除[driveItem][] |
| [更新捆绑包][bundle-update]            | [driveItem][]            | 更新捆绑包元数据 |
| [删除捆绑包][bundle-delete]            | 无                     | 删除捆绑包 |


## <a name="properties"></a>属性

| 属性名称 | 类型      | 说明
|:--------------|:----------|:------------------------------------------------
| childCount    | Int32     | 此容器包含的直接子项数量。
| album         | [album][] | 如果捆绑包是[唱片集][]，则会`album`将该属性包含

## <a name="json-representation"></a>JSON 表示形式

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.bundle" } -->
```json
{
  "childCount": 3,
  "album": { "@odata.type": "microsoft.graph.album" },
}
```

[album]: album.md
[drive]: drive.md
[driveItem]: driveItem.md

[bundle-list]: ../api/bundle-list.md
[bundle-get]: ../api/bundle-get.md
[bundle-create]: ../api/drive-post-bundles.md
[bundle-add-item]: ../api/bundle-addItem.md
[bundle-remove-item]: ../api/bundle-removeItem.md
[bundle-update]: ../api/bundle-update.md
[bundle-delete]: ../api/bundle-delete.md
