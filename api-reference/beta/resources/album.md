---
author: JeremyKelley
ms.author: jeremyke
title: 唱集资源类型
description: 描述属于相册的捆绑包的 Facet。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 59717995870cbfe970fd23b160377d32cb722835
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974449"
---
# <a name="album-resource-type"></a>唱集资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

相册是在[捆绑包][]中将[driveitem][driveItem]与[照片][]facet 组合在一起的一种方式。 此类型的捆绑包将在[捆绑][]资源上设置**唱集**属性。

## <a name="properties"></a>属性

| 属性名称     | 类型   | 说明
|:------------------|:-------|:------------------------------------------------
| coverImageItemId | String | [DriveItem][]的唯一标识符, 它是唱片集的封面。

**注意:** 如果尚未设置**coverImageItemId** , 则会自动选择影集的缩略图。
设置**coverImageItemId**后, 影集的缩略图将始终为与该 id 关联的项目。您可以通过修补[捆绑包项目][捆绑]并将**coverImageItemId**属性设置`album`为包含在影集中的图像的 id 来覆盖默认封面。
若要删除自定义设置的封面, 可以将**coverImageItemId**属性设置为 null, 并再次自动选择默认属性。

## <a name="json-representation"></a>JSON 表示形式

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.album" } -->

```json
{
  "coverImageItemId": "string"
}
```

[bundle]: bundle.md
[driveItem]: driveItem.md
[photo]: photo.md
