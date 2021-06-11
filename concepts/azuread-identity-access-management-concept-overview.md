---
title: Azure AD 标识和访问管理 API 概述
description: 'Azure Active Directory (Azure AD) 有助于集中化标识和访问管理 (IAM)，实现应用、设备、服务和基础结构之间的安全和高效访问。 组织可以使用 Azure AD 来管理标识，并控制本地、混合及云环境中的访问。  '
author: jackson-woods
localization_priority: Priority
ms.prod: identity-and-access
ms.custom: scenarios:getting-started
ms.openlocfilehash: e15685f1cf561713b25dc70b87264edd36168067
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870757"
---
# <a name="azure-ad-identity-and-access-management-api-overview"></a><span data-ttu-id="4f4e3-104">Azure AD 标识和访问管理 API 概述</span><span class="sxs-lookup"><span data-stu-id="4f4e3-104">Azure AD identity and access management API overview</span></span>

<span data-ttu-id="4f4e3-105">Azure Active Directory (Azure AD) 有助于集中化标识和访问管理 (IAM)，实现应用、设备、服务和基础结构之间的安全和高效访问。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-105">Azure Active Directory (Azure AD) helps centralize identity and access management (IAM) to enable secure and productive access between apps, devices, services, and infrastructure.</span></span> <span data-ttu-id="4f4e3-106">组织可以使用 Azure AD 来管理标识，并控制本地、混合及云环境中的访问。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-106">Organizations can use Azure AD to manage identities and control access in on-premises, hybrid, and cloud environments.</span></span>

<span data-ttu-id="4f4e3-107">可以使用 Microsoft Graph 中的 Azure AD REST API 在 Azure AD [资源](/graph/api/resources/azure-ad-overview)和第三方服务之间创建独特的工作流。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-107">You can use the Azure AD REST APIs in Microsoft Graph to create unique workflows between Azure AD [resources](/graph/api/resources/azure-ad-overview) and third-party services.</span></span>

## <a name="why-use-the-azure-ad-apis"></a><span data-ttu-id="4f4e3-108">为什么使用 Azure AD API？</span><span class="sxs-lookup"><span data-stu-id="4f4e3-108">Why use the Azure AD APIs?</span></span>

<span data-ttu-id="4f4e3-109">超过 1,500 万个组织在订阅 Microsoft 云服务（如 Microsoft 365、Microsoft Azure 和企业移动性套件）的同时使用 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-109">More than 15 million organizations use Azure AD while subscribing to Microsoft cloud services like Microsoft 365, Microsoft Azure, and Enterprise Mobility Suite.</span></span>

<span data-ttu-id="4f4e3-110">企业开发者使用 Microsoft Graph 集成 Azure AD 标识管理和其他服务，以实现管理工作流的自动化，例如员工入职和离职、个人资料维护、许可证部署等。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-110">Enterprise developers use Microsoft Graph to integrate Azure AD identity management and other services to automate administrative workflows, such as employee onboarding (and termination), profile maintenance, license deployment, and more.</span></span>

<span data-ttu-id="4f4e3-111">对于许多企业开发者来说，Microsoft Graph 和 Azure AD 可帮助将现有应用程序“提升并转移到”云中，从而加速组织的数字化转型。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-111">For many enterprise developers, Microsoft Graph and Azure AD help "lift and shift" existing applications to the cloud, speeding an organization's digital transformation.</span></span> <span data-ttu-id="4f4e3-112">可以利用 Azure AD 功能向应用程序添加访问控制机制，包括验证用户组成员身份、目录角色或管理单位成员身份。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-112">You can take advantage of Azure AD capabilities to add access control mechanisms to applications, including verifying a user's group membership, directory role, or administrative unit membership.</span></span>

<span data-ttu-id="4f4e3-113">你可以将 Microsoft Graph 和 Azure AD 用作轻松快速地访问超过 1,500 万个组织的方式，其中包括 90% 已使用 Azure AD 服务的财富 500 强公司。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-113">You can use Microsoft Graph and Azure AD as a way to quickly and easily reach more than 15 million organizations, including 90% of the Fortune 500 companies that already use Azure AD services.</span></span> <span data-ttu-id="4f4e3-114">集成的应用程序具有无缝登录体验，可以使用现有组织数据创建个性化体验。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-114">Integrated applications feature seamless sign-in experiences and can use existing organizational data to create personalized experiences.</span></span>

<span data-ttu-id="4f4e3-115">你可以使用 Microsoft Graph 中的 Azure AD API 来查询用户配置文件、查找其他用户、管理组织关系、跟踪任务或创建包含现有组织数据的原始解决方案。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-115">You can use the Azure AD APIs in Microsoft Graph to query the user's profile, find other users, manage organizational relationships, track assignments, or create original solutions that incorporate existing organizational data.</span></span> <span data-ttu-id="4f4e3-116">这些 API 提供了坚实基础，可将自定义业务应用程序无缝集成到组织现有的数字服务。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-116">These APIs provide a solid foundation to seamlessly integrate custom business applications into an organization's existing digital services.</span></span>

### <a name="access-users-and-groups"></a><span data-ttu-id="4f4e3-117">访问用户和组</span><span class="sxs-lookup"><span data-stu-id="4f4e3-117">Access users and groups</span></span>

<span data-ttu-id="4f4e3-118">可以将 Microsoft Graph 中的 Azure AD API 用于：</span><span class="sxs-lookup"><span data-stu-id="4f4e3-118">You can use Azure AD APIs in Microsoft Graph to:</span></span>

- <span data-ttu-id="4f4e3-119">查找和管理组织中用户的[用户配置文件](/graph/api/resources/user)信息（例如，姓名、照片、电子邮件地址、职务、办公地点等）。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-119">Look up and manage [user profile](/graph/api/resources/user) information for users in your organization, such as name, photo, email address, job title, office location, and more.</span></span>
- <span data-ttu-id="4f4e3-120">为组织中的项目和团队创建[组](/graph/api/resources/groups-overview)。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-120">Create [groups](/graph/api/resources/groups-overview) for projects and teams in your organization.</span></span> <span data-ttu-id="4f4e3-121">从组中添加和删除成员，以控制对资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-121">Add and remove members from the group to control access to resources.</span></span> <span data-ttu-id="4f4e3-122">（动态组可根据用户属性值自动更改成员身份。）</span><span class="sxs-lookup"><span data-stu-id="4f4e3-122">(Dynamic groups can automatically change membership based on user property values.)</span></span>
- <span data-ttu-id="4f4e3-123">要控制访问权限，你可以在组列表中检查[可传递成员资格](/graph/api/user-checkmembergroups)，或从[常规资源 ID](/graph/api/directoryobject-getbyids) 列表中获取指定类型的所有资源（如用户或组）。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-123">To control access, you can check for [transitive membership](/graph/api/user-checkmembergroups) in a list of groups or get all the resources of a specified type (like user or group) from a list of [generic resource IDs](/graph/api/directoryobject-getbyids).</span></span>

### <a name="manage-directory-roles"></a><span data-ttu-id="4f4e3-124">管理目录角色</span><span class="sxs-lookup"><span data-stu-id="4f4e3-124">Manage directory roles</span></span>

<span data-ttu-id="4f4e3-125">你可以将用户分配给预定义的 Azure AD 管理[目录角色](/graph/api/resources/directoryrole)，该角色授予执行特定任务的权限。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-125">You can assign users to predefined Azure AD administrative [directory roles](/graph/api/resources/directoryrole), which grants permission to perform specific tasks.</span></span>

### <a name="manage-devices"></a><span data-ttu-id="4f4e3-126">管理设备</span><span class="sxs-lookup"><span data-stu-id="4f4e3-126">Manage devices</span></span>

<span data-ttu-id="4f4e3-p107">[管理组织中的注册设备](/azure/active-directory/device-management-introduction)。设备已注册给用户，包括笔记本电脑、台式机、平板电脑和移动电话等。设备通常是在云中使用 Device Registration Service 或由 Microsoft Intune 创建。通过条件访问策略使用它们时将进行多重身份验证。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-p107">[Manage devices](/azure/active-directory/device-management-introduction) registered in the organization. Devices are registered to users and include items like laptops, desktops, tablets, and mobile phones. Devices are typically created in the cloud using the Device Registration Service or by Microsoft Intune. They're used by conditional access policies for multifactor authentication.</span></span>

### <a name="partner-tenant-management"></a><span data-ttu-id="4f4e3-131">合作伙伴租户管理</span><span class="sxs-lookup"><span data-stu-id="4f4e3-131">Partner tenant management</span></span>

<span data-ttu-id="4f4e3-132">转售和管理 Microsoft Online Services（如 Microsoft 365、Microsoft Azure 和 CRM Online）的 Microsoft 合作伙伴可以查看他们目前管理的[组织租户](/graph/api/resources/contract)。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-132">Microsoft partners that resell and manage Microsoft Online Services (such as Microsoft 365, Microsoft Azure, and CRM Online) can view the [organization tenants](/graph/api/resources/contract) they currently manage.</span></span>

<span data-ttu-id="4f4e3-133">你还可以[管理与租户关联的域](/graph/api/resources/domain)。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-133">You can also [manage domains](/graph/api/resources/domain) associated with a tenant.</span></span> <span data-ttu-id="4f4e3-134">借助域操作，Microsoft 合作伙伴可以对 Microsoft 365 等服务自动执行域注册。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-134">Domain operations enable Microsoft partners to automate domain registration for services such as Microsoft 365.</span></span>

### <a name="tenant-management"></a><span data-ttu-id="4f4e3-135">租户管理</span><span class="sxs-lookup"><span data-stu-id="4f4e3-135">Tenant management</span></span>

<span data-ttu-id="4f4e3-136">用于租户管理的 Azure AD API 允许执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="4f4e3-136">Azure AD APIs for tenant management allow you to:</span></span>

- <span data-ttu-id="4f4e3-137">获取[组织](/graph/api/resources/organization)的相关信息，如公司办公地址、技术和通知联系人、活动服务预订及其关联域。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-137">Get information about an [organization](/graph/api/resources/organization), such as its business address, technical and notification contacts, active service subscriptions, and the domains associated with it.</span></span>
- <span data-ttu-id="4f4e3-138">获取公司订阅的[服务 SKU](/graph/api/resources/subscribedsku) 的相关信息。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-138">Get information about the [service SKUs](/graph/api/resources/subscribedsku) that a company is subscribed to.</span></span>
- <span data-ttu-id="4f4e3-139">[邀请外部](/graph/api/resources/invitation)（来宾）用户加入组织。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-139">[Invite external](/graph/api/resources/invitation) (guest) users to an organization.</span></span>

### <a name="monitor-identity-risks-preview"></a><span data-ttu-id="4f4e3-140">监视标识风险（预览版）</span><span class="sxs-lookup"><span data-stu-id="4f4e3-140">Monitor identity risks (preview)</span></span>

<span data-ttu-id="4f4e3-141">大多数安全漏洞都会导致攻击者窃取用户的身份，攻击者利用第三方漏洞、密码喷洒攻击和复杂的网络钓鱼攻击，从而使攻击变得非常有效。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-141">Most security breaches are the result of attackers stealing a user’s identity, and attackers have become terrifyingly effective in taking advantage of third-party breaches, password spray attacks, and sophisticated phishing attacks.</span></span> <span data-ttu-id="4f4e3-142">这就意味着，你需要保护所有用户帐户免受这些攻击，并主动防止泄露的身份信息被滥用。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-142">This means you need to protect all your user accounts from these attacks and proactively prevent compromised identities from being abused.</span></span>

<span data-ttu-id="4f4e3-143">Azure AD 使用自适应机器学习算法和启发，检测表明帐户可能已遭入侵的异常。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-143">Azure AD uses adaptive machine learning algorithms and heuristics to detect anomalies that indicate potentially compromised accounts.</span></span> <span data-ttu-id="4f4e3-144">使用此类数据，Azure AD Identity Protection 可使用基于风险的条件访问策略来保护用户，并根据检测结果生成报告和警报。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-144">Using this data, Azure AD Identity Protection protects your users with risk-based conditional access policies and generates reports and alerts on its detections.</span></span>

<span data-ttu-id="4f4e3-145">现在，Azure AD Premium P2 客户可以通过 Microsoft Graph 轻松[查询 Identity Protection 检测到的风险事件](/graph/api/resources/identityprotection-root)，包括风险事件类型、严重性、日期、时间、位置、受影响用户等。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-145">Today, Microsoft Graph gives easy access to customers of Azure AD Premium P2 to [query risk events detected by Identity Protection](/graph/api/resources/identityprotection-root), including the risk event’s type, severity, date, time, location, impacted user, and more.</span></span> <span data-ttu-id="4f4e3-146">然后，客户可以在 SIEM 系统和安全应用中使用这些事件。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-146">Customers can then use those events in SIEM systems and security applications.</span></span>

### <a name="activate-users-into-privileged-roles-preview"></a><span data-ttu-id="4f4e3-147">激活用户的特权角色（预览版）</span><span class="sxs-lookup"><span data-stu-id="4f4e3-147">Activate users into privileged roles (preview)</span></span>

<span data-ttu-id="4f4e3-148">你可以通过按需激活管理权限来保护对资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-148">You can get secure access to resources by activating administrative privileges on-demand.</span></span> <span data-ttu-id="4f4e3-149">[Privileged Identity Management](/graph/api/resources/privilegedidentitymanagement-root) 是一项 Azure AD Premium P2 功能。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-149">[Privileged Identity Management](/graph/api/resources/privilegedidentitymanagement-root) is featured in Azure AD Premium P2.</span></span>

### <a name="manage-user-access-reviews-preview"></a><span data-ttu-id="4f4e3-150">管理用户访问评审（预览版）</span><span class="sxs-lookup"><span data-stu-id="4f4e3-150">Manage user access reviews (preview)</span></span>

<span data-ttu-id="4f4e3-151">可以配置组成员资格和应用访问权限的访问评审。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-151">You can configure access reviews of group memberships and application access.</span></span> <span data-ttu-id="4f4e3-152">[访问评审](/graph/api/resources/accessreviews-root)是一项 Azure AD Premium P2 功能。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-152">[Access reviews](/graph/api/resources/accessreviews-root) is featured in Azure AD Premium P2.</span></span>

## <a name="api-reference"></a><span data-ttu-id="4f4e3-153">API 参考</span><span class="sxs-lookup"><span data-stu-id="4f4e3-153">API reference</span></span>

<span data-ttu-id="4f4e3-154">在查找此服务的 API 参考？</span><span class="sxs-lookup"><span data-stu-id="4f4e3-154">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="4f4e3-155">Microsoft Graph v1.0 中的 Azure AD 标识和访问管理 API</span><span class="sxs-lookup"><span data-stu-id="4f4e3-155">Azure AD identity and access management API in Microsoft Graph v1.0</span></span>](/graph/api/resources/azure-ad-overview?view=graph-rest-1.0&preserve-view=true)
- [<span data-ttu-id="4f4e3-156">Microsoft Graph beta 中的 Azure AD 标识和访问管理 API</span><span class="sxs-lookup"><span data-stu-id="4f4e3-156">Azure AD identity and access management API in Microsoft Graph beta</span></span>](/graph/api/resources/azure-ad-overview?view=graph-rest-beta&preserve-view=true)

## <a name="next-steps"></a><span data-ttu-id="4f4e3-157">后续步骤</span><span class="sxs-lookup"><span data-stu-id="4f4e3-157">Next steps</span></span>

- <span data-ttu-id="4f4e3-158">了解到如何[使用 Azure AD REST API](/graph/api/resources/azure-ad-overview)。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-158">Find out how to [Use the Azure AD REST APIs](/graph/api/resources/azure-ad-overview).</span></span>
- <span data-ttu-id="4f4e3-159">使用 Azure AD 对 Microsoft Graph [进行身份验证](./auth/index.yml)。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-159">Use Azure AD to [authenticate](./auth/index.yml) to Microsoft Graph.</span></span>
- <span data-ttu-id="4f4e3-160">将 [Azure AD 登录](https://azure.microsoft.com/develop/identity/signin/)集成到应用或网站中。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-160">Integrate [Azure AD sign-in](https://azure.microsoft.com/develop/identity/signin/) into your app or website.</span></span>
- <span data-ttu-id="4f4e3-161">有关 Azure AD API 中新增功能的信息，请参阅[更改日志](changelog.md)。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-161">See the [Changelog](changelog.md) for information about what's new in the Azure AD APIs.</span></span>
- <span data-ttu-id="4f4e3-162">浏览[示例](https://developer.microsoft.com/graph/graph/examples)，了解有关如何使用 Microsoft Graph 的更多信息。</span><span class="sxs-lookup"><span data-stu-id="4f4e3-162">Explore [examples](https://developer.microsoft.com/graph/graph/examples) for more ideas about how to use Microsoft Graph.</span></span>
