---
title: roleAssignment 资源类型
description: 表示托管租户的已登录用户的角色分配。
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 8455036941676bd304f12d957220dd982530b6db
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096352"
---
# <a name="roleassignment-resource-type"></a>roleAssignment 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示托 [管租户](../resources/managedtenants-tenant.md)的已登录用户的角色分配。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|assignmentType|delegatedPrivilegeStatus|与角色分配关联 () 管理关系的类型。 可取值为：`none`、`delegatedAdminPrivileges`、`unknownFutureValue`、`granularDelegatedAdminPrivileges`、`delegatedAndGranularDelegetedAdminPrivileges`。 请注意，必须使用`Prefer: include-unknown-enum-members`请求标头从此[可旋转枚举](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations)中获取以下值： `granularDelegatedAdminPrivileges` `delegatedAndGranularDelegetedAdminPrivileges`|
|roles|[microsoft.graph.managedTenants.roleDefinition](../resources/managedtenants-roledefinition.md) 集合|分配的角色的集合。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.roleAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.roleAssignment",
  "assignmentType": "String",
  "roles": [
    {
      "@odata.type": "microsoft.graph.managedTenants.roleDefinition"
    }
  ]
}
```
