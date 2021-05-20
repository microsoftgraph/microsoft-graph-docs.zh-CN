---
title: Privileged Identity Management
description: 适合于 Azure AD Privileged Identity Management 的 API，用于管理 Azure Active Directory 角色和 Azure 资源角色。
localization_priority: Priority
doc_type: conceptualPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 31f19ab4c6dbb79c5bbf60c045b3367e2d819ee9
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546075"
---
# <a name="privileged-identity-management"></a><span data-ttu-id="eb58f-103">Privileged Identity Management</span><span class="sxs-lookup"><span data-stu-id="eb58f-103">Privileged Identity Management</span></span>

<span data-ttu-id="eb58f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb58f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb58f-105">[Azure Active Directory (Azure AD) Privileged Identity Management (PIM)](/azure/active-directory/privileged-identity-management/pim-configure) 是可便于管理、控制和监视对组织中重要资源的访问的服务。</span><span class="sxs-lookup"><span data-stu-id="eb58f-105">[Azure Active Directory (Azure AD) Privileged Identity Management (PIM)](/azure/active-directory/privileged-identity-management/pim-configure) is a service that enables you to manage, control, and monitor access to important resources in your organization.</span></span> <span data-ttu-id="eb58f-106">这包括访问 Azure AD、Azure 资源和其他 Microsoft Online Services（例如 Microsoft 365 或 Microsoft Intune）中的资源。</span><span class="sxs-lookup"><span data-stu-id="eb58f-106">This includes access to resources in Azure AD, Azure resources, and other Microsoft Online Services like Microsoft 365 or Microsoft Intune.</span></span> <span data-ttu-id="eb58f-107">Microsoft Graph 提供有你可用于管理 Azure AD 角色和 Azure 资源角色的 API。</span><span class="sxs-lookup"><span data-stu-id="eb58f-107">Microsoft Graph provides APIs that you can use to manage Azure AD roles and Azure resource roles.</span></span>

- [<span data-ttu-id="eb58f-108">适用于 Azure AD 橘色的 API</span><span class="sxs-lookup"><span data-stu-id="eb58f-108">APIs for Azure AD roles</span></span>](privilegedidentitymanagement-directory.md)
- [<span data-ttu-id="eb58f-109">适用于 Azure 资源角色 的 API</span><span class="sxs-lookup"><span data-stu-id="eb58f-109">APIs for Azure resource roles</span></span>](privilegedidentitymanagement-resources.md)

> [!IMPORTANT]
> <span data-ttu-id="eb58f-110">用于管理 Azure AD 角色的 API 对于大多数租户已弃用，但使用较旧版本 Privileged Identity Management (PIM) 的少数租户除外。</span><span class="sxs-lookup"><span data-stu-id="eb58f-110">The API to manage Azure AD roles is deprecated for most tenants except for a few that use an older version of Privileged Identity Management (PIM).</span></span> <span data-ttu-id="eb58f-111">有关 PIM 版本的详细信息，请参阅[确定 PIM 的版本](/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?tabs=new#determine-your-version-of-pim)。</span><span class="sxs-lookup"><span data-stu-id="eb58f-111">For more information about PIM versions, see [Determine your version of PIM](/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?tabs=new#determine-your-version-of-pim).</span></span> <span data-ttu-id="eb58f-112">如果你使用的是新版本，并且收到 **TenantEnabledInAadRoleMigration** 错误，你可以等待，直至新 API 在 Azure AD 角色的 [unifiedRoleManagement](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta&preserve-view=true) API 下可用于 PIM 功能，或者你可以使用 Azure AD 角色的 [Azure 资源](/graph/api/resources/privilegedidentitymanagement-resources?view=graph-rest-beta&preserve-view=true) API。</span><span class="sxs-lookup"><span data-stu-id="eb58f-112">If you are using the new version and are recieving a **TenantEnabledInAadRoleMigration** error, you can wait until a new API is available for PIM functionality under the [unifiedRoleManagement](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta&preserve-view=true) API for Azure AD roles, or you can use the [Azure Resource](/graph/api/resources/privilegedidentitymanagement-resources?view=graph-rest-beta&preserve-view=true) API for your Azure AD roles.</span></span> <span data-ttu-id="eb58f-113">若要使用 **Azure 资源** API，请将 `azureResources` 替换为 `provider_id` 的 `aadRoles`，然后将租户 ID 用于 `resource_id`。</span><span class="sxs-lookup"><span data-stu-id="eb58f-113">To use the **Azure resource** API, replace `azureResources` with `aadRoles` for `provider_id` and use your tenant id for `resource_id`.</span></span> <span data-ttu-id="eb58f-114">建议等待新 API。</span><span class="sxs-lookup"><span data-stu-id="eb58f-114">We recommend that you wait for the new API.</span></span> <span data-ttu-id="eb58f-115">新 API 可用后，你将能够继续使用 **Azure 资源** API。</span><span class="sxs-lookup"><span data-stu-id="eb58f-115">You will be able to continue using the **Azure resource** API after the new API is available.</span></span> <span data-ttu-id="eb58f-116">Azure 门户中提供的任何新功能也将通过新 API 专门提供。</span><span class="sxs-lookup"><span data-stu-id="eb58f-116">Any new features made available in the Azure portal will also be made exclusively available through the new API.</span></span>

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
