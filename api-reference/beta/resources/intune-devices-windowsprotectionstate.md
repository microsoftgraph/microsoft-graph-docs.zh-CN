---
title: windowsProtectionState 资源类型
description: 设备保护状态实体。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 39ee7f404ffc54a31a29fec2cac5f6876884f1db
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59040006"
---
# <a name="windowsprotectionstate-resource-type"></a>windowsProtectionState 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备保护状态实体。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 windowsProtectionState](../api/intune-devices-windowsprotectionstate-get.md)|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|读取 [windowsProtectionState 对象的属性和](../resources/intune-devices-windowsprotectionstate.md) 关系。|
|[更新 windowsProtectionState](../api/intune-devices-windowsprotectionstate-update.md)|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|更新 [windowsProtectionState 对象](../resources/intune-devices-windowsprotectionstate.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设备保护状态对象的唯一标识符。 这是设备的设备 ID|
|malwareProtectionEnabled|Boolean|反恶意软件是否已启用|
|deviceState|[windowsDeviceHealthState](../resources/intune-devices-windowsdevicehealthstate.md)|计算机的状态 (干净或挂起完全扫描或挂起重启等) 。 可取值为：`clean`、`fullScanPending`、`rebootPending`、`manualStepsPending`、`offlineScanPending`、`critical`。|
|realTimeProtectionEnabled|Boolean|实时保护是否已启用？|
|networkInspectionSystemEnabled|Boolean|网络检查系统是否已启用？|
|quickScanOverdue|Boolean|快速扫描是否过期？|
|fullScanOverdue|Boolean|完全扫描是否过期？|
|signatureUpdateOverdue|Boolean|签名是否过期？|
|rebootRequired|Boolean|是否要求重新启动？|
|fullScanRequired|Boolean|是否要求进行完全扫描？|
|engineVersion|String|当前终结点保护引擎的版本|
|signatureVersion|String|当前恶意软件定义版本|
|antiMalwareVersion|String|当前反恶意软件版本|
|lastQuickScanDateTime|DateTimeOffset|上次快速扫描日期/时间|
|lastFullScanDateTime|DateTimeOffset|上次快速扫描日期/时间|
|lastQuickScanSignatureVersion|String|上次快速扫描签名版本|
|lastFullScanSignatureVersion|String|上次完全扫描签名版本|
|lastReportedDateTime|DateTimeOffset|上次设备运行状况报告时间|
|productStatus|[windowsDefenderProductStatus](../resources/intune-devices-windowsdefenderproductstatus.md)|产品状态Windows Defender 防病毒。 可能的值是 `noStatus` `serviceNotRunning` `serviceStartedWithoutMalwareProtection` ：、、、、、、、、、、。 `pendingFullScanDueToThreatAction` `pendingRebootDueToThreatAction` `pendingManualStepsDueToThreatAction` `avSignaturesOutOfDate` `asSignaturesOutOfDate` `noQuickScanHappenedForSpecifiedPeriod` `noFullScanHappenedForSpecifiedPeriod` `systemInitiatedScanInProgress` `systemInitiatedCleanInProgress` `samplesPendingSubmission` `productRunningInEvaluationMode` `productRunningInNonGenuineMode` `productExpired` `offlineScanRequired` `serviceShutdownAsPartOfSystemShutdown` `threatRemediationFailedCritically` `threatRemediationFailedNonCritically` `noStatusFlagsSet` `platformOutOfDate` `platformUpdateInProgress` `platformAboutToBeOutdated` `signatureOrPlatformEndOfLifeIsPastOrIsImpending` `windowsSModeSignaturesInUseOnNonWin10SInstall`|
|isVirtualMachine|Boolean|指示设备是否是虚拟机。|
|tamperProtectionEnabled|Boolean|指示是否Windows Defender篡改保护功能。|

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
  "lastReportedDateTime": "String (timestamp)",
  "productStatus": "String",
  "isVirtualMachine": true,
  "tamperProtectionEnabled": true
}
```



