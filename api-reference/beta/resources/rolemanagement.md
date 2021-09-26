---
title: roleManagement 资源类型
description: RBAC 角色管理资源
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: e401d0442c25ffcacb5887a0033c1d149ed51380
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59766745"
---
# <a name="rolemanagement-resource-type"></a>roleManagement 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示一Microsoft 365 RBAC 角色管理实体，该实体提供对各种 RBAC 提供程序显示的角色定义和角色分配的访问权限。 

统一角色管理 API 当前支持以下 RBAC Microsoft 365：
- 云电脑 
- Intune (设备) 
-  (Azure AD 目录角色) 
- Azure AD (权限管理策略中的授权) 
 
有关详细信息，请参阅： 
* [Microsoft 365中的角色，包括 Azure AD、特定于服务和跨服务的角色](/azure/active-directory/roles/concept-understand-roles#how-azure-ad-roles-are-different-from-other-microsoft-365-roles) 
* [Azure Active Directory 中的管理员角色权限](/azure/active-directory/users-groups-roles/directory-assign-admin-roles)。
* [Azure AD 权利管理中的委派和角色](/azure/active-directory/governance/entitlement-management-delegate)。
* [Microsoft Intune 中的基于角色的访问控制 (RBAC)](/mem/intune/fundamentals/role-based-access-control)。

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性

无。

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|cloudPC|[rbacApplicationMultiple](rbacapplicationmultiple.md)|提供对云电脑 RBAC 提供程序的角色定义和角色分配的访问权限。 只读。 可为 null。|
|deviceManagement|[rbacApplicationMultiple](rbacapplicationmultiple.md)| 提供对 Intune RBAC 提供程序的角色定义和角色分配的访问权限。 只读。 可为 null。|
|directory|[rbacApplication](rbacapplication.md)|提供对 Azure AD RBAC 提供程序的角色定义和角色分配的访问权限。 只读。 可为 null。|
|entitlementManagement|[rbacApplication](rbacapplication.md)| 提供对 Azure AD 权利管理的角色定义和角色分配的访问权限。 只读。 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

无。

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "roleManagement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
