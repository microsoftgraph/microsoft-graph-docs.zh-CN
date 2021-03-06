---
title: windowsDeliveryOptimizationConfiguration 资源类型
description: Windows 传递优化配置
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7e93f26c94715733fe1f41a7d5b7f149904aaf96
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49276208"
---
# <a name="windowsdeliveryoptimizationconfiguration-resource-type"></a>windowsDeliveryOptimizationConfiguration 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows 传递优化配置


继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsDeliveryOptimizationConfigurations](../api/intune-deviceconfig-windowsdeliveryoptimizationconfiguration-list.md)|[windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) 集合|列出 [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) 对象的属性和关系。|
|[获取 windowsDeliveryOptimizationConfiguration](../api/intune-deviceconfig-windowsdeliveryoptimizationconfiguration-get.md)|[windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)|读取 [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) 对象的属性和关系。|
|[创建 windowsDeliveryOptimizationConfiguration](../api/intune-deviceconfig-windowsdeliveryoptimizationconfiguration-create.md)|[windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)|创建新的 [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) 对象。|
|[删除 windowsDeliveryOptimizationConfiguration](../api/intune-deviceconfig-windowsdeliveryoptimizationconfiguration-delete.md)|无|删除 [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)。|
|[更新 windowsDeliveryOptimizationConfiguration](../api/intune-deviceconfig-windowsdeliveryoptimizationconfiguration-update.md)|[windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)|更新 [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|实体的键。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|String 集合|此实体实例的范围标记列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Boolean|指示基础设备配置是否支持作用域标记的分配。 如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。 这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|适用于此策略的操作系统版本。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|此策略的操作系统版本适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|此策略的设备模式适用性规则。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|description|字符串|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|字符串|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deliveryOptimizationMode|[windowsDeliveryOptimizationMode](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|指定传递优化可用于管理大型内容分布方案的网络带宽消耗的下载方法。 可取值为：`userDefined`、`httpOnly`、`httpWithPeeringNat`、`httpWithPeeringPrivateGroup`、`httpWithInternetPeering`、`simpleDownload` 或 `bypassMode`。|
|restrictPeerSelectionBy|[deliveryOptimizationRestrictPeerSelectionByOptions](../resources/intune-deviceconfig-deliveryoptimizationrestrictpeerselectionbyoptions.md)|指定通过选中的选项来限制对等方选择。
Option 1 (子网掩码) 仅适用于传递优化模式下载模式 LAN (1) 和组 (2) 。 可取值为：`notConfigured`、`subnetMask`。|
|groupIdSource|[deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)|指定将对等选择限制为特定源。
此策略中设置的选项仅适用于传递优化模式组 (2) 下载模式。 如果组 (2) 未设置为下载模式，此策略将被忽略。 对于选项 3-DHCP 选项 ID，客户端将查询 DHCP 选项 ID 234，并使用返回的 GUID 值作为组 ID。|
|bandwidthMode|[deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)|指定使用百分比、absolutes 或小时的前景色和背景带宽使用情况。|
|backgroundDownloadFromHttpDelayInSeconds|Int64|指定允许使用对等的后台下载中的 HTTP 源延迟的秒数。 有效值为0至4294967295|
|foregroundDownloadFromHttpDelayInSeconds|Int64|指定在允许使用对等 (0-86400) 的前台下载中延迟 HTTP 源的秒数。 有效值为0至86400
指定0将传递优化设置为使用云服务管理此设置。 有效值为0至86400|
|minimumRamAllowedToPeerInGigabytes|Int32|指定使用对等缓存 (1-100000) 的最小 RAM 大小（以 GB 为单位）。 有效值为1至100000|
|minimumDiskSizeAllowedToPeerInGigabytes|Int32|指定使用对等缓存 (1-100000) 的最小磁盘大小（以 GB 为单位）。 有效值为1至100000
建议值： 64 GB 到 256 GB。 有效值为1至100000|
|minimumFileSizeToCacheInMegabytes|Int32|指定启用以使用对等缓存 (1-100000) 的最小内容文件大小（以 MB 为单位）。 有效值为1至100000
推荐值： 1 MB 到 100000 MB。 有效值为1至100000|
|minimumBatteryPercentageAllowedToUpload|Int32|指定允许设备上传 (0-100) 数据的最小电池百分比。 有效值为 0 至 100
默认值为 0。 值 0 (零) 表示 "不受限制"，将使用云服务默认值。 有效值为 0 至 100|
|modifyCacheLocation|字符串|指定传递优化应用于其缓存的驱动器。|
|maximumCacheAgeInDays|Int32|指定在成功下载 (0-3650) 后，每个文件在传递优化缓存中保留的最长时间（以天为单位）。 有效值为0至3650|
|maximumCacheSize|[deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)|指定传递优化的最大缓存大小（以百分比或 GB 为单位）。|
|vpnPeerCaching|[启用](../resources/intune-shared-enablement.md)|指定是否允许设备在通过 VPN 连接到域网络时参与对等缓存。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|cacheServerHostNames|String 集合|指定缓存服务器的主机名。|
|cacheServerForegroundDownloadFallbackToHttpDelayInSeconds|Int32|指定前台下载延迟从缓存服务器回退到 HTTP 源的秒数。 有效的值为0到2592000。|
|cacheServerBackgroundDownloadFallbackToHttpDelayInSeconds|Int32|指定从缓存服务器回退到用于后台下载的 HTTP 源的秒数。 有效的值为0到2592000。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) 集合|设备配置文件的组分配列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合|设备配置文件的分配列表。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合|按设备的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合|按用户的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合|设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDeliveryOptimizationConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDeliveryOptimizationConfiguration",
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
  "restrictPeerSelectionBy": "String",
  "groupIdSource": {
    "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdSource"
  },
  "bandwidthMode": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidth"
  },
  "backgroundDownloadFromHttpDelayInSeconds": 1024,
  "foregroundDownloadFromHttpDelayInSeconds": 1024,
  "minimumRamAllowedToPeerInGigabytes": 1024,
  "minimumDiskSizeAllowedToPeerInGigabytes": 1024,
  "minimumFileSizeToCacheInMegabytes": 1024,
  "minimumBatteryPercentageAllowedToUpload": 1024,
  "modifyCacheLocation": "String",
  "maximumCacheAgeInDays": 1024,
  "maximumCacheSize": {
    "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSize"
  },
  "vpnPeerCaching": "String",
  "cacheServerHostNames": [
    "String"
  ],
  "cacheServerForegroundDownloadFallbackToHttpDelayInSeconds": 1024,
  "cacheServerBackgroundDownloadFallbackToHttpDelayInSeconds": 1024
}
```




