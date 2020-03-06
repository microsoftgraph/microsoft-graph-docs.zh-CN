---
author: JeremyKelley
description: 图像资源将与图像相关的属性分组到一个单一结构。
ms.date: 09/10/2017
title: 图像
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 06d9c5b22c4786fc92e8156dbfea066c77d219f3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496535"
---
# <a name="image-resource-type"></a>图像资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**图像**资源将与图像相关的属性分组到一个单一结构。如果 [**DriveItem**](driveitem.md)具有一个非 null **图像**方面，则该项表示一个位图图像。

**注意：** 如果该服务无法确定图像的宽度和高度，**图像**资源可能为空。

## <a name="json-representation"></a>JSON 表示形式

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.image" } -->
```json
{
  "width": 100,
  "height": 200
}
```

## <a name="properties"></a>属性

| 属性   | 类型  | 说明                                |
|:-----------|:------|:-------------------------------------------|
| **高度** | Int32 | 可选。图像的高度，以像素为单位。只读。 |
| **width**  | Int32 | 可选。图像的宽度，以像素为单位。只读。  |

## <a name="remarks"></a>注解

在 OneDrive for Business 中，基于文件扩展名在应为图像的项中返回此类资源。

有关 DriveItem 上 Facet 的详细信息，请参阅 [DriveItem](driveitem.md)。


<!--
{
  "type": "#page.annotation",
  "description": "The image facet describes properties of an image like width and height",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Image",
  "suppressions": []
}
-->
