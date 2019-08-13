---
title: deviceProtectionOverview 资源类型
description: 给定设备的硬件信息。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bcae979d81034155b715a634476b8dc4aa7a9c4a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369953"
---
# <a name="deviceprotectionoverview-resource-type"></a>deviceProtectionOverview 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

给定设备的硬件信息。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|totalReportedDeviceCount|Int32|设备计数总数。|
|inactiveThreatAgentDeviceCount|Int32|带有非活动威胁代理计数的设备|
|unknownStateThreatAgentDeviceCount|Int32|包含威胁代理状态的设备作为未知计数。|
|pendingSignatureUpdateDeviceCount|Int32|具有旧签名计数的设备。|
|cleanDeviceCount|Int32|清洗设备计数。|
|pendingFullScanDeviceCount|Int32|正在等待完全扫描设备计数。|
|pendingRestartDeviceCount|Int32|等待重新启动设备计数。|
|pendingManualStepsDeviceCount|Int32|正在等待手动步骤设备计数。|
|pendingOfflineScanDeviceCount|Int32|等待脱机扫描设备计数。|
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



