---
title: iosUpdateConfiguration 资源类型
description: IOS 更新配置，允许配置一周内的时间范围，用于安装 iOS 更新。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 451ed00d45556572ba28617430174afb7bc19843
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754718"
---
# <a name="iosupdateconfiguration-resource-type"></a>iosUpdateConfiguration 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

IOS 更新配置，允许配置一周内的时间范围，用于安装 iOS 更新。


继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
|[List iosUpdateConfigurations](../api/intune-deviceconfig-iosupdateconfiguration-list.md)|[iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 集合|列出 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 对象的属性和关系。|
|[Get iosUpdateConfiguration](../api/intune-deviceconfig-iosupdateconfiguration-get.md)|[iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md)|读取 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 对象的属性和关系。|
|[Create iosUpdateConfiguration](../api/intune-deviceconfig-iosupdateconfiguration-create.md)|[iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md)|创建新的 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 对象。|
|[Delete iosUpdateConfiguration](../api/intune-deviceconfig-iosupdateconfiguration-delete.md)|无|删除 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md)。|
|[Update iosUpdateConfiguration](../api/intune-deviceconfig-iosupdateconfiguration-update.md)|[iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md)|更新 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|说明|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|activeHoursStart|TimeOfDay|使用时段开始时间（使用时段表示不应发生更新安装的时间范围）|
|activeHoursEnd|TimeOfDay|使用时段结束时间（使用时段表示不应发生更新安装的时间范围）|
|scheduledInstallDays|[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) 集合|配置为使用时段所对应的一周的某一天。 该集合最多可包含 7 个元素。|
|utcTimeOffsetInMinutes|Int32|UTC 时间偏移，用分钟表示|

## <a name="relationships"></a>关系
|关系|类型|Description|
|:---|:---|:---|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合|设备配置文件的分配列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合|按设备的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合|用户的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合|设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosUpdateConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "activeHoursStart": "String (time of day)",
  "activeHoursEnd": "String (time of day)",
  "scheduledInstallDays": [
    "String"
  ],
  "utcTimeOffsetInMinutes": 1024
}
```




