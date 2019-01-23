---
title: deviceAndAppManagementRoleDefinition 资源类型
description: 角色定义资源。 角色定义是在 Intune 中基于角色访问的基础。 角色组合了 Intune 资源（例如，移动应用）和关联的角色权限（例如，资源的创建和读取）。 有内置和自定义两种角色类型。 内置角色无法修改。 内置角色和自定义角色必须具有强制执行的分配。 如果要定义一个允许将任意可用资源和角色权限合并到单个角色中的角色，请创建自定义角色。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4cc3bd898799ef2c2da6fca5a0043fc86ee5bd8f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411979"
---
# <a name="deviceandappmanagementroledefinition-resource-type"></a>deviceAndAppManagementRoleDefinition 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

角色定义资源。 角色定义是在 Intune 中基于角色访问的基础。 角色组合了 Intune 资源（例如，移动应用）和关联的角色权限（例如，资源的创建和读取）。 有内置和自定义两种角色类型。 内置角色无法修改。 内置角色和自定义角色必须具有强制执行的分配。 如果要定义一个允许将任意可用资源和角色权限合并到单个角色中的角色，请创建自定义角色。


继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List deviceAndAppManagementRoleDefinitions](../api/intune-rbac-deviceandappmanagementroledefinition-list.md)|[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 集合|列出 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象的属性和关系。|
|[Get deviceAndAppManagementRoleDefinition](../api/intune-rbac-deviceandappmanagementroledefinition-get.md)|[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|读取 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象的属性和关系。|
|[Create deviceAndAppManagementRoleDefinition](../api/intune-rbac-deviceandappmanagementroledefinition-create.md)|[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|创建新的 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象。|
|[Delete deviceAndAppManagementRoleDefinition](../api/intune-rbac-deviceandappmanagementroledefinition-delete.md)|无|删除 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)。|
|[Update deviceAndAppManagementRoleDefinition](../api/intune-rbac-deviceandappmanagementroledefinition-update.md)|[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|更新 [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 此为只读，且自动生成。 继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)|
|displayName|String|角色定义的显示名称。 继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)|
|description|String|角色定义的说明。 继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)|
|permissions|[rolePermission](../resources/intune-rbac-rolepermission.md) 集合|允许此角色执行的角色权限列表。 它们必须与定义为 rolePermission 一部分的 actionName 匹配。 继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)|
|rolePermissions|[rolePermission](../resources/intune-rbac-rolepermission.md) 集合|允许此角色执行的角色权限列表。 它们必须与定义为 rolePermission 一部分的 actionName 匹配。 继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)|
|isBuiltInRoleDefinition|Boolean|角色类型。 如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。 继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)|
|isBuiltIn|Boolean|角色类型。 如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。 继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)|
|roleScopeTagIds|String 集合|此实体实例范围标记的列表。 继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|roleAssignments|[roleAssignment](../resources/intune-rbac-roleassignment.md) 集合|此角色定义的角色分配列表。 继承自 [roleDefinition](../resources/intune-rbac-roledefinition.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAndAppManagementRoleDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "permissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "String"
      ],
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "String"
          ],
          "notAllowedResourceActions": [
            "String"
          ]
        }
      ]
    }
  ],
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "String"
      ],
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "String"
          ],
          "notAllowedResourceActions": [
            "String"
          ]
        }
      ]
    }
  ],
  "isBuiltInRoleDefinition": true,
  "isBuiltIn": true,
  "roleScopeTagIds": [
    "String"
  ]
}
```




