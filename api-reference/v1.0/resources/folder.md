---
author: JeremyKelley
ms.date: 09/10/2017
title: Folder
ms.localizationpriority: medium
description: '文件夹资源将与文件夹相关的数据项分组到一个单一结构。 '
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: f744620c34b2ddbe084d3c7d07b7783cce4fecd8
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900060"
---
# <a name="folder-resource-type"></a>文件夹资源类型

命名空间：microsoft.graph

**文件夹** 资源将与文件夹相关的数据项分组到一个单一结构。具有非 null **文件夹** 方面的 **[DriveItems](driveitem.md)** 是其他 DriveItems 的容器。

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

[folderView]: folderview.md
[DriveItem]: driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The Folder facet describes properties of a folder",
  "keywords": "folder,item,facet",
  "section": "documentation",
  "tocPath&quot;: &quot;Facets/Folder"
} -->

