---
title: deviceManagementConfigurationPolicyAssignment 资源类型
description: DeviceManagementConfigurationPolicyAssignment 实体将特定 DeviceManagementConfigurationPolicy 分配给 AAD 组。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5e571983c36c2832aef5c43478d1cccca7361aca
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157664"
---
# <a name="devicemanagementconfigurationpolicyassignment-resource-type"></a>deviceManagementConfigurationPolicyAssignment 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

DeviceManagementConfigurationPolicyAssignment 实体将特定 DeviceManagementConfigurationPolicy 分配给 AAD 组。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementConfigurationPolicyAssignments](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-list.md)|[deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) 集合|列出 [deviceManagementConfigurationPolicyAssignment 对象的属性和](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) 关系。|
|[获取 deviceManagementConfigurationPolicyAssignment](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-get.md)|[deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|读取 [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) 对象的属性和关系。|
|[创建 deviceManagementConfigurationPolicyAssignment](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-create.md)|[deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|创建新的 [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) 对象。|
|[删除 deviceManagementConfigurationPolicyAssignment](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-delete.md)|无|删除 [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)。|
|[更新 deviceManagementConfigurationPolicyAssignment](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-update.md)|[deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|更新 [deviceManagementConfigurationPolicyAssignment 对象](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|分配的键。|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|DeviceManagementConfigurationPolicy 的分配目标。|

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
  }
}
```




