---
title: 策略 API 概述
description: Azure Active Directory 使用策略来控制组织中 Azure AD 功能的行为。
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 39e45d28491ace2502aa8f1df0df9af0273c54da
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132645"
---
# <a name="azure-ad-policy-overview"></a><span data-ttu-id="01737-103">Azure AD 策略概述</span><span class="sxs-lookup"><span data-stu-id="01737-103">Azure AD policy overview</span></span>

<span data-ttu-id="01737-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01737-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01737-105">Azure Active Directory (Azure AD) 使用策略来控制你的组织中 Azure AD 功能行为。</span><span class="sxs-lookup"><span data-stu-id="01737-105">Azure Active Directory (Azure AD) uses policies to control Azure AD feature behaviors in your organization.</span></span> <span data-ttu-id="01737-106">策略是可以在应用程序、服务主体、组或分配给其的整个组织上强制执行的自定义规则。</span><span class="sxs-lookup"><span data-stu-id="01737-106">Policies are custom rules that you can enforce on applications, service principals, groups, or on the entire organization they are assigned to.</span></span>

## <a name="what-policies-are-available"></a><span data-ttu-id="01737-107">哪些策略可用？</span><span class="sxs-lookup"><span data-stu-id="01737-107">What policies are available?</span></span>

| <span data-ttu-id="01737-108">策略类型</span><span class="sxs-lookup"><span data-stu-id="01737-108">Policy type</span></span>       | <span data-ttu-id="01737-109">说明</span><span class="sxs-lookup"><span data-stu-id="01737-109">Description</span></span> | <span data-ttu-id="01737-110">示例</span><span class="sxs-lookup"><span data-stu-id="01737-110">Examples</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="01737-111">activityBasedTimeoutPolicies</span><span class="sxs-lookup"><span data-stu-id="01737-111">activityBasedTimeoutPolicies</span></span>](activityBasedTimeoutPolicy.md)| <span data-ttu-id="01737-112">表示一个策略，该策略控制支持基于活动的超时功能的应用程序在一段时间不活动后自动注销 Web 会话。</span><span class="sxs-lookup"><span data-stu-id="01737-112">Represents a policy that controls automatic sign-out for web sessions after a period of inactivity, for applications that support activity-based timeout functionality.</span></span>| <span data-ttu-id="01737-113">将 Azure 门户配置为不活动超时 15 分钟。</span><span class="sxs-lookup"><span data-stu-id="01737-113">Configure the Azure portal to have an inactivity timeout of 15 minutes.</span></span> |
|[<span data-ttu-id="01737-114">authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="01737-114">authorizationPolicy</span></span>](authorizationpolicy.md)| <span data-ttu-id="01737-115">表示可以控制 Azure Active Directory 的授权设置的策略。</span><span class="sxs-lookup"><span data-stu-id="01737-115">Represents a policy that can control authorization settings of Azure Active Directory.</span></span> | <span data-ttu-id="01737-116">配置 Azure AD 以阻止租户中的 MSOL PowerShell。</span><span class="sxs-lookup"><span data-stu-id="01737-116">Configure Azure AD to block MSOL PowerShell in the tenant.</span></span> |
|[<span data-ttu-id="01737-117">claimsMappingPolicies</span><span class="sxs-lookup"><span data-stu-id="01737-117">claimsMappingPolicies</span></span>](claimsMappingPolicy.md)| <span data-ttu-id="01737-118">表示 WS-Fed、SAML、OAuth 2.0 和 OpenID Connect 协议声明映射策略，用于颁发给特定应用程序的令牌。</span><span class="sxs-lookup"><span data-stu-id="01737-118">Represents the claim-mapping policies for WS-Fed, SAML, OAuth 2.0, and OpenID Connect protocols, for tokens issued to a specific application.</span></span> | <span data-ttu-id="01737-119">创建并分配策略以从颁发给服务主体的令牌中省略基本声明。</span><span class="sxs-lookup"><span data-stu-id="01737-119">Create and assign a policy to omit the basic claims from tokens issued to a service principal.</span></span> |
|[<span data-ttu-id="01737-120">homeRealmDiscoveryPolicies</span><span class="sxs-lookup"><span data-stu-id="01737-120">homeRealmDiscoveryPolicies</span></span>](homeRealmDiscoveryPolicy.md)| <span data-ttu-id="01737-121">表示用于控制联盟用户的 Azure Active Directory 身份验证行为的策略，特别是针对联合域中的自动加速和用户身份验证限制。</span><span class="sxs-lookup"><span data-stu-id="01737-121">Represents a policy to control Azure Active Directory authentication behavior for federated users, in particular for auto-acceleration and user authentication restrictions in federated domains.</span></span>| <span data-ttu-id="01737-122">将所有用户配置为跳过主领域发现，并直接路由到 ADFS 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="01737-122">Configure all users to skip home realm discovery and be routed directly to ADFS for authentication.</span></span> |
|[<span data-ttu-id="01737-123">tokenLifetimePolicies</span><span class="sxs-lookup"><span data-stu-id="01737-123">tokenLifetimePolicies</span></span>](tokenlifetimepolicy.md)|<span data-ttu-id="01737-124">表示用于访问受保护资源的访问令牌的生存期持续时间。</span><span class="sxs-lookup"><span data-stu-id="01737-124">Represents the lifetime duration of access tokens used to access protected resources.</span></span>| <span data-ttu-id="01737-125">将特别敏感的应用程序配置为比默认令牌生存期更短的应用程序。</span><span class="sxs-lookup"><span data-stu-id="01737-125">Configure a particularly sensitive application with a shorter than default token lifetime.</span></span>|
|[<span data-ttu-id="01737-126">tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="01737-126">tokenIssuancePolicy</span></span>](tokenIssuancePolicy.md)|<span data-ttu-id="01737-127">表示用于指定 Azure AD 颁发的 SAML 令牌特征的策略。</span><span class="sxs-lookup"><span data-stu-id="01737-127">Represents the policy to specify the characteristics of SAML tokens issued by Azure AD.</span></span>| <span data-ttu-id="01737-128">配置要用于颁发 SAML 令牌的签名算法或 SAML 令牌版本。</span><span class="sxs-lookup"><span data-stu-id="01737-128">Configure the signing algorithm or SAML token version to be used to issue the SAML token.</span></span>
|[<span data-ttu-id="01737-129">identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="01737-129">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md)|<span data-ttu-id="01737-130">表示 Azure AD 安全默认策略。</span><span class="sxs-lookup"><span data-stu-id="01737-130">Represents the Azure AD security defaults policy.</span></span>| <span data-ttu-id="01737-131">配置 Azure AD 安全默认策略，以防范常见攻击。</span><span class="sxs-lookup"><span data-stu-id="01737-131">Configure the Azure AD security defaults policy to protect against common attacks.</span></span>

## <a name="next-steps"></a><span data-ttu-id="01737-132">后续步骤</span><span class="sxs-lookup"><span data-stu-id="01737-132">Next steps</span></span>

* <span data-ttu-id="01737-133">查看上面列出的不同策略选择类型及其各种方法。</span><span class="sxs-lookup"><span data-stu-id="01737-133">Review the different policy resouce types listed above and their various methods.</span></span>
* <span data-ttu-id="01737-134">请尝试 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中的 API。</span><span class="sxs-lookup"><span data-stu-id="01737-134">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>


