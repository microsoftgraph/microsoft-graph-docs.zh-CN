---
title: roleScopeTagAutoAssignment 资源类型
description: 包含用于将角色作用域标记自动分配给要应用于设备的组的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 63a6800281731b4c96fef0524658d7aca6171e37
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42773131"
---
# <a name="rolescopetagautoassignment-resource-type"></a>roleScopeTagAutoAssignment 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含用于将角色作用域标记自动分配给要应用于设备的组的属性。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 roleScopeTagAutoAssignments](../api/intune-rbac-rolescopetagautoassignment-list.md)|[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)集合|列出[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)对象的属性和关系。|
|[获取 roleScopeTagAutoAssignment](../api/intune-rbac-rolescopetagautoassignment-get.md)|[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)|读取[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)对象的属性和关系。|
|[创建 roleScopeTagAutoAssignment](../api/intune-rbac-rolescopetagautoassignment-create.md)|[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)|创建新的[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)对象。|
|[删除 roleScopeTagAutoAssignment](../api/intune-rbac-rolescopetagautoassignment-delete.md)|None|删除[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)。|
|[更新 roleScopeTagAutoAssignment](../api/intune-rbac-rolescopetagautoassignment-update.md)|[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)|更新[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|特定角色范围标记的自动分配目标。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleScopeTagAutoAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



