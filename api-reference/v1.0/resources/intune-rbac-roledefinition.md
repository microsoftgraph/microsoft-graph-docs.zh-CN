---
title: roleDefinition 资源类型
description: 角色定义资源。 角色定义是在 Intune 中基于角色访问的基础。 角色组合了 Intune 资源（例如，移动应用）和关联的角色权限（例如，资源的创建和读取）。 有内置和自定义两种角色类型。 内置角色无法修改。 内置角色和自定义角色必须具有强制执行的分配。 如果要定义一个允许将任意可用资源和角色权限合并到单个角色中的角色，请创建自定义角色。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ff5403f7741191021d45aeb6dfb87b2a299f4b85
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751186"
---
# <a name="roledefinition-resource-type"></a>roleDefinition 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

角色定义资源。 角色定义是在 Intune 中基于角色访问的基础。 角色组合了 Intune 资源（例如，移动应用）和关联的角色权限（例如，资源的创建和读取）。 有内置和自定义两种角色类型。 内置角色无法修改。 内置角色和自定义角色必须具有强制执行的分配。 如果要定义一个允许将任意可用资源和角色权限合并到单个角色中的角色，请创建自定义角色。

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
|[List roleDefinitions](../api/intune-rbac-roledefinition-list.md)|[roleDefinition](../resources/intune-rbac-roledefinition.md) 集合|列出 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象的属性和关系。|
|[Get roleDefinition](../api/intune-rbac-roledefinition-get.md)|[roleDefinition](../resources/intune-rbac-roledefinition.md)|读取 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象的属性和关系。|
|[Create roleDefinition](../api/intune-rbac-roledefinition-create.md)|[roleDefinition](../resources/intune-rbac-roledefinition.md)|创建新的 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象。|
|[Delete roleDefinition](../api/intune-rbac-roledefinition-delete.md)|无|删除 [roleDefinition](../resources/intune-rbac-roledefinition.md)。|
|[Update roleDefinition](../api/intune-rbac-roledefinition-update.md)|[roleDefinition](../resources/intune-rbac-roledefinition.md)|更新 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 此为只读，且自动生成。|
|displayName|String|角色定义的显示名称。|
|说明|String|角色定义的说明。|
|rolePermissions|[rolePermission](../resources/intune-rbac-rolepermission.md) 集合|允许此角色执行的角色权限列表。 它们必须与定义为 rolePermission 一部分的 actionName 匹配。|
|isBuiltIn|Boolean|角色类型。 如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。|

## <a name="relationships"></a>关系
|关系|类型|Description|
|:---|:---|:---|
|roleAssignments|[roleAssignment](../resources/intune-rbac-roleassignment.md) 集合|此角色定义的角色分配列表|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
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
  "isBuiltIn": true
}
```




