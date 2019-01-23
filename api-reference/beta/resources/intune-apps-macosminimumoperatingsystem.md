---
title: macOSMinimumOperatingSystem 资源类型
description: 最低操作系统要求 MacOS 应用程序。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d1b5bb3c31f876cb7444ff90cad5060c08d2f60b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425923"
---
# <a name="macosminimumoperatingsystem-resource-type"></a>macOSMinimumOperatingSystem 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

最低操作系统要求 MacOS 应用程序。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|v10_7|Boolean|Mac OS 10.7 或更高版本。|
|v10_8|Boolean|Mac OS 10.8 或更高版本。|
|v10_9|Boolean|Mac OS 10.9 或更高版本。|
|v10_10|Boolean|Mac OS 10.10 或更高版本。|
|v10_11|Boolean|Mac OS 10.11 或更高版本。|
|v10_12|Boolean|Mac OS 10.12 或更高版本。|
|v10_13|Boolean|Mac OS 10.13 或更高版本。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSMinimumOperatingSystem",
  "v10_7": true,
  "v10_8": true,
  "v10_9": true,
  "v10_10": true,
  "v10_11": true,
  "v10_12": true,
  "v10_13": true
}
```




