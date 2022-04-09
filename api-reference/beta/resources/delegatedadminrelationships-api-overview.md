---
title: " (DAP) API 概述委派的管理员权限"
description: 委派的管理员权限允许 Microsoft 合作伙伴配置和请求对其客户环境的粒度和时间限制的访问权限，从而允许客户对 Microsoft 合作伙伴强制实施最低特权的访问权限。
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: resourcePageType
ms.openlocfilehash: 2c59e78f1b8f2da00eaf56b4d24c09cbad397941
ms.sourcegitcommit: 1e8ba243e77ca344e267f16dfeb321fb5a7463e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2022
ms.locfileid: "64733261"
---
# <a name="delegated-admin-privileges-dap-api-overview"></a> (DAP) API 概述委派的管理员权限

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

作为 Microsoft 合作伙伴中心生态系统的一部分，云解决方案提供商、增值经销商或顾问计划中的 Microsoft 合作伙伴可以对其客户租户执行管理操作，以帮助管理客户的服务，例如Azure AD和Microsoft 365。 此功能以前允许合作伙伴无限期地在客户租户中担任全局管理员角色，从而产生潜在的安全风险并限制市场潜力。

**委派的管理员权限 (DAP)** 为合作伙伴提供对客户租户的最低特权访问权限，遵循 [零信任网络安全模型](/security/zero-trust/)。 通过 DAP，合作伙伴配置并请求对客户环境的粒度和限时访问权限，客户必须显式向合作伙伴授予此最低特权的访问权限。 此外，合作伙伴必须在一定的时间内请求客户租户管理的特定角色。 此控件消除了合作伙伴在其客户的租户中具有全局管理员角色的需求，但是，他们现在拥有委派的管理任务绝对需要的特权更低的权限。

有关 DAP 的详细信息，请参阅：
+ [GDAP)  (粒度委派管理员权限简介 ](/partner-center/gdap-introduction)
+ [按任务分配的最小特权角色](/partner-center/gdap-least-privileged-roles-by-task)

## <a name="use-cases-for-delegated-admin-apis"></a>委派管理员 API 的用例

本部分介绍 Microsoft 合作伙伴以编程方式管理客户委派的管理员关系的方式。

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

## <a name="permissions"></a>权限

若要管理委派的管理员关系，调用主体必须在合作伙伴租户中，并被授予适当的 [委派管理员权限](/graph/permissions-reference#delegated-admin-relationship-permissions)。
