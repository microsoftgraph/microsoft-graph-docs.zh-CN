---
title: windowsMinimumOperatingSystem 资源类型
description: Windows 移动应用需要的最低操作系统。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4544ac21f01c7b210a61f6ce91d9880bacd4a02e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49284321"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a>windowsMinimumOperatingSystem 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows 移动应用需要的最低操作系统。

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|v8_0|布尔值|Windows 版本 8.0 或更高版本。|
|v8_1|布尔值|Windows 版本 8.1 或更高版本。|
|v10_0|布尔值|Windows 版本 10.0 或更高版本。|
|v10_1607|Boolean|Windows 10 1607 或更高版本。|
|v10_1703|Boolean|Windows 10 1703 或更高版本。|
|v10_1709|Boolean|Windows 10 1709 或更高版本。|
|v10_1803|Boolean|Windows 10 1803 或更高版本。|
|v10_1809|Boolean|Windows 10 1809 或更高版本。|
|v10_1903|Boolean|Windows 10 1903 或更高版本。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsMinimumOperatingSystem",
  "v8_0": true,
  "v8_1": true,
  "v10_0": true,
  "v10_1607": true,
  "v10_1703": true,
  "v10_1709": true,
  "v10_1803": true,
  "v10_1809": true,
  "v10_1903": true
}
```




