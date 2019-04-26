---
title: androidMinimumOperatingSystem 资源类型
description: 包含 Android 移动应用需要的最低操作系统的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f2402ad007b794e7d6824e52cce8ff7144c6c33b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32560870"
---
# <a name="androidminimumoperatingsystem-resource-type"></a>androidMinimumOperatingSystem 资源类型

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

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
  "v5_1": true
}
```



