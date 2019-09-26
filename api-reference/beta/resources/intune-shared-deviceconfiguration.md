---
title: deviceConfiguration 资源类型
description: 设备配置。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b595f8fdcc680ff93693f0fcee7f618386aa0740
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199940"
---
# <a name="deviceconfiguration-resource-type"></a>deviceConfiguration 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备配置。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List deviceConfigurations](../api/intune-shared-deviceconfiguration-list.md)|[deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) 集合|列出 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) 对象的属性和关系。|
|[Get deviceConfiguration](../api/intune-shared-deviceconfiguration-get.md)|[deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|读取 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) 对象的属性和关系。|
|**设备配置**|
|[分配操作](../api/intune-shared-deviceconfiguration-assign.md)|deviceConfigurationAssignment 集合|尚未记录|
|[windowsPrivacyAccessControls 操作](../api/intune-shared-deviceconfiguration-windowsprivacyaccesscontrols.md)|无|尚未记录|
|[assignedAccessMultiModeProfiles 操作](../api/intune-shared-deviceconfiguration-assignedaccessmultimodeprofiles.md)|无|尚未记录|
|[getTargetedUsersAndDevices 操作](../api/intune-shared-deviceconfiguration-gettargetedusersanddevices.md)|deviceConfigurationTargetedUserAndDevice 集合|尚未记录|
|**策略集**|
|[hasPayloadLinks 操作](../api/intune-shared-deviceconfiguration-haspayloadlinks.md)|[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)集合|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|实体的键。|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。|
|supportsScopeTags|Boolean|指示基础设备配置是否支持作用域标记的分配。 如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。 这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。 此属性是只读的。|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|适用于此策略的操作系统版本。|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|此策略的操作系统版本适用性规则。|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|此策略的设备模式适用性规则。|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。|
|说明|String|管理员提供的设备配置说明。|
|displayName|String|管理员提供的设备配置名称。|
|version|Int32|设备配置的版本。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|**设备配置**|
|groupAssignments|deviceConfigurationGroupAssignment 集合|设备配置文件的组分配列表。|
|assignments|deviceConfigurationAssignment 集合|设备配置文件的分配列表。|
|deviceStatuses|deviceConfigurationDeviceStatus 集合|按设备的设备配置安装状态。|
|userStatuses|deviceConfigurationUserStatus 集合|按用户的设备配置安装状态。|
|deviceStatusOverview|deviceConfigurationDeviceOverview|设备配置设备状态概述|
|userStatusOverview|deviceConfigurationUserOverview|设备配置用户状态概述|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合|设备配置设置状态设备摘要|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfiguration",
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
  "version": 1024
}
```



