---
title: managedDevice 资源类型
description: 通过 Intune 托管或预注册的设备
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3203b99766c861f4a7b89401ef3c0cc14383fa2f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59118304"
---
# <a name="manageddevice-resource-type"></a>managedDevice 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

通过 Intune 托管或预注册的设备

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List managedDevices](../api/intune-devices-manageddevice-list.md)|[managedDevice](../resources/intune-devices-manageddevice.md) 集合|列出 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的属性和关系。|
|[Get managedDevice](../api/intune-devices-manageddevice-get.md)|[managedDevice](../resources/intune-devices-manageddevice.md)|读取 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的属性和关系。|
|[Create managedDevice](../api/intune-devices-manageddevice-create.md)|[managedDevice](../resources/intune-devices-manageddevice.md)|创建新的 [managedDevice](../resources/intune-devices-manageddevice.md) 对象。|
|[Delete managedDevice](../api/intune-devices-manageddevice-delete.md)|无|删除 [managedDevice](../resources/intune-devices-manageddevice.md)。|
|[Update managedDevice](../api/intune-devices-manageddevice-update.md)|[managedDevice](../resources/intune-devices-manageddevice.md)|更新 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的属性。|
|[retire 操作](../api/intune-devices-manageddevice-retire.md)|无|停用设备|
|[wipe 操作](../api/intune-devices-manageddevice-wipe.md)|无|擦除设备|
|[resetPasscode 操作](../api/intune-devices-manageddevice-resetpasscode.md)|无|重置密码|
|[remoteLock 操作](../api/intune-devices-manageddevice-remotelock.md)|无|远程锁定|
|[requestRemoteAssistance 操作](../api/intune-devices-manageddevice-requestremoteassistance.md)|无|请求远程协助|
|[disableLostMode 操作](../api/intune-devices-manageddevice-disablelostmode.md)|无|禁用丢失模式|
|[locateDevice 操作](../api/intune-devices-manageddevice-locatedevice.md)|无|查找设备|
|[bypassActivationLock 操作](../api/intune-devices-manageddevice-bypassactivationlock.md)|无|跳过激活锁|
|[rebootNow 操作](../api/intune-devices-manageddevice-rebootnow.md)|无|重新启动设备|
|[shutDown 操作](../api/intune-devices-manageddevice-shutdown.md)|无|关闭设备|
|[recoverPasscode 操作](../api/intune-devices-manageddevice-recoverpasscode.md)|无|恢复密码|
|[cleanWindowsDevice 操作](../api/intune-devices-manageddevice-cleanwindowsdevice.md)|无|干净的 Windows 设备|
|[logoutSharedAppleDeviceActiveUser 操作](../api/intune-devices-manageddevice-logoutsharedappledeviceactiveuser.md)|无|注销共享 Apple 设备活动用户|
|[deleteUserFromSharedAppleDevice 操作](../api/intune-devices-manageddevice-deleteuserfromsharedappledevice.md)|无|从共享 Apple 设备中删除用户|
|[syncDevice 操作](../api/intune-devices-manageddevice-syncdevice.md)|无|尚未记录|
|[windowsDefenderScan 操作](../api/intune-devices-manageddevice-windowsdefenderscan.md)|无|尚未记录|
|[windowsDefenderUpdateSignatures 操作](../api/intune-devices-manageddevice-windowsdefenderupdatesignatures.md)|无|尚未记录|
|[updateWindowsDeviceAccount 操作](../api/intune-devices-manageddevice-updatewindowsdeviceaccount.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设备的唯一标识符。 此属性是只读的。|
|userId|String|与设备关联的用户的唯一标识符。 此属性是只读的。|
|deviceName|String|设备的名称。 此属性是只读的。|
|managedDeviceOwnerType|[managedDeviceOwnerType](../resources/intune-devices-manageddeviceownertype.md)|设备的所有权。 可以是"公司"或"个人"。 可取值为：`unknown`、`company`、`personal`。|
|deviceActionResults|[deviceActionResult](../resources/intune-devices-deviceactionresult.md) 集合|ComplexType deviceActionResult 对象的列表。 此属性是只读的。|
|enrolledDateTime|DateTimeOffset|设备的注册时间。 此属性是只读的。|
|lastSyncDateTime|DateTimeOffset|设备上次成功完成与 Intune 同步的日期和时间。 此属性是只读的。|
|operatingSystem|String|设备的操作系统。 Windows、iOS 等。此属性为只读。|
|complianceState|[complianceState](../resources/intune-devices-compliancestate.md)|设备的符合性状态。 此属性是只读的。 可取值为：`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager`。|
|jailBroken|String|设备是否已越狱或取得 root 权限。 此属性是只读的。|
|managementAgent|[managementAgentType](../resources/intune-devices-managementagenttype.md)|设备的管理通道。 Intune、EAS 等此属性为只读。 可取值为：`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`。|
|osVersion|String|设备的操作系统版本。 此属性是只读的。|
|easActivated|Boolean|设备是否已激活 Exchange ActiveSync。 此属性是只读的。|
|easDeviceId|String|设备的 Exchange ActiveSync ID。 此属性是只读的。|
|easActivationDateTime|DateTimeOffset|设备的 Exchange ActivationSync 激活时间。 此属性是只读的。|
|azureADRegistered|Boolean|设备是否已注册 Azure Active Directory。 此属性是只读的。|
|deviceEnrollmentType|[deviceEnrollmentType](../resources/intune-shared-deviceenrollmenttype.md)|设备的注册类型。 此属性是只读的。 可能的值是：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`、`windowsAzureADJoinUsingDeviceAuth`、`appleUserEnrollment`、`appleUserEnrollmentWithServiceAccount`。|
|activationLockBypassCode|String|允许绕过设备上的激活锁的代码。 此属性是只读的。|
|emailAddress|String|电子邮件 () 设备关联的用户的邮箱。 此属性是只读的。|
|azureADDeviceId|String|Azure Active Directory 设备的唯一标识符。 只读。 此属性是只读的。|
|deviceRegistrationState|[deviceRegistrationState](../resources/intune-devices-deviceregistrationstate.md)|设备注册状态。 此属性是只读的。 可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。|
|deviceCategoryDisplayName|String|设备类别显示名称。 此属性是只读的。|
|isSupervised|Boolean|设备监督状态。 此属性是只读的。|
|exchangeLastSuccessfulSyncDateTime|DateTimeOffset|设备上次与 Exchange 联系的时间。 此属性是只读的。|
|exchangeAccessState|[deviceManagementExchangeAccessState](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|Exchange 中设备的访问状态。 此属性是只读的。 可取值为：`none`、`unknown`、`allowed`、`blocked`、`quarantined`。|
|exchangeAccessStateReason|[deviceManagementExchangeAccessStateReason](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|Exchange 中设备访问状态的出现原因。 此属性是只读的。 可取值为：`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp`。|
|remoteAssistanceSessionUrl|String|允许与设备建立远程协助会话的 URL。 此属性是只读的。|
|remoteAssistanceSessionErrorDetails|String|用于在创建远程协助会话对象时识别问题的错误字符串。 此属性是只读的。|
|isEncrypted|Boolean|设备加密状态。 此属性是只读的。|
|userPrincipalName|String|设备用户主体名称。 此属性是只读的。|
|model|String|设备型号。 此属性是只读的。|
|manufacturer|String|设备的制造商。 此属性是只读的。|
|imei|String|IMEI。 此属性是只读的。|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|设备合规性宽限期到期的 DateTime。 此属性是只读的。|
|serialNumber|String|SerialNumber。 此属性是只读的。|
|phoneNumber|String|电话设备的数量。 此属性是只读的。|
|androidSecurityPatchLevel|String|Android 安全修补程序级别。 此属性是只读的。|
|userDisplayName|String|用户显示名称。 此属性是只读的。|
|configurationManagerClientEnabledFeatures|[configurationManagerClientEnabledFeatures](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|ConfigrMgr 客户端启用的功能。 此属性是只读的。|
|wiFiMacAddress|String|Wi-Fi MAC。 此属性是只读的。|
|deviceHealthAttestationState|[deviceHealthAttestationState](../resources/intune-devices-devicehealthattestationstate.md)|设备运行状况证明状态。 此属性是只读的。|
|subscriberCarrier|String|订阅者运营商。 此属性是只读的。|
|meid|String|MEID。 此属性是只读的。|
|totalStorageSpaceInBytes|Int64|总存储字节数。 此属性是只读的。|
|freeStorageSpaceInBytes|Int64|可用存储字节为单位。 此属性是只读的。|
|managedDeviceName|String|用于识别设备的自动生成的名称。 可以覆盖为用户友好名称。|
|partnerReportedThreatState|[managedDevicePartnerReportedHealthState](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|指示帐户和设备正在使用移动威胁防护合作伙伴时设备的威胁状态。 只读。 此属性是只读的。 可取值为：`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured`。|
|iccid|String|集成的电路卡标识符，它是 SIM 卡的唯一标识号。 此属性是只读的。|
|udid|String|iOS 和 macOS 设备的唯一设备标识符。 此属性是只读的。|
|notes|String|IT 管理员在设备上创建的备注|
|ethernetMacAddress|String|以太网 MAC。 此属性是只读的。|
|physicalMemoryInBytes|Int64|内存总量（以字节为单位）。 此属性是只读的。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|deviceCategory|[deviceCategory](../resources/intune-devices-devicecategory.md)|设备类别|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "String (identifier)",
  "userId": "String",
  "deviceName": "String",
  "managedDeviceOwnerType": "String",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "String",
      "actionState": "String",
      "startDateTime": "String (timestamp)",
      "lastUpdatedDateTime": "String (timestamp)"
    }
  ],
  "enrolledDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "operatingSystem": "String",
  "complianceState": "String",
  "jailBroken": "String",
  "managementAgent": "String",
  "osVersion": "String",
  "easActivated": true,
  "easDeviceId": "String",
  "easActivationDateTime": "String (timestamp)",
  "azureADRegistered": true,
  "deviceEnrollmentType": "String",
  "activationLockBypassCode": "String",
  "emailAddress": "String",
  "azureADDeviceId": "String",
  "deviceRegistrationState": "String",
  "deviceCategoryDisplayName": "String",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "String (timestamp)",
  "exchangeAccessState": "String",
  "exchangeAccessStateReason": "String",
  "remoteAssistanceSessionUrl": "String",
  "remoteAssistanceSessionErrorDetails": "String",
  "isEncrypted": true,
  "userPrincipalName": "String",
  "model": "String",
  "manufacturer": "String",
  "imei": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "serialNumber": "String",
  "phoneNumber": "String",
  "androidSecurityPatchLevel": "String",
  "userDisplayName": "String",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
    "inventory": true,
    "modernApps": true,
    "resourceAccess": true,
    "deviceConfiguration": true,
    "compliancePolicy": true,
    "windowsUpdateForBusiness": true
  },
  "wiFiMacAddress": "String",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "String",
    "contentNamespaceUrl": "String",
    "deviceHealthAttestationStatus": "String",
    "contentVersion": "String",
    "issuedDateTime": "String (timestamp)",
    "attestationIdentityKey": "String",
    "resetCount": 1024,
    "restartCount": 1024,
    "dataExcutionPolicy": "String",
    "bitLockerStatus": "String",
    "bootManagerVersion": "String",
    "codeIntegrityCheckVersion": "String",
    "secureBoot": "String",
    "bootDebugging": "String",
    "operatingSystemKernelDebugging": "String",
    "codeIntegrity": "String",
    "testSigning": "String",
    "safeMode": "String",
    "windowsPE": "String",
    "earlyLaunchAntiMalwareDriverProtection": "String",
    "virtualSecureMode": "String",
    "pcrHashAlgorithm": "String",
    "bootAppSecurityVersion": "String",
    "bootManagerSecurityVersion": "String",
    "tpmVersion": "String",
    "pcr0": "String",
    "secureBootConfigurationPolicyFingerPrint": "String",
    "codeIntegrityPolicy": "String",
    "bootRevisionListInfo": "String",
    "operatingSystemRevListInfo": "String",
    "healthStatusMismatchInfo": "String",
    "healthAttestationSupportedStatus": "String"
  },
  "subscriberCarrier": "String",
  "meid": "String",
  "totalStorageSpaceInBytes": 1024,
  "freeStorageSpaceInBytes": 1024,
  "managedDeviceName": "String",
  "partnerReportedThreatState": "String",
  "iccid": "String",
  "udid": "String",
  "notes": "String",
  "ethernetMacAddress": "String",
  "physicalMemoryInBytes": 1024
}
```




