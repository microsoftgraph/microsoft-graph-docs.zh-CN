---
title: roleManagement 资源类型
description: RBAC 角色管理资源
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 241de0b72a9ffad507975fca408fe49f0b0a90f0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440122"
---
# <a name="rolemanagement-resource-type"></a>roleManagement 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表 Microsoft 365 RBAC 角色管理实体。 提供对 RBAC 提供程序中出现的角色定义和角色分配的访问权限。 目前， (支持 Azure AD) 和 deviceManagement (Intune) 目录。 

有关详细信息，请参阅： 
* [Azure Active Directory 中的管理员角色权限](/azure/active-directory/users-groups-roles/directory-assign-admin-roles)。
* [使用 Microsoft Intune (基于角色) RBAC](/mem/intune/fundamentals/role-based-access-control)

## <a name="methods"></a>Methods

无。

## <a name="properties"></a>属性

无。

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|目录|[rbacApplication](rbacapplication.md)| 只读。 可为 NULL。|
|deviceManagement|[rbacApplicationMultiple](rbacapplicationmultiple.md)| 只读。可为空。|

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
