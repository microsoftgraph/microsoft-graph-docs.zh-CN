---
title: roleAssignment 资源类型
description: 角色分配资源。 角色分配将角色定义与成员和作用域绑定在一起。 每个角色可以具有一个或多个角色分配。 这适用于自定义和内置角色。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0afe1b3bbc06d634759e98aa6f04765177fb2126
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58806920"
---
# <a name="roleassignment-resource-type"></a>roleAssignment 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

角色分配资源。 角色分配将角色定义与成员和作用域绑定在一起。 每个角色可以具有一个或多个角色分配。 这适用于自定义和内置角色。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List roleAssignments](../api/intune-rbac-roleassignment-list.md)|[roleAssignment](../resources/intune-rbac-roleassignment.md) 集合|列出 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象的属性和关系。|
|[Get roleAssignment](../api/intune-rbac-roleassignment-get.md)|[roleAssignment](../resources/intune-rbac-roleassignment.md)|读取 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象的属性和关系。|
|[Create roleAssignment](../api/intune-rbac-roleassignment-create.md)|[roleAssignment](../resources/intune-rbac-roleassignment.md)|创建新的 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象。|
|[Delete roleAssignment](../api/intune-rbac-roleassignment-delete.md)|无|删除 [roleAssignment](../resources/intune-rbac-roleassignment.md)。|
|[Update roleAssignment](../api/intune-rbac-roleassignment-update.md)|[roleAssignment](../resources/intune-rbac-roleassignment.md)|更新 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 此为只读，且自动生成。|
|displayName|String|角色分配的显示或友好名称。|
|description|String|角色分配的说明。|
|scopeMembers|String collection|角色作用域成员安全组的 ID 列表。  这些是 Azure Active Directory 中的 ID。|
|scopeType|[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md)|指定角色分配的范围类型。 默认类型"ResourceScope"允许分配 ResourceScopes。 对于"AllDevices"、"AllLicensedUsers"和"AllDevicesAndLicensedUsers"，ResourceScopes 属性应留空。 可能的值是：`resourceScope`、`allDevices`、`allLicensedUsers`、`allDevicesAndLicensedUsers`。|
|resourceScopes|String collection|角色作用域成员安全组的 ID 列表。  这些是 Azure Active Directory 中的 ID。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|roleDefinition|[roleDefinition](../resources/intune-rbac-roledefinition.md)|此分配所属的角色定义。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "scopeMembers": [
    "String"
  ],
  "scopeType": "String",
  "resourceScopes": [
    "String"
  ]
}
```



