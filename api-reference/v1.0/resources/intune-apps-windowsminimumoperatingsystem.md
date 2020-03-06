---
title: windowsMinimumOperatingSystem 资源类型
description: Windows 移动应用需要的最低操作系统。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 24ac15200fa293cc65a6207a91e5dc1132df1759
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531071"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a>windowsMinimumOperatingSystem 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows 移动应用需要的最低操作系统。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|v8_0|Boolean|Windows 版本 8.0 或更高版本。|
|v8_1|布尔值|Windows 版本 8.1 或更高版本。|
|v10_0|布尔值|Windows 版本 10.0 或更高版本。|

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
  "v10_0": true
}
```




