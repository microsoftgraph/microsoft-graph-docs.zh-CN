---
title: 更新 windowsProtectionState
description: 更新 windowsProtectionState 对象的属性。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 92174fd5788a424ceaab08815d143ae229ef7e5e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59024542"
---
# <a name="update-windowsprotectionstate"></a>更新 windowsProtectionState

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [windowsProtectionState 对象](../resources/intune-devices-windowsprotectionstate.md) 的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementManagedDevices.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) 对象的 JSON 表示形式。

下表显示创建 [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)时所需的属性。

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
|productStatus|[windowsDefenderProductStatus](../resources/intune-devices-windowsdefenderproductstatus.md)|产品状态Windows Defender 防病毒。 可能的值是 `noStatus` `serviceNotRunning` `serviceStartedWithoutMalwareProtection` ：、、、、、、、、、、 `pendingFullScanDueToThreatAction` `pendingRebootDueToThreatAction` `pendingManualStepsDueToThreatAction` `avSignaturesOutOfDate` `asSignaturesOutOfDate` `noQuickScanHappenedForSpecifiedPeriod` `noFullScanHappenedForSpecifiedPeriod` `systemInitiatedScanInProgress` `systemInitiatedCleanInProgress` `samplesPendingSubmission` `productRunningInEvaluationMode` `productRunningInNonGenuineMode` `productExpired` `offlineScanRequired` `serviceShutdownAsPartOfSystemShutdown` `threatRemediationFailedCritically` `threatRemediationFailedNonCritically` `noStatusFlagsSet` `platformOutOfDate` `platformUpdateInProgress` `platformAboutToBeOutdated` `signatureOrPlatformEndOfLifeIsPastOrIsImpending` `windowsSModeSignaturesInUseOnNonWin10SInstall` 、|
|isVirtualMachine|Boolean|指示设备是否是虚拟机。|
|tamperProtectionEnabled|Boolean|指示是否Windows Defender篡改保护功能。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
Content-type: application/json
Content-length: 971

{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "malwareProtectionEnabled": true,
  "deviceState": "fullScanPending",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "Engine Version value",
  "signatureVersion": "Signature Version value",
  "antiMalwareVersion": "Anti Malware Version value",
  "lastQuickScanDateTime": "2016-12-31T23:58:27.5900669-08:00",
  "lastFullScanDateTime": "2017-01-01T00:01:44.9405639-08:00",
  "lastQuickScanSignatureVersion": "Last Quick Scan Signature Version value",
  "lastFullScanSignatureVersion": "Last Full Scan Signature Version value",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "productStatus": "serviceNotRunning",
  "isVirtualMachine": true,
  "tamperProtectionEnabled": true
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1020

{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "id": "1ac6ea5a-ea5a-1ac6-5aea-c61a5aeac61a",
  "malwareProtectionEnabled": true,
  "deviceState": "fullScanPending",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "Engine Version value",
  "signatureVersion": "Signature Version value",
  "antiMalwareVersion": "Anti Malware Version value",
  "lastQuickScanDateTime": "2016-12-31T23:58:27.5900669-08:00",
  "lastFullScanDateTime": "2017-01-01T00:01:44.9405639-08:00",
  "lastQuickScanSignatureVersion": "Last Quick Scan Signature Version value",
  "lastFullScanSignatureVersion": "Last Full Scan Signature Version value",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "productStatus": "serviceNotRunning",
  "isVirtualMachine": true,
  "tamperProtectionEnabled": true
}
```



