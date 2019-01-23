---
title: defaultDeviceCompliancePolicy 资源类型
description: 默认设备合规性策略规则的强制实施帐户范围。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 465afd96b96eb7ddbc9b1ce31bf577e63a67279f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402543"
---
# <a name="defaultdevicecompliancepolicy-resource-type"></a>defaultDeviceCompliancePolicy 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

默认设备合规性策略规则的强制实施帐户范围。


继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 defaultDeviceCompliancePolicies](../api/intune-deviceconfig-defaultdevicecompliancepolicy-list.md)|[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)集合|列出属性和[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)对象之间的关系。|
|[获取 defaultDeviceCompliancePolicy](../api/intune-deviceconfig-defaultdevicecompliancepolicy-get.md)|[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)|读取属性和[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)对象的关系。|
|[创建 defaultDeviceCompliancePolicy](../api/intune-deviceconfig-defaultdevicecompliancepolicy-create.md)|[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)|创建新的[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)对象。|
|[删除 defaultDeviceCompliancePolicy](../api/intune-deviceconfig-defaultdevicecompliancepolicy-delete.md)|无|删除[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)。|
|[更新 defaultDeviceCompliancePolicy](../api/intune-deviceconfig-defaultdevicecompliancepolicy-update.md)|[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)|更新[defaultDeviceCompliancePolicy](../resources/intune-deviceconfig-defaultdevicecompliancepolicy.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|roleScopeTagIds|String 集合|此实体实例范围标记的列表。 继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|id|String|实体的键。 继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|description|String|管理员提供的设备配置的说明。 继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|version|Int32|设备配置的版本。 继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|scheduledActionsForRule|[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 集合|此规则的计划操作的列表 继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|deviceStatuses|[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 集合|DeviceComplianceDeviceStatus 的列表。 继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|userStatuses|[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) 集合|DeviceComplianceUserStatus 的列表。 继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|deviceStatusOverview|[deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|设备合规性设备状态概述 继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|userStatusOverview|[deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|设备合规性用户状态概述 继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合|合规性设置状态设备摘要 继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|
|assignments|[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合|此合规性策略的作业集合。 继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.defaultDeviceCompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.defaultDeviceCompliancePolicy",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```




