---
title: deviceOperatingSystemSummary 资源类型
description: 设备操作系统摘要。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3457894e43c1aed78d953c25ef862e08cc5c2ff1aee19ef43aa86aee8e02dc9c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54205659"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a>deviceOperatingSystemSummary 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备操作系统摘要。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|androidCount|Int32|Android 设备计数。|
|iosCount|Int32|iOS 设备计数。|
|macOSCount|Int32|Mac OS X 设备计数。|
|windowsMobileCount|Int32|Windows 移动设备计数。|
|windowsCount|Int32|Windows 设备计数。|
|unknownCount|Int32|未知设备计数。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceOperatingSystemSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceOperatingSystemSummary",
  "androidCount": 1024,
  "iosCount": 1024,
  "macOSCount": 1024,
  "windowsMobileCount": 1024,
  "windowsCount": 1024,
  "unknownCount": 1024
}
```




