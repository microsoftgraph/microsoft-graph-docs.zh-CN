---
title: macOSSoftwareUpdateConfiguration 资源类型
description: MacOS 软件更新配置
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4d68af2fe63dce5a398672ae8cca35c9152d6d179b6c65b11c6e053386562024
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54209852"
---
# <a name="macossoftwareupdateconfiguration-resource-type"></a>macOSSoftwareUpdateConfiguration 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

MacOS 软件更新配置


继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 macOSSoftwareUpdateConfigurations](../api/intune-deviceconfig-macossoftwareupdateconfiguration-list.md)|[macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md) 集合|列出 [macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md) 对象的属性和关系。|
|[获取 macOSSoftwareUpdateConfiguration](../api/intune-deviceconfig-macossoftwareupdateconfiguration-get.md)|[macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md)|读取 [macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md) 对象的属性和关系。|
|[创建 macOSSoftwareUpdateConfiguration](../api/intune-deviceconfig-macossoftwareupdateconfiguration-create.md)|[macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md)|创建新的 [macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md) 对象。|
|[删除 macOSSoftwareUpdateConfiguration](../api/intune-deviceconfig-macossoftwareupdateconfiguration-delete.md)|无|删除 [macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md)。|
|[更新 macOSSoftwareUpdateConfiguration](../api/intune-deviceconfig-macossoftwareupdateconfiguration-update.md)|[macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md)|更新 [macOSSoftwareUpdateConfiguration 对象](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|实体的键。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|布尔值|指示基础设备配置是否支持分配范围标记。 当此值为 false 且实体对范围用户不可见时，不允许分配给 ScopeTags 属性。 这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|此策略的操作系统版本适用性。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|此策略的操作系统版本适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|此策略的设备模式适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|description|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|字符串|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|criticalUpdateBehavior|[macOSSoftwareUpdateBehavior](../resources/intune-deviceconfig-macossoftwareupdatebehavior.md)|关键更新的更新行为。 可取值为：`notConfigured`、`default`。|
|configDataUpdateBehavior|[macOSSoftwareUpdateBehavior](../resources/intune-deviceconfig-macossoftwareupdatebehavior.md)|配置文件更新的更新行为。 可取值为：`notConfigured`、`default`。|
|firmwareUpdateBehavior|[macOSSoftwareUpdateBehavior](../resources/intune-deviceconfig-macossoftwareupdatebehavior.md)|固件更新的更新行为。 可取值为：`notConfigured`、`default`。|
|allOtherUpdateBehavior|[macOSSoftwareUpdateBehavior](../resources/intune-deviceconfig-macossoftwareupdatebehavior.md)|所有其他更新的更新行为。 可取值为：`notConfigured`、`default`。|
|updateScheduleType|[macOSSoftwareUpdateScheduleType](../resources/intune-deviceconfig-macossoftwareupdatescheduletype.md)|更新计划类型。 可取值为：`alwaysUpdate`、`updateDuringTimeWindows`、`updateOutsideOfTimeWindows`。|
|customUpdateTimeWindows|[customUpdateTimeWindow](../resources/intune-deviceconfig-customupdatetimewindow.md) 集合|允许或阻止更新的自定义时间窗口。 此集合最多可包含 20 个元素。|
|updateTimeWindowUtcOffsetInMinutes|Int32|指示每个更新时间窗口的 UTC 偏移的分钟数|

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
  "@odata.type": "microsoft.graph.macOSSoftwareUpdateConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateConfiguration",
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
  "criticalUpdateBehavior": "String",
  "configDataUpdateBehavior": "String",
  "firmwareUpdateBehavior": "String",
  "allOtherUpdateBehavior": "String",
  "updateScheduleType": "String",
  "customUpdateTimeWindows": [
    {
      "@odata.type": "microsoft.graph.customUpdateTimeWindow",
      "startDay": "String",
      "endDay": "String",
      "startTime": "String (time of day)",
      "endTime": "String (time of day)"
    }
  ],
  "updateTimeWindowUtcOffsetInMinutes": 1024
}
```




