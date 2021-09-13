---
title: windowsUpdateForBusinessConfiguration 资源类型
description: 适用于企业的 Windows 更新配置。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5c8715a0d8fa2018ddce58806a4f6a4d23569d44
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59147876"
---
# <a name="windowsupdateforbusinessconfiguration-resource-type"></a>windowsUpdateForBusinessConfiguration 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

适用于企业的 Windows 更新配置。


继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List windowsUpdateForBusinessConfigurations](../api/intune-deviceconfig-windowsupdateforbusinessconfiguration-list.md)|[windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 集合|列出 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象的属性和关系。|
|[Get windowsUpdateForBusinessConfiguration](../api/intune-deviceconfig-windowsupdateforbusinessconfiguration-get.md)|[windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md)|读取 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象的属性和关系。|
|[Create windowsUpdateForBusinessConfiguration](../api/intune-deviceconfig-windowsupdateforbusinessconfiguration-create.md)|[windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md)|创建新的 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象。|
|[Delete windowsUpdateForBusinessConfiguration](../api/intune-deviceconfig-windowsupdateforbusinessconfiguration-delete.md)|无|删除 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md)。|
|[Update windowsUpdateForBusinessConfiguration](../api/intune-deviceconfig-windowsupdateforbusinessconfiguration-update.md)|[windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md)|更新 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象的属性。|
|[extendFeatureUpdatesPause 操作](../api/intune-deviceconfig-windowsupdateforbusinessconfiguration-extendfeatureupdatespause.md)|无|扩展适用于企业更新环Windows暂停功能更新。|
|[extendQualityUpdatesPause 操作](../api/intune-deviceconfig-windowsupdateforbusinessconfiguration-extendqualityupdatespause.md)|无|扩展适用于企业更新环Windows质量更新暂停。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|字符串集合|此实体实例的范围标记列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Boolean|指示基础设备配置是否支持分配范围标记。 当此值为 false 且实体对范围用户不可见时，不允许分配给 ScopeTags 属性。 这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|此策略的操作系统版本适用性。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|此策略的操作系统版本适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|此策略的设备模式适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|说明|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deliveryOptimizationMode|[windowsDeliveryOptimizationMode](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|传递优化模式。 可取值为：`userDefined`、`httpOnly`、`httpWithPeeringNat`、`httpWithPeeringPrivateGroup`、`httpWithInternetPeering`、`simpleDownload` 或 `bypassMode`。|
|prereleaseFeatures|[prereleaseFeatures](../resources/intune-deviceconfig-prereleasefeatures.md)|预发布功能。 可取值为：`userDefined`、`settingsOnly`、`settingsAndExperimentations`、`notAllowed`。|
|automaticUpdateMode|[automaticUpdateMode](../resources/intune-deviceconfig-automaticupdatemode.md)|自动更新模式。 可取值为：`userDefined`、`notifyDownload`、`autoInstallAtMaintenanceTime`、`autoInstallAndRebootAtMaintenanceTime`、`autoInstallAndRebootAtScheduledTime`、`autoInstallAndRebootWithoutEndUserControl` 或 `windowsDefault`。|
|microsoftUpdateServiceAllowed|Boolean|允许 Microsoft 更新服务|
|driversExcluded|Boolean|排除 Windows 更新驱动程序|
|installationSchedule|[windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|安装计划|
|qualityUpdatesDeferralPeriodInDays|Int32|推迟质量更新的天数|
|featureUpdatesDeferralPeriodInDays|Int32|推迟功能更新的天数|
|qualityUpdatesPaused|Boolean|暂停质量更新|
|featureUpdatesPaused|Boolean|暂停功能更新|
|qualityUpdatesPauseExpiryDateTime|DateTimeOffset|质量更新暂停到期日期/时间|
|featureUpdatesPauseExpiryDateTime|DateTimeOffset|功能更新暂停到期日期/时间|
|businessReadyUpdatesOnly|[windowsUpdateType](../resources/intune-deviceconfig-windowsupdatetype.md)|确定接收更新的分支设备。 可取值为：`userDefined`、`all`、`businessReadyOnly`、`windowsInsiderBuildFast`、`windowsInsiderBuildSlow`、`windowsInsiderBuildRelease`。|
|skipChecksBeforeRestart|Boolean|设置为在重启前跳过所有检查：电池电量 = 40%，用户状态、需要显示、演示模式、全屏模式、电话呼叫状态、游戏模式等。 |
|updateWeeks|[windowsUpdateForBusinessUpdateWeeks](../resources/intune-deviceconfig-windowsupdateforbusinessupdateweeks.md)|将更新安装安排在当月中的几周。 可取值为：`userDefined`、`firstWeek`、`secondWeek`、`thirdWeek`、`fourthWeek`、`everyWeek`。|
|qualityUpdatesPauseStartDate|日期|质量更新 暂停开始日期。 此属性是只读的。|
|featureUpdatesPauseStartDate|日期|功能更新 暂停开始日期。 此属性是只读的。|
|featureUpdatesRollbackWindowInDays|Int32|回滚有效的功能更新后的天数|
|qualityUpdatesWillBeRolledBack|Boolean|指定是否在下一次设备签入时回滚质量更新|
|featureUpdatesWillBeRolledBack|Boolean|指定是否在下一次设备签入时回滚功能更新|
|qualityUpdatesRollbackStartDateTime|DateTimeOffset|质量更新回滚 开始日期时间|
|featureUpdatesRollbackStartDateTime|DateTimeOffset|功能更新回滚开始日期时间|
|engagedRestartDeadlineInDays|Int32|在使用时段外自动计划和执行挂起重启的截止时间（以天表示，有效范围为 2 到 30 天）|
|engagedRestartSnoozeScheduleInDays|Int32|用户可以暂停使用重启提醒通知的天数，有效范围为 1 到 3 天|
|engagedRestartTransitionScheduleInDays|Int32|从使用时段外计划的自动重启转换到预定重启（需要用户计划）前的天数，有效范围为 0 到 30 天|
|deadlineForFeatureUpdatesInDays|Int32|自动安装功能更新的天数，有效范围为 2 到 30 天|
|deadlineForQualityUpdatesInDays|Int32|自动安装质量更新的天数，有效范围为 2 到 30 天|
|deadlineGracePeriodInDays|Int32|自截止时间到重启自动发生的天数，有效范围为 0 到 7 天|
|postponeRebootUntilAfterDeadline|Boolean|指定设备是否等到使用时段外重启的截止时间|
|autoRestartNotificationDismissal|[autoRestartNotificationDismissalMethod](../resources/intune-deviceconfig-autorestartnotificationdismissalmethod.md)|指定消除所需的自动重启通知的方法。 可取值为：`notConfigured`、`automatic`、`user`。|
|scheduleRestartWarningInHours|Int32|指定自动重启警告提醒通知的时间段。 支持的值：2、4、8、12 或 24 小时 (小时) 。|
|scheduleImminentRestartWarningInMinutes|Int32|指定自动重启即将发生的警告通知的时间段。 支持的值：15、30 或 60 (分钟) 。|
|userPauseAccess|[enablement](../resources/intune-shared-enablement.md)|指定是否允许最终用户暂停软件更新。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|userWindowsUpdateScanAccess|[enablement](../resources/intune-shared-enablement.md)|指定是否禁用用户对"更新"Windows扫描。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|updateNotificationLevel|[windowsUpdateNotificationDisplayOption](../resources/intune-deviceconfig-windowsupdatenotificationdisplayoption.md)|指定更新Windows用户看到哪些内容。 可取值为：`notConfigured`、`defaultNotifications`、`restartWarningsOnly`、`disableAllNotifications`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) 集合|设备配置文件的组分配列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合|设备配置文件的分配列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合|按设备的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合|用户的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合|设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceUpdateStates|[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) 集合|Windows配置设备状态更新。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdateForBusinessConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "deliveryOptimizationMode": "String",
  "prereleaseFeatures": "String",
  "automaticUpdateMode": "String",
  "microsoftUpdateServiceAllowed": true,
  "driversExcluded": true,
  "installationSchedule": {
    "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
    "scheduledInstallDay": "String",
    "scheduledInstallTime": "String (time of day)"
  },
  "qualityUpdatesDeferralPeriodInDays": 1024,
  "featureUpdatesDeferralPeriodInDays": 1024,
  "qualityUpdatesPaused": true,
  "featureUpdatesPaused": true,
  "qualityUpdatesPauseExpiryDateTime": "String (timestamp)",
  "featureUpdatesPauseExpiryDateTime": "String (timestamp)",
  "businessReadyUpdatesOnly": "String",
  "skipChecksBeforeRestart": true,
  "updateWeeks": "String",
  "qualityUpdatesPauseStartDate": "String (Date)",
  "featureUpdatesPauseStartDate": "String (Date)",
  "featureUpdatesRollbackWindowInDays": 1024,
  "qualityUpdatesWillBeRolledBack": true,
  "featureUpdatesWillBeRolledBack": true,
  "qualityUpdatesRollbackStartDateTime": "String (timestamp)",
  "featureUpdatesRollbackStartDateTime": "String (timestamp)",
  "engagedRestartDeadlineInDays": 1024,
  "engagedRestartSnoozeScheduleInDays": 1024,
  "engagedRestartTransitionScheduleInDays": 1024,
  "deadlineForFeatureUpdatesInDays": 1024,
  "deadlineForQualityUpdatesInDays": 1024,
  "deadlineGracePeriodInDays": 1024,
  "postponeRebootUntilAfterDeadline": true,
  "autoRestartNotificationDismissal": "String",
  "scheduleRestartWarningInHours": 1024,
  "scheduleImminentRestartWarningInMinutes": 1024,
  "userPauseAccess": "String",
  "userWindowsUpdateScanAccess": "String",
  "updateNotificationLevel": "String"
}
```



