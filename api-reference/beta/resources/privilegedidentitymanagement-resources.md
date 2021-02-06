---
title: Privileged Identity Management - Azure 资源
description: 使用适合于 Azure AD Privileged Identity Management 的 API 管理 Azure 资源。
localization_priority: Priority
author: shauliu
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: a64a60258369226ca58c4be070494e20f0d1403a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136548"
---
# <a name="privileged-identity-management---azure-resources"></a><span data-ttu-id="e4d48-103">Privileged Identity Management - Azure 资源</span><span class="sxs-lookup"><span data-stu-id="e4d48-103">Privileged Identity Management - Azure resources</span></span>

<span data-ttu-id="e4d48-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4d48-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4d48-105">可以使用适合于 Azure 资源的 [Azure Active Directory (Azure AD) Privileged Identity Management (PIM)](/azure/active-directory/privileged-identity-management/pim-configure) 为管理组、订阅、资源组和资源级别的 Azure 基础结构角色设置实时访问工作流。</span><span class="sxs-lookup"><span data-stu-id="e4d48-105">You can use [Azure Active Directory (Azure AD) Privileged Identity Management (PIM)](/azure/active-directory/privileged-identity-management/pim-configure) for Azure resources to set up just-in-time access workflow for your Azure infrastructure roles at a management group, subscription, resource group, and resource level.</span></span> <span data-ttu-id="e4d48-106">这些包括诸如所有者和参与者之类的内置角色以及自定义 RBAC 角色。</span><span class="sxs-lookup"><span data-stu-id="e4d48-106">These include built-in roles like Owner and Contributor as well as custom RBAC roles.</span></span>

## <a name="common-use-cases-for-pim-and-azure-resources-using-a-rest-api"></a><span data-ttu-id="e4d48-107">使用 REST API 的 PIM 和 Azure 资源的常见用例</span><span class="sxs-lookup"><span data-stu-id="e4d48-107">Common use cases for PIM and Azure resources using a REST API</span></span>

| <span data-ttu-id="e4d48-108">用例</span><span class="sxs-lookup"><span data-stu-id="e4d48-108">Use case</span></span> | <span data-ttu-id="e4d48-109">资源</span><span class="sxs-lookup"><span data-stu-id="e4d48-109">Resource</span></span> | <span data-ttu-id="e4d48-110">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e4d48-110">See also</span></span> |
| --- | --- | --- |
| <span data-ttu-id="e4d48-111">为 PIM 管理载入资源（订阅、资源组、资源等），列出请求者可访问的所有托管资源并检索托管资源的关系。</span><span class="sxs-lookup"><span data-stu-id="e4d48-111">Onboard a resource (subscriptions, resource group, resource etc.) for PIM management, list all the managed resources requester have access to, and retrieve relationships of a managed resource.</span></span> | [<span data-ttu-id="e4d48-112">governanceResource</span><span class="sxs-lookup"><span data-stu-id="e4d48-112">governanceResource</span></span>](governanceresource.md) | [<span data-ttu-id="e4d48-113">角色发现和管理</span><span class="sxs-lookup"><span data-stu-id="e4d48-113">Role discovery and management</span></span>](/azure/active-directory/privileged-identity-management/pim-resource-roles-discover-resources) |
| <span data-ttu-id="e4d48-114">列出资源的所有角色，或者特定资源中的特殊角色的详细信息。</span><span class="sxs-lookup"><span data-stu-id="e4d48-114">List all the roles for a resource or get details of a particular role in a specified resource.</span></span> | [<span data-ttu-id="e4d48-115">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="e4d48-115">governanceRoleDefinition</span></span>](governanceroledefinition.md) |  |
| <span data-ttu-id="e4d48-116">检索资源的所有角色设置，或更新角色设置</span><span class="sxs-lookup"><span data-stu-id="e4d48-116">Retrieve all role settings for a resource or make an update to a role setting</span></span> | [<span data-ttu-id="e4d48-117">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="e4d48-117">governanceRoleSetting</span></span>](governancerolesetting.md) | [<span data-ttu-id="e4d48-118">配置角色设置</span><span class="sxs-lookup"><span data-stu-id="e4d48-118">Configure role setting</span></span>](/azure/active-directory/privileged-identity-management/pim-resource-roles-configure-role-settings) |
| <span data-ttu-id="e4d48-119">列出并导出资源的所有角色分配。</span><span class="sxs-lookup"><span data-stu-id="e4d48-119">List and export all role assignments for a resource.</span></span> | [<span data-ttu-id="e4d48-120">governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="e4d48-120">governanceRoleAssignment</span></span>](governanceroleassignment.md) | [<span data-ttu-id="e4d48-121">导出角色分配</span><span class="sxs-lookup"><span data-stu-id="e4d48-121">Export role assignments</span></span>](/azure/active-directory/privileged-identity-management/azure-pim-resource-rbac#export-role-assignments-with-children) |
| <span data-ttu-id="e4d48-122">创建或删除符合条件或活动的角色分配，激活/禁用符合条件的分配，查看待处理请求列表，批准或拒绝待处理请求或取消自己的待处理请求。</span><span class="sxs-lookup"><span data-stu-id="e4d48-122">Create or remove an eligible or active role assignment, activate/deactivate an eligible assignment, view a list of pending requests, approve or deny a pending request or cancel your own pending request.</span></span> | [<span data-ttu-id="e4d48-123">governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="e4d48-123">governanceRoleAssignmentRequest</span></span>](governanceroleassignmentrequest.md) | [<span data-ttu-id="e4d48-124">角色分配</span><span class="sxs-lookup"><span data-stu-id="e4d48-124">Role Assignment</span></span>](/azure/active-directory/privileged-identity-management/pim-resource-roles-assign-roles)<br/>[<span data-ttu-id="e4d48-125">角色激活</span><span class="sxs-lookup"><span data-stu-id="e4d48-125">Role activation</span></span>](/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles)<br/>[<span data-ttu-id="e4d48-126">审批请求</span><span class="sxs-lookup"><span data-stu-id="e4d48-126">Approve requests</span></span>](/azure/active-directory/privileged-identity-management/azure-ad-pim-approval-workflow) |

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
