---
title: roleManagement 资源类型
description: Microsoft 365基于角色的访问控制 (RBAC) 资源。
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 055e90c1fe006cf7babfdea4f7c585d66ff295d0
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63394507"
---
# <a name="rolemanagement-resource-type"></a>roleManagement 资源类型

命名空间：microsoft.graph

表示基于Microsoft 365角色的访问控制 (RBAC) 角色管理实体。 此资源提供对 RBAC 提供程序中提供的角色定义和角色分配的访问权限。 **directory** (Azure Active Directory) 、**entitlementManagement** 和 **deviceManagement** (Intune) 提供程序当前受支持。

有关更多信息，请参阅： 
* [Azure Active Directory 中的管理员角色权限](/azure/active-directory/roles/custom-overview)。
* [授权管理中的Azure AD角色](/azure/active-directory/governance/entitlement-management-delegate)。
* [Microsoft Intune 中的基于角色的访问控制 (RBAC)](/mem/intune/fundamentals/role-based-access-control)。

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性

无。

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|directory|[rbacApplication](rbacapplication.md)| 只读。可为 Null。|
|entitlementManagement|[rbacApplication](rbacapplication.md)| 权利管理资源 [的角色和分配的](entitlementmanagement.md) 容器。|

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