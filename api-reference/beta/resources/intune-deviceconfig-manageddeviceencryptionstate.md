---
title: managedDeviceEncryptionState 资源类型
description: 每个设备的加密报告
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 792b9c0d3e62394b4ea06d389ba3891c133fa63322bb20b157d3803f8afd49e9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54236330"
---
# <a name="manageddeviceencryptionstate-resource-type"></a>managedDeviceEncryptionState 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

每个设备的加密报告

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 managedDeviceEncryptionStates](../api/intune-deviceconfig-manageddeviceencryptionstate-list.md)|[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) 集合|列出 [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) 对象的属性和关系。|
|[获取 managedDeviceEncryptionState](../api/intune-deviceconfig-manageddeviceencryptionstate-get.md)|[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|读取 [managedDeviceEncryptionState 对象的属性和](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) 关系。|
|[创建 managedDeviceEncryptionState](../api/intune-deviceconfig-manageddeviceencryptionstate-create.md)|[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|创建新的 [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) 对象。|
|[删除 managedDeviceEncryptionState](../api/intune-deviceconfig-manageddeviceencryptionstate-delete.md)|无|删除 [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)。|
|[更新 managedDeviceEncryptionState](../api/intune-deviceconfig-manageddeviceencryptionstate-update.md)|[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|更新 [managedDeviceEncryptionState 对象](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|userPrincipalName|字符串|用户名|
|deviceType|[deviceTypes](../resources/intune-deviceconfig-devicetypes.md)|设备平台。 可能的值是 `desktop` `windowsRT` `winMO6` ：、、、、、、、、、、 `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `blackberry` `palm` `unknown` 。|
|osVersion|String|设备的操作系统版本|
|tpmSpecificationVersion|String|设备 TPM 版本|
|deviceName|String|设备名称|
|encryptionReadinessState|[encryptionReadinessState](../resources/intune-deviceconfig-encryptionreadinessstate.md)|加密就绪状态。 可取值为：`notReady`、`ready`。|
|encryptionState|[encryptionState](../resources/intune-deviceconfig-encryptionstate.md)|设备加密状态。 可取值为：`notEncrypted`、`encrypted`。|
|encryptionPolicySettingState|[complianceStatus](../resources/intune-shared-compliancestatus.md)|加密策略设置状态。 可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。|
|advancedBitLockerStates|[advancedBitLockerState](../resources/intune-deviceconfig-advancedbitlockerstate.md)|高级 BitLocker 状态。 可能的值是 `success` `noUserConsent` `osVolumeUnprotected` ：、、、、、、、、、 `osVolumeTpmRequired` `osVolumeTpmOnlyRequired` `osVolumeTpmPinRequired` `osVolumeTpmStartupKeyRequired` `osVolumeTpmPinStartupKeyRequired` `osVolumeEncryptionMethodMismatch` `recoveryKeyBackupFailed` `fixedDriveNotEncrypted` `fixedDriveEncryptionMethodMismatch` `loggedOnUserNonAdmin` `windowsRecoveryEnvironmentNotConfigured` `tpmNotAvailable` `tpmNotReady` `networkError` 。|
|fileVaultStates|[fileVaultState](../resources/intune-deviceconfig-filevaultstate.md)|FileVault 状态。 可取值为：`success`、`driveEncryptedByUser`、`userDeferredEncryption`、`escrowNotEnabled`。|
|policyDetails|[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) 集合|策略详细信息|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceEncryptionState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceEncryptionState",
  "id": "String (identifier)",
  "userPrincipalName": "String",
  "deviceType": "String",
  "osVersion": "String",
  "tpmSpecificationVersion": "String",
  "deviceName": "String",
  "encryptionReadinessState": "String",
  "encryptionState": "String",
  "encryptionPolicySettingState": "String",
  "advancedBitLockerStates": "String",
  "fileVaultStates": "String",
  "policyDetails": [
    {
      "@odata.type": "microsoft.graph.encryptionReportPolicyDetails",
      "policyId": "String",
      "policyName": "String"
    }
  ]
}
```




