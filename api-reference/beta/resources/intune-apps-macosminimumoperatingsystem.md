---
title: macOSMinimumOperatingSystem 资源类型
description: MacOS 应用程序所需的最低操作系统。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 20a08b6be50608bebf4482e61f032b9587b04566
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49281766"
---
# <a name="macosminimumoperatingsystem-resource-type"></a>macOSMinimumOperatingSystem 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

MacOS 应用程序所需的最低操作系统。

## <a name="properties"></a>属性
|属性|类型|Description|
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
  "v10_15": true
}
```




