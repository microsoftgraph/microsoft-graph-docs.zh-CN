---
title: windowsMinimumOperatingSystem 资源类型
description: Windows 移动应用需要的最低操作系统。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 03d270408e383d21cb63cb512dcccb58a155cb08
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58256085"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a>windowsMinimumOperatingSystem 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows 移动应用需要的最低操作系统。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|v8_0|布尔值|Windows 版本 8.0 或更高版本。|
|v8_1|布尔值|Windows 版本 8.1 或更高版本。|
|v10_0|布尔值|Windows 版本 10.0 或更高版本。|
|v10_1607|布尔值|Windows 10 1607 或更高版本。|
|v10_1703|布尔值|Windows 10 1703 或更高版本。|
|v10_1709|布尔值|Windows 10 1709 或更高版本。|
|v10_1803|布尔值|Windows 10 1803 或更高版本。|
|v10_1809|布尔值|Windows 10 1809 或更高版本。|
|v10_1903|布尔值|Windows 10 1903 或更高版本。|
|v10_1909|布尔值|Windows 10 1909 或更高版本。|
|v10_2004|布尔值|Windows 10 2004 或更高版本。|
|v10_2H20|布尔值|Windows 10 2H20 或更高版本。|
|v10_21H1|布尔值|Windows 10 21H1 或更高版本。|

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
  "v10_1903": true,
  "v10_1909": true,
  "v10_2004": true,
  "v10_2H20": true,
  "v10_21H1": true
}
```




