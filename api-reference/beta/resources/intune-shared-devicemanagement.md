---
title: deviceManagement 资源类型
description: 'DeviceManagement 资源表示的容器其内容因工作流，包括：  '
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: a2f4348da007a3d69d1618151718789d1b72e3e1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961335"
---
# <a name="devicemanagement-resource-type"></a>deviceManagement 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

DeviceManagement 资源表示的容器其内容因工作流，包括：  

- Android for Work 设置
- 审核事件
- 企业条款和条件 
- 公司注册配置文件
- 设备配置设置
- 设备管理
- 电子 SIM (ESIM)
- 防御
- 通知
- 入职培训策略、 设置和详细信息
- 远程访问
- 远程协助合作伙伴
- 基于角色的访问控制 (RBAC) 策略
- 电信广度，管理合作伙伴
- 事件的故障排除
- Windows 信息保护摘要

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 deviceManagement](../api/intune-shared-devicemanagement-get.md)|读取 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的属性和关系。|
|[更新 deviceManagement](../api/intune-shared-devicemanagement-update.md)|更新 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的属性。|
|**设备配置**|
|[enableLegacyPcManagement 操作](../api/intune-shared-devicemanagement-enablelegacypcmanagement.md)|无|尚未记录|
|**设备管理**|
|[sendCustomNotificationToCompanyPortal 操作](../api/intune-shared-devicemanagement-sendcustomnotificationtocompanyportal.md)|无|尚未记录|
|**入职培训**|
|[verifyWindowsEnrollmentAutoDiscovery function](../api/intune-shared-devicemanagement-verifywindowsenrollmentautodiscovery.md)|布尔值|尚未记录|
|**基于角色的访问控制 (RBAC)**|
|[getEffectivePermissions 函数](../api/intune-shared-devicemanagement-geteffectivepermissions.md)|[rolePermission](../resources/intune-rbac-rolepermission.md) 集合|检索当前验证的用户的有效权限|
|[getRoleScopeTagsByIds 函数](../api/intune-shared-devicemanagement-getrolescopetagsbyids.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)集合|尚未记录|
|[getRoleScopeTagsByResource 函数](../api/intune-shared-devicemanagement-getrolescopetagsbyresource.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)集合|尚未记录|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|与设备关联的唯一标识符。|
|**设备配置**|
|intuneAccountId|Guid|Intune 帐户 ID 给定租户|
|legacyPcManangementEnabled|Boolean|若要启用非 MDM 属性托管旧 PC 管理此帐户。 此属性是只读的。|
|maximumDepTokens|Int32|允许每个租户的 DEP 令牌的最大数量。|
|settings|[deviceManagementSettings](../resources/intune-deviceconfig-devicemanagementsettings.md)|帐户级别设置。|
|**设备管理**|
|accountMoveCompletionDateTime|DateTimeOffset|日期 & 时间时 scaleunits 之间移动租户数据。|
|adminConsent|[adminConsent](../resources/intune-devices-adminconsent.md)|管理许可信息。|
|deviceProtectionOverview|[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md)|设备 protection overview。|
|managedDeviceCleanupSettings|[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md)|设备清理规则|
|subscriptionState|[deviceManagementSubscriptionState](../resources/intune-devices-devicemanagementsubscriptionstate.md)|租户移动设备管理订阅状态。 可取值为：`pending`、`active`、`warning`、`disabled`、`deleted`、`blocked`、`lockedOut`。|
|订阅|[deviceManagementSubscriptions](../resources/intune-devices-devicemanagementsubscriptions.md)|租户的订阅。 可取值为：`none`、`intune`、`office365`、`intunePremium`、`intune_EDU`、`intune_SMB`。|
|windowsMalwareOverview|[windowsMalwareOverview](../resources/intune-devices-windowsmalwareoverview.md)|恶意软件 overview for windows 设备。|
|**入职培训**|
|intuneBrand|[intuneBrand](../resources/intune-onboarding-intunebrand.md)|intuneBrand 包含在自定义公司门户应用程序以及最终用户网页版门户的外观时使用的数据。|

## <a name="relationships"></a>关系
|关系|类型|说明&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|
|:---|:---|:---|
|**用于 android**|
|androidDeviceOwnerEnrollmentProfiles|[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)集合|Android 设备所有者注册配置文件实体。|
|androidForWorkAppConfigurationSchemas|[androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 集合|Android for Work 应用配置架构实体。|
|androidForWorkEnrollmentProfiles|[androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) 集合|Android for Work 注册配置文件实体。|
|androidForWorkSettings|[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)|Android for Work 设置单例实体。|
|androidManagedStoreAccountEnterpriseSettings|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)|Android 托管 singleton 存储帐户企业设置实体。|
|androidManagedStoreAppConfigurationSchemas|[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)集合|Android 企业应用程序配置架构实体。|
|**审核**|
|auditEvents|[auditEvent](../resources/intune-auditing-auditevent.md) 集合|审核事件|
|**公司术语**|
|termsAndConditions|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 集合|与公司的设备管理关联的条款和条件。|
|**公司注册**|
|enrollmentProfiles|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)集合|注册配置文件。|
|importedAppleDeviceIdentities|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)集合|导入的 Apple 设备标识。|
|importedDeviceIdentities|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)集合|导入的设备标识。|
|**设备配置**|
|advancedThreatProtectionOnboardingStateSummary|[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|此帐户 ATP 入职培训状态摘要状态。|
|cartToClassAssociations|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)集合|类关联到购物车。|
|deviceCompliancePolicies|[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 集合|设备符合性策略。|
|deviceCompliancePolicyDeviceStateSummary|[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|此帐户的设备符合性状态摘要。|
|deviceCompliancePolicySettingStateSummaries|[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 集合|此帐户的符合性设置的摘要状态。|
|deviceConfigurationConflictSummary|[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)集合|此帐户的冲突状态中的策略的摘要。|
|deviceConfigurationDeviceStateSummaries|[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|此帐户的设备配置设备状态摘要。|
|deviceConfigurationRestrictedAppsViolations|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)集合|限制为此帐户的应用程序冲突。|
|deviceConfigurations|[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) 集合|设备配置。|
|deviceConfigurationUserStateSummaries|[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)|设备配置用户状态为此帐户摘要。|
|iosUpdateStatuses|[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) 集合|此帐户的 IOS 软件更新安装状态。|
|ndesConnectors|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)集合|此帐户 Ndes 连接器的集合。|
|softwareUpdateStatusSummary|[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|软件更新状态摘要。|
|**设备管理**|
|applePushNotificationCertificate|[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)|Apple 推送通知证书。|
|dataSharingConsents|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)集合|数据共享同意。|
|detectedApps|[detectedApp](../resources/intune-devices-detectedapp.md) 集合|检测到与设备关联的应用的列表。|
|deviceManagementScripts|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)集合|设备管理脚本租户相关联的列表。|
|managedDeviceOverview|[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)|设备概述|
|managedDevices|[managedDevice](../resources/intune-devices-manageddevice.md) 集合|托管设备列表。|
|remoteActionAudits|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)集合|使用租户审核的设备远程操作的列表。|
|windowsMalwareInformation|[windowsMalwareInformation](../resources/intune-devices-windowsmalwareinformation.md)集合|受影响的恶意软件为租户中的列表。|
|**注册**|
|depOnboardingSettings|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)集合|多个 DEP 标记每个租户的此集合。|
|importedDeviceIdentities|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)集合|导入的设备标识。|
|importedWindowsAutopilotDeviceIdentities|[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 集合|导入的 Windows AutoPilot 设备的集合。|
|importedWindowsAutopilotDeviceIdentityUploads|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)集合|Windows 自动执行某些操作设备上载的集合。|
|windowsAutopilotDeploymentProfiles|[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)集合|Windows 自动试点部署配置文件|
|windowsAutopilotDeviceIdentities|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)集合|Windows 自动执行某些操作设备标识包含集合。|
|windowsAutopilotSettings|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|Windows 自动执行某些操作帐户设置。|
|**嵌入的 SIM**|
|embeddedSIMActivationCodePools|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)集合|嵌入的 SIM 激活代码池创建的此帐户。|
|**防御**|
|managementConditions|[managementCondition](../resources/intune-fencing-managementcondition.md)集合|与公司的设备管理相关的管理条件。|
|managementConditionStatements|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)集合|设备管理的公司相关联的管理条件语句。|
|**通知**|
|notificationMessageTemplates|[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 集合|通知消息模板。|
|**入职培训**|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|Exchange 本地条件访问设置。 本地条件访问需要设备注册并符合邮件访问要求|
|deviceCategories|[deviceCategory](../resources/intune-shared-devicecategory.md) 集合|租户的设备类别列表。|
|deviceEnrollmentConfigurations|[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) 集合|设备注册配置列表|
|deviceManagementPartners|[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 集合|由租户配置的设备管理合作伙伴列表。|
|exchangeConnectors|[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 集合|由租户配置的 Exchange 连接器列表。|
|exchangeOnPremisesPolicies|[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)集合|由租户配置 Exchange 上 Premisis 策略的列表。|
|exchangeOnPremisesPolicy|[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|用于控制对本地 Exchange 的移动设备访问策略|
|mobileThreatDefenseConnectors|[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 集合|由租户配置的移动威胁防护连接器列表。|
|**远程访问**|
|userPfxCertificates|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)集合|PFX 证书与用户关联的集合。|
|**远程协助**|
|remoteAssistancePartners|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 集合|远程帮助合作伙伴。|
|**基于角色的访问控制 (RBAC)**|
|resourceOperations|[resourceOperation](../resources/intune-rbac-resourceoperation.md) 集合|资源操作。|
|roleAssignments|[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 集合|角色分配。|
|roleDefinitions|[roleDefinition](../resources/intune-rbac-roledefinition.md) 集合|角色定义。|
|roleScopeTags|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)集合|角色作用域标记。|
|**电信支出管理 （项目）**|
|telecomExpenseManagementPartners|[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 集合|电信费用管理合作伙伴。|
|**问题排查**|
|troubleshootingEvents|[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 集合|租户的故障排除事件列表。|
|**Windows 信息保护**|
|intuneBrandingProfiles|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)集合|Intune 品牌目标设定为 AAD 组配置文件|
|windowsInformationProtectionAppLearningSummaries|[windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 集合|Windows 信息保护应用学习摘要。|
|windowsInformationProtectionNetworkLearningSummaries|[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 集合|Windows 信息保护网络学习摘要。|


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "subscriptionState": "String"
}
```



