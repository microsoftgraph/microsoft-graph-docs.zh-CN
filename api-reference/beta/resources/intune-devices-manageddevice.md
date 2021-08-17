---
title: managedDevice 资源类型
description: 通过 Intune 托管或预注册的设备
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 085d2bd3af9b0a977079359a8c96f4bd29ea46c6
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58262625"
---
# <a name="manageddevice-resource-type"></a>managedDevice 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

通过 Intune 托管或预注册的设备

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[Get managedDevice](../api/intune-devices-manageddevice-get.md)|[managedDevice](../resources/intune-devices-manageddevice.md)|读取 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的属性和关系。|
|[Update managedDevice](../api/intune-devices-manageddevice-update.md)|[managedDevice](../resources/intune-devices-manageddevice.md)|更新 [managedDevice](../resources/intune-devices-manageddevice.md) 对象的属性。|
|[executeAction 操作](../api/intune-devices-manageddevice-executeaction.md)|[bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md)|尚未记录|
|[enableLostMode 操作](../api/intune-devices-manageddevice-enablelostmode.md)|无|启用丢失模式|
|[playLostModeSound 操作](../api/intune-devices-manageddevice-playlostmodesound.md)|无|远程锁定|
|[setDeviceName 操作](../api/intune-devices-manageddevice-setdevicename.md)|无|设置设备的设备名称。|
|[activateDeviceEsim 操作](../api/intune-devices-manageddevice-activatedeviceesim.md)|无|在设备上激活 eSIM。|
|[rotateFileVaultKey 操作](../api/intune-devices-manageddevice-rotatefilevaultkey.md)|无|尚未记录|
|[getFileVaultKey 函数](../api/intune-devices-manageddevice-getfilevaultkey.md)|String|尚未记录|
|[createDeviceLogCollectionRequest 操作](../api/intune-devices-manageddevice-createdevicelogcollectionrequest.md)|[deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)|尚未记录|
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
|[revokeAppleVppLicenses 操作](../api/intune-devices-manageddevice-revokeapplevpplicenses.md)|无|撤销设备的所有 Apple Vpp 许可证|
|[rotateBitLockerKeys 操作](../api/intune-devices-manageddevice-rotatebitlockerkeys.md)|无|旋转 BitLockerKeys|
|[sendCustomNotificationToCompanyPortal 操作](../api/intune-devices-manageddevice-sendcustomnotificationtocompanyportal.md)|无|尚未记录|
|[triggerConfigurationManagerAction 操作](../api/intune-devices-manageddevice-triggerconfigurationmanageraction.md)|无|在 ConfigurationManager 客户端上触发操作|
|[deprovision 操作](../api/intune-devices-manageddevice-deprovision.md)|无|尚未记录|
|[禁用操作](../api/intune-devices-manageddevice-disable.md)|无|尚未记录|
|[可重新enable 操作](../api/intune-devices-manageddevice-reenable.md)|无|尚未记录|
|[moveDevicesToOU 操作](../api/intune-devices-manageddevice-movedevicestoou.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设备的唯一标识符。 此属性是只读的。|
|userId|字符串|与设备关联的用户的唯一标识符。 此属性是只读的。|
|deviceName|String|设备的名称。 此属性是只读的。|
|hardwareInformation|[hardwareInformation](../resources/intune-devices-hardwareinformation.md)|设备的硬向详细信息。  包括存储空间、制造商、序列号等信息。此属性为只读。|
|ownerType|[ownerType](../resources/intune-shared-ownertype.md)|设备的所有权。 可以是"公司"或"个人"。 可取值为：`unknown`、`company`、`personal`。|
|managedDeviceOwnerType|[managedDeviceOwnerType](../resources/intune-shared-manageddeviceownertype.md)|设备的所有权。 可以是"公司"或"个人"。 可取值为：`unknown`、`company`、`personal`。|
|deviceActionResults|[deviceActionResult](../resources/intune-devices-deviceactionresult.md) 集合|ComplexType deviceActionResult 对象的列表。 此属性是只读的。|
|managementState|[managementState](../resources/intune-devices-managementstate.md)|设备的管理状态。 此属性是只读的。 可取值为：`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered`。|
|enrolledDateTime|DateTimeOffset|设备的注册时间。 此属性是只读的。|
|lastSyncDateTime|DateTimeOffset|设备上次成功完成与 Intune 同步的日期和时间。 此属性是只读的。|
|chassisType|[chassisType](../resources/intune-devices-chassistype.md)|设备的机架类型。 此属性是只读的。 可取值为：`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown`。|
|operatingSystem|String|设备的操作系统。 Windows、iOS 等。此属性为只读。|
|deviceType|[deviceType](../resources/intune-devices-devicetype.md)|设备平台。 此属性是只读的。 可能的值是 `desktop` `windowsRT` `winMO6` ：、、、、、、、、、、 `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `chromeOS` `linux` `blackberry` `palm` `unknown` `cloudPC` 、|
|complianceState|[complianceState](../resources/intune-devices-compliancestate.md)|设备的符合性状态。 此属性是只读的。 可取值为：`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager`。|
|jailBroken|String|设备是否已越狱或取得 root 权限。 此属性是只读的。|
|managementAgent|[managementAgentType](../resources/intune-devices-managementagenttype.md)|设备的管理通道。 Intune、EAS 等此属性为只读。 可能的值是 `eas` `mdm` `easMdm` ：、、、、、、、、、、。 `intuneClient` `easIntuneClient` `configurationManagerClient` `configurationManagerClientMdm` `configurationManagerClientMdmEas` `unknown` `jamf` `googleCloudDevicePolicyController` `microsoft365ManagedMdm` `msSense` `intuneAosp`|
|osVersion|String|设备的操作系统版本。 此属性是只读的。|
|easActivated|Boolean|设备是否已激活 Exchange ActiveSync。 此属性是只读的。|
|easDeviceId|String|设备的 Exchange ActiveSync ID。 此属性是只读的。|
|easActivationDateTime|DateTimeOffset|设备的 Exchange ActivationSync 激活时间。 此属性是只读的。|
|aadRegistered|Boolean|设备是否已注册 Azure Active Directory。 此属性是只读的。|
|azureADRegistered|Boolean|设备是否已注册 Azure Active Directory。 此属性是只读的。|
|deviceEnrollmentType|[deviceEnrollmentType](../resources/intune-devices-deviceenrollmenttype.md)|设备的注册类型。 此属性是只读的。 可能的值是 `unknown` `userEnrollment` `deviceEnrollmentManager` ：、、、、、、、、、 `appleBulkWithUser` `appleBulkWithoutUser` `windowsAzureADJoin` `windowsBulkUserless` `windowsAutoEnrollment` `windowsBulkAzureDomainJoin` `windowsCoManagement` `windowsAzureADJoinUsingDeviceAuth` `appleUserEnrollment` `appleUserEnrollmentWithServiceAccount` `azureAdJoinUsingAzureVmExtension` `androidEnterpriseDedicatedDevice` `androidEnterpriseFullyManaged` `androidEnterpriseCorporateWorkProfile` 。|
|lostModeState|[lostModeState](../resources/intune-devices-lostmodestate.md)|指示是启用还是禁用丢失模式。 此属性是只读的。 可取值为：`disabled`、`enabled`。|
|activationLockBypassCode|String|允许绕过设备上的激活锁的代码。 此属性是只读的。|
|emailAddress|String|电子邮件 () 设备关联的用户的邮箱。 此属性是只读的。|
|azureActiveDirectoryDeviceId|String|Azure Active Directory 设备的唯一标识符。 只读。 此属性是只读的。|
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
|retireAfterDateTime|DateTimeOffset|指示设备因计划操作而自动停用的时间。 此属性是只读的。|
|usersLoggedOn|[loggedOnUser](../resources/intune-devices-loggedonuser.md) 集合|指示设备上最后一次登录的用户。 此属性是只读的。|
|preferMdmOverGroupPolicyAppliedDateTime|DateTimeOffset|报告 DateTime 设置了 preferMdmOverGroupPolicy 设置。  设置后，如果存在冲突，Intune MDM 设置将覆盖组策略设置。 只读。 此属性是只读的。|
|autopilotEnrolled|布尔值|报告托管设备是否通过自动试点注册。 此属性是只读的。|
|requireUserEnrollmentApproval|布尔值|报告托管 iOS 设备是否注册用户审批。 此属性是只读的。|
|managementCertificateExpirationDate|DateTimeOffset|报告设备管理证书到期日期。 此属性是只读的。|
|iccid|String|集成的电路卡标识符，它是 SIM 卡的唯一标识号。 此属性是只读的。|
|udid|字符串|iOS 和 macOS 设备的唯一设备标识符。 此属性是只读的。|
|roleScopeTagIds|String collection|此设备实例的范围标记标识列表。|
|windowsActiveMalwareCount|Int32|此 Windows 设备的活动恶意软件计数。 此属性是只读的。|
|windowsRemediatedMalwareCount|Int32|此 Windows 设备的已修复恶意软件计数。 此属性是只读的。|
|notes|String|IT 管理员在设备上创建的备注|
|configurationManagerClientHealthState|[configurationManagerClientHealthState](../resources/intune-devices-configurationmanagerclienthealthstate.md)|配置管理器客户端运行状况状态，仅对 MDM/ConfigMgr 代理管理的设备有效|
|configurationManagerClientInformation|[configurationManagerClientInformation](../resources/intune-devices-configurationmanagerclientinformation.md)|配置管理器客户端信息，仅对 ConfigMgr 代理托管、duel 托管或三管理的设备有效|
|ethernetMacAddress|String|以太网 MAC。 此属性是只读的。|
|physicalMemoryInBytes|Int64|内存总量（以字节为单位）。 此属性是只读的。|
|processorArchitecture|[managedDeviceArchitecture](../resources/intune-devices-manageddevicearchitecture.md)|处理器体系结构。 此属性是只读的。 可取值为：`unknown`、`x86`、`x64`、`arm`、`arM64`。|
|specificationVersion|String|规范版本。 此属性是只读的。|
|joinType|[joinType](../resources/intune-devices-jointype.md)|设备加入类型。 可取值为：`unknown`、`azureADJoined`、`azureADRegistered`、`hybridAzureADJoined`。|
|skuFamily|字符串|设备 sku 系列|
|skuNumber|Int32|设备 sku 号，另请参阅 https://docs.microsoft.com/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo ：。 有效值为 0 到 2147483647。 此属性是只读的。|
|managementFeatures|[managedDeviceManagementFeatures](../resources/intune-devices-manageddevicemanagementfeatures.md)|设备管理功能。 可取值为：`none`、`microsoftManagedDesktop`。|
|chromeOSDeviceInfo|[chromeOSDeviceProperty](../resources/intune-devices-chromeosdeviceproperty.md) 集合|ChromeOS 设备的属性列表。|
|enrollmentProfileName|字符串|分配给设备的注册配置文件的名称。 默认值为空字符串，表示未对注册配置文件进行分页。 此属性是只读的。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|detectedApps|[detectedApp](../resources/intune-devices-detectedapp.md) 集合|设备上当前安装的所有应用程序|
|deviceCategory|[deviceCategory](../resources/intune-shared-devicecategory.md)|设备类别|
|windowsProtectionState|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|设备保护状态。|
|users|[user](../resources/intune-shared-user.md) 集合|与托管设备关联的主要用户。|
|logCollectionRequests|[deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) 集合|日志集合请求列表|

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
    "batterySerialNumber": "String",
    "batteryHealthPercentage": 1024,
    "batteryChargeCycles": 1024,
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
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "String",
    "osBuildNumber": "String",
    "operatingSystemProductType": 1024,
    "ipAddressV4": "String",
    "subnetAddress": "String",
    "esimIdentifier": "String",
    "systemManagementBIOSVersion": "String",
    "tpmManufacturer": "String",
    "tpmVersion": "String"
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
  "retireAfterDateTime": "String (timestamp)",
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
  },
  "configurationManagerClientInformation": {
    "@odata.type": "microsoft.graph.configurationManagerClientInformation",
    "clientIdentifier": "String",
    "isBlocked": true
  },
  "ethernetMacAddress": "String",
  "physicalMemoryInBytes": 1024,
  "processorArchitecture": "String",
  "specificationVersion": "String",
  "joinType": "String",
  "skuFamily": "String",
  "skuNumber": 1024,
  "managementFeatures": "String",
  "chromeOSDeviceInfo": [
    {
      "@odata.type": "microsoft.graph.chromeOSDeviceProperty",
      "name": "String",
      "value": "String",
      "valueType": "String",
      "updatable": true
    }
  ],
  "enrollmentProfileName": "String"
}
```




