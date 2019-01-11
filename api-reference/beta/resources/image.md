---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Image
localization_priority: Normal
ms.openlocfilehash: 2b5e084294c528a83f80b0c49badbf8f1e96ca41
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889724"
---
# <a name="image-resource-type"></a>图像资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

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

有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。


<!-- {
  "type": "#page.annotation",
  "description": "The image facet describes properties of an image like width and height",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Image"
} -->
