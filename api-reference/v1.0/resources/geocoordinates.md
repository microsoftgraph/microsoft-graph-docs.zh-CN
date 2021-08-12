---
author: JeremyKelley
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
description: GeoCoordinates 资源基于文件中包含的元数据提供位置的地理坐标和海拔。
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: f5f61b07cf9c6940fdd56aa2f34f1fc70a8211decf3e34e19ff8eeac9e839da8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54175271"
---
# <a name="geocoordinates-resource-type"></a>GeoCoordinates 资源类型

命名空间：microsoft.graph

**GeoCoordinates** 资源基于文件中包含的元数据提供位置的地理坐标和海拔。如果 [**DriveItem**](driveitem.md) 具有一个非 null **位置** 方面，则该项表示一个已知位置和与其相关的文件。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.geoCoordinates"
}-->

```json
{
  "altitude": 1024.13,
  "latitude": 26.13246,
  "longitude": 24.34616
}
```

## <a name="properties"></a>属性

| 属性  | 类型   | 说明
|:----------|:-------|:--------------------------------------------------------
| 海拔  | Double | 可选。此项高于海平面的高度（以英尺为单位）。只读。
| 纬度  | Double | 可选。此项的纬度（以十进制表示）。只读。
| 经度 | Double | 可选。此项的经度（以十进制表示）。只读。

## <a name="remarks"></a>注解

有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。

<!-- {
  "type": "#page.annotation",
  "description": "The location facet provides geographic location related properties for an item",
  "keywords": "location,geographic,item,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Location"
} -->

