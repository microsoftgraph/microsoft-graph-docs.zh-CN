---
title: roleManagement 资源类型
description: RBAC 角色管理资源
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 3997ccd1d08637a7662b6f7c2f21712936259337
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534023"
---
# <a name="rolemanagement-resource-type"></a>roleManagement 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示一Microsoft 365 RBAC 角色管理实体，该实体提供对各种 RBAC 提供程序显示的角色定义和角色分配的访问权限。 

统一角色管理 API 当前支持以下 RBAC Microsoft 365：
- 云电脑 
- Intune (设备) 
- directory (Azure AD directory roles) 
- 授权管理 (Azure AD 权利管理) 
 
有关更多信息，请参阅： 
* [Microsoft 365中的角色，包括 Azure AD、特定于服务和跨服务的角色](/azure/active-directory/roles/concept-understand-roles#how-azure-ad-roles-are-different-from-other-microsoft-365-roles) 
* [Azure Active Directory 中的管理员角色权限](/azure/active-directory/users-groups-roles/directory-assign-admin-roles)。
* [Azure AD 权利管理中的委派和角色](/azure/active-directory/governance/entitlement-management-delegate)。
* [Microsoft Intune 中的基于角色的访问控制 (RBAC)](/mem/intune/fundamentals/role-based-access-control)。

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性

无。

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|cloudPC|[rbacApplicationMultiple](rbacapplicationmultiple.md)|提供对云电脑 RBAC 提供程序的角色定义和角色分配的访问权限。 只读。 可为空。|
|deviceManagement|[rbacApplicationMultiple](rbacapplicationmultiple.md)| 提供对 Intune RBAC 提供程序的角色定义和角色分配的访问权限。 只读。 可为空。|
|directory|[rbacApplication](rbacapplication.md)|提供对 Azure AD RBAC 提供程序的角色定义和角色分配的访问权限。 只读。 可为空。|
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
