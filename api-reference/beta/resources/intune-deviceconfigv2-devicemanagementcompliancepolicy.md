---
title: deviceManagementCompliancePolicy 资源类型
description: 设备管理合规性策略
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cb7655aea442d23116ee45c94c3becc92676240f
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2021
ms.locfileid: "60676777"
---
# <a name="devicemanagementcompliancepolicy-resource-type"></a>deviceManagementCompliancePolicy 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备管理合规性策略

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementCompliancePolicies](../api/intune-deviceconfigv2-devicemanagementcompliancepolicy-list.md)|[deviceManagementCompliancePolicy](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md) 集合|列出 [deviceManagementCompliancePolicy](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md) 对象的属性和关系。|
|[获取 deviceManagementCompliancePolicy](../api/intune-deviceconfigv2-devicemanagementcompliancepolicy-get.md)|[deviceManagementCompliancePolicy](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md)|读取 [deviceManagementCompliancePolicy 对象的属性和](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md) 关系。|
|[创建 deviceManagementCompliancePolicy](../api/intune-deviceconfigv2-devicemanagementcompliancepolicy-create.md)|[deviceManagementCompliancePolicy](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md)|创建新的 [deviceManagementCompliancePolicy](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md) 对象。|
|[删除 deviceManagementCompliancePolicy](../api/intune-deviceconfigv2-devicemanagementcompliancepolicy-delete.md)|无|删除 [deviceManagementCompliancePolicy](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md)。|
|[更新 deviceManagementCompliancePolicy](../api/intune-deviceconfigv2-devicemanagementcompliancepolicy-update.md)|[deviceManagementCompliancePolicy](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md)|更新 [deviceManagementCompliancePolicy 对象](../resources/intune-deviceconfigv2-devicemanagementcompliancepolicy.md) 的属性。|
|[分配操作](../api/intune-deviceconfigv2-devicemanagementcompliancepolicy-assign.md)|[deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) 集合|尚未记录|
|[setScheduledActions 操作](../api/intune-deviceconfigv2-devicemanagementcompliancepolicy-setscheduledactions.md)|[deviceManagementComplianceScheduledActionForRule](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md) 集合|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|策略文档的键。 自动生成。|
|name|String|策略名称|
|说明|String|策略说明|
|平台|[deviceManagementConfigurationPlatforms](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|此策略的平台。 可取值为：`none`、`android`、`iOS`、`macOS`、`windows10X`、`windows10`。|
|technologies|[deviceManagementConfigurationTechnologies](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|此策略的技术。 可取值为：`none`、`mdm`、`windows10XManagement`、`configManager`、`microsoftSense`、`exchangeOnline`、`linuxMdm`、`unknownFutureValue`。|
|createdDateTime|DateTimeOffset|策略创建日期和时间。 此属性是只读的。|
|lastModifiedDateTime|DateTimeOffset|策略上次修改日期和时间。 此属性是只读的。|
|settingCount|Int32|设置数。 此属性是只读的。|
|creationSource|字符串|策略创建源|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。|
|isAssigned|Boolean|策略分配状态。 此属性是只读的。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|settings|[deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) 集合|策略设置|
|assignments|[deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) 集合|策略分配|
|scheduledActionsForRule|[deviceManagementComplianceScheduledActionForRule](../resources/intune-deviceconfigv2-devicemanagementcompliancescheduledactionforrule.md) 集合|此规则的计划操作列表|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementCompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementCompliancePolicy",
  "id": "String (identifier)",
  "name": "String",
  "description": "String",
  "platforms": "String",
  "technologies": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "settingCount": 1024,
  "creationSource": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "isAssigned": true
}
```



