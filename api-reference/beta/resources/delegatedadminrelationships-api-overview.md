---
title: GDAP) API 概述 (粒度委派的管理员权限
description: GDAP) GDAP (粒度委派的管理员权限允许 Microsoft 合作伙伴配置和请求对其客户环境的粒度和时间限制的访问权限，从而允许客户对 Microsoft 合作伙伴强制实施最低特权的访问权限。
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: resourcePageType
ms.openlocfilehash: 2d4876f6017219c655b38bc303ce6bbca81db8d2
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65821246"
---
# <a name="granular-delegated-admin-privileges-gdap-api-overview"></a>GDAP) API 概述 (粒度委派的管理员权限

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

作为 Microsoft 合作伙伴中心生态系统的一部分，云解决方案提供商、增值经销商或顾问程序中的 Microsoft 合作伙伴可以对其客户租户执行管理操作，以帮助管理客户的服务，例如 Azure AD 和Microsoft 365。 此功能以前允许合作伙伴无限期地在客户租户中担任全局管理员角色，从而产生潜在的安全风险并限制市场潜力。

**GDAP (粒度委派的管理员权限)** 为合作伙伴提供对客户租户的最低特权访问权限，遵循 [零信任网络安全模型](/security/zero-trust/)。 通过 GDAP，合作伙伴配置并请求对其客户环境的粒度和限时访问权限，客户必须显式向合作伙伴授予此最低特权的访问权限。 此外，合作伙伴必须在一定的时间内请求客户租户管理的特定角色。 此控件消除了合作伙伴在其客户的租户中具有全局管理员角色的需求，但是，他们现在拥有委派的管理任务绝对需要的特权更低的权限。

有关 GDAP 的详细信息，请参阅：
+ [GDAP)  (粒度委派管理员权限简介 ](/partner-center/gdap-introduction)
+ [按任务分配的最小特权角色](/partner-center/gdap-least-privileged-roles-by-task)

## <a name="use-cases-for-gdap-apis"></a>GDAP API 的用例

本部分介绍 Microsoft 合作伙伴使用 GDAP API 以编程方式管理客户委派的管理员关系的方式。

### <a name="delegated-admin-relationship"></a>委派的管理员关系

| 用例 | API |
|--|--|
| 创建新的委派管理员关系以供任何客户批准 <br/> 创建新的委派管理员关系以供特定客户批准 | [创建 delegatedAdminRelationship](../api/tenantrelationship-post-delegatedadminrelationships.md) |
| 列出合作伙伴的所有委派管理员关系 <br/> 列出特定客户的所有委派管理员关系 | [列出 delegatedAdminRelationships](../api/tenantrelationship-list-delegatedadminrelationships.md) |
| 按 ID 获取委派的管理员关系 | [获取 delegatedAdminRelationship](../api/delegatedadminrelationship-get.md)  |
| 删除委派的管理员关系 | [删除 delegatedAdminRelationship](../api/delegatedadminrelationship-delete.md) |

### <a name="delegated-admin-relationship-request"></a>委派的管理员关系请求

| 用例 | API |
|--|--|
| 创建委托的管理员关系请求，锁定关系以供客户批准或终止现有关系。 | [创建请求](../api/delegatedadminrelationship-post-requests.md) |
| 按 ID 获取委派的管理员关系请求 | [获取 delegatedAdminRelationshipRequest](../api/delegatedadminrelationshiprequest-get.md) |
| 列出给定关系的所有委派管理员关系请求 | [列出请求](../api/delegatedadminrelationship-list-requests.md) |


### <a name="role-assignments"></a>角色分配

| 用例 | API |
|--|--|
| 为委派的管理员关系创建新的委派管理员访问分配 | [创建 accessAssignments](../api/delegatedadminrelationship-post-accessassignments.md) |
| 列出委派管理关系的访问分配 | [列出 accessAssignments](../api/delegatedadminrelationship-list-accessassignments.md) |
| 按 ID 获取委派的管理员关系访问分配 | [获取 delegatedAdminAccessAssignment](../api/delegatedadminaccessassignment-get.md) |
| 删除委派管理员关系的访问分配 | [删除 delegatedAdminAccessAssignment](../api/delegatedadminaccessassignment-delete.md) |
| 更新委派管理员关系访问分配的角色分配 | [更新 delegatedAdminAccessAssignment](../api/delegatedadminaccessassignment-update.md) |

### <a name="long-running-operations"></a>长时间运行的操作

| 用例 | API |
|--|--|
| 列出委派管理关系的所有长时间运行的操作 | [列举操作](../api/delegatedadminrelationship-list-operations.md) |
| 获取委派的管理员关系的长时间运行操作 | [获取 delegatedAdminRelationshipOperation](../api/delegatedadminrelationshipoperation-get.md) |


### <a name="delegated-admin-customers"></a>委派的管理员客户

| 用例 | API |
|--|--|
| 列出所有委派的管理员客户 | [列出 delegatedAdminCustomers](../api/tenantrelationship-list-delegatedadmincustomers.md)|
| 按 ID 获取单个委派的管理员客户 | [获取 delegatedAdminCustomer](../api/delegatedadmincustomer-get.md) |
| 获取委派管理员客户的服务管理详细信息 | [List serviceManagementDetails](../api/delegatedadmincustomer-list-servicemanagementdetails.md) |


## <a name="gdap-workflow"></a>GDAP 工作流

### <a name="gdap-relationship-status-transition"></a>GDAP 关系状态转换

委派管理员关系转换的状态如下所示：

![委托管理员关系状态转换图](relationship-status-transitions.png)

1. [创建 delegatedAdminRelationship](../api/tenantrelationship-post-delegatedadminrelationships.md)
2. [更新 delegatedAdminRelationship](../api/delegatedadminrelationship-update.md)
3. [创建 delegatedAdminRelationshipRequest](../api/delegatedadminrelationship-post-requests.md) (操作：lockForApproval) 
4. [创建 delegatedAdminRelationshipRequest](../api/delegatedadminrelationship-post-requests.md) (操作：终止) 

### <a name="gdap-relationship-access-assignment-status-transition"></a>GDAP 关系访问分配状态转换

委派管理员访问分配的状态。 状态转换如下所示：

![委派管理员访问分配状态转换关系图](access-assignment-status-transitions.png)

1. [创建 delegatedAdminAccessAssignment](../api/delegatedadminrelationship-post-accessassignments.md)
2. [删除 delegatedAdminAccessAssignment](../api/delegatedadminaccessassignment-delete.md)

## <a name="permissions"></a>权限

若要管理委派的管理员关系，调用主体必须在合作伙伴租户中，并被授予适当的 [粒度委派管理员权限](/graph/permissions-reference#delegated-admin-relationship-permissions)。


## <a name="see-also"></a>另请参阅

+ [GDAP)  (粒度委派管理员权限简介 ](/partner-center/gdap-introduction)