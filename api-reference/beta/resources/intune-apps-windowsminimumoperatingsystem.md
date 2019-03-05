---
title: windowsMinimumOperatingSystem 资源类型
description: Windows 移动应用需要的最低操作系统。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9f230ed4860e3ff8bad7968367ce5337b59521d4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152883"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a>windowsMinimumOperatingSystem 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows 移动应用需要的最低操作系统。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|v8_0|Boolean|Windows 版本 8.0 或更高版本。|
|v8_1|Boolean|Windows 版本 8.1 或更高版本。|
|v10_0|布尔值|Windows 版本 10.0 或更高版本。|
|v10_1607|Boolean|Windows 10 1607 或更高版本。|
|v10_1703|Boolean|Windows 10 1703 或更高版本。|
|v10_1709|Boolean|Windows 10 1709 或更高版本。|
|v10_1803|Boolean|Windows 10 1803 或更高版本。|

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
  "v10_1803": true
}
```




