---
title: windows10DeviceFirmwareConfigurationInterface 资源类型
description: 'Graph固件配置接口的一些属性 '
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6f32cb742be586c5d1eb26be9046024a2dddf3b7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59146084"
---
# <a name="windows10devicefirmwareconfigurationinterface-resource-type"></a>windows10DeviceFirmwareConfigurationInterface 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Graph固件配置接口的一些属性 


继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windows10DeviceFirmwareConfigurationInterfaces](../api/intune-deviceconfig-windows10devicefirmwareconfigurationinterface-list.md)|[windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) 集合|列出 [windows10DeviceFirmwareConfigurationInterface 对象的属性和](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) 关系。|
|[获取 windows10DeviceFirmwareConfigurationInterface](../api/intune-deviceconfig-windows10devicefirmwareconfigurationinterface-get.md)|[windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md)|读取 [windows10DeviceFirmwareConfigurationInterface 对象的属性和](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) 关系。|
|[创建 windows10DeviceFirmwareConfigurationInterface](../api/intune-deviceconfig-windows10devicefirmwareconfigurationinterface-create.md)|[windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md)|创建新的 [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) 对象。|
|[删除 windows10DeviceFirmwareConfigurationInterface](../api/intune-deviceconfig-windows10devicefirmwareconfigurationinterface-delete.md)|无|删除 [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md)。|
|[更新 windows10DeviceFirmwareConfigurationInterface](../api/intune-deviceconfig-windows10devicefirmwareconfigurationinterface-update.md)|[windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md)|更新 [windows10DeviceFirmwareConfigurationInterface 对象](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) 的属性。|

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
|changeUefiSettingsPermission|[changeUefiSettingsPermission](../resources/intune-deviceconfig-changeuefisettingspermission.md)|定义授予用户更改 UEFI 设置的权限级别。 可取值为：`notConfiguredOnly`、`none`。|
|virtualizationOfCpuAndIO|[enablement](../resources/intune-shared-enablement.md)|定义是否启用 CPU 和 IO 虚拟化。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|相机|[enablement](../resources/intune-shared-enablement.md)|定义是否启用内置相机。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|microphonesAndSpeakers|[enablement](../resources/intune-shared-enablement.md)|定义是否启用内置麦克风或扬声器。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|无线电广播|[enablement](../resources/intune-shared-enablement.md)|定义是否启用内置无线电（如 WIFI、NFC、蓝牙等）。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|bootFromExternalMedia|[enablement](../resources/intune-shared-enablement.md)|定义是否允许用户从外部媒体启动。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|bootFromBuiltInNetworkAdapters|[enablement](../resources/intune-shared-enablement.md)|定义是否允许用户从内置网络适配器启动。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|windowsPlatformBinaryTable|[enablement](../resources/intune-shared-enablement.md)|定义是否允许用户启用Windows二进制表。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|simultaneousMultiThreading|[enablement](../resources/intune-shared-enablement.md)|定义是否允许用户启用同时多线程。 可取值为：`notConfigured`、`enabled`、`disabled`。|

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
  "bootFromBuiltInNetworkAdapters": "String",
  "windowsPlatformBinaryTable": "String",
  "simultaneousMultiThreading": "String"
}
```



