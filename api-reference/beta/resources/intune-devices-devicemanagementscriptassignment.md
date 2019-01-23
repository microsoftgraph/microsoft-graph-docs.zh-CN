---
title: deviceManagementScriptAssignment 资源类型
description: 包含用于分配给组的设备管理脚本的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c6e153842e0b820a845260bc125154df7cef0cb8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413848"
---
# <a name="devicemanagementscriptassignment-resource-type"></a>deviceManagementScriptAssignment 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含用于分配给组的设备管理脚本的属性。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 deviceManagementScriptAssignments](../api/intune-devices-devicemanagementscriptassignment-list.md)|[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)集合|列出属性和[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象之间的关系。|
|[获取 deviceManagementScriptAssignment](../api/intune-devices-devicemanagementscriptassignment-get.md)|[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)|读取属性和[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象的关系。|
|[创建 deviceManagementScriptAssignment](../api/intune-devices-devicemanagementscriptassignment-create.md)|[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)|创建新的[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象。|
|[删除 deviceManagementScriptAssignment](../api/intune-devices-devicemanagementscriptassignment-delete.md)|无|删除[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)。|
|[更新 deviceManagementScriptAssignment](../api/intune-devices-devicemanagementscriptassignment-update.md)|[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)|更新[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设备管理脚本组工作分配实体的键。|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Azure Active Directory 组的 Id 目标脚本。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




