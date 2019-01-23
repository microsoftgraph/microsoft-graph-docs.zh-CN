---
title: windowsProtectionState 资源类型
description: 设备的保护状态实体。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1ef6c86983475abc687055ac2322ba02fae27ecd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423585"
---
# <a name="windowsprotectionstate-resource-type"></a>windowsProtectionState 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备的保护状态实体。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 windowsProtectionState](../api/intune-devices-windowsprotectionstate-get.md)|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|读取属性和[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)对象的关系。|
|[更新 windowsProtectionState](../api/intune-devices-windowsprotectionstate-update.md)|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|更新[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设备保护状态对象的唯一标识符。 这是设备的设备 id|
|malwareProtectionEnabled|Boolean|反恶意软件被启用还是没有|
|deviceState|[windowsDeviceHealthState](../resources/intune-devices-windowsdevicehealthstate.md)|计算机的状态 （如清理挂起完全扫描或挂起的重新启动等）。 可取值为：`clean`、`fullScanPending`、`rebootPending`、`manualStepsPending`、`offlineScanPending`、`critical`。|
|realTimeProtectionEnabled|Boolean|是否启用实时保护？|
|networkInspectionSystemEnabled|Boolean|启用或不网络检查系统？|
|quickScanOverdue|Boolean|快速扫描过期，或不？|
|fullScanOverdue|Boolean|或不完全扫描过期？|
|signatureUpdateOverdue|Boolean|过期的签名或不？|
|rebootRequired|Boolean|需要或不重新启动？|
|fullScanRequired|Boolean|所需或不完全扫描？|
|engineVersion|String|当前终结点保护引擎的版本|
|特征码版本|String|当前的恶意软件定义版本|
|antiMalwareVersion|String|当前防恶意软件版本|
|lastQuickScanDateTime|DateTimeOffset|最后一个快速扫描 datetime|
|lastFullScanDateTime|DateTimeOffset|最后一个快速扫描 datetime|
|lastQuickScanSignatureVersion|String|最后一个快速扫描病毒特征版本|
|lastFullScanSignatureVersion|String|最后一个完全扫描病毒特征版本|
|lastReportedDateTime|DateTimeOffset|最后一个设备运行状况状态报告的时间|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|detectedMalwareState|[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md)集合|设备恶意软件的列表|

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




