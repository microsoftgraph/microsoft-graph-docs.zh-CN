---
title: deviceAndAppManagementRoleAssignment 资源类型
description: 角色分配资源。 角色分配将角色定义与成员和作用域绑定在一起。 每个角色可以具有一个或多个角色分配。 这适用于自定义和内置角色。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c391ccea9848e62b1ca5fcf58c2ae212669f00f1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369274"
---
# <a name="deviceandappmanagementroleassignment-resource-type"></a>deviceAndAppManagementRoleAssignment 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

角色分配资源。 角色分配将角色定义与成员和作用域绑定在一起。 每个角色可以具有一个或多个角色分配。 这适用于自定义和内置角色。


继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceAndAppManagementRoleAssignments](../api/intune-rbac-deviceandappmanagementroleassignment-list.md)|[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 集合|列出 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性和关系。|
|[获取 deviceAndAppManagementRoleAssignment](../api/intune-rbac-deviceandappmanagementroleassignment-get.md)|[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|读取 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性和关系。|
|[创建 deviceAndAppManagementRoleAssignment](../api/intune-rbac-deviceandappmanagementroleassignment-create.md)|[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|创建新的 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象。|
|[删除 deviceAndAppManagementRoleAssignment](../api/intune-rbac-deviceandappmanagementroleassignment-delete.md)|无|删除 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)。|
|[更新 deviceAndAppManagementRoleAssignment](../api/intune-rbac-deviceandappmanagementroleassignment-update.md)|[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|更新 [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|实体的键。 此为只读，且自动生成。 继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)|
|displayName|String|角色分配的显示或友好名称。 继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)|
|说明|String|角色分配的说明。 继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)|
|scopeMembers|String collection|角色作用域成员安全组的 ID 列表。  这些是 Azure Active Directory 中的 ID。 继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)|
|scopeType|[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md)|指定角色分配的作用域的类型。 默认类型 "ResourceScope" 允许分配 ResourceScopes。 对于 "AllDevices"、"AllLicensedUsers" 和 "AllDevicesAndLicensedUsers", ResourceScopes 属性应保留为空。 继承自[roleAssignment](../resources/intune-rbac-roleassignment.md)。 可取值为：`resourceScope`、`allDevices`、`allLicensedUsers`、`allDevicesAndLicensedUsers`。|
|resourceScopes|String collection|角色作用域成员安全组的 ID 列表。  这些是 Azure Active Directory 中的 ID。 继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)|
|members|String collection|角色成员安全组的 ID 列表。 这些是来自 Azure Active Directory 的 ID。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|roleDefinition|[roleDefinition](../resources/intune-rbac-roledefinition.md)|此分配所属的角色定义。 继承自 [roleAssignment](../resources/intune-rbac-roleassignment.md)|
|roleScopeTags|[roleScopeTag](../resources/intune-rbac-rolescopetag.md)集合|在角色分配上定义的一组角色范围标记。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAndAppManagementRoleAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "scopeMembers": [
    "String"
  ],
  "scopeType": "String",
  "resourceScopes": [
    "String"
  ],
  "members": [
    "String"
  ]
}
```



