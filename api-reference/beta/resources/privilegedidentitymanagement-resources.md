---
title: Privileged Identity Management - Azure 资源
description: 使用适合于 Azure AD Privileged Identity Management 的 API 管理 Azure 资源。
ms.localizationpriority: high
author: carolinetempleton
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: ec3c67b8ffcb35a223f1491a40bab55e92563c28
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "64477928"
---
# <a name="privileged-identity-management---azure-resources"></a>Privileged Identity Management - Azure 资源

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2ResourceRoles-deprecation](../../includes/pim-v2ResourceRoles-deprecation.md)]

可以将 [Azure Active Directory (Azure AD) 特权标识管理 (PIM)](/azure/active-directory/privileged-identity-management/pim-configure) 用于 Azure 资源，以在管理组、订阅、资源组和资源级别为 Azure 基础结构角色设置即时访问工作流。其中包括所有者和参与者等内置角色以及自定义 RBAC 角色。

## <a name="common-use-cases-for-pim-and-azure-resources-using-a-rest-api"></a>使用 REST API 的 PIM 和 Azure 资源的常见用例

| 用例 | 资源 | 另请参阅 |
| --- | --- | --- |
| 为 PIM 管理载入资源（订阅、资源组、资源等），列出请求者可访问的所有托管资源并检索托管资源的关系。 | [governanceResource](governanceresource.md) | [角色发现和管理](/azure/active-directory/privileged-identity-management/pim-resource-roles-discover-resources) |
| 列出资源的所有角色，或者特定资源中的特殊角色的详细信息。 | [governanceRoleDefinition](governanceroledefinition.md) |  |
| 检索资源的所有角色设置，或更新角色设置 | [governanceRoleSetting](governancerolesetting.md) | [配置角色设置](/azure/active-directory/privileged-identity-management/pim-resource-roles-configure-role-settings) |
| 列出并导出资源的所有角色分配。 | [governanceRoleAssignment](governanceroleassignment.md) | [导出角色分配](/azure/active-directory/privileged-identity-management/azure-pim-resource-rbac#export-role-assignments-with-children) |
| 创建或删除符合条件或活动的角色分配，激活/禁用符合条件的分配，查看待处理请求列表，批准或拒绝待处理请求或取消自己的待处理请求。 | [governanceRoleAssignmentRequest](governanceroleassignmentrequest.md) | [角色分配](/azure/active-directory/privileged-identity-management/pim-resource-roles-assign-roles)<br/>[角色激活](/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles)<br/>[审批请求](/azure/active-directory/privileged-identity-management/azure-ad-pim-approval-workflow) |

[!INCLUDE [pimv2AzureResources-migration](../../includes/pimv2AzureResources-migration.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
