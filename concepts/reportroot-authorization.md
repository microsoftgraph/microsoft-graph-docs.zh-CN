---
title: 授权 API 读取 Office 365 使用情况报告
description: 可通过 Microsoft Graph 报告 API 访问的报告数据是敏感数据，并受到权限和 Azure Active Directory (Azure AD) 角色的保护。
author: yixia
localization_priority: Priority
ms.prod: reports
ms.openlocfilehash: 4fbdd9bec46db414cfd9f330b698c93ddcad9e27
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871589"
---
# <a name="authorization-for-apis-to-read-office-365-usage-reports"></a><span data-ttu-id="dad55-103">授权 API 读取 Office 365 使用情况报告</span><span class="sxs-lookup"><span data-stu-id="dad55-103">Authorization for APIs to read Office 365 usage reports</span></span>

<span data-ttu-id="dad55-104">可通过 Microsoft Graph 报告 API 访问的报告数据是敏感数据。</span><span class="sxs-lookup"><span data-stu-id="dad55-104">Report data accessible via the Microsoft Graph reports API is sensitive.</span></span> <span data-ttu-id="dad55-105">具体而言，Office 365 使用情况报告受权限和 Azure Active Directory (Azure AD) 角色的保护。</span><span class="sxs-lookup"><span data-stu-id="dad55-105">In particular, Office 365 usage reports are protected by both permissions and Azure Active Directory (Azure AD) roles.</span></span> <span data-ttu-id="dad55-106">本文中的信息适用于读取 Office 365 使用情况报告的报告 API。</span><span class="sxs-lookup"><span data-stu-id="dad55-106">The information in this article applies to the reports API that reads Office 365 usage reports.</span></span>

<span data-ttu-id="dad55-107">用于读取 Office 365 使用情况报告的 API 支持两种类型的授权：</span><span class="sxs-lookup"><span data-stu-id="dad55-107">The APIs to read Office 365 usage reports support two types of authorization:</span></span>

- <span data-ttu-id="dad55-108">**应用程序级别授权** - 允许应用在没有登录用户的情况下读取所有服务使用情况报告。</span><span class="sxs-lookup"><span data-stu-id="dad55-108">Allows an app to read all service usage reports without a signed-in user.</span></span> <span data-ttu-id="dad55-109">授权由授予给应用程序的权限决定。</span><span class="sxs-lookup"><span data-stu-id="dad55-109">The permissions granted to the application determine authorization.</span></span> 
- <span data-ttu-id="dad55-110">**用户委派的授权** - 允许应用代表已登录的用户读取所有服务使用情况报告。</span><span class="sxs-lookup"><span data-stu-id="dad55-110">**User delegated authorization** - Allows an app to read all service usage reports on behalf of the signed-in user.</span></span> <span data-ttu-id="dad55-111">除了向应用授予所需权限之外，用户必须是 Azure AD 受限管理员角色的成员。</span><span class="sxs-lookup"><span data-stu-id="dad55-111">In addition to the app having been granted the required permissions, the user must be a member of an Azure AD limited administrator role.</span></span> <span data-ttu-id="dad55-112">可以是以下角色之一：公司管理员、Exchange 管理员、SharePoint 管理员、Lync 管理员、全局读取者或报告读取者。</span><span class="sxs-lookup"><span data-stu-id="dad55-112">This can be one of the following roles: company administrator, Exchange administrator, SharePoint administrator, Lync administrator, global reader, or reports reader.</span></span>

<span data-ttu-id="dad55-113">如果从 Graph 浏览器调用 API：</span><span class="sxs-lookup"><span data-stu-id="dad55-113">If you're calling the Microsoft Graph Security API from Graph Explorer:</span></span>

- <span data-ttu-id="dad55-114">Azure AD 租户管理员必须对 Graph 浏览器应用程序显式授予所请求的权限。</span><span class="sxs-lookup"><span data-stu-id="dad55-114">The Azure AD tenant admin must explicitly grant consent for the requested permissions to the Graph Explorer application.</span></span>
- <span data-ttu-id="dad55-115">对于上面列出的用户委派的授权，该用户必须是 Azure AD 受限管理员角色的成员。</span><span class="sxs-lookup"><span data-stu-id="dad55-115">The user must be a member of a limited administrator role in Azure AD, listed above for user-delegated authorization.</span></span>

><span data-ttu-id="dad55-116">**注意**：Graph 浏览器不支持应用程序级别授权。</span><span class="sxs-lookup"><span data-stu-id="dad55-116">**Note**: Graph Explorer does not support application-level authorization.</span></span>

<span data-ttu-id="dad55-117">如果从应用程序调用 API：</span><span class="sxs-lookup"><span data-stu-id="dad55-117">If you're calling the APIs from an application:</span></span>

- <span data-ttu-id="dad55-118">Azure AD 租户管理员必须对你的应用程序显式授权。</span><span class="sxs-lookup"><span data-stu-id="dad55-118">The Azure AD tenant admin must explicitly grant consent to your application.</span></span> <span data-ttu-id="dad55-119">应用程序级别授权和用户委派的授权都需要满足此要求。</span><span class="sxs-lookup"><span data-stu-id="dad55-119">This is required both for application-level authorization and user delegated authorization.</span></span>
- <span data-ttu-id="dad55-120">如果使用的是用户委派的授权，已登录的用户必须是 Azure AD 受限管理员角色的成员。</span><span class="sxs-lookup"><span data-stu-id="dad55-120">If you're using user delegated authorization, the user must be a member of the Security Reader or Security Administrator Limited Admin role in Azure AD.</span></span>

## <a name="assign-azure-ad-roles-to-users"></a><span data-ttu-id="dad55-121">向用户分配 Azure AD 角色</span><span class="sxs-lookup"><span data-stu-id="dad55-121">Assign Azure AD roles to users</span></span>

<span data-ttu-id="dad55-122">应用程序被授予权限后，每个可以访问该应用程序的人（即 Azure AD 租户的成员）都将获得所授予的权限。</span><span class="sxs-lookup"><span data-stu-id="dad55-122">After an application is granted permissions, everyone with access to the application (that is, members of the Azure AD tenant) receives the granted permissions.</span></span> <span data-ttu-id="dad55-123">为了进一步保护敏感的报告数据，租户管理员必须为应用程序的用户分配相应的 Azure AD 角色。</span><span class="sxs-lookup"><span data-stu-id="dad55-123">To further protect sensitive reports data, tenant administrators must assign users of the application the appropriate Azure AD roles.</span></span> <span data-ttu-id="dad55-124">有关详细信息，请参阅 [Azure Active Directory 中的管理员角色权限](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles-azure-portal)和 [为具有 Azure Active Directory 的用户分配管理员和非管理员角色](https://docs.microsoft.com/azure/active-directory/active-directory-users-assign-role-azure-portal)。</span><span class="sxs-lookup"><span data-stu-id="dad55-124">For details, see [Administrator role permissions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles-azure-portal) and [Assign administrator and non-administrator roles to users with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-users-assign-role-azure-portal).</span></span>

><span data-ttu-id="dad55-125">**注意：** 必须是租户管理员才能执行此步骤。</span><span class="sxs-lookup"><span data-stu-id="dad55-125">**Note:** You must be a tenant admin to perform this step.</span></span>

<span data-ttu-id="dad55-126">向用户分配角色：</span><span class="sxs-lookup"><span data-stu-id="dad55-126">To assign a role to a user:</span></span>

1. <span data-ttu-id="dad55-127">登录到 [Azure 门户](https://portal.azure.com) (https://portal.azure.com)。</span><span class="sxs-lookup"><span data-stu-id="dad55-127">Sign in to the [Azure portal](https://portal.azure.com) (https://portal.azure.com).</span></span>
2. <span data-ttu-id="dad55-128">单击左上角的图标以展开 Azure 门户菜单。</span><span class="sxs-lookup"><span data-stu-id="dad55-128">Click the icon in the top left to expand the Azure portal menu.</span></span> <span data-ttu-id="dad55-129">选择“**Azure Active Directory**” > “**用户**”。</span><span class="sxs-lookup"><span data-stu-id="dad55-129">Select **Azure Active Directory** > **Users**.</span></span>
3. <span data-ttu-id="dad55-130">单击相应用户的姓名。</span><span class="sxs-lookup"><span data-stu-id="dad55-130">Click the name of the user.</span></span>
4. <span data-ttu-id="dad55-131">选择“**分配的角色**”，然后选择“**添加分配**”。</span><span class="sxs-lookup"><span data-stu-id="dad55-131">Choose **Assigned roles**, and then **Add assignment**.</span></span>
5. <span data-ttu-id="dad55-132">选择适当的角色，并单击“**添加**”。</span><span class="sxs-lookup"><span data-stu-id="dad55-132">Select the appropriate role, and click **Add**.</span></span>
