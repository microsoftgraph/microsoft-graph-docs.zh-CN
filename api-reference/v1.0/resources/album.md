---
author: JeremyKelley
title: 相册资源类型
description: 描述作为相册的捆绑包的 Facet。
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 342391184cfdb59fc2dfb3742635c640994d82d7
ms.sourcegitcommit: f5382652b6880fab42040df40a08de7cb2d74d35
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/17/2022
ms.locfileid: "63561584"
---
# <a name="album-resource-type"></a>相册资源类型

命名空间：microsoft.graph

相册是一种在捆绑包中将具有照片 Facet 的 [driveItemsdriveItem][] 组合在一起[的方法][]。[][] 此类型的捆绑包将在 **bundle** 资源上设置 [相册][] 属性。

## <a name="properties"></a>属性

| 属性名称     | 类型   | 说明
|:------------------|:-------|:------------------------------------------------
| coverImageItemId | 字符串 | 作为专辑封面的 [driveItem][] 的唯一标识符。

**注意：** 如果 **之前尚未设置 coverImageItemId** ，则会自动选择专辑的缩略图。
设置 **coverImageItemId** 后，相册的缩略图将始终与该 ID 关联。你可以替代默认封面，方法为 PATCHing the [bundle] [itembundle]，将 上的 **coverImageItemId** `album` 属性设置为相册中包含的图像的 ID。
若要删除自定义集封面，可以将 **coverImageItemId** 属性设置为 null，并且将自动再次选择默认覆盖。

## <a name="json-representation"></a>JSON 表示形式

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.album" } -->

```json
{
  "coverImageItemId": "string"
}
```

[bundle]: bundle.md
[driveItem]: driveItem.md
[照片]: photo.md


