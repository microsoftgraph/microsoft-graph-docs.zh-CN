---
title: deviceOperatingSystemSummary 资源类型
description: 设备操作系统摘要。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2147034c060fa15e8e799d5ddbe72aabe635af08
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975643"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a>deviceOperatingSystemSummary 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

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



