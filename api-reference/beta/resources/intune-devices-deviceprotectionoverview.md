---
title: deviceProtectionOverview 资源类型
description: 硬件的给定设备的信息。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 902e3a6062d2aa50c96c27eb9d542905bf9a029d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418986"
---
# <a name="deviceprotectionoverview-resource-type"></a>deviceProtectionOverview 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

硬件的给定设备的信息。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|totalReportedDeviceCount|Int32|总设备计数。|
|inactiveThreatAgentDeviceCount|Int32|非活动威胁代理计数设备|
|unknownStateThreatAgentDeviceCount|Int32|与为未知计数的威胁代理状态的设备。|
|pendingSignatureUpdateDeviceCount|Int32|使用旧签名计数的设备。|
|cleanDeviceCount|Int32|清理设备计数。|
|pendingFullScanDeviceCount|Int32|待处理的完全扫描设备计数。|
|pendingRestartDeviceCount|Int32|挂起的重新启动设备计数。|
|pendingManualStepsDeviceCount|Int32|待处理的手动步骤设备计数。|
|pendingOfflineScanDeviceCount|Int32|待处理的脱机扫描设备计数。|
|criticalFailuresDeviceCount|Int32|严重故障设备计数。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceProtectionOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceProtectionOverview",
  "totalReportedDeviceCount": 1024,
  "inactiveThreatAgentDeviceCount": 1024,
  "unknownStateThreatAgentDeviceCount": 1024,
  "pendingSignatureUpdateDeviceCount": 1024,
  "cleanDeviceCount": 1024,
  "pendingFullScanDeviceCount": 1024,
  "pendingRestartDeviceCount": 1024,
  "pendingManualStepsDeviceCount": 1024,
  "pendingOfflineScanDeviceCount": 1024,
  "criticalFailuresDeviceCount": 1024
}
```




