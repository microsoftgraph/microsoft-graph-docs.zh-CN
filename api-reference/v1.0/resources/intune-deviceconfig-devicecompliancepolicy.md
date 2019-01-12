---
title: deviceCompliancePolicy 资源类型
description: '这是符合性策略的基类。 符合性策略特定于平台，每个平台的符合性策略相互独立，且继承自此处。 '
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 85a82c981c16370603e3622f6536755bf9146343
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990395"
---
# <a name="devicecompliancepolicy-resource-type"></a>deviceCompliancePolicy 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

这是符合性策略的基类。 符合性策略特定于平台，每个平台的符合性策略相互独立，且继承自此处。 
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List deviceCompliancePolicies](../api/intune-deviceconfig-devicecompliancepolicy-list.md)|[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 集合|列出 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 对象的属性和关系。|
|[Get deviceCompliancePolicy](../api/intune-deviceconfig-devicecompliancepolicy-get.md)|[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)|读取 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) 对象的属性和关系。|
|[assign 操作](../api/intune-deviceconfig-devicecompliancepolicy-assign.md)|[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合|尚未记录|
|[scheduleActionsForRules 操作](../api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。|
|description|String|管理员提供的设备配置说明。|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。|
|displayName|String|管理员提供的设备配置名称。|
|version|Int32|设备配置的版本。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|scheduledActionsForRule|[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) 集合|此规则的计划操作列表|
|deviceStatuses|[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 集合|DeviceComplianceDeviceStatus 的列表。|
|userStatuses|[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) 集合|DeviceComplianceUserStatus 的列表。|
|deviceStatusOverview|[deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|设备符合性设备状态概述|
|userStatusOverview|[deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|设备符合性用户状态概述|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合|符合性设置状态设备摘要|
|assignments|[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) 集合|此符合性策略的分配集合。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```



