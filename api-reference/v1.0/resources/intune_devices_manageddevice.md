# <a name="manageddevice-resource-type"></a>managedDevice 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

通过 Intune 托管或预注册的设备
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List managedDevices](../api/intune_devices_manageddevice_list.md)|[managedDevice](../resources/intune_devices_manageddevice.md) 集合|列出 [managedDevice](../resources/intune_devices_manageddevice.md) 对象的属性和关系。|
|[Get managedDevice](../api/intune_devices_manageddevice_get.md)|[managedDevice](../resources/intune_devices_manageddevice.md)|读取 [managedDevice](../resources/intune_devices_manageddevice.md) 对象的属性和关系。|
|[Create managedDevice](../api/intune_devices_manageddevice_create.md)|[managedDevice](../resources/intune_devices_manageddevice.md)|创建新的 [managedDevice](../resources/intune_devices_manageddevice.md) 对象。|
|[Delete managedDevice](../api/intune_devices_manageddevice_delete.md)|无|删除 [managedDevice](../resources/intune_devices_manageddevice.md)。|
|[Update managedDevice](../api/intune_devices_manageddevice_update.md)|[managedDevice](../resources/intune_devices_manageddevice.md)|更新 [managedDevice](../resources/intune_devices_manageddevice.md) 对象的属性。|
|[retire 操作](../api/intune_devices_manageddevice_retire.md)|无|停用设备|
|[wipe 操作](../api/intune_devices_manageddevice_wipe.md)|无|擦除设备|
|[resetPasscode 操作](../api/intune_devices_manageddevice_resetpasscode.md)|无|重置密码|
|[remoteLock 操作](../api/intune_devices_manageddevice_remotelock.md)|无|远程锁定|
|[requestRemoteAssistance 操作](../api/intune_devices_manageddevice_requestremoteassistance.md)|无|请求远程协助|
|[disableLostMode 操作](../api/intune_devices_manageddevice_disablelostmode.md)|无|禁用丢失模式|
|[locateDevice 操作](../api/intune_devices_manageddevice_locatedevice.md)|无|查找设备|
|[bypassActivationLock 操作](../api/intune_devices_manageddevice_bypassactivationlock.md)|无|跳过激活锁|
|[rebootNow 操作](../api/intune_devices_manageddevice_rebootnow.md)|无|重新启动设备|
|[shutDown 操作](../api/intune_devices_manageddevice_shutdown.md)|无|关闭设备|
|[recoverPasscode 操作](../api/intune_devices_manageddevice_recoverpasscode.md)|无|恢复密码|
|[cleanWindowsDevice 操作](../api/intune_devices_manageddevice_cleanwindowsdevice.md)|无|干净的 Windows 设备|
|[logoutSharedAppleDeviceActiveUser 操作](../api/intune_devices_manageddevice_logoutsharedappledeviceactiveuser.md)|无|注销共享 Apple 设备活动用户|
|[deleteUserFromSharedAppleDevice 操作](../api/intune_devices_manageddevice_deleteuserfromsharedappledevice.md)|无|从共享 Apple 设备中删除用户|
|[syncDevice 操作](../api/intune_devices_manageddevice_syncdevice.md)|无|尚未记录|
|[windowsDefenderScan 操作](../api/intune_devices_manageddevice_windowsdefenderscan.md)|无|尚未记录|
|[windowsDefenderUpdateSignatures 操作](../api/intune_devices_manageddevice_windowsdefenderupdatesignatures.md)|无|尚未记录|
|[updateWindowsDeviceAccount 操作](../api/intune_devices_manageddevice_updatewindowsdeviceaccount.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设备唯一标识符|
|userId|String|与设备关联的用户的唯一标识符|
|deviceName|String|设备的名称|
|managedDeviceOwnerType|[managedDeviceOwnerType](../resources/intune_devices_manageddeviceownertype.md)|设备的所有权。 可以是公司或个人。 可取值为：`unknown`、`company`、`personal`。|
|deviceActionResults|[deviceActionResult](../resources/intune_devices_deviceactionresult.md) 集合|ComplexType deviceActionResult 对象的列表。|
|enrolledDateTime|DateTimeOffset|设备的注册时间。|
|lastSyncDateTime|DateTimeOffset|设备上次成功完成与 Intune 同步的日期和时间。|
|operatingSystem|String|设备的操作系统。 Windows、iOS 等。|
|complianceState|[complianceState](../resources/intune_devices_compliancestate.md)|设备的符合性状态。 可取值为：`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager`。|
|jailBroken|String|设备是否已越狱或取得 root 权限。|
|managementAgent|[managementAgentType](../resources/intune_devices_managementagenttype.md)|设备的管理通道。 Intune、EAS 等 可取值为：`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`。|
|osVersion|String|设备的操作系统版本。|
|easActivated|Boolean|设备是否已激活 Exchange ActiveSync。|
|easDeviceId|String|设备的 Exchange ActiveSync ID。|
|easActivationDateTime|DateTimeOffset|设备的 Exchange ActivationSync 激活时间。|
|azureADRegistered|Boolean|设备是否已注册 Azure Active Directory。|
|deviceEnrollmentType|[deviceEnrollmentType](../resources/intune_devices_deviceenrollmenttype.md)|设备的注册类型。 可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`。|
|activationLockBypassCode|String|允许绕过设备上的激活锁的代码。|
|emailAddress|String|与设备关联的用户的电子邮件。|
|azureADDeviceId|String|Azure Active Directory 设备的唯一标识符。 只读。|
|deviceRegistrationState|[deviceRegistrationState](../resources/intune_devices_deviceregistrationstate.md)|设备注册状态。 可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。|
|deviceCategoryDisplayName|String|设备类别显示名称。|
|isSupervised|Boolean|设备受监督状态|
|exchangeLastSuccessfulSyncDateTime|DateTimeOffset|设备上次与 Exchange 联系的时间。|
|exchangeAccessState|[deviceManagementExchangeAccessState](../resources/intune_devices_devicemanagementexchangeaccessstate.md)|Exchange 中设备的访问状态。 可取值为：`none`、`unknown`、`allowed`、`blocked`、`quarantined`。|
|exchangeAccessStateReason|[deviceManagementExchangeAccessStateReason](../resources/intune_devices_devicemanagementexchangeaccessstatereason.md)|Exchange 中设备访问状态的出现原因。 可取值为：`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp`。|
|remoteAssistanceSessionUrl|String|允许与设备建立远程协助会话的 URL。|
|remoteAssistanceSessionErrorDetails|String|用于在创建远程协助会话对象时识别问题的错误字符串。|
|isEncrypted|Boolean|设备加密状态|
|userPrincipalName|String|设备用户主体名称|
|model|String|设备的型号|
|manufacturer|String|设备的制造商|
|imei|String|IMEI|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|设备符合性宽限期的到期日期/时间|
|serialNumber|String|序列号|
|phoneNumber|String|设备的电话号码|
|androidSecurityPatchLevel|String|Android 安全修补程序级别|
|userDisplayName|String|用户显示名称|
|configurationManagerClientEnabledFeatures|[configurationManagerClientEnabledFeatures](../resources/intune_devices_configurationmanagerclientenabledfeatures.md)|ConfigrMgr 客户端启用的功能|
|wiFiMacAddress|String|Wi-Fi MAC|
|deviceHealthAttestationState|[deviceHealthAttestationState](../resources/intune_devices_devicehealthattestationstate.md)|设备运行状况证明状态。|
|subscriberCarrier|String|订阅者运营商|
|meid|String|MEID|
|totalStorageSpaceInBytes|Int64|存储空间总字节数|
|freeStorageSpaceInBytes|Int64|可用存储空间字节数|
|managedDeviceName|String|用于识别设备的自动生成的名称。 可以覆盖为用户友好名称。|
|partnerReportedThreatState|[managedDevicePartnerReportedHealthState](../resources/intune_devices_manageddevicepartnerreportedhealthstate.md)|指示帐户和设备正在使用移动威胁防护合作伙伴时设备的威胁状态。 只读。 可取值为：`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured`。|

## <a name="relationships"></a>Relationships
|关系|类型|说明|
|:---|:---|:---|
|deviceCategory|[deviceCategory](../resources/intune_shared_devicecategory.md)|设备类别|

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
  "partnerReportedThreatState": "String"
}
```



