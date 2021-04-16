---
title: deviceHealthScriptAssignment 资源类型
description: 包含用于将设备管理脚本分配给组的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 276104e49a12ff64fcbc585b3a5ce07570377397
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867325"
---
# <a name="devicehealthscriptassignment-resource-type"></a>deviceHealthScriptAssignment 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含用于将设备管理脚本分配给组的属性。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceHealthScriptAssignments](../api/intune-devices-devicehealthscriptassignment-list.md)|[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) 集合|列出 [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) 对象的属性和关系。|
|[获取 deviceHealthScriptAssignment](../api/intune-devices-devicehealthscriptassignment-get.md)|[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)|读取 [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) 对象的属性和关系。|
|[创建 deviceHealthScriptAssignment](../api/intune-devices-devicehealthscriptassignment-create.md)|[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)|创建新的 [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) 对象。|
|[删除 deviceHealthScriptAssignment](../api/intune-devices-devicehealthscriptassignment-delete.md)|无|删除 [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)。|
|[更新 deviceHealthScriptAssignment](../api/intune-devices-devicehealthscriptassignment-update.md)|[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)|更新 [deviceHealthScriptAssignment 对象](../resources/intune-devices-devicehealthscriptassignment.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设备运行状况脚本分配实体的键。 此属性是只读的。|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|我们将脚本定向到的 Azure Active Directory 组|
|runRemediationScript|Boolean|确定是仅运行检测脚本还是同时运行检测脚本和修正脚本|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceHealthScriptAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  },
  "runRemediationScript": true
}
```




