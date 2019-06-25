---
title: Privileged Identity Management
description: 适合于 Azure AD Privileged Identity Management 的 API，用于管理 Azure Active Directory 角色和 Azure 资源角色。
localization_priority: Priority
ms.openlocfilehash: e8d61cb767b5471b76bc956dc5a0aeb9dc5af19f
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2019
ms.locfileid: "35133808"
---
# <a name="privileged-identity-management"></a><span data-ttu-id="34422-103">Privileged Identity Management</span><span class="sxs-lookup"><span data-stu-id="34422-103">Privileged Identity Management</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34422-104">[Azure Active Directory (Azure AD) Privileged Identity Management (PIM)](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure) 是可便于管理、控制和监视对组织中重要资源的访问的服务。</span><span class="sxs-lookup"><span data-stu-id="34422-104">[Azure Active Directory (Azure AD) Privileged Identity Management (PIM)](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure) is a service that enables you to manage, control, and monitor access to important resources in your organization.</span></span> <span data-ttu-id="34422-105">这包括访问 Azure AD、Azure 资源和其他 Microsoft Online Services（例如 Office 365 或 Microsoft Intune）中的资源。</span><span class="sxs-lookup"><span data-stu-id="34422-105">This includes access to resources in Azure AD, Azure resources, and other Microsoft Online Services like Office 365 or Microsoft Intune.</span></span> <span data-ttu-id="34422-106">Microsoft Graph 提供有你可用于管理 Azure AD 角色和 Azure 资源角色的 API。</span><span class="sxs-lookup"><span data-stu-id="34422-106">Microsoft Graph provides APIs that you can use to manage Azure AD roles and Azure resource roles.</span></span>

- [<span data-ttu-id="34422-107">适用于 Azure AD 橘色的 API</span><span class="sxs-lookup"><span data-stu-id="34422-107">APIs for Azure AD roles</span></span>](privilegedidentitymanagement-directory.md)
- [<span data-ttu-id="34422-108">适用于 Azure 资源角色 的 API</span><span class="sxs-lookup"><span data-stu-id="34422-108">APIs for Azure resource roles</span></span>](privilegedidentitymanagement-resources.md)

> [!IMPORTANT]
> <span data-ttu-id="34422-109">在 2019 年 6 月到 7 月，用于管理 Azure AD 角色的 API 将发生更改，以遵守以下 [Azure 资源 API](privilegedidentitymanagement-resources.md) 命名空间和约定。</span><span class="sxs-lookup"><span data-stu-id="34422-109">The API to manage Azure AD roles will change between June and November of 2019 to follow the namespace and convention of the [Azure resource API](privilegedidentitymanagement-resources.md).</span></span> <span data-ttu-id="34422-110">Azure AD PIM 将变成采用 Azure 资源约定的资源。</span><span class="sxs-lookup"><span data-stu-id="34422-110">Azure AD PIM will become a resource under the Azure resource convention.</span></span> <span data-ttu-id="34422-111">如果此更改直接影响你的租户，请填写 [Azure AD PIM 的 Graph API 变更表](https://forms.office.com/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbRzfBSoy7dT5DqNLWwotW3OFUNFFMRlRLSUtRNEdDWEZHN05LT09IWjkyTS4u)，以获取其他信息、支持以及为此 API 变更安排时间的功能。</span><span class="sxs-lookup"><span data-stu-id="34422-111">If this change will directly affect your tenant, please complete the [Graph API change for Azure AD PIM form](https://forms.office.com/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbRzfBSoy7dT5DqNLWwotW3OFUNFFMRlRLSUtRNEdDWEZHN05LT09IWjkyTS4u) to get additional information, support, and the ability to schedule a time for this API change.</span></span>

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
