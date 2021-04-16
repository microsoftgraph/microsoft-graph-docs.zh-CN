---
title: windowsManagedDevice 资源类型
description: 通过 Intune 托管或预注册的 Windows 设备
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1e66d2daf58d8c659af56dd69a9c41134295cd33
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867621"
---
# <a name="windowsmanageddevice-resource-type"></a>windowsManagedDevice 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

通过 Intune 托管或预注册的 Windows 设备


继承自 [managedDevice](../resources/intune-devices-manageddevice.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsManagedDevices](../api/intune-devices-windowsmanageddevice-list.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) 集合|列出 [windowsManagedDevice 对象的属性和](../resources/intune-devices-windowsmanageddevice.md) 关系。|
|[获取 windowsManagedDevice](../api/intune-devices-windowsmanageddevice-get.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)|读取 [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) 对象的属性和关系。|
|[创建 windowsManagedDevice](../api/intune-devices-windowsmanageddevice-create.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)|创建新的 [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) 对象。|
|[删除 windowsManagedDevice](../api/intune-devices-windowsmanageddevice-delete.md)|无|删除 [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)。|
|[更新 windowsManagedDevice](../api/intune-devices-windowsmanageddevice-update.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)|更新 [windowsManagedDevice 对象](../resources/intune-devices-windowsmanageddevice.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设备的唯一标识符。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|userId|String|与设备关联的用户的唯一标识符。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceName|String|设备的名称。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|hardwareInformation|[hardwareInformation](../resources/intune-devices-hardwareinformation.md)|设备的硬向详细信息。  包括存储空间、制造商、序列号等信息。此属性为只读。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|ownerType|[ownerType](../resources/intune-shared-ownertype.md)|设备的所有权。 可以是"company"或"personal"继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。 可取值为：`unknown`、`company`、`personal`。|
|managedDeviceOwnerType|[managedDeviceOwnerType](../resources/intune-shared-manageddeviceownertype.md)|设备的所有权。 可以是"company"或"personal"继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。 可取值为：`unknown`、`company`、`personal`。|
|deviceActionResults|[deviceActionResult](../resources/intune-devices-deviceactionresult.md) 集合|ComplexType deviceActionResult 对象的列表。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|managementState|[managementState](../resources/intune-devices-managementstate.md)|设备的管理状态。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。 可取值为：`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered`。|
|enrolledDateTime|DateTimeOffset|设备的注册时间。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|lastSyncDateTime|DateTimeOffset|设备上次成功完成与 Intune 同步的日期和时间。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|chassisType|[chassisType](../resources/intune-devices-chassistype.md)|设备的机架类型。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。 可取值为：`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown`。|
|operatingSystem|String|设备的操作系统。 Windows、iOS 等。此属性为只读。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceType|[deviceType](../resources/intune-shared-devicetype.md)|设备平台。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。 可能的值是 `desktop` `windowsRT` `winMO6` ：、、、、、、、、、、 `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `linux` `blackberry` `palm` `unknown` `cloudPC` 、|
|complianceState|[complianceState](../resources/intune-devices-compliancestate.md)|设备的符合性状态。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。 可取值为：`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager`。|
|jailBroken|String|设备是否已越狱或取得 root 权限。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|managementAgent|[managementAgentType](../resources/intune-shared-managementagenttype.md)|设备的管理通道。 Intune、EAS 等此属性为只读。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。 可能的值是：`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`、`microsoft365ManagedMdm`、`msSense`。|
|osVersion|String|设备的操作系统版本。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|easActivated|Boolean|设备是否已激活 Exchange ActiveSync。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|easDeviceId|String|设备的 Exchange ActiveSync ID。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|easActivationDateTime|DateTimeOffset|设备的 Exchange ActivationSync 激活时间。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|aadRegistered|Boolean|设备是否已注册 Azure Active Directory。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|azureADRegistered|Boolean|设备是否已注册 Azure Active Directory。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceEnrollmentType|[deviceEnrollmentType](../resources/intune-shared-deviceenrollmenttype.md)|设备的注册类型。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。 可能的值是 `unknown` `userEnrollment` `deviceEnrollmentManager` ：、、、、、、、、、 `appleBulkWithUser` `appleBulkWithoutUser` `windowsAzureADJoin` `windowsBulkUserless` `windowsAutoEnrollment` `windowsBulkAzureDomainJoin` `windowsCoManagement` `windowsAzureADJoinUsingDeviceAuth` `appleUserEnrollment` `appleUserEnrollmentWithServiceAccount` `azureAdJoinUsingAzureVmExtension` `androidEnterpriseDedicatedDevice` `androidEnterpriseFullyManaged` `androidEnterpriseCorporateWorkProfile` 。|
|lostModeState|[lostModeState](../resources/intune-devices-lostmodestate.md)|指示是启用还是禁用丢失模式。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。 可取值为：`disabled`、`enabled`。|
|activationLockBypassCode|String|允许绕过设备上的激活锁的代码。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|emailAddress|String|电子邮件 () 设备关联的用户的邮箱。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|azureActiveDirectoryDeviceId|String|Azure Active Directory 设备的唯一标识符。 只读。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|azureADDeviceId|String|Azure Active Directory 设备的唯一标识符。 只读。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceRegistrationState|[deviceRegistrationState](../resources/intune-devices-deviceregistrationstate.md)|设备注册状态。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。 可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。|
|deviceCategoryDisplayName|String|设备类别显示名称。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|isSupervised|Boolean|设备监督状态。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|exchangeLastSuccessfulSyncDateTime|DateTimeOffset|设备上次与 Exchange 联系的时间。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|exchangeAccessState|[deviceManagementExchangeAccessState](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|Exchange 中设备的访问状态。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。 可取值为：`none`、`unknown`、`allowed`、`blocked`、`quarantined`。|
|exchangeAccessStateReason|[deviceManagementExchangeAccessStateReason](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|Exchange 中设备访问状态的出现原因。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。 可取值为：`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp`。|
|remoteAssistanceSessionUrl|String|允许与设备建立远程协助会话的 URL。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|remoteAssistanceSessionErrorDetails|String|用于在创建远程协助会话对象时识别问题的错误字符串。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|isEncrypted|Boolean|设备加密状态。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|userPrincipalName|String|设备用户主体名称。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|model|String|设备型号。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|manufacturer|String|设备的制造商。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|imei|String|IMEI。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|设备合规性宽限期到期的 DateTime。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|serialNumber|String|SerialNumber。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|phoneNumber|String|设备的电话号码。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|androidSecurityPatchLevel|String|Android 安全修补程序级别。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|userDisplayName|String|用户显示名称。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|configurationManagerClientEnabledFeatures|[configurationManagerClientEnabledFeatures](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|ConfigrMgr 客户端启用的功能。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|wiFiMacAddress|String|Wi-Fi MAC。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceHealthAttestationState|[deviceHealthAttestationState](../resources/intune-devices-devicehealthattestationstate.md)|设备运行状况证明状态。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|subscriberCarrier|String|订阅者运营商。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|meid|String|MEID。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|totalStorageSpaceInBytes|Int64|总存储（以字节为单位）。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|freeStorageSpaceInBytes|Int64|可用存储空间（以字节为单位）。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|managedDeviceName|String|用于识别设备的自动生成的名称。 可以覆盖为用户友好名称。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|partnerReportedThreatState|[managedDevicePartnerReportedHealthState](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|指示帐户和设备正在使用移动威胁防护合作伙伴时设备的威胁状态。 只读。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。 可取值为：`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured`。|
|retireAfterDateTime|DateTimeOffset|指示设备因计划操作而自动停用的时间。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|usersLoggedOn|[loggedOnUser](../resources/intune-devices-loggedonuser.md) 集合|指示设备上最后一次登录的用户。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|preferMdmOverGroupPolicyAppliedDateTime|DateTimeOffset|报告 DateTime 设置了 preferMdmOverGroupPolicy 设置。  设置后，如果存在冲突，Intune MDM 设置将覆盖组策略设置。 只读。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|autopilotEnrolled|Boolean|报告托管设备是否通过自动试点注册。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|requireUserEnrollmentApproval|Boolean|报告托管 iOS 设备是否注册用户审批。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|managementCertificateExpirationDate|DateTimeOffset|报告设备管理证书到期日期。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|iccid|String|集成的电路卡标识符，它是 SIM 卡的唯一标识号。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|udid|String|iOS 和 macOS 设备的唯一设备标识符。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|roleScopeTagIds|String 集合|此设备实例的范围标记标识列表。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|windowsActiveMalwareCount|Int32|此 Windows 设备的活动恶意软件计数。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|windowsRemediatedMalwareCount|Int32|此 Windows 设备的已修复恶意软件计数。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|notes|String|由 IT 管理员创建的设备的备注 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|configurationManagerClientHealthState|[configurationManagerClientHealthState](../resources/intune-devices-configurationmanagerclienthealthstate.md)|配置管理器客户端运行状况状态，仅对 MDM/ConfigMgr 代理管理的设备有效。继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|configurationManagerClientInformation|[configurationManagerClientInformation](../resources/intune-devices-configurationmanagerclientinformation.md)|配置管理器客户端信息，仅对由 ConfigMgr 代理托管、duel 托管或三管理的设备有效。继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|ethernetMacAddress|String|以太网 MAC。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|physicalMemoryInBytes|Int64|内存总量（以字节为单位）。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|processorArchitecture|[managedDeviceArchitecture](../resources/intune-devices-manageddevicearchitecture.md)|处理器体系结构。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。 可取值为：`unknown`、`x86`、`x64`、`arm`、`arM64`。|
|specificationVersion|String|规范版本。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|joinType|[joinType](../resources/intune-devices-jointype.md)|设备加入类型 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。 可取值为：`unknown`、`azureADJoined`、`azureADRegistered`、`hybridAzureADJoined`。|
|skuFamily|String|设备 sku 系列 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|skuNumber|Int32|设备 sku 号，另请参阅 https://docs.microsoft.com/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo ：。 有效值为 0 到 2147483647。 此属性是只读的。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|managementFeatures|[managedDeviceManagementFeatures](../resources/intune-devices-manageddevicemanagementfeatures.md)|设备管理功能 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)。 可取值为：`none`、`microsoftManagedDesktop`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|detectedApps|[detectedApp](../resources/intune-devices-detectedapp.md) 集合|设备上当前安装的所有应用程序 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceCategory|[deviceCategory](../resources/intune-shared-devicecategory.md)|设备类别 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|windowsProtectionState|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|设备保护状态。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|users|[user](../resources/intune-shared-user.md) 集合|与托管设备关联的主要用户。 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|
|logCollectionRequests|[deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) 集合|日志集合请求列表 继承自 [managedDevice](../resources/intune-devices-manageddevice.md)|

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
  "managementFeatures": "String"
}
```




