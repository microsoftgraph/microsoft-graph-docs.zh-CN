---
title: iosMinimumOperatingSystem 资源类型
description: 包含 iOS 移动应用需要的最低操作系统的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 833285b4549ddd829ab8d6bf98e8ba09875fa48f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532836"
---
# <a name="iosminimumoperatingsystem-resource-type"></a>iosMinimumOperatingSystem 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含 iOS 移动应用需要的最低操作系统的属性。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|v8_0|Boolean|版本 8.0 或更高版本。|
|v9_0|Boolean|版本 9.0 或更高版本。|
|v10_0|Boolean|版本 10.0 或更高版本。|
|v11_0|布尔值|版本 11.0 或更高版本。|
|v12_0|Boolean|版本12.0 或更高版本。|
|v13_0|Boolean|版本13.0 或更高版本。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMinimumOperatingSystem",
  "v8_0": true,
  "v9_0": true,
  "v10_0": true,
  "v11_0": true,
  "v12_0": true,
  "v13_0": true
}
```




