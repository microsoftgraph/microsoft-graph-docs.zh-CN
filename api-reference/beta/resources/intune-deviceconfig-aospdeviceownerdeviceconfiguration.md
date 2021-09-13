---
title: aospDeviceOwnerDeviceConfiguration 资源类型
description: 本主题提供由 AndroidDeviceOwnerAOSPDeviceConfiguration 资源公开的已声明方法、属性和关系的说明。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5b08761f4e4da3fa71038a94e7098328d308bb47
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59148002"
---
# <a name="aospdeviceownerdeviceconfiguration-resource-type"></a>aospDeviceOwnerDeviceConfiguration 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

本主题提供由 AndroidDeviceOwnerAOSPDeviceConfiguration 资源公开的已声明方法、属性和关系的说明。


继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 aospDeviceOwnerDeviceConfigurations](../api/intune-deviceconfig-aospdeviceownerdeviceconfiguration-list.md)|[aospDeviceOwnerDeviceConfiguration](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md) 集合|列出 [aospDeviceOwnerDeviceConfiguration](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md) 对象的属性和关系。|
|[获取 aospDeviceOwnerDeviceConfiguration](../api/intune-deviceconfig-aospdeviceownerdeviceconfiguration-get.md)|[aospDeviceOwnerDeviceConfiguration](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md)|读取 [aospDeviceOwnerDeviceConfiguration 对象的属性和](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md) 关系。|
|[创建 aospDeviceOwnerDeviceConfiguration](../api/intune-deviceconfig-aospdeviceownerdeviceconfiguration-create.md)|[aospDeviceOwnerDeviceConfiguration](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md)|创建新的 [aospDeviceOwnerDeviceConfiguration](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md) 对象。|
|[删除 aospDeviceOwnerDeviceConfiguration](../api/intune-deviceconfig-aospdeviceownerdeviceconfiguration-delete.md)|无|删除 [aospDeviceOwnerDeviceConfiguration](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md)。|
|[更新 aospDeviceOwnerDeviceConfiguration](../api/intune-deviceconfig-aospdeviceownerdeviceconfiguration-update.md)|[aospDeviceOwnerDeviceConfiguration](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md)|更新 [aospDeviceOwnerDeviceConfiguration 对象](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md) 的属性。|

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
|appsAllowInstallFromUnknownSources|Boolean|指示是否允许用户启用未知源设置。|
|bluetoothBlocked|Boolean|指示是否禁用蓝牙的使用。 设置为 true 时，无法在设备上启用蓝牙。|
|bluetoothBlockConfiguration|Boolean|指示是否阻止用户配置蓝牙。|
|bluetoothBlockContactSharing|Boolean|指示是否阻止用户通过蓝牙共享联系人。|
|cameraBlocked|Boolean|指示是否禁用相机的使用。|
|cellularBlockWiFiTethering|Boolean|指示是否阻止 Wi-Fi 网络共享。|
|factoryResetBlocked|Boolean|指示设置中的恢复出厂设置选项是否已禁用。|
|passwordMinimumLength|Int32|指示设备上所需的密码的最小长度。 有效值为 4 至 16|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|屏幕超时之前的不活动分钟数。|
|passwordRequiredType|[androidDeviceOwnerRequiredPasswordType](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|指示设备上所需的最低密码质量。 可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`customPassword`。|
|passwordSignInFailureCountBeforeFactoryReset|Int32|指示擦除设备之前用户可以输入错误密码次数。 有效值为 4 至 11|
|screenCaptureBlocked|Boolean|指示是否禁用屏幕截图功能。|
|securityAllowDebuggingFeatures|Boolean|指示是否阻止用户在设备上启用调试功能。|
|storageAllowUsb|Boolean|指示是否阻止 USB 存储。|
|storageBlockExternalMedia|Boolean|指示是否阻止外部媒体。|
|storageBlockUsbFileTransfer|Boolean|指示是否阻止 USB 文件传输。|
|backupBlocked|Boolean|指示是否阻止备份服务。|
|wifiBlockEditConfigurations|Boolean|指示是否阻止用户编辑 wifi 连接设置。|

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
  "@odata.type": "microsoft.graph.aospDeviceOwnerDeviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.aospDeviceOwnerDeviceConfiguration",
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
  "appsAllowInstallFromUnknownSources": true,
  "bluetoothBlocked": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "factoryResetBlocked": true,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordRequiredType": "String",
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "backupBlocked": true,
  "wifiBlockEditConfigurations": true
}
```



