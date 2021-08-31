---
title: macOSMinimumOperatingSystem 资源类型
description: MacOS 应用所需的最低操作系统。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 718af8c04e604cb136537b6f0e1763c9d3a4ae53
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58786395"
---
# <a name="macosminimumoperatingsystem-resource-type"></a>macOSMinimumOperatingSystem 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

MacOS 应用所需的最低操作系统。

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
|v10_14|Boolean|Mac OS 10.14 或更高版本。|
|v10_15|Boolean|Mac OS 10.15 或更高版本。|
|v11_0|布尔值|Mac OS 11.0 或更高版本。|
|v12_0|Boolean|Mac OS 12.0 或更高版本。|

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
  "v10_13": true,
  "v10_14": true,
  "v10_15": true,
  "v11_0": true,
  "v12_0": true
}
```



