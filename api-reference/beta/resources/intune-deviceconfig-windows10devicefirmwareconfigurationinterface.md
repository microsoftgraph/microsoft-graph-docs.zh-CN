---
title: windows10DeviceFirmwareConfigurationInterface 资源类型
description: '设备固件配置接口的图形属性 '
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 21b9fe45375dfda0fef0173c14a135d0cff7651f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337844"
---
# <a name="windows10devicefirmwareconfigurationinterface-resource-type"></a>windows10DeviceFirmwareConfigurationInterface 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备固件配置接口的图形属性 


继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windows10DeviceFirmwareConfigurationInterfaces](../api/intune-deviceconfig-windows10devicefirmwareconfigurationinterface-list.md)|[windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md)集合|列出[windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md)对象的属性和关系。|
|[获取 windows10DeviceFirmwareConfigurationInterface](../api/intune-deviceconfig-windows10devicefirmwareconfigurationinterface-get.md)|[windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md)|读取[windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md)对象的属性和关系。|
|[创建 windows10DeviceFirmwareConfigurationInterface](../api/intune-deviceconfig-windows10devicefirmwareconfigurationinterface-create.md)|[windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md)|创建新的[windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md)对象。|
|[删除 windows10DeviceFirmwareConfigurationInterface](../api/intune-deviceconfig-windows10devicefirmwareconfigurationinterface-delete.md)|无|删除[windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md)。|
|[更新 windows10DeviceFirmwareConfigurationInterface](../api/intune-deviceconfig-windows10devicefirmwareconfigurationinterface-update.md)|[windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md)|更新[windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|实体的键。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|Boolean|指示基础设备配置是否支持作用域标记的分配。 如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。 这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|适用于此策略的操作系统版本。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|此策略的操作系统版本适用性规则。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|此策略的设备模式适用性规则。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|说明|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|changeUefiSettingsPermission|[changeUefiSettingsPermission](../resources/intune-deviceconfig-changeuefisettingspermission.md)|定义授予用户更改 UEFI 设置的权限级别。 可取值为：`notConfiguredOnly`、`none`。|
|virtualizationOfCpuAndIO|[启用](../resources/intune-shared-enablement.md)|定义是否启用 CPU 和 IO 虚拟化。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|照相机|[启用](../resources/intune-shared-enablement.md)|定义是否启用内置相机。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|microphonesAndSpeakers|[启用](../resources/intune-shared-enablement.md)|定义是否启用内置麦克风或扬声器。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|收发|[启用](../resources/intune-shared-enablement.md)|定义是否启用内置无线收发器 (例如, WLAN、NFC、蓝牙)。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|bootFromExternalMedia|[启用](../resources/intune-shared-enablement.md)|定义是否允许用户从外部媒体进行引导。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|bootFromBuiltInNetworkAdapters|[启用](../resources/intune-shared-enablement.md)|定义是否允许用户从内置网络适配器启动。 可取值为：`notConfigured`、`enabled`、`disabled`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合|设备配置文件的组分配列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合|设备配置文件的分配列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合|按设备的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合|按用户的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合|设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10DeviceFirmwareConfigurationInterface"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10DeviceFirmwareConfigurationInterface",
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
  "changeUefiSettingsPermission": "String",
  "virtualizationOfCpuAndIO": "String",
  "cameras": "String",
  "microphonesAndSpeakers": "String",
  "radios": "String",
  "bootFromExternalMedia": "String",
  "bootFromBuiltInNetworkAdapters": "String"
}
```



