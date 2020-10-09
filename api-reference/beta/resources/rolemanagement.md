---
title: roleManagement 资源类型
description: RBAC 角色管理资源
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 531412e826d730b634ff7506386963e0e465127b
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48400601"
---
# <a name="rolemanagement-resource-type"></a>roleManagement 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Microsoft 365 RBAC 角色管理实体。 提供对在 RBAC 提供程序中呈现的角色定义和角色分配的访问权限。 当前目录 (支持 Azure AD) 和 deviceManagement (Intune) 提供程序。 

有关详细信息，请参阅： 
* [Azure Active Directory 中的管理员角色权限](/azure/active-directory/users-groups-roles/directory-assign-admin-roles)。
* [使用 Microsoft Intune (RBAC) 的基于角色的访问控制](/mem/intune/fundamentals/role-based-access-control)

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性

无。

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|文件夹|[rbacApplication](rbacapplication.md)| 只读。 可为 NULL。|
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