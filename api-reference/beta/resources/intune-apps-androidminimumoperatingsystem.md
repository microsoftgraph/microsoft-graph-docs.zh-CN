---
title: androidMinimumOperatingSystem 资源类型
description: 包含 Android 移动应用需要的最低操作系统的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3f18e21dcc6e67eb7285bf15c29e76d2c64eff18
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153807"
---
# <a name="androidminimumoperatingsystem-resource-type"></a>androidMinimumOperatingSystem 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含 Android 移动应用需要的最低操作系统的属性。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|v4_0|Boolean|版本 4.0 或更高版本。|
|v4_0_3|Boolean|版本 4.0.3 或更高版本。|
|v4_1|Boolean|版本 4.1 或更高版本。|
|v4_2|Boolean|版本 4.2 或更高版本。|
|v4_3|Boolean|版本 4.3 或更高版本。|
|v4_4|Boolean|版本 4.4 或更高版本。|
|v5_0|Boolean|版本 5.0 或更高版本。|
|v5_1|Boolean|版本 5.1 或更高版本。|
|v6_0|Boolean|版本6.0 或更高版本。|
|v7_0|Boolean|版本7.0 或更高版本。|
|v7_1|Boolean|版本7.1 或更高版本。|
|v8_0|Boolean|版本 8.0 或更高版本。|
|v8_1|Boolean|版本8.1 或更高版本。|
|v9_0|布尔值|版本 9.0 或更高版本。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidMinimumOperatingSystem",
  "v4_0": true,
  "v4_0_3": true,
  "v4_1": true,
  "v4_2": true,
  "v4_3": true,
  "v4_4": true,
  "v5_0": true,
  "v5_1": true,
  "v6_0": true,
  "v7_0": true,
  "v7_1": true,
  "v8_0": true,
  "v8_1": true,
  "v9_0": true
}
```




