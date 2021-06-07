---
title: deviceManagement 资源类型
description: 'deviceManagement 资源表示其内容因工作流而异的容器，包括：  '
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 83d3f3cda24c5961a34cb5c38de3ee43d6f5fe44
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732375"
---
# <a name="devicemanagement-resource-type"></a>deviceManagement 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

deviceManagement 资源表示其内容因工作流而异的容器，包括：  

- 审核事件  
- 公司条款和条件   
- 设备配置设置  
- 设备管理  
- 终结点保护  
- 注册配置文件  
- 通知  
- 载入策略、设置和详细信息  
- 基于角色的访问控制 (RBAC) 策略  
- 远程协助合作伙伴  
- 电信业务管理合作伙伴  
- 事件疑难解答  
- Windows信息保护摘要  

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
|[获取 deviceManagement](../api/intune-shared-devicemanagement-get.md)|[deviceManagement](../resources/intune-shared-devicemanagement.md)|读取 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的属性和关系。|
|[更新 deviceManagement](../api/intune-shared-devicemanagement-update.md)|[deviceManagement](../resources/intune-shared-devicemanagement.md)|更新 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的属性。|
|**载入**|
|[verifyWindowsEnrollmentAutoDiscovery function](../api/intune-shared-devicemanagement-verifywindowsenrollmentautodiscovery.md)|布尔值|尚未记录|
|**RBAC**|
|[getEffectivePermissions 函数](../api/intune-shared-devicemanagement-geteffectivepermissions.md)|[rolePermission](../resources/intune-rbac-rolepermission.md) 集合或字符串集合|检索当前验证的用户的有效权限|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设备唯一标识符|
|**设备配置**|
|settings|[deviceManagementSettings](../resources/intune-deviceconfig-devicemanagementsettings.md)|帐户级别设置。|
|**设备管理**|
|subscriptionState|String|租户移动设备管理订阅状态。 可取值包括：`pending`、`active`、`warning`、`disabled`、`deleted`、`blocked`、`lockedOut`。|
|**载入**|
|intuneBrand|[intuneBrand](../resources/intune-onboarding-intunebrand.md)|intuneBrand 包含在自定义公司门户应用程序以及最终用户网页版门户的外观时使用的数据。|

## <a name="relationships"></a>关系
|关系|类型|Description|
|:---|:---|:---|
|**公司条款和条件**|
|termsAndConditions|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md) 集合|与公司的设备管理关联的条款和条件。|
|**设备配置**|
|intuneAccountId|Guid|给定租户的 Intune 帐户 ID。|
|deviceCompliancePolicies|[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 集合|设备符合性策略。|
|deviceCompliancePolicyDeviceStateSummary|[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|此帐户的设备符合性状态摘要。|
|deviceCompliancePolicySettingStateSummaries|[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 集合|此帐户的符合性设置的摘要状态。|
|deviceConfigurationDeviceStateSummaries|[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|此帐户的设备配置设备状态摘要。|
|deviceConfigurations|[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) 集合|设备配置。|
|iosUpdateStatuses|[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) 集合|此帐户的 IOS 软件更新安装状态。|
|softwareUpdateStatusSummary|[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|软件更新状态摘要。|
|**设备管理**|
|applePushNotificationCertificate|[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)|Apple 推送通知证书。|
|detectedApps|[detectedApp](../resources/intune-devices-detectedapp.md) 集合|检测到与设备关联的应用的列表。|
|managedDeviceOverview|[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)|设备概述|
|managedDevices|[managedDevice](../resources/intune-devices-manageddevice.md) 集合|托管设备列表。|
|**通知**|
|notificationMessageTemplates|[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 集合|通知消息模板。|
|**载入**|
|conditionalAccessSettings|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|Exchange 本地条件访问设置。 本地条件访问需要设备注册并符合邮件访问要求|
|deviceCategories|[deviceCategory](../resources/intune-shared-devicecategory.md) 集合|租户的设备类别列表。|
|deviceEnrollmentConfigurations|[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) 集合|设备注册配置列表|
|deviceManagementPartners|[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 集合|由租户配置的设备管理合作伙伴列表。|
|complianceManagementPartners|[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) 集合|租户配置的合规性管理合作伙伴列表。|
|exchangeConnectors|[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 集合|由租户配置的 Exchange 连接器列表。|
|mobileThreatDefenseConnectors|[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 集合|由租户配置的移动威胁防护连接器列表。|
|**RBAC**|
|resourceOperations|[resourceOperation](../resources/intune-rbac-resourceoperation.md) 集合|资源操作。|
|roleAssignments|[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 集合|角色分配。|
|roleDefinitions|[roleDefinition](../resources/intune-rbac-roledefinition.md) 集合|角色定义。|
|**远程协助**|
|remoteAssistancePartners|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) 集合|远程帮助合作伙伴。|
|**电信费用管理**|
|telecomExpenseManagementPartners|[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 集合|电信费用管理合作伙伴。|
|**疑难解答**|
|troubleshootingEvents|[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 集合|租户的故障排除事件列表。|
|**Windows 信息保护**|
|windowsInformationProtectionAppLearningSummaries|[windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 集合|Windows 信息保护应用学习摘要。|
|windowsInformationProtectionNetworkLearningSummaries|[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 集合|Windows 信息保护网络学习摘要。|


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









