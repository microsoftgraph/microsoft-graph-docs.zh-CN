---
title: deviceProtectionOverview 资源类型
description: 硬件的给定设备的信息。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f7b7c28474692c1b1df3b1d6a703e3dd43d05a15
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944318"
---
# <a name="deviceprotectionoverview-resource-type"></a>deviceProtectionOverview 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

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

## <a name="relationships"></a>Relationships
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





