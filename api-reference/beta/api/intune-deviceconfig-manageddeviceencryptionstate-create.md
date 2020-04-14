---
title: 创建 managedDeviceEncryptionState
description: 创建新的 managedDeviceEncryptionState 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e07632944ff5ba2230b25214dd767aed94d47f05
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43431970"
---
# <a name="create-manageddeviceencryptionstate"></a>创建 managedDeviceEncryptionState

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDeviceEncryptionStates
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 managedDeviceEncryptionState 对象的 JSON 表示形式。

下表显示创建 managedDeviceEncryptionState 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|userPrincipalName|String|用户名|
|deviceType|[deviceTypes](../resources/intune-deviceconfig-devicetypes.md)|设备的平台。 可能的值为`desktop`： `windowsRT`、 `winMO6`、 `nokia` `windowsPhone` `mac` `winCE` `palm` `unknown`、、、、、、、、、、、、、、、、、、、。 `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `blackberry`|
|osVersion|String|设备的操作系统版本|
|tpmSpecificationVersion|String|设备 TPM 版本|
|deviceName|String|设备名称|
|encryptionReadinessState|[encryptionReadinessState](../resources/intune-deviceconfig-encryptionreadinessstate.md)|加密准备情况状态。 可取值为：`notReady`、`ready`。|
|encryptionState|[encryptionState](../resources/intune-deviceconfig-encryptionstate.md)|设备加密状态。 可取值为：`notEncrypted`、`encrypted`。|
|encryptionPolicySettingState|[complianceStatus](../resources/intune-shared-compliancestatus.md)|加密策略设置状态。 可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。|
|advancedBitLockerStates|[advancedBitLockerState](../resources/intune-deviceconfig-advancedbitlockerstate.md)|高级 BitLocker 状态。 可能的值是`success`： `noUserConsent`、 `osVolumeEncryptionMethodMismatch`、 `osVolumeTpmRequired` `osVolumeTpmOnlyRequired` `osVolumeTpmPinRequired` `osVolumeTpmStartupKeyRequired` `osVolumeTpmPinStartupKeyRequired` `osVolumeUnprotected` `recoveryKeyBackupFailed` `networkError`、、 `fixedDriveNotEncrypted`、、、、、、、、、、、、。 `fixedDriveEncryptionMethodMismatch` `loggedOnUserNonAdmin` `windowsRecoveryEnvironmentNotConfigured` `tpmNotAvailable` `tpmNotReady`|
|fileVaultStates|[fileVaultState](../resources/intune-deviceconfig-filevaultstate.md)|FileVault 状态。 可取值为：`success`、`driveEncryptedByUser`、`userDeferredEncryption`、`escrowNotEnabled`。|
|policyDetails|[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md)集合|策略详细信息|



## <a name="response"></a>响应
如果成功，此方法在响应`201 Created`正文中返回响应代码和[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDeviceEncryptionStates
Content-type: application/json
Content-length: 704

{
  "@odata.type": "#microsoft.graph.managedDeviceEncryptionState",
  "userPrincipalName": "User Principal Name value",
  "deviceType": "windowsRT",
  "osVersion": "Os Version value",
  "tpmSpecificationVersion": "Tpm Specification Version value",
  "deviceName": "Device Name value",
  "encryptionReadinessState": "ready",
  "encryptionState": "encrypted",
  "encryptionPolicySettingState": "notApplicable",
  "advancedBitLockerStates": "noUserConsent",
  "fileVaultStates": "driveEncryptedByUser",
  "policyDetails": [
    {
      "@odata.type": "microsoft.graph.encryptionReportPolicyDetails",
      "policyId": "Policy Id value",
      "policyName": "Policy Name value"
    }
  ]
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 753

{
  "@odata.type": "#microsoft.graph.managedDeviceEncryptionState",
  "id": "f09b4ab6-4ab6-f09b-b64a-9bf0b64a9bf0",
  "userPrincipalName": "User Principal Name value",
  "deviceType": "windowsRT",
  "osVersion": "Os Version value",
  "tpmSpecificationVersion": "Tpm Specification Version value",
  "deviceName": "Device Name value",
  "encryptionReadinessState": "ready",
  "encryptionState": "encrypted",
  "encryptionPolicySettingState": "notApplicable",
  "advancedBitLockerStates": "noUserConsent",
  "fileVaultStates": "driveEncryptedByUser",
  "policyDetails": [
    {
      "@odata.type": "microsoft.graph.encryptionReportPolicyDetails",
      "policyId": "Policy Id value",
      "policyName": "Policy Name value"
    }
  ]
}
```



