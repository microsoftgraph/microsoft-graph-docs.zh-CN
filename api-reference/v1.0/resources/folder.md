---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Folder
ms.openlocfilehash: c0ab787f1c1f04ff77eeb69979dc6a825d4f3c33
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2018
ms.locfileid: "23266560"
---
# <a name="folder-resource-type"></a>Folder 资源类型

**文件夹**资源将与文件夹相关的数据项分组到一个单一结构。具有非 null **文件夹**方面的 [**DriveItems**](driveitem.md) 是其他 DriveItems 的容器。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.folder"
}-->

```json
{
  "childCount": 1024,
  "view": { "@odata.type": "microsoft.graph.folderView" }
}
```

## <a name="properties"></a>属性

| 属性       | 类型           | 说明
|:---------------|:---------------|:-------------------------------------------
| **childCount** | Int32          | 此容器包含的直接子项数量。
| **view**       | [folderView][] | 用于定义文件夹的推荐视图的属性集合。

## <a name="remarks"></a>注解 

有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem][]。

[folderView]: folderView.md
[DriveItem]: driveItem.md

<!-- {
  "type": "#page.annotation",
  "description": "The Folder facet describes properties of a folder",
  "keywords": "folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Folder"
} -->
