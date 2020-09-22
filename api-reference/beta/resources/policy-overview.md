---
title: 策略 API 概述
description: Azure Active Directory 使用策略控制组织中的 Azure AD 功能行为。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 5abecc785db2b2dcd141b528814642e6356abfa7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033634"
---
# <a name="azure-ad-policy-overview"></a><span data-ttu-id="d4cac-103">Azure AD 策略概述</span><span class="sxs-lookup"><span data-stu-id="d4cac-103">Azure AD policy overview</span></span>

<span data-ttu-id="d4cac-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4cac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4cac-105">Azure Active Directory (Azure AD) 使用策略控制组织中的 Azure AD 功能行为。</span><span class="sxs-lookup"><span data-stu-id="d4cac-105">Azure Active Directory (Azure AD) uses policies to control Azure AD feature behaviors in your organization.</span></span> <span data-ttu-id="d4cac-106">策略是您可以在应用程序、服务主体、组或其分配到的整个组织上实施的自定义规则。</span><span class="sxs-lookup"><span data-stu-id="d4cac-106">Policies are custom rules that you can enforce on applications, service principals, groups, or on the entire organization they are assigned to.</span></span>

## <a name="what-policies-are-available"></a><span data-ttu-id="d4cac-107">有哪些策略可用？</span><span class="sxs-lookup"><span data-stu-id="d4cac-107">What policies are available?</span></span>

| <span data-ttu-id="d4cac-108">策略类型</span><span class="sxs-lookup"><span data-stu-id="d4cac-108">Policy type</span></span>       | <span data-ttu-id="d4cac-109">说明</span><span class="sxs-lookup"><span data-stu-id="d4cac-109">Description</span></span> | <span data-ttu-id="d4cac-110">示例</span><span class="sxs-lookup"><span data-stu-id="d4cac-110">Examples</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="d4cac-111">activityBasedTimeoutPolicies</span><span class="sxs-lookup"><span data-stu-id="d4cac-111">activityBasedTimeoutPolicies</span></span>](activityBasedTimeoutPolicy.md)| <span data-ttu-id="d4cac-112">表示在一段时间不活动后控制 web 会话的自动注销的策略，适用于支持基于活动的超时功能的应用程序。</span><span class="sxs-lookup"><span data-stu-id="d4cac-112">Represents a policy that controls automatic sign-out for web sessions after a period of inactivity, for applications that support activity-based timeout functionality.</span></span>| <span data-ttu-id="d4cac-113">将 Azure 门户配置为使非活动超时为15分钟。</span><span class="sxs-lookup"><span data-stu-id="d4cac-113">Configure the Azure portal to have an inactivity timeout of 15 minutes.</span></span> |
|[<span data-ttu-id="d4cac-114">authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="d4cac-114">authorizationPolicy</span></span>](authorizationpolicy.md)| <span data-ttu-id="d4cac-115">表示可控制 Azure Active Directory 的授权设置的策略。</span><span class="sxs-lookup"><span data-stu-id="d4cac-115">Represents a policy that can control authorization settings of Azure Active Directory.</span></span> | <span data-ttu-id="d4cac-116">将 Azure AD 配置为阻止租户中的 MSOL PowerShell。</span><span class="sxs-lookup"><span data-stu-id="d4cac-116">Configure Azure AD to block MSOL PowerShell in the tenant.</span></span> |
|[<span data-ttu-id="d4cac-117">claimsMappingPolicies</span><span class="sxs-lookup"><span data-stu-id="d4cac-117">claimsMappingPolicies</span></span>](claimsMappingPolicy.md)| <span data-ttu-id="d4cac-118">表示对颁发给特定应用程序的令牌的 WS 馈送、SAML、OAuth 2.0 和 OpenID Connect 协议的声明映射策略。</span><span class="sxs-lookup"><span data-stu-id="d4cac-118">Represents the claim-mapping policies for WS-Fed, SAML, OAuth 2.0, and OpenID Connect protocols, for tokens issued to a specific application.</span></span> | <span data-ttu-id="d4cac-119">创建和分配策略以省略颁发给服务主体的令牌中的基本声明。</span><span class="sxs-lookup"><span data-stu-id="d4cac-119">Create and assign a policy to omit the basic claims from tokens issued to a service principal.</span></span> |
|[<span data-ttu-id="d4cac-120">homeRealmDiscoveryPolicies</span><span class="sxs-lookup"><span data-stu-id="d4cac-120">homeRealmDiscoveryPolicies</span></span>](homeRealmDiscoveryPolicy.md)| <span data-ttu-id="d4cac-121">表示用于控制联盟用户的 Azure Active Directory 身份验证行为的策略，尤其适用于联合域中的自动加速和用户身份验证限制。</span><span class="sxs-lookup"><span data-stu-id="d4cac-121">Represents a policy to control Azure Active Directory authentication behavior for federated users, in particular for auto-acceleration and user authentication restrictions in federated domains.</span></span>| <span data-ttu-id="d4cac-122">将所有用户配置为跳过 "主页领域发现"，并将其直接路由到 ADFS 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="d4cac-122">Configure all users to skip home realm discovery and be routed directly to ADFS for authentication.</span></span> |
|[<span data-ttu-id="d4cac-123">tokenLifetimePolicies</span><span class="sxs-lookup"><span data-stu-id="d4cac-123">tokenLifetimePolicies</span></span>](tokenlifetimepolicy.md)|<span data-ttu-id="d4cac-124">表示用于访问受保护的资源的访问令牌的生存期持续时间。</span><span class="sxs-lookup"><span data-stu-id="d4cac-124">Represents the lifetime duration of access tokens used to access protected resources.</span></span>| <span data-ttu-id="d4cac-125">配置一个具有短于默认令牌生存期的特别敏感的应用程序。</span><span class="sxs-lookup"><span data-stu-id="d4cac-125">Configure a particularly sensitive application with a shorter than default token lifetime.</span></span>|
|[<span data-ttu-id="d4cac-126">tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="d4cac-126">tokenIssuancePolicy</span></span>](tokenIssuancePolicy.md)|<span data-ttu-id="d4cac-127">表示指定由 Azure AD 颁发的 SAML 令牌的特征的策略。</span><span class="sxs-lookup"><span data-stu-id="d4cac-127">Represents the policy to specify the characteristics of SAML tokens issued by Azure AD.</span></span>| <span data-ttu-id="d4cac-128">配置用于发出 SAML 令牌的签名算法或 SAML 令牌版本。</span><span class="sxs-lookup"><span data-stu-id="d4cac-128">Configure the signing algorithm or SAML token version to be used to issue the SAML token.</span></span>
|[<span data-ttu-id="d4cac-129">identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="d4cac-129">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md)|<span data-ttu-id="d4cac-130">代表 "Azure AD 安全性默认策略"。</span><span class="sxs-lookup"><span data-stu-id="d4cac-130">Represents the Azure AD security defaults policy.</span></span>| <span data-ttu-id="d4cac-131">配置 Azure AD 安全性默认策略以防止受到常见攻击。</span><span class="sxs-lookup"><span data-stu-id="d4cac-131">Configure the Azure AD security defaults policy to protect against common attacks.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d4cac-132">后续步骤</span><span class="sxs-lookup"><span data-stu-id="d4cac-132">Next steps</span></span>

* <span data-ttu-id="d4cac-133">查看上面列出的不同策略资源类型及其各种方法。</span><span class="sxs-lookup"><span data-stu-id="d4cac-133">Review the different policy resouce types listed above and their various methods.</span></span>
* <span data-ttu-id="d4cac-134">在 [Graph 资源管理器](https://developer.microsoft.com/graph/graph-explorer)中试用 API。</span><span class="sxs-lookup"><span data-stu-id="d4cac-134">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>


