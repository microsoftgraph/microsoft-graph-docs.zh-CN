---
title: windowsManagedDevice 资源类型
description: 通过 Intune 管理或预注册的 Windows 设备
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e217dc423000850be1f2da6eed8c771813e3c6d3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562739"
---
# <a name="windowsmanageddevice-resource-type"></a>windowsManagedDevice 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

通过 Intune 管理或预注册的 Windows 设备


继承自[managedDevice](../resources/intune-devices-manageddevice.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsManagedDevices](../api/intune-devices-windowsmanageddevice-list.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)集合|列出[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)对象的属性和关系。|
|[获取 windowsManagedDevice](../api/intune-devices-windowsmanageddevice-get.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)|读取[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)对象的属性和关系。|
|[创建 windowsManagedDevice](../api/intune-devices-windowsmanageddevice-create.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)|创建新的[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)对象。|
|[删除 windowsManagedDevice](../api/intune-devices-windowsmanageddevice-delete.md)|无|删除[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)。|
|[更新 windowsManagedDevice](../api/intune-devices-windowsmanageddevice-update.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)|更新[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|继承自[managedDevice](../resources/intune-devices-manageddevice.md)的设备的唯一标识符|
|userId|String|与继承自[managedDevice](../resources/intune-devices-manageddevice.md)的设备关联的用户的唯一标识符|
|deviceName|String|继承自[managedDevice](../resources/intune-devices-manageddevice.md)的设备的名称|
|hardwareInformation|[hardwareInformation](../resources/intune-devices-hardwareinformation.md)|设备的 hardward 详细信息。  包括存储空间、制造商、序列号等信息。继承自[managedDevice](../resources/intune-devices-manageddevice.md)|
|所有者|[所有者](../resources/intune-devices-ownertype.md)|设备的所有权。 可以是从[managedDevice](../resources/intune-devices-manageddevice.md)继承的 "公司" 或 "个人"。 可取值为：`unknown`、`company`、`personal`。|
|managedDeviceOwnerType|[managedDeviceOwnerType](../resources/intune-devices-manageddeviceownertype.md)|设备的所有权。 可以是从[managedDevice](../resources/intune-devices-manageddevice.md)继承的 "公司" 或 "个人"。 可取值为：`unknown`、`company`、`personal`。|
|deviceActionResults|[deviceActionResult](../resources/intune-devices-deviceactionresult.md) 集合|ComplexType deviceActionResult 对象的列表。 继承自[managedDevice](../resources/intune-devices-manageddevice.md)|
|managementState|[managementState](../resources/intune-devices-managementstate.md)|设备的管理状态。 继承自[managedDevice](../resources/intune-devices-manageddevice.md)。 可取值为：`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered`。|
|enrolledDateTime|DateTimeOffset|设备的注册时间。 继承自[managedDevice](../resources/intune-devices-manageddevice.md)|
|lastSyncDateTime|DateTimeOffset|设备上次成功完成与 Intune 同步的日期和时间。 继承自[managedDevice](../resources/intune-devices-manageddevice.md)|
|chassisType|[chassisType](../resources/intune-devices-chassistype.md)|设备的机箱类型。 继承自[managedDevice](../resources/intune-devices-manageddevice.md)。 可取值为：`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown`。|
|operatingSystem|String|设备的操作系统。 Windows、iOS 等。继承自[managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceType|[deviceType](../resources/intune-shared-devicetype.md)|设备的平台。 继承自[managedDevice](../resources/intune-devices-manageddevice.md)。 可能的值为`desktop`: `windowsRT`、 `winMO6`、 `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer`、、、、、、、、、、、、、、、、 `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.|
|complianceState|[complianceState](../resources/intune-devices-compliancestate.md)|设备的符合性状态。 继承自[managedDevice](../resources/intune-devices-manageddevice.md)。 可取值为：`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager`。|
|jailBroken|String|设备是否已越狱或取得 root 权限。 继承自[managedDevice](../resources/intune-devices-manageddevice.md)|
|managementAgent|[managementAgentType](../resources/intune-devices-managementagenttype.md)|设备的管理通道。 Intune、EAS 等。继承自[managedDevice](../resources/intune-devices-manageddevice.md)。 可取值为：`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`、`microsoft365ManagedMdm`。|
|osVersion|String|设备的操作系统版本。 继承自[managedDevice](../resources/intune-devices-manageddevice.md)|
|easActivated|Boolean|设备是否已激活 Exchange ActiveSync。 继承自[managedDevice](../resources/intune-devices-manageddevice.md)|
|easDeviceId|String|设备的 Exchange ActiveSync ID。 继承自[managedDevice](../resources/intune-devices-manageddevice.md)|
|easActivationDateTime|DateTimeOffset|设备的 Exchange ActivationSync 激活时间。 继承自[managedDevice](../resources/intune-devices-manageddevice.md)|
|aadRegistered|Boolean|设备是否已注册 Azure Active Directory。 继承自[managedDevice](../resources/intune-devices-manageddevice.md)|
|azureADRegistered|Boolean|设备是否已注册 Azure Active Directory。 继承自[managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceEnrollmentType|[deviceEnrollmentType](../resources/intune-shared-deviceenrollmenttype.md)|设备的注册类型。 继承自[managedDevice](../resources/intune-devices-manageddevice.md)。 可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`。|
|lostModeState|[lostModeState](../resources/intune-devices-lostmodestate.md)|指示是否已启用或禁用从[managedDevice](../resources/intune-devices-manageddevice.md)继承的已丢失模式。 可取值为：`disabled`、`enabled`。|
|activationLockBypassCode|String|允许绕过设备上的激活锁的代码。 继承自[managedDevice](../resources/intune-devices-manageddevice.md)|
|emailAddress|String|与从[managedDevice](../resources/intune-devices-manageddevice.md)继承的设备关联的用户的电子邮件|
|azureActiveDirectoryDeviceId|String|Azure Active Directory 设备的唯一标识符。 只读。 继承自[managedDevice](../resources/intune-devices-manageddevice.md)|
|azureADDeviceId|String|Azure Active Directory 设备的唯一标识符。 只读。 继承自[managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceRegistrationState|[deviceRegistrationState](../resources/intune-devices-deviceregistrationstate.md)|设备注册状态。 继承自[managedDevice](../resources/intune-devices-manageddevice.md)。 可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。|
|deviceCategoryDisplayName|String|继承自[managedDevice](../resources/intune-devices-manageddevice.md)的设备类别显示名称|
|isSupervised|Boolean|从[managedDevice](../resources/intune-devices-manageddevice.md)继承的设备监督状态|
|exchangeLastSuccessfulSyncDateTime|DateTimeOffset|设备上次与 Exchange 联系的时间。 继承自[managedDevice](../resources/intune-devices-manageddevice.md)|
|exchangeAccessState|[deviceManagementExchangeAccessState](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|Exchange 中设备的访问状态。 继承自[managedDevice](../resources/intune-devices-manageddevice.md)。 可取值为：`none`、`unknown`、`allowed`、`blocked`、`quarantined`。|
|exchangeAccessStateReason|[deviceManagementExchangeAccessStateReason](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|Exchange 中设备访问状态的出现原因。 继承自[managedDevice](../resources/intune-devices-manageddevice.md)。 可取值为：`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp`。|
|remoteAssistanceSessionUrl|String|允许与设备建立远程协助会话的 URL。 继承自[managedDevice](../resources/intune-devices-manageddevice.md)|
|remoteAssistanceSessionErrorDetails|String|用于在创建远程协助会话对象时识别问题的错误字符串。 继承自[managedDevice](../resources/intune-devices-manageddevice.md)|
|isEncrypted|Boolean|从[managedDevice](../resources/intune-devices-manageddevice.md)继承的设备加密状态|
|userPrincipalName|String|从[managedDevice](../resources/intune-devices-manageddevice.md)继承的设备用户主体名称|
|model|String|继承自[managedDevice](../resources/intune-devices-manageddevice.md)的设备的模型|
|manufacturer|String|继承自[managedDevice](../resources/intune-devices-manageddevice.md)的设备的制造商|
|imei|String|从[managedDevice](../resources/intune-devices-manageddevice.md)继承的 IMEI|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|设备符合性宽限期过期时间从[managedDevice](../resources/intune-devices-manageddevice.md)继承的日期/时间|
|serialNumber|字符串|SerialNumber 继承自[managedDevice](../resources/intune-devices-manageddevice.md)|
|phoneNumber|String|继承自[managedDevice](../resources/intune-devices-manageddevice.md)的设备的电话号码|
|androidSecurityPatchLevel|String|从[managedDevice](../resources/intune-devices-manageddevice.md)继承的 Android 安全修补程序级别|
|userDisplayName|String|从[managedDevice](../resources/intune-devices-manageddevice.md)继承的用户显示名称|
|configurationManagerClientEnabledFeatures|[configurationManagerClientEnabledFeatures](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|继承自[managedDevice](../resources/intune-devices-manageddevice.md)的 ConfigrMgr 客户端启用的功能|
|wiFiMacAddress|String|从[managedDevice](../resources/intune-devices-manageddevice.md)继承的 wi-fi MAC|
|deviceHealthAttestationState|[deviceHealthAttestationState](../resources/intune-devices-devicehealthattestationstate.md)|设备运行状况证明状态。 继承自[managedDevice](../resources/intune-devices-manageddevice.md)|
|subscriberCarrier|String|从[managedDevice](../resources/intune-devices-manageddevice.md)继承的订阅者运营商|
|meid|String|MEID 继承自[managedDevice](../resources/intune-devices-manageddevice.md)|
|totalStorageSpaceInBytes|Int64|从[managedDevice](../resources/intune-devices-manageddevice.md)继承的总存储量 (以字节为单位)|
|freeStorageSpaceInBytes|Int64|从[managedDevice](../resources/intune-devices-manageddevice.md)继承的可用存储量 (以字节为单位)|
|managedDeviceName|String|用于识别设备的自动生成的名称。 可以覆盖为用户友好名称。 继承自[managedDevice](../resources/intune-devices-manageddevice.md)|
|partnerReportedThreatState|[managedDevicePartnerReportedHealthState](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|指示帐户和设备正在使用移动威胁防护合作伙伴时设备的威胁状态。 只读。 继承自[managedDevice](../resources/intune-devices-manageddevice.md)。 可取值为：`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured`。|
|usersLoggedOn|[loggedOnUser](../resources/intune-devices-loggedonuser.md)集合|指示从[managedDevice](../resources/intune-devices-manageddevice.md)继承的设备的上次登录用户|
|preferMdmOverGroupPolicyAppliedDateTime|DateTimeOffset|报告设置了 preferMdmOverGroupPolicy 设置的 DateTime。  设置后, 如果存在冲突, Intune MDM 设置将覆盖组策略设置。 只读。 继承自[managedDevice](../resources/intune-devices-manageddevice.md)|
|autopilotEnrolled|Boolean|如果托管设备是通过自动引导注册的, 则报告。 继承自[managedDevice](../resources/intune-devices-manageddevice.md)|
|requireUserEnrollmentApproval|Boolean|如果托管 iOS 设备是用户审批注册, 则报告。 继承自[managedDevice](../resources/intune-devices-manageddevice.md)|
|managementCertificateExpirationDate|DateTimeOffset|报告设备管理证书到期日期继承自[managedDevice](../resources/intune-devices-manageddevice.md)|
|iccid|String|集成的电路卡标识符, 它是 SIM 卡的唯一标识号。 继承自[managedDevice](../resources/intune-devices-manageddevice.md)|
|udid|String|iOS 和 macOS 设备的唯一设备标识符。 继承自[managedDevice](../resources/intune-devices-manageddevice.md)|
|roleScopeTagIds|String collection|此设备实例的范围标记 id 的列表。 继承自[managedDevice](../resources/intune-devices-manageddevice.md)|
|windowsActiveMalwareCount|Int32|从[managedDevice](../resources/intune-devices-manageddevice.md)继承的此 windows 设备的活动恶意软件的计数|
|windowsRemediatedMalwareCount|Int32|从[managedDevice](../resources/intune-devices-manageddevice.md)继承的此 windows 设备的修正的恶意软件的计数|
|notes|String|由 IT 管理员创建的设备上的注释继承自[managedDevice](../resources/intune-devices-manageddevice.md)|
|configurationManagerClientHealthState|[configurationManagerClientHealthState](../resources/intune-devices-configurationmanagerclienthealthstate.md)|Configuration manager 客户端运行状况状态, 仅适用于从[managedDevice](../resources/intune-devices-manageddevice.md)继承的 MDM/ConfigMgr 代理所管理的设备|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|detectedApps|[detectedApp](../resources/intune-devices-detectedapp.md) 集合|从[managedDevice](../resources/intune-devices-manageddevice.md)继承的设备上当前安装的所有应用程序|
|deviceCategory|[deviceCategory](../resources/intune-shared-devicecategory.md)|继承自[managedDevice](../resources/intune-devices-manageddevice.md)的设备类别|
|windowsProtectionState|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|设备保护状态。 继承自[managedDevice](../resources/intune-devices-manageddevice.md)|
|users|[user](../resources/intune-shared-user.md) 集合|与托管设备关联的主要用户。 继承自[managedDevice](../resources/intune-devices-manageddevice.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagedDevice",
  "id": "String (identifier)",
  "userId": "String",
  "deviceName": "String",
  "hardwareInformation": {
    "@odata.type": "microsoft.graph.hardwareInformation",
    "serialNumber": "String",
    "totalStorageSpace": 1024,
    "freeStorageSpace": 1024,
    "imei": "String",
    "meid": "String",
    "manufacturer": "String",
    "model": "String",
    "phoneNumber": "String",
    "subscriberCarrier": "String",
    "cellularTechnology": "String",
    "wifiMac": "String",
    "operatingSystemLanguage": "String",
    "isSupervised": true,
    "isEncrypted": true,
    "isSharedDevice": true,
    "sharedDeviceCachedUsers": [
      {
        "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
        "userPrincipalName": "String",
        "dataToSync": true,
        "dataQuota": 1024,
        "dataUsed": 1024
      }
    ],
    "tpmSpecificationVersion": "String",
    "operatingSystemEdition": "String",
    "deviceFullQualifiedDomainName": "String",
    "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "String",
    "deviceGuardVirtualizationBasedSecurityState": "String",
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "String"
  },
  "ownerType": "String",
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
  "managementState": "String",
  "enrolledDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "chassisType": "String",
  "operatingSystem": "String",
  "deviceType": "String",
  "complianceState": "String",
  "jailBroken": "String",
  "managementAgent": "String",
  "osVersion": "String",
  "easActivated": true,
  "easDeviceId": "String",
  "easActivationDateTime": "String (timestamp)",
  "aadRegistered": true,
  "azureADRegistered": true,
  "deviceEnrollmentType": "String",
  "lostModeState": "String",
  "activationLockBypassCode": "String",
  "emailAddress": "String",
  "azureActiveDirectoryDeviceId": "String",
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
    "windowsUpdateForBusiness": true,
    "endpointProtection": true,
    "officeApps": true
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
  "usersLoggedOn": [
    {
      "@odata.type": "microsoft.graph.loggedOnUser",
      "userId": "String",
      "lastLogOnDateTime": "String (timestamp)"
    }
  ],
  "preferMdmOverGroupPolicyAppliedDateTime": "String (timestamp)",
  "autopilotEnrolled": true,
  "requireUserEnrollmentApproval": true,
  "managementCertificateExpirationDate": "String (timestamp)",
  "iccid": "String",
  "udid": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "windowsActiveMalwareCount": 1024,
  "windowsRemediatedMalwareCount": 1024,
  "notes": "String",
  "configurationManagerClientHealthState": {
    "@odata.type": "microsoft.graph.configurationManagerClientHealthState",
    "state": "String",
    "errorCode": 1024,
    "lastSyncDateTime": "String (timestamp)"
  }
}
```





