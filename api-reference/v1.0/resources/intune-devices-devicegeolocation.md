---
title: deviceGeoLocation 资源类型
description: 设备位置
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: eb11f4c8d4d2ce87d28d92f13e359ce213c3ca9c
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356979"
---
# <a name="devicegeolocation-resource-type"></a>deviceGeoLocation 资源类型

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备位置

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|lastCollectedDateTime|DateTimeOffset|记录位置时的时间，相对于 UTC|
|longitude|双精度数|设备位置的经度坐标|
|latitude|双精度|设备位置的纬度坐标|
|altitude|双精度|高度，以高出海平面的米数表示|
|horizontalAccuracy|双精度|经度和纬度的准确度，以米为单位|
|verticalAccuracy|双精度|高度的准确度，以米为单位|
|heading|双精度|相对于真北的方位，以度为单位|
|speed|Double|设备的移动速度，以米/秒为单位|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceGeoLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceGeoLocation",
  "lastCollectedDateTime": "String (timestamp)",
  "longitude": "<Unknown Primitive Type Edm.Double>",
  "latitude": "<Unknown Primitive Type Edm.Double>",
  "altitude": "<Unknown Primitive Type Edm.Double>",
  "horizontalAccuracy": "<Unknown Primitive Type Edm.Double>",
  "verticalAccuracy": "<Unknown Primitive Type Edm.Double>",
  "heading": "<Unknown Primitive Type Edm.Double>",
  "speed": "<Unknown Primitive Type Edm.Double>"
}
```




