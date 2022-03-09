---
title: rbacApplication 资源类型
description: 基于角色的访问控制Microsoft 365 RBAC 提供程序的角色定义 (角色) 容器
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 294bf357465002a180549e5654fbfd7f2baabac6
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63393471"
---
# <a name="rbacapplication-resource-type"></a>rbacApplication 资源类型

命名空间：microsoft.graph

用于基于角色的访问控制提供程序的统一角色定义Microsoft 365角色分配 (RBAC) 容器。 角色分配仅支持单个主体和单个作用域。 目前 **，目录****和 entitlementManagement** 是支持的两个 RBAC 提供程序。

## <a name="methods"></a>方法

None

## <a name="properties"></a>属性

无

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|roleAssignments|[unifiedRoleAssignment](../resources/unifiedroleassignment.md) 集合| 向用户或组授予访问权限的资源。 |
|roleDefinitions|[unifiedRoleDefinition](../resources/unifiedroledefinition.md) 集合| 表示 RBAC 提供程序允许的角色以及分配给角色的权限的资源。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rbacApplication",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rbacApplication"
}
```
