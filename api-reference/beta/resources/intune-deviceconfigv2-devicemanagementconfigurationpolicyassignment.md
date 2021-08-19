---
title: deviceManagementConfigurationPolicyAssignment 资源类型
description: DeviceManagementConfigurationPolicyAssignment 实体将特定 DeviceManagementConfigurationPolicy 分配给 AAD 组。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2b5b7feec442991265c358fbfbd7e7ae2dbd2754
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58265009"
---
# <a name="devicemanagementconfigurationpolicyassignment-resource-type"></a>deviceManagementConfigurationPolicyAssignment 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

DeviceManagementConfigurationPolicyAssignment 实体将特定 DeviceManagementConfigurationPolicy 分配给 AAD 组。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementConfigurationPolicyAssignments](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-list.md)|[deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) 集合|列出 [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) 对象的属性和关系。|
|[获取 deviceManagementConfigurationPolicyAssignment](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-get.md)|[deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|读取 [deviceManagementConfigurationPolicyAssignment 对象的属性和](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) 关系。|
|[创建 deviceManagementConfigurationPolicyAssignment](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-create.md)|[deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|创建新的 [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) 对象。|
|[删除 deviceManagementConfigurationPolicyAssignment](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-delete.md)|无|删除 [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)。|
|[更新 deviceManagementConfigurationPolicyAssignment](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-update.md)|[deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|更新 [deviceManagementConfigurationPolicyAssignment 对象](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|分配的键。|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|DeviceManagementConfigurationPolicy 的分配目标。|
|source|[deviceAndAppManagementAssignmentSource](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|设备合规性策略的分配源，即 direct 或更新/policySet。 可取值为：`direct`、`policySets`。|
|sourceId|String|工作分配的源的标识符。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationPolicyAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  },
  "source": "String",
  "sourceId": "String"
}
```




