---
title: windowsProtectionState 资源类型
description: 设备保护状态实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 63ac9a9e5f6dd153238ea2666cf0bffd88ebf9da
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731034"
---
# <a name="windowsprotectionstate-resource-type"></a>windowsProtectionState 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备保护状态实体。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 windowsProtectionState](../api/intune-devices-windowsprotectionstate-get.md)|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|读取 [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) 对象的属性和关系。|
|[更新 windowsProtectionState](../api/intune-devices-windowsprotectionstate-update.md)|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|更新 [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设备保护状态对象的唯一标识符。 这是设备的设备 id|
|malwareProtectionEnabled|布尔|已启用反恶意软件|
|deviceState|[windowsDeviceHealthState](../resources/intune-devices-windowsdevicehealthstate.md)|计算机的状态 (如干净或挂起的完全扫描或挂起的重新启动等) 。 可取值为：`clean`、`fullScanPending`、`rebootPending`、`manualStepsPending`、`offlineScanPending`、`critical`。|
|realTimeProtectionEnabled|布尔|是否启用了实时保护？|
|networkInspectionSystemEnabled|布尔|网络检查系统是否已启用？|
|quickScanOverdue|布尔|快速扫描是否过期？|
|fullScanOverdue|布尔|完全扫描逾期？|
|signatureUpdateOverdue|布尔|签名是否已过期？|
|rebootRequired|布尔|是否需要重新启动？|
|fullScanRequired|布尔|需要完全扫描吗？|
|engineVersion|String|当前 endpoint protection 引擎的版本|
|signatureVersion|String|当前恶意软件定义版本|
|antiMalwareVersion|String|当前反恶意软件版本|
|lastQuickScanDateTime|DateTimeOffset|上次快速扫描日期时间|
|lastFullScanDateTime|DateTimeOffset|上次快速扫描日期时间|
|lastQuickScanSignatureVersion|String|上次快速扫描签名版本|
|lastFullScanSignatureVersion|String|上次完全扫描签名版本|
|lastReportedDateTime|DateTimeOffset|上次设备运行状况状态报告时间|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|detectedMalwareState|[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) 集合|设备恶意软件列表|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsProtectionState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "id": "String (identifier)",
  "malwareProtectionEnabled": true,
  "deviceState": "String",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "String",
  "signatureVersion": "String",
  "antiMalwareVersion": "String",
  "lastQuickScanDateTime": "String (timestamp)",
  "lastFullScanDateTime": "String (timestamp)",
  "lastQuickScanSignatureVersion": "String",
  "lastFullScanSignatureVersion": "String",
  "lastReportedDateTime": "String (timestamp)"
}
```





