# <a name="devicemanagement-resource-type"></a>deviceManagement 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

DeviceManagement 资源表示内容因工作流而异的容器，包括：  

- 审核事件
- 企业条款和条件 
- 公司注册配置文件
- 设备配置设置
- 设备管理
- 端点保护
- 注册配置文件
- 通知
- 员工就职状态策略、设置和详细信息
- 基于角色的访问控制 (RBAC) 策略
- 远程协助合作伙伴
- 电信费用管理合作伙伴
- 事件故障排除
- Windows 信息保护摘要

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 deviceManagement](../api/intune_shared_devicemanagement_get.md)|[deviceManagement](../resources/intune_shared_devicemanagement.md)|读取 [deviceManagement](../resources/intune_shared_devicemanagement.md) 对象的属性和关系。|
|[更新 deviceManagement](../api/intune_shared_devicemanagement_update.md)|[deviceManagement](../resources/intune_shared_devicemanagement.md)|更新 [deviceManagement](../resources/intune_shared_devicemanagement.md) 对象的属性。|
|**加入**|
|[verifyWindowsEnrollmentAutoDiscovery function](../api/intune_shared_devicemanagement_verifywindowsenrollmentautodiscovery.md)|布尔值|尚未记录|
|**RBAC**|
|[getEffectivePermissions 函数](../api/intune_shared_devicemanagement_geteffectivepermissions.md)|[rolePermission](../resources/intune_rbac_rolepermission.md) 集合或字符串集合|检索当前验证的用户的有效权限|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ID|字符串|设备唯一标识符|
|**设备配置**|
|settings|[deviceManagementSettings](../resources/intune_deviceconfig_devicemanagementsettings.md)|帐户级别设置。|
|**设备管理**|
|subscriptionState|字符串|租户移动设备管理订阅状态。 可取值为：`pending`、`active`、`warning`、`disabled`、`deleted`、`blocked`、`lockedOut`。|
|**加入**|
|intuneBrand|[intuneBrand](../resources/intune_onboarding_intunebrand.md)|intuneBrand 包含在自定义公司门户应用程序以及最终用户网页版门户的外观时使用的数据。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|**审核**|
|auditEvents|[auditEvent](../resources/intune_auditing_auditevent.md) 集合|审核事件|
|**企业条款和条件**|
|termsAndConditions|[termsAndConditions](../resources/intune_companyterms_termsandconditions.md) 集合|与公司的设备管理关联的条款和条件。|
|**设备配置**|
|deviceCompliancePolicies|[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) 集合|设备合规性策略。|
|deviceCompliancePolicyDeviceStateSummary|[deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md)|此帐户的设备符合性状态摘要。|
|deviceCompliancePolicySettingStateSummaries|[deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) 集合|此帐户的符合性设置的摘要状态。|
|deviceConfigurationDeviceStateSummaries|[deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md)|此帐户的设备配置设备状态摘要。|
|deviceConfigurations|[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) 集合|设备配置。|
|iosUpdateStatuses|[iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) 集合|此帐户的 IOS 软件更新安装状态。|
|softwareUpdateStatusSummary|[softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md)|软件更新状态摘要。|
|**设备管理**|
|applePushNotificationCertificate|[applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md)|Apple 推送通知证书。|
|detectedApps|[detectedApp](../resources/intune_devices_detectedapp.md) 集合|检测到与设备关联的应用的列表。|
|managedDeviceOverview|[managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md)|设备概述|
|managedDevices|[managedDevice](../resources/intune_devices_manageddevice.md) 集合|托管设备列表。|
|**注册**|
|importedWindowsAutopilotDeviceIdentities|[importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) 集合|导入的 Windows AutoPilot 设备的集合。|
|importedWindowsAutopilotDeviceIdentityUploads|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) 集合|上传 Windows AutoPilot 设备的集合。|
|**通知**|
|notificationMessageTemplates|[notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md) 集合|通知消息模板。|
|**加入**|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)|Exchange 本地条件访问设置。 本地条件访问需要设备注册并符合邮件访问要求|
|deviceCategories|[deviceCategory](../resources/intune_shared_devicecategory.md) 集合|租户的设备类别列表。|
|deviceEnrollmentConfigurations|[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) 集合|设备注册配置列表|
|deviceManagementPartners|[deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) 集合|由租户配置的设备管理合作伙伴列表。|
|exchangeConnectors|[deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) 集合|由租户配置的 Exchange 连接器列表。|
|mobileThreatDefenseConnectors|[mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) 集合|由租户配置的移动威胁防护连接器列表。|
|**RBAC**|
|resourceOperations|[resourceOperation](../resources/intune_rbac_resourceoperation.md) 集合|资源操作。|
|roleAssignments|[deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) 集合|角色分配。|
|roleDefinitions|[roleDefinition](../resources/intune_rbac_roledefinition.md) 集合|角色定义。|
|**远程协助**|
|remoteAssistancePartners|[remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) 集合|远程协助合作伙伴。|
|**电信费用管理**|
|telecomExpenseManagementPartners|[telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) 集合|电信费用管理合作伙伴。|
|**疑难解答**|
|troubleshootingEvents|[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) 集合|租户的故障排除事件列表。|
|**Windows 信息保护**|
|windowsInformationProtectionAppLearningSummaries|[windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) 集合|Windows 信息保护应用学习摘要。|
|windowsInformationProtectionNetworkLearningSummaries|[windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) 集合|Windows 信息保护网络学习摘要。|


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "intuneBrand": {"@odata.type": "microsoft.graph.intuneBrand"},
  "subscriptionState": "String",
  "settings": {"@odata.type": "microsoft.graph.deviceManagementSettings"}
}
```



