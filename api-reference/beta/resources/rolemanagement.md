---
title: roleManagement 资源类型
description: RBAC 角色管理资源
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 71c59c1e44123b60dd46b2c72e71aabfc7a64c25
ms.sourcegitcommit: feebe30e62aa19ce5cb8e8338e043326e464ed9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991780"
---
# <a name="rolemanagement-resource-type"></a>roleManagement 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Microsoft 365 RBAC 角色管理实体。 提供对在 RBAC 提供程序中呈现的角色定义和角色分配的访问权限。 支持当前目录（Azure AD）和 deviceManagement （Intune）提供程序。 

有关详细信息，请参阅： 
* [Azure Active Directory 中的管理员角色权限](/azure/active-directory/users-groups-roles/directory-assign-admin-roles)。
* [使用 Microsoft Intune 的基于角色的访问控制（RBAC）](https://docs.microsoft.com/mem/intune/fundamentals/role-based-access-control)

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性

无。

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|文件夹|[rbacApplication](rbacapplication.md)| 只读。 可为 Null。|
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
