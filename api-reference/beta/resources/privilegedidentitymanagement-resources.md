---
title: Privileged Identity Management - Azure 资源
description: 使用适合于 Azure AD Privileged Identity Management 的 API 管理 Azure 资源。
localization_priority: Priority
ms.openlocfilehash: b4b6a85e92784c14f95003e2e6d7d18ebde89b74
ms.sourcegitcommit: f80282ff00d5aafc3e575bce447543d7dd23963d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/23/2019
ms.locfileid: "34425143"
---
# <a name="privileged-identity-management---azure-resources"></a><span data-ttu-id="1dcd0-103">Privileged Identity Management - Azure 资源</span><span class="sxs-lookup"><span data-stu-id="1dcd0-103">Privileged Identity Management - Azure resources</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1dcd0-104">可以使用适合于 Azure 资源的 [Azure Active Directory (Azure AD) Privileged Identity Management (PIM)](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure) 为管理组、订阅、资源组和资源级别的 Azure 基础结构角色设置实时访问工作流。</span><span class="sxs-lookup"><span data-stu-id="1dcd0-104">You can use [Azure Active Directory (Azure AD) Privileged Identity Management (PIM)](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure) for Azure resources to set up just-in-time access workflow for your Azure infrastructure roles at a management group, subscription, resource group, and resource level.</span></span> <span data-ttu-id="1dcd0-105">这些包括诸如所有者和参与者之类的内置角色以及自定义 RBAC 角色。</span><span class="sxs-lookup"><span data-stu-id="1dcd0-105">These include built-in roles like Owner and Contributor as well as custom RBAC roles.</span></span>

## <a name="common-use-cases-for-pim-and-azure-resources-using-a-rest-api"></a><span data-ttu-id="1dcd0-106">使用 REST API 的 PIM 和 Azure 资源的常见用例</span><span class="sxs-lookup"><span data-stu-id="1dcd0-106">Common use cases for PIM and Azure resources using a REST API</span></span>

| <span data-ttu-id="1dcd0-107">用例</span><span class="sxs-lookup"><span data-stu-id="1dcd0-107">Use case</span></span> | <span data-ttu-id="1dcd0-108">资源</span><span class="sxs-lookup"><span data-stu-id="1dcd0-108">Resource</span></span> | <span data-ttu-id="1dcd0-109">另请参阅</span><span class="sxs-lookup"><span data-stu-id="1dcd0-109">See also</span></span> |
| --- | --- | --- |
| <span data-ttu-id="1dcd0-110">为 PIM 管理载入资源（订阅、资源组、资源等），列出请求者可访问的所有托管资源并检索托管资源的关系。</span><span class="sxs-lookup"><span data-stu-id="1dcd0-110">Onboard a resource (subscriptions, resource group, resource etc.) for PIM management, list all the managed resources requester have access to, and retrieve relationships of a managed resource.</span></span> | [<span data-ttu-id="1dcd0-111">governanceResource</span><span class="sxs-lookup"><span data-stu-id="1dcd0-111">governanceResource</span></span>](governanceresource.md) | [<span data-ttu-id="1dcd0-112">角色发现和管理</span><span class="sxs-lookup"><span data-stu-id="1dcd0-112">Role discovery and management</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-discover-resources) |
| <span data-ttu-id="1dcd0-113">列出资源的所有角色，或者特定资源中的特殊角色的详细信息。</span><span class="sxs-lookup"><span data-stu-id="1dcd0-113">List all the roles for a resource or get details of a particular role in a specified resource.</span></span> | [<span data-ttu-id="1dcd0-114">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="1dcd0-114">governanceRoleDefinition</span></span>](governanceroledefinition.md) |  |
| <span data-ttu-id="1dcd0-115">检索资源的所有角色设置，或更新角色设置</span><span class="sxs-lookup"><span data-stu-id="1dcd0-115">Retrieve all role settings for a resource or make an update to a role setting</span></span> | [<span data-ttu-id="1dcd0-116">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="1dcd0-116">governanceRoleSetting</span></span>](governancerolesetting.md) | [<span data-ttu-id="1dcd0-117">配置角色设置</span><span class="sxs-lookup"><span data-stu-id="1dcd0-117">Configure role setting</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-configure-role-settings) |
| <span data-ttu-id="1dcd0-118">列出并导出资源的所有角色分配。</span><span class="sxs-lookup"><span data-stu-id="1dcd0-118">List and export all role assignments for a resource.</span></span> | [<span data-ttu-id="1dcd0-119">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="1dcd0-119">governanceRoleAssignment</span></span>](governanceroleassignment.md) | [<span data-ttu-id="1dcd0-120">导出角色分配</span><span class="sxs-lookup"><span data-stu-id="1dcd0-120">Export role assignments</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/azure-pim-resource-rbac#export-role-assignments-with-children) |
| <span data-ttu-id="1dcd0-121">创建或删除符合条件或活动的角色分配，激活/禁用符合条件的分配，查看待处理请求列表，批准或拒绝待处理请求或取消自己的待处理请求。</span><span class="sxs-lookup"><span data-stu-id="1dcd0-121">Create or remove an eligible or active role assignment, activate/deactivate an eligible assignment, view a list of pending requests, approve or deny a pending request or cancel your own pending request.</span></span> | [<span data-ttu-id="1dcd0-122">governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="1dcd0-122">governanceRoleAssignmentRequest</span></span>](governanceroleassignmentrequest.md) | [<span data-ttu-id="1dcd0-123">角色分配</span><span class="sxs-lookup"><span data-stu-id="1dcd0-123">Role assignment</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-assign-roles)<br/>[<span data-ttu-id="1dcd0-124">角色激活</span><span class="sxs-lookup"><span data-stu-id="1dcd0-124">Role activation</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles)<br/>[<span data-ttu-id="1dcd0-125">审批请求</span><span class="sxs-lookup"><span data-stu-id="1dcd0-125">Approve or deny requests</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/azure-ad-pim-approval-workflow) |

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
