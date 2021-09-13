---
title: rbacApplication 资源类型
description: 基于角色的访问控制Microsoft 365 RBAC 提供程序的角色定义 (角色) 容器
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: eeb36364691fb31f30bde2313598b62ab06f950f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59148503"
---
# <a name="rbacapplication-resource-type"></a>rbacApplication 资源类型

命名空间：microsoft.graph

用于基于角色的访问控制或 RBAC 提供程序Microsoft 365统一角色定义 (角色) 容器。 角色分配仅支持单个主体和单个作用域。 目前 **，目录** 是唯一受支持的 RBAC 提供程序。

## <a name="methods"></a>方法

无

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
