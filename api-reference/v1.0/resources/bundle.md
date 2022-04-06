---
author: JeremyKelley
title: 捆绑资源类型
description: 描述作为其他 driveItems 的逻辑分组的 driveItem 的 Facet
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 9edf98faebc01fe23de16201fe5810eaa6db34fb
ms.sourcegitcommit: f5382652b6880fab42040df40a08de7cb2d74d35
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/17/2022
ms.locfileid: "63561585"
---
# <a name="bundle-resource-type"></a>捆绑资源类型

命名空间：microsoft.graph

捆绑包是文件的逻辑分组，用于一次共享多个文件。 它由包含 Facet 的 [driveItem][] `bundle` 实体表示，并且可以与任何其他 driveItem 相同的方式共享。

[driveItem][] `bundle` 上的 Facet 将项标识为捆绑包，将特定于捆绑包的信息分组到单个结构中。 它仅包含在从捆绑包终结点返回的 [driveItem][] **资源** 中。

请注意，资源 `bundle` 类型本身不是其自身的实体，只是 [driveItem 上的一个 Facet][]。 驱动器 `bundles` 上 [的集合的类型为][] [driveItem][]，而不是 `bundle`。

## <a name="methods"></a>方法

|                        方法             |         返回类型      | 说明        |
| :---------------------------------------- | :----------------------- | :------------------|
| [列出捆绑包][bundle-list]               | [driveItem][] 集合 | 列出驱动器中所有捆绑包 |
| [获取捆绑包][bundle-get]                  | [driveItem][]            | 获取捆绑包元数据 |
| [创建捆绑包][bundle-create]            | [driveItem][]            | 创建新的捆绑包 |
| [添加项][bundle-add-item]               | 无                     | 将 [driveItem][] 添加到现有捆绑包 |
| [删除项目][bundle-remove-item]         | 无                     | 从现有[捆绑包中删除 driveItem][] |
| [更新捆绑包][bundle-update]            | [driveItem][]            | 更新捆绑包元数据 |
| [删除捆绑包][bundle-delete]            | 无                     | 删除捆绑包 |


## <a name="properties"></a>属性

| 属性名称 | 类型      | 说明
|:--------------|:----------|:------------------------------------------------
| childCount    | Int32     | 此容器包含的直接子项数量。
| album         | [album][] | 如果捆绑包是 [专辑][]，则包含 `album` 属性

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


