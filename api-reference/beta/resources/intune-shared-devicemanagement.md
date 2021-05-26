---
title: deviceManagement 资源类型
description: 'deviceManagement 资源表示其内容因工作流而异的容器，包括：  '
localization_priority: Normal
author: rolyon
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1423a165bb66e89dbb67b40aa97c2d1dddb395b7
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665565"
---
# <a name="devicemanagement-resource-type"></a>deviceManagement 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

deviceManagement 资源表示其内容因工作流而异的容器，包括：  

- Android for Work 设置
- 审核事件
- 公司条款和条件 
- 公司注册配置文件
- 设备配置设置
- 设备意图设置
- 设备管理
- ESIM (ESIM) 
- Fencing
- 组策略分析
- 通知
- 载入策略、设置和详细信息
- 策略集
- 资源访问策略
- 远程访问
- 远程协助合作伙伴
- 基于角色的访问控制 (RBAC) 策略
- Reporting
- 电信业务管理合作伙伴
- 事件疑难解答
- Windows信息保护摘要

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 deviceManagement](../api/intune-shared-devicemanagement-get.md)|读取 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的属性和关系。|
|[更新 deviceManagement](../api/intune-shared-devicemanagement-update.md)|更新 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的属性。|
|**设备配置**|
|[enableLegacyPcManagement 操作](../api/intune-shared-devicemanagement-enablelegacypcmanagement.md)|无|尚未记录|
|**设备管理**|
|[sendCustomNotificationToCompanyPortal 操作](../api/intune-shared-devicemanagement-sendcustomnotificationtocompanyportal.md)|无|尚未记录|
|**载入**|
|[verifyWindowsEnrollmentAutoDiscovery function](../api/intune-shared-devicemanagement-verifywindowsenrollmentautodiscovery.md)|布尔值|尚未记录|
|**基于角色的访问控制 (RBAC)**|
|[getEffectivePermissions 函数](../api/intune-shared-devicemanagement-geteffectivepermissions.md)|[rolePermission](../resources/intune-rbac-rolepermission.md) 集合|检索当前验证的用户的有效权限|
|[getRoleScopeTagsByIds 函数](../api/intune-shared-devicemanagement-getrolescopetagsbyids.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md) 集合|尚未记录|
|[getRoleScopeTagsByResource 函数](../api/intune-shared-devicemanagement-getrolescopetagsbyresource.md)|[roleScopeTag](../resources/intune-rbac-rolescopetag.md) 集合|尚未记录|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|与设备关联的唯一标识符。|
|**设备配置**|
|intuneAccountId|Guid|给定租户的 Intune 帐户 ID|
|legacyPcManangementEnabled|布尔值|用于为此帐户启用非 MDM 托管旧版电脑管理的 属性。 此属性是只读的。|
|maximumDepTokens|Int32|允许每个租户使用的最大 DEP 令牌数。|
|settings|[deviceManagementSettings](../resources/intune-deviceconfig-devicemanagementsettings.md)|帐户级别设置。|
|**设备管理**|
|accountMoveCompletionDateTime|DateTimeOffset|租户&之间移动时的日期。|
|adminConsent|[adminConsent](../resources/intune-devices-adminconsent.md)|管理员同意信息。|
|deviceProtectionOverview|[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md)|设备保护概述。|
|managedDeviceCleanupSettings|[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md)|设备清理规则|
|subscriptionState|[deviceManagementSubscriptionState](../resources/intune-devices-devicemanagementsubscriptionstate.md)|租户移动设备管理订阅状态。 可取值为：`pending`、`active`、`warning`、`disabled`、`deleted`、`blocked`、`lockedOut`。|
|订阅|[deviceManagementSubscriptions](../resources/intune-devices-devicemanagementsubscriptions.md)|租户的订阅。 可取值为：`none`、`intune`、`office365`、`intunePremium`、`intune_EDU`、`intune_SMB`。|
|windowsMalwareOverview|[windowsMalwareOverview](../resources/intune-devices-windowsmalwareoverview.md)|Windows 设备的恶意软件概述。|
|**组策略分析**|
|groupPolicyObjectFiles|[groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) 集合|已上载的组策略对象文件的列表。|
|**载入**|
|intuneBrand|[intuneBrand](../resources/intune-onboarding-intunebrand.md)|intuneBrand 包含在自定义公司门户应用程序以及最终用户 Web 门户的外观时使用的数据。|
|**Odj**|
|domainJoinConnectors|[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) 集合|连接器对象的列表。|

## <a name="relationships"></a>关系
|关系|类型|说明&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|
|:---|:---|:---|
|**Android for Work**|
|androidDeviceOwnerEnrollmentProfiles|[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) 集合|Android 设备所有者注册配置文件实体。|
|androidForWorkAppConfigurationSchemas|[androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) 集合|Android for Work 应用配置架构实体。|
|androidForWorkEnrollmentProfiles|[androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) 集合|Android for Work 注册配置文件实体。|
|androidForWorkSettings|[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)|Android for Work 设置单例实体。|
|androidManagedStoreAccountEnterpriseSettings|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)|单一的 Android 托管存储帐户企业设置实体。|
|androidManagedStoreAppConfigurationSchemas|[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) 集合|Android Enterprise应用配置架构实体。|
|**审核**|
|auditEvents|[auditEvent](../resources/intune-auditing-auditevent.md) 集合|审核事件|
|**公司条款**|
|termsAndConditions|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 集合|与公司的设备管理关联的条款和条件。|
|**公司注册**|
|enrollmentProfiles|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) 集合|注册配置文件。|
|importedAppleDeviceIdentities|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) 集合|导入的 Apple 设备标识。|
|importedDeviceIdentities|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) 集合|导入的设备标识。|
|**设备配置**|
|advancedThreatProtectionOnboardingStateSummary|[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|此帐户的 ATP 载入状态摘要状态。|
|cartToClassAssociations|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) 集合|购物车到类关联。|
|deviceCompliancePolicies|[deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) 集合|设备符合性策略。|
|deviceCompliancePolicyDeviceStateSummary|[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|此帐户的设备符合性状态摘要。|
|deviceCompliancePolicySettingStateSummaries|[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 集合|此帐户的符合性设置的摘要状态。|
|deviceConfigurationConflictSummary|[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) 集合|此帐户冲突状态的策略摘要。|
|deviceConfigurationDeviceStateSummaries|[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|此帐户的设备配置设备状态摘要。|
|deviceConfigurationRestrictedAppsViolations|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) 集合|此帐户的受限应用冲突。|
|deviceConfigurations|[deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) 集合|设备配置。|
|deviceConfigurationUserStateSummaries|[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)|此帐户的设备配置用户状态摘要。|
|iosUpdateStatuses|[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) 集合|此帐户的 IOS 软件更新安装状态。|
|ndesConnectors|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) 集合|此帐户的 Ndes 连接器的集合。|
|softwareUpdateStatusSummary|[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|软件更新状态摘要。|
|**设备意图**|
|intents|[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) 集合|设备管理意图|
|settingDefinitions|[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) 集合|设备管理意图设置定义|
|模板|[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) 集合|可用模板|
|categories|[deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) 集合|可用类别|
|**设备管理**|
|applePushNotificationCertificate|[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)|Apple 推送通知证书。|
|dataSharingConsents|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md) 集合|数据共享许可。|
|detectedApps|[detectedApp](../resources/intune-devices-detectedapp.md) 集合|检测到与设备关联的应用的列表。|
|deviceManagementScripts|[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) 集合|与租户关联的设备管理脚本列表。|
|deviceShellScripts|[deviceShellScript](../resources/intune-devices-deviceshellscript.md) 集合|与租户关联的设备 shell 脚本列表。|
|deviceHealthScripts|[deviceHealthScript](../resources/intune-devices-devicehealthscript.md) 集合|与租户关联的设备运行状况脚本列表。|
|managedDeviceOverview|[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)|设备概述|
|managedDevices|[managedDevice](../resources/intune-devices-manageddevice.md) 集合|托管设备列表。|
|remoteActionAudits|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) 集合|租户的设备远程操作审核列表。|
|windowsMalwareInformation|[windowsMalwareInformation](../resources/intune-devices-windowsmalwareinformation.md) 集合|租户中受影响的恶意软件列表。|
|mobileAppTroubleshootingEvents|[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) 集合|MobileAppTroubleshootingEvent 的集合属性。|
|userExperienceAnalyticsOverview|[userExperienceAnalyticsOverview](../resources/intune-devices-userExperienceAnalyticsOverview.md)|用户体验分析概述|
|userExperienceAnalyticsBaselines|[userExperienceAnalyticsBaseline](../resources/intune-devices-userExperienceAnalyticsBaseline.md) 集合|用户体验分析基线|
|userExperienceAnalyticsCategories|[userExperienceAnalyticsCategory](../resources/intune-devices-userExperienceAnalyticsCategory.md) 集合|用户体验分析类别|
|userExperienceAnalyticsDevicePerformance|[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userExperienceAnalyticsDevicePerformance.md) 集合|用户体验分析设备性能|
|userExperienceAnalyticsRegressionSummary|[userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userExperienceAnalyticsRegressionSummary.md)|用户体验分析回归摘要|
|userExperienceAnalyticsDeviceStartupHistory|[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userExperienceAnalyticsDeviceStartupHistory.md) 集合|用户体验分析设备启动历史记录|
|userExperienceAnalyticsDeviceStartupProcesses|[userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userExperienceAnalyticsDeviceStartupProcess.md) 集合|用户体验分析设备启动过程|
|userExperienceAnalyticsDeviceStartupProcessPerformance|[userExperienceAnalyticsDeviceStartupProcessPerformance](../resources/intune-devices-userExperienceAnalyticsDeviceStartupProcessPerformance.md) 集合|用户体验分析设备启动过程性能|
|depOnboardingSettings|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) 集合|每个租户多个 DEP 令牌的集合。|
|importedDeviceIdentities|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) 集合|导入的设备标识。|
|importedWindowsAutopilotDeviceIdentities|[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) 集合|导入的 Windows AutoPilot 设备的集合。|
|windowsAutopilotDeploymentProfiles|[windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md) 集合|Windows自动试点部署配置文件|
|windowsAutopilotDeviceIdentities|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) 集合|该Windows autopilot 设备标识包含集合。|
|windowsAutopilotSettings|[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)|the Windows autopilot account settings.|
|**嵌入式 SIM 卡**|
|embeddedSIMActivationCodePools|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) 集合|此帐户创建的嵌入式 SIM 卡激活代码池。|
|**Fencing**|
|managementConditions|[managementCondition](../resources/intune-fencing-managementcondition.md) 集合|与公司的设备管理相关的管理条件。|
|managementConditionStatements|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) 集合|与公司设备管理相关的管理条件声明。|
|**组策略分析**|
|groupPolicyMigrationReports|[groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) 集合|组策略迁移报告的列表。|
|**通知**|
|notificationMessageTemplates|[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 集合|通知消息模板。|
|**载入**|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|Exchange 本地条件访问设置。 本地条件访问需要设备注册并符合邮件访问要求|
|deviceCategories|[deviceCategory](../resources/intune-shared-devicecategory.md) 集合|租户的设备类别列表。|
|deviceEnrollmentConfigurations|[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 集合|设备注册配置列表|
|deviceManagementPartners|[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 集合|由租户配置的设备管理合作伙伴列表。|
|exchangeConnectors|[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 集合|由租户配置的 Exchange 连接器列表。|
|exchangeOnPremisesPolicies|[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) 集合|租户配置的Exchange预配置策略的列表。|
|exchangeOnPremisesPolicy|[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|控制移动设备对本地移动设备Exchange的策略|
|mobileThreatDefenseConnectors|[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 集合|由租户配置的移动威胁防护连接器列表。|
|**策略集**|
|deviceManagementScripts|[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) 集合|与租户关联的设备管理脚本列表。|
|deviceConfigurations|[deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) 集合|与租户关联的设备配置列表。|
|deviceCompliancePolicies|[deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) 集合|与租户关联的设备合规性策略列表。|
|windowsAutopilotDeploymentProfiles|[windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md) 集合|Windows自动试点部署配置文件|
|deviceEnrollmentConfigurations|[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 集合|设备注册配置列表|
|**资源访问 Polcy**|
|derivedCredentials|[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) 集合|与帐户关联的派生凭据设置的集合。|
|**远程访问**|
|userPfxCertificates|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) 集合|与用户关联的 PFX 证书的集合。|
|**远程协助**|
|remoteAssistancePartners|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 集合|远程帮助合作伙伴。|
|**基于角色的访问控制 (RBAC)**|
|resourceOperations|[resourceOperation](../resources/intune-rbac-resourceoperation.md) 集合|资源操作。|
|roleAssignments|[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 集合|角色分配。|
|roleDefinitions|[roleDefinition](../resources/intune-rbac-roledefinition.md) 集合|角色定义。|
|roleScopeTags|[roleScopeTag](../resources/intune-rbac-rolescopetag.md) 集合|角色作用域标记。|
|**报告**|
|reports|[deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md)|报告单一ton|
|**软件更新**|
|windowsFeatureUpdateProfiles|[windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) 集合|Windows 功能更新配置文件的集合|
|**电信费用 (TEM)**|
|telecomExpenseManagementPartners|[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 集合|电信费用管理合作伙伴。|
|**疑难解答**|
|troubleshootingEvents|[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 集合|租户的故障排除事件列表。|
|**Windows 信息保护**|
|intuneBrandingProfiles|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) 集合|面向 AAD 组的 Intune 品牌打造配置文件|
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




