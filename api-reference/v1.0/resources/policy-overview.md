---
title: 策略 API 概述
description: Azure Active Directory 使用策略控制组织中的 Azure AD 功能行为。
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: cbaf736f8296ef7125b8f22ae231169b6c4b2202
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845930"
---
# <a name="azure-ad-policy-overview"></a><span data-ttu-id="6bed5-103">Azure AD 策略概述</span><span class="sxs-lookup"><span data-stu-id="6bed5-103">Azure AD policy overview</span></span>

<span data-ttu-id="6bed5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6bed5-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="6bed5-105">Azure Active Directory （Azure AD）使用策略控制组织中的 Azure AD 功能行为。</span><span class="sxs-lookup"><span data-stu-id="6bed5-105">Azure Active Directory (Azure AD) uses policies to control Azure AD feature behaviors in your organization.</span></span> <span data-ttu-id="6bed5-106">策略是您可以在应用程序、服务主体、组或其分配到的整个组织上实施的自定义规则。</span><span class="sxs-lookup"><span data-stu-id="6bed5-106">Policies are custom rules that you can enforce on applications, service principals, groups, or on the entire organization they are assigned to.</span></span>

## <a name="what-policies-are-available"></a><span data-ttu-id="6bed5-107">有哪些策略可用？</span><span class="sxs-lookup"><span data-stu-id="6bed5-107">What policies are available?</span></span>

| <span data-ttu-id="6bed5-108">策略类型</span><span class="sxs-lookup"><span data-stu-id="6bed5-108">Policy type</span></span>       | <span data-ttu-id="6bed5-109">说明</span><span class="sxs-lookup"><span data-stu-id="6bed5-109">Description</span></span> | <span data-ttu-id="6bed5-110">示例</span><span class="sxs-lookup"><span data-stu-id="6bed5-110">Examples</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="6bed5-111">activityBasedTimeoutPolicies</span><span class="sxs-lookup"><span data-stu-id="6bed5-111">activityBasedTimeoutPolicies</span></span>](activityBasedTimeoutPolicy.md)| <span data-ttu-id="6bed5-112">表示在一段时间不活动后控制 web 会话的自动注销的策略，适用于支持基于活动的超时功能的应用程序。</span><span class="sxs-lookup"><span data-stu-id="6bed5-112">Represents a policy that controls automatic sign-out for web sessions after a period of inactivity, for applications that support activity-based timeout functionality.</span></span>| <span data-ttu-id="6bed5-113">将 Azure 门户配置为使非活动超时为15分钟。</span><span class="sxs-lookup"><span data-stu-id="6bed5-113">Configure the Azure portal to have an inactivity timeout of 15 minutes.</span></span> |
|[<span data-ttu-id="6bed5-114">claimsMappingPolicies</span><span class="sxs-lookup"><span data-stu-id="6bed5-114">claimsMappingPolicies</span></span>](claimsMappingPolicy.md)| <span data-ttu-id="6bed5-115">表示对颁发给特定应用程序的令牌的 WS 馈送、SAML、OAuth 2.0 和 OpenID Connect 协议的声明映射策略。</span><span class="sxs-lookup"><span data-stu-id="6bed5-115">Represents the claim-mapping policies for WS-Fed, SAML, OAuth 2.0, and OpenID Connect protocols, for tokens issued to a specific application.</span></span> | <span data-ttu-id="6bed5-116">创建和分配策略以省略颁发给服务主体的令牌中的基本声明。</span><span class="sxs-lookup"><span data-stu-id="6bed5-116">Create and assign a policy to omit the basic claims from tokens issued to a service principal.</span></span> |
|[<span data-ttu-id="6bed5-117">homeRealmDiscoveryPolicies</span><span class="sxs-lookup"><span data-stu-id="6bed5-117">homeRealmDiscoveryPolicies</span></span>](homeRealmDiscoveryPolicy.md)| <span data-ttu-id="6bed5-118">表示用于控制联盟用户的 Azure Active Directory 身份验证行为的策略，尤其适用于联合域中的自动加速和用户身份验证限制。</span><span class="sxs-lookup"><span data-stu-id="6bed5-118">Represents a policy to control Azure Active Directory authentication behavior for federated users, in particular for auto-acceleration and user authentication restrictions in federated domains.</span></span>| <span data-ttu-id="6bed5-119">将所有用户配置为跳过 "主页领域发现"，并将其直接路由到 ADFS 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="6bed5-119">Configure all users to skip home realm discovery and be routed directly to ADFS for authentication.</span></span> |
|[<span data-ttu-id="6bed5-120">tokenLifetimePolicies</span><span class="sxs-lookup"><span data-stu-id="6bed5-120">tokenLifetimePolicies</span></span>](tokenlifetimepolicy.md)|<span data-ttu-id="6bed5-121">表示用于访问受保护的资源的访问令牌的生存期持续时间。</span><span class="sxs-lookup"><span data-stu-id="6bed5-121">Represents the lifetime duration of access tokens used to access protected resources.</span></span>| <span data-ttu-id="6bed5-122">配置一个具有短于默认令牌生存期的特别敏感的应用程序。</span><span class="sxs-lookup"><span data-stu-id="6bed5-122">Configure a particularly sensitive application with a shorter than default token lifetime.</span></span>|
|[<span data-ttu-id="6bed5-123">tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="6bed5-123">tokenIssuancePolicy</span></span>](tokenIssuancePolicy.md)|<span data-ttu-id="6bed5-124">表示指定由 Azure AD 颁发的 SAML 令牌的特征的策略。</span><span class="sxs-lookup"><span data-stu-id="6bed5-124">Represents the policy to specify the characteristics of SAML tokens issued by Azure AD.</span></span>| <span data-ttu-id="6bed5-125">配置用于发出 SAML 令牌的签名算法或 SAML 令牌版本。</span><span class="sxs-lookup"><span data-stu-id="6bed5-125">Configure the signing algorithm or SAML token version to be used to issue the SAML token.</span></span>

## <a name="next-steps"></a><span data-ttu-id="6bed5-126">后续步骤</span><span class="sxs-lookup"><span data-stu-id="6bed5-126">Next steps</span></span>

* <span data-ttu-id="6bed5-127">查看上面列出的不同策略资源类型及其各种方法。</span><span class="sxs-lookup"><span data-stu-id="6bed5-127">Review the different policy resouce types listed above and their various methods.</span></span>
* <span data-ttu-id="6bed5-128">请尝试 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中的 API。</span><span class="sxs-lookup"><span data-stu-id="6bed5-128">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
