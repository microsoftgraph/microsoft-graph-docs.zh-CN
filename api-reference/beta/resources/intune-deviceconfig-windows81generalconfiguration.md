---
title: windows81GeneralConfiguration 资源类型
description: 本主题提供由 windows81GeneralConfiguration 资源公开的已声明方法、属性和关系的说明。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7ed40025a392b66b8bff0421259a111139315771
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59145979"
---
# <a name="windows81generalconfiguration-resource-type"></a>windows81GeneralConfiguration 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

本主题提供由 windows81GeneralConfiguration 资源公开的已声明方法、属性和关系的说明。


继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List windows81GeneralConfigurations](../api/intune-deviceconfig-windows81generalconfiguration-list.md)|[windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 集合|列出 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 对象的属性和关系。|
|[Get windows81GeneralConfiguration](../api/intune-deviceconfig-windows81generalconfiguration-get.md)|[windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md)|读取 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 对象的属性和关系。|
|[Create windows81GeneralConfiguration](../api/intune-deviceconfig-windows81generalconfiguration-create.md)|[windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md)|创建新的 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 对象。|
|[Delete windows81GeneralConfiguration](../api/intune-deviceconfig-windows81generalconfiguration-delete.md)|无|删除 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md)。|
|[Update windows81GeneralConfiguration](../api/intune-deviceconfig-windows81generalconfiguration-update.md)|[windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md)|更新 [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) 对象的属性。|

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
|accountsBlockAddingNonMicrosoftAccountEmail|Boolean|指示是否阻止用户将电子邮件帐户添加到未与 Microsoft 帐户关联的设备。|
|applyOnlyToWindows81|Boolean|指示此策略是否仅适用于 Windows 8.1 的值。 此属性是只读的。|
|browserBlockAutofill|Boolean|指示是否阻止自动填充。|
|browserBlockAutomaticDetectionOfIntranetSites|Boolean|指示是否阻止自动检测 Intranet 站点。|
|browserBlockEnterpriseModeAccess|Boolean|指示是否阻止企业模式访问。|
|browserBlockJavaScript|Boolean|指示是否阻止用户使用 JavaScript。|
|browserBlockPlugins|Boolean|指示是否阻止插件。|
|browserBlockPopups|Boolean|指示是否阻止弹出窗口。|
|browserBlockSendingDoNotTrackHeader|Boolean|指示是否阻止用户发送 Do Not Track 标头。|
|browserBlockSingleWordEntryOnIntranetSites|Boolean|指示是否阻止在 Intranet 站点上使用单字条目。|
|browserRequireSmartScreen|Boolean|指示是否要求用户使用智能屏幕筛选器。|
|browserEnterpriseModeSiteListLocation|String|企业模式网站列表位置。 可能是本地文件、本地网络或 http 位置。|
|browserInternetSecurityLevel|[internetSiteSecurityLevel](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|Internet 安全级别。 可取值为：`userDefined`、`medium`、`mediumHigh`、`high`。|
|browserIntranetSecurityLevel|[siteSecurityLevel](../resources/intune-deviceconfig-sitesecuritylevel.md)|Intranet 安全级别。 可取值为：`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high`。|
|browserLoggingReportLocation|String|日志记录报表位置。|
|browserRequireHighSecurityForRestrictedSites|Boolean|指示是否要求受限站点具有高安全性。|
|browserRequireFirewall|Boolean|指示是否需要防火墙。|
|browserRequireFraudWarning|Boolean|指示是否需要诈骗警告。|
|browserTrustedSitesSecurityLevel|[siteSecurityLevel](../resources/intune-deviceconfig-sitesecuritylevel.md)|受信任的站点安全级别。 可取值为：`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high`。|
|cellularBlockDataRoaming|Boolean|指示是否阻止数据漫游。|
|diagnosticsBlockDataSubmission|Boolean|指示是否阻止诊断数据提交。|
|passwordBlockPicturePasswordAndPin|Boolean|指示是否阻止用户使用图片密码和 PIN。|
|passwordExpirationDays|Int32|密码过期天数。|
|passwordMinimumLength|Int32|密码最短长度。|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|屏幕超时之前的不活动分钟数。|
|passwordMinimumCharacterSetCount|Int32|密码中必需的字符集数。|
|passwordPreviousPasswordBlockCount|Int32|防止重复使用的先前密码的数量。 有效值为 0 至 24|
|passwordRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|必需的密码类型。 可取值为：`deviceDefault`、`alphanumeric`、`numeric`。|
|passwordSignInFailureCountBeforeFactoryReset|Int32|恢复出厂设置之前登录失败的次数。|
|storageRequireDeviceEncryption|Boolean|指示是否要求对移动设备加密。|
|minimumAutoInstallClassification|[updateClassification](../resources/intune-deviceconfig-updateclassification.md)|要自动安装的最低更新分类。 可取值为：`userDefined`、`recommendedAndImportant`、`important`、`none`。|
|updatesMinimumAutoInstallClassification|[updateClassification](../resources/intune-deviceconfig-updateclassification.md)|要自动安装的最低更新分类。 可取值为：`userDefined`、`recommendedAndImportant`、`important`、`none`。|
|updatesRequireAutomaticUpdates|Boolean|指示是否需要自动更新。|
|userAccountControlSettings|[windowsUserAccountControlSettings](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|用户帐户控制设置。 可取值为：`userDefined`、`alwaysNotify`、`notifyOnAppChanges`、`notifyOnAppChangesWithoutDimming`、`neverNotify`。|
|workFoldersUrl|String|工作文件夹 url。|

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

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows81GeneralConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
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
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "String",
  "browserInternetSecurityLevel": "String",
  "browserIntranetSecurityLevel": "String",
  "browserLoggingReportLocation": "String",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "String",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordRequiredType": "String",
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "storageRequireDeviceEncryption": true,
  "minimumAutoInstallClassification": "String",
  "updatesMinimumAutoInstallClassification": "String",
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "String",
  "workFoldersUrl": "String"
}
```



