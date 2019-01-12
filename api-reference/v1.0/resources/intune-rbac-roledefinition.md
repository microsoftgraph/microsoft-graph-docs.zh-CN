---
title: roleDefinition 资源类型
description: 角色定义资源。 角色定义是在 Intune 中基于角色访问的基础。 角色组合了 Intune 资源（例如，移动应用）和关联的角色权限（例如，资源的创建和读取）。 有内置和自定义两种角色类型。 内置角色无法修改。 内置角色和自定义角色必须具有强制执行的分配。 如果要定义一个允许将任意可用资源和角色权限合并到单个角色中的角色，请创建自定义角色。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: f09b94649f30909c2efc2d9851503b5b8db14127
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971870"
---
# <a name="roledefinition-resource-type"></a>roleDefinition 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

角色定义资源。 角色定义是在 Intune 中基于角色访问的基础。 角色组合了 Intune 资源（例如，移动应用）和关联的角色权限（例如，资源的创建和读取）。 有内置和自定义两种角色类型。 内置角色无法修改。 内置角色和自定义角色必须具有强制执行的分配。 如果要定义一个允许将任意可用资源和角色权限合并到单个角色中的角色，请创建自定义角色。
## <a name="methods"></a>方法
|方法|返回类型|说明|
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
|关系|类型|说明|
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



