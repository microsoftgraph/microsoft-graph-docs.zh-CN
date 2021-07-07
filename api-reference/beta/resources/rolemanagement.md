---
title: roleManagement 资源类型
description: RBAC 角色管理资源
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 42cad38bf690b6bb6958cfde99282f049a1a1d10
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317019"
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
 
有关详细信息，请参阅： 
* [Microsoft 365中的角色，包括 Azure AD、特定于服务和跨服务的角色](/azure/active-directory/roles/concept-understand-roles#how-azure-ad-roles-are-different-from-other-microsoft-365-roles) 
* [Azure Active Directory 中的管理员角色权限](/azure/active-directory/users-groups-roles/directory-assign-admin-roles)。
* [Azure AD 权利管理中的委派和角色](/azure/active-directory/governance/entitlement-management-delegate)。
* [Microsoft Intune 中的基于角色的访问控制 (RBAC)](/mem/intune/fundamentals/role-based-access-control)。

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>Methods

无。

## <a name="properties"></a>属性

无。

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|cloudPC|[rbacApplicationMultiple](rbacapplicationmultiple.md)|提供对云电脑 RBAC 提供程序的角色定义和角色分配的访问权限。 只读。 可为 Null。|
|deviceManagement|[rbacApplicationMultiple](rbacapplicationmultiple.md)| 提供对 Intune RBAC 提供程序的角色定义和角色分配的访问权限。 只读。 可为 Null。|
|directory|[rbacApplication](rbacapplication.md)|提供对 Azure AD RBAC 提供程序的角色定义和角色分配的访问权限。 只读。 可为 Null。|
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
