---
title: androidMinimumOperatingSystem 资源类型
description: 包含 Android 移动应用需要的最低操作系统的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4328cfe06180be138b2c33840c72620efdaa277b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403124"
---
# <a name="androidminimumoperatingsystem-resource-type"></a>androidMinimumOperatingSystem 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含 Android 移动应用需要的最低操作系统的属性。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|v4_0|布尔值|版本 4.0 或更高版本。|
|v4_0_3|布尔值|版本 4.0.3 或更高版本。|
|v4_1|布尔值|版本 4.1 或更高版本。|
|v4_2|布尔值|版本 4.2 或更高版本。|
|v4_3|布尔值|版本 4.3 或更高版本。|
|v4_4|布尔值|版本 4.4 或更高版本。|
|v5_0|布尔值|版本 5.0 或更高版本。|
|v5_1|布尔值|版本 5.1 或更高版本。|
|v6_0|Boolean|版本 6.0 或更高版本。|
|v7_0|Boolean|7.0 版或更高版本。|
|v7_1|Boolean|7.1 或更高版本。|
|v8_0|布尔值|版本 8.0 或更高版本。|
|v8_1|布尔值|8.1 或更高版本。|
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




