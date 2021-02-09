---
title: iosMinimumOperatingSystem 资源类型
description: 包含 iOS 移动应用需要的最低操作系统的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9038d3cf058e8c9930b5f083709f3a5ed286300a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154443"
---
# <a name="iosminimumoperatingsystem-resource-type"></a>iosMinimumOperatingSystem 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含 iOS 移动应用需要的最低操作系统的属性。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|v8_0|布尔值|版本 8.0 或更高版本。|
|v9_0|布尔值|版本 9.0 或更高版本。|
|v10_0|布尔值|版本 10.0 或更高版本。|
|v11_0|布尔值|版本 11.0 或更高版本。|
|v12_0|布尔|版本 12.0 或更高版本。|
|v13_0|布尔|版本 13.0 或更高版本。|
|v14_0|布尔|版本 14.0 或更高版本。|

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
  "v13_0": true,
  "v14_0": true
}
```




