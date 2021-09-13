---
title: deviceProtectionOverview 资源类型
description: 给定设备的硬件信息。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 310d7e8623dad1baac2d77b6b8e23e527e4e4709
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59125860"
---
# <a name="deviceprotectionoverview-resource-type"></a>deviceProtectionOverview 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

给定设备的硬件信息。

## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|totalReportedDeviceCount|Int32|设备总数。|
|inactiveThreatAgentDeviceCount|Int32|具有非活动威胁代理计数的设备|
|unknownStateThreatAgentDeviceCount|Int32|威胁代理状态为未知计数的设备。|
|pendingSignatureUpdateDeviceCount|Int32|具有旧签名计数的设备。|
|cleanDeviceCount|Int32|清理设备计数。|
|pendingFullScanDeviceCount|Int32|挂起的完全扫描设备计数。|
|pendingRestartDeviceCount|Int32|挂起的重启设备计数。|
|pendingManualStepsDeviceCount|Int32|挂起的手动步骤设备计数。|
|pendingOfflineScanDeviceCount|Int32|挂起脱机扫描设备计数。|
|criticalFailuresDeviceCount|Int32|严重故障设备计数。|
|pendingQuickScanDeviceCount|Int32|挂起快速扫描设备计数。 有效值 -2147483648 2147483647|

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
  "criticalFailuresDeviceCount": 1024,
  "pendingQuickScanDeviceCount": 1024
}
```



