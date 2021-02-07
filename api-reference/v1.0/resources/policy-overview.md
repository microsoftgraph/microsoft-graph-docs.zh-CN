---
title: 策略 API 概述
description: Azure Active Directory 使用策略来控制组织中 Azure AD 功能的行为。
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 4f1b705b13518bdd1b5ede0c85c20dad0a593e2a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128475"
---
# <a name="azure-ad-policy-overview"></a><span data-ttu-id="aab11-103">Azure AD 策略概述</span><span class="sxs-lookup"><span data-stu-id="aab11-103">Azure AD policy overview</span></span>

<span data-ttu-id="aab11-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aab11-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="aab11-105">Azure Active Directory (Azure AD) 使用策略来控制你的组织中 Azure AD 功能行为。</span><span class="sxs-lookup"><span data-stu-id="aab11-105">Azure Active Directory (Azure AD) uses policies to control Azure AD feature behaviors in your organization.</span></span> <span data-ttu-id="aab11-106">策略是可以在应用程序、服务主体、组或分配给其的整个组织上强制执行的自定义规则。</span><span class="sxs-lookup"><span data-stu-id="aab11-106">Policies are custom rules that you can enforce on applications, service principals, groups, or on the entire organization they are assigned to.</span></span>

## <a name="what-policies-are-available"></a><span data-ttu-id="aab11-107">哪些策略可用？</span><span class="sxs-lookup"><span data-stu-id="aab11-107">What policies are available?</span></span>

| <span data-ttu-id="aab11-108">策略类型</span><span class="sxs-lookup"><span data-stu-id="aab11-108">Policy type</span></span>       | <span data-ttu-id="aab11-109">说明</span><span class="sxs-lookup"><span data-stu-id="aab11-109">Description</span></span> | <span data-ttu-id="aab11-110">示例</span><span class="sxs-lookup"><span data-stu-id="aab11-110">Examples</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="aab11-111">activityBasedTimeoutPolicies</span><span class="sxs-lookup"><span data-stu-id="aab11-111">activityBasedTimeoutPolicies</span></span>](activityBasedTimeoutPolicy.md)| <span data-ttu-id="aab11-112">表示一个策略，该策略控制支持基于活动的超时功能的应用程序在一段时间不活动后自动注销 Web 会话。</span><span class="sxs-lookup"><span data-stu-id="aab11-112">Represents a policy that controls automatic sign-out for web sessions after a period of inactivity, for applications that support activity-based timeout functionality.</span></span>| <span data-ttu-id="aab11-113">将 Azure 门户配置为不活动超时 15 分钟。</span><span class="sxs-lookup"><span data-stu-id="aab11-113">Configure the Azure portal to have an inactivity timeout of 15 minutes.</span></span> |
|[<span data-ttu-id="aab11-114">claimsMappingPolicies</span><span class="sxs-lookup"><span data-stu-id="aab11-114">claimsMappingPolicies</span></span>](claimsMappingPolicy.md)| <span data-ttu-id="aab11-115">表示 WS-Fed、SAML、OAuth 2.0 和 OpenID Connect 协议声明映射策略，用于颁发给特定应用程序的令牌。</span><span class="sxs-lookup"><span data-stu-id="aab11-115">Represents the claim-mapping policies for WS-Fed, SAML, OAuth 2.0, and OpenID Connect protocols, for tokens issued to a specific application.</span></span> | <span data-ttu-id="aab11-116">创建并分配策略以从颁发给服务主体的令牌中省略基本声明。</span><span class="sxs-lookup"><span data-stu-id="aab11-116">Create and assign a policy to omit the basic claims from tokens issued to a service principal.</span></span> |
|[<span data-ttu-id="aab11-117">homeRealmDiscoveryPolicies</span><span class="sxs-lookup"><span data-stu-id="aab11-117">homeRealmDiscoveryPolicies</span></span>](homeRealmDiscoveryPolicy.md)| <span data-ttu-id="aab11-118">表示用于控制联盟用户的 Azure Active Directory 身份验证行为的策略，特别是针对联合域中的自动加速和用户身份验证限制。</span><span class="sxs-lookup"><span data-stu-id="aab11-118">Represents a policy to control Azure Active Directory authentication behavior for federated users, in particular for auto-acceleration and user authentication restrictions in federated domains.</span></span>| <span data-ttu-id="aab11-119">将所有用户配置为跳过主领域发现，并直接路由到 ADFS 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="aab11-119">Configure all users to skip home realm discovery and be routed directly to ADFS for authentication.</span></span> |
|[<span data-ttu-id="aab11-120">tokenLifetimePolicies</span><span class="sxs-lookup"><span data-stu-id="aab11-120">tokenLifetimePolicies</span></span>](tokenlifetimepolicy.md)|<span data-ttu-id="aab11-121">表示用于访问受保护资源的访问令牌的生存期持续时间。</span><span class="sxs-lookup"><span data-stu-id="aab11-121">Represents the lifetime duration of access tokens used to access protected resources.</span></span>| <span data-ttu-id="aab11-122">将特别敏感的应用程序配置为比默认令牌生存期更短的应用程序。</span><span class="sxs-lookup"><span data-stu-id="aab11-122">Configure a particularly sensitive application with a shorter than default token lifetime.</span></span>|
|[<span data-ttu-id="aab11-123">tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="aab11-123">tokenIssuancePolicy</span></span>](tokenIssuancePolicy.md)|<span data-ttu-id="aab11-124">表示用于指定 Azure AD 颁发的 SAML 令牌特征的策略。</span><span class="sxs-lookup"><span data-stu-id="aab11-124">Represents the policy to specify the characteristics of SAML tokens issued by Azure AD.</span></span>| <span data-ttu-id="aab11-125">配置要用于颁发 SAML 令牌的签名算法或 SAML 令牌版本。</span><span class="sxs-lookup"><span data-stu-id="aab11-125">Configure the signing algorithm or SAML token version to be used to issue the SAML token.</span></span>
|[<span data-ttu-id="aab11-126">identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="aab11-126">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md)|<span data-ttu-id="aab11-127">表示 Azure AD 安全默认策略。</span><span class="sxs-lookup"><span data-stu-id="aab11-127">Represents the Azure AD security defaults policy.</span></span>| <span data-ttu-id="aab11-128">配置 Azure AD 安全默认策略，以防范常见攻击。</span><span class="sxs-lookup"><span data-stu-id="aab11-128">Configure the Azure AD security defaults policy to protect against common attacks.</span></span>

## <a name="next-steps"></a><span data-ttu-id="aab11-129">后续步骤</span><span class="sxs-lookup"><span data-stu-id="aab11-129">Next steps</span></span>

* <span data-ttu-id="aab11-130">查看上面列出的不同策略选择类型及其各种方法。</span><span class="sxs-lookup"><span data-stu-id="aab11-130">Review the different policy resouce types listed above and their various methods.</span></span>
* <span data-ttu-id="aab11-131">尝试在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中调用 API。</span><span class="sxs-lookup"><span data-stu-id="aab11-131">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

