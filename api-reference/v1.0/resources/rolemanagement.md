---
title: roleManagement 资源类型
description: Microsoft 365基于角色的访问控制 (RBAC) 资源。
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 6f28f6e682ebba03740e5cd07d17de838d2aea18
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59097837"
---
# <a name="rolemanagement-resource-type"></a>roleManagement 资源类型

命名空间：microsoft.graph

表示基于Microsoft 365角色的访问控制 (RBAC) 角色管理实体。 此资源提供对 RBAC 提供程序中提供的角色定义和角色分配的访问权限。 **directory** (Azure Active Directory) 和 **deviceManagement** (Intune) 提供程序当前受支持。

有关详细信息，请参阅： 
* [Azure Active Directory 中的管理员角色权限](/azure/active-directory/roles/custom-overview)。
* [Microsoft Intune 中的基于角色的访问控制 (RBAC)](/mem/intune/fundamentals/role-based-access-control)。

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性

无。

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|directory|[rbacApplication](rbacapplication.md)| 只读。可为空。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.roleManagement",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleManagement"
}
```