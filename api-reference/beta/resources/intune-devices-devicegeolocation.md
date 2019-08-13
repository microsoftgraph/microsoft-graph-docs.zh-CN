---
title: deviceGeoLocation 资源类型
description: 设备位置
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1da2a612a777491731fa0b85e2f754605ffa04bc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370163"
---
# <a name="devicegeolocation-resource-type"></a>deviceGeoLocation 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备位置

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|lastCollectedDateTimeUtc|DateTimeOffset|记录位置时的时间，相对于 UTC|
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
  "lastCollectedDateTimeUtc": "String (timestamp)",
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



