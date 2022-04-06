---
title: aospDeviceOwnerWiFiConfiguration 资源类型
description: 通过在此配置文件中提供配置，你可以指示 AOSP 设备连接到所需的 Wi-Fi 终结点。 通过指定 Wi-Fi 终结点预期的身份验证方法和安全类型，Wi-Fi最终用户实现无缝连接。 此配置文件提供的安全类型有限且比 Enterprise Wi-Fi简单。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4424ea9a066b3e1adcd801ea3fb488e203425337
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2022
ms.locfileid: "64631191"
---
# <a name="aospdeviceownerwificonfiguration-resource-type"></a>aospDeviceOwnerWiFiConfiguration 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

通过在此配置文件中提供配置，你可以指示 AOSP 设备连接到所需的 Wi-Fi 终结点。 通过指定 Wi-Fi 终结点预期的身份验证方法和安全类型，Wi-Fi最终用户实现无缝连接。 此配置文件提供的安全类型有限且比 Enterprise Wi-Fi简单。


继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 aospDeviceOwnerWiFiConfigurations](../api/intune-deviceconfig-aospdeviceownerwificonfiguration-list.md)|[aospDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerwificonfiguration.md) 集合|列出 [aospDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerwificonfiguration.md) 对象的属性和关系。|
|[获取 aospDeviceOwnerWiFiConfiguration](../api/intune-deviceconfig-aospdeviceownerwificonfiguration-get.md)|[aospDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerwificonfiguration.md)|读取 [aospDeviceOwnerWiFiConfiguration 对象的属性和](../resources/intune-deviceconfig-aospdeviceownerwificonfiguration.md) 关系。|
|[创建 aospDeviceOwnerWiFiConfiguration](../api/intune-deviceconfig-aospdeviceownerwificonfiguration-create.md)|[aospDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerwificonfiguration.md)|创建新的 [aospDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerwificonfiguration.md) 对象。|
|[删除 aospDeviceOwnerWiFiConfiguration](../api/intune-deviceconfig-aospdeviceownerwificonfiguration-delete.md)|无|删除 [aospDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerwificonfiguration.md)。|
|[更新 aospDeviceOwnerWiFiConfiguration](../api/intune-deviceconfig-aospdeviceownerwificonfiguration-update.md)|[aospDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerwificonfiguration.md)|更新 [aospDeviceOwnerWiFiConfiguration 对象](../resources/intune-deviceconfig-aospdeviceownerwificonfiguration.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Boolean|指示基础设备配置是否支持分配范围标记。 当此值为 false 且实体对范围用户不可见时，不允许分配给 ScopeTags 属性。 这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|此策略的操作系统版本适用性。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|此策略的操作系统版本适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|此策略的设备模式适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|说明|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|networkName|String|网络名|
|ssid|String|这是广播到所有Wi-Fi网络的名称。|
|connectAutomatically|Boolean|此网络在范围内时自动连接。 如果设置为 true，将跳过用户提示，并自动将设备Wi-Fi网络。|
|connectWhenNetworkNameIsHidden|Boolean|设置为 true 时，此配置文件会强制设备连接到未将其 SSID 广播到所有设备的网络。|
|wiFiSecurityType|[aospDeviceOwnerWiFiSecurityType](../resources/intune-deviceconfig-aospdeviceownerwifisecuritytype.md)|指示Wi-Fi是否使用基于 EAP 的安全类型。 可取值为：`open`、`wep`、`wpaPersonal`、`wpaEnterprise`。|
|preSharedKey|String|这是 WPA 个人共享网络的预共享Wi-Fi密钥。|
|preSharedKeyIsSet|Boolean|这是 WPA 个人共享网络的预共享Wi-Fi密钥。|

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
  "@odata.type": "microsoft.graph.aospDeviceOwnerWiFiConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.aospDeviceOwnerWiFiConfiguration",
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
  "networkName": "String",
  "ssid": "String",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "String",
  "preSharedKey": "String",
  "preSharedKeyIsSet": true
}
```




