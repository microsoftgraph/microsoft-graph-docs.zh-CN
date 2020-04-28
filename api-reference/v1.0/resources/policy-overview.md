---
title: 策略 API 概述
description: Azure Active Directory 使用策略控制组织中的 Azure AD 功能行为。
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: c34d8114e90aaf3c680ed89da4d16cd12880e71e
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2020
ms.locfileid: "43917549"
---
# <a name="azure-ad-policy-overview"></a><span data-ttu-id="eb250-103">Azure AD 策略概述</span><span class="sxs-lookup"><span data-stu-id="eb250-103">Azure AD policy overview</span></span>

<span data-ttu-id="eb250-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb250-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="eb250-105">Azure Active Directory （Azure AD）使用策略控制组织中的 Azure AD 功能行为。</span><span class="sxs-lookup"><span data-stu-id="eb250-105">Azure Active Directory (Azure AD) uses policies to control Azure AD feature behaviors in your organization.</span></span> <span data-ttu-id="eb250-106">策略是您可以在应用程序、服务主体、组或其分配到的整个组织上实施的自定义规则。</span><span class="sxs-lookup"><span data-stu-id="eb250-106">Policies are custom rules that you can enforce on applications, service principals, groups, or on the entire organization they are assigned to.</span></span>

## <a name="what-policies-are-available"></a><span data-ttu-id="eb250-107">有哪些策略可用？</span><span class="sxs-lookup"><span data-stu-id="eb250-107">What policies are available?</span></span>

| <span data-ttu-id="eb250-108">策略类型</span><span class="sxs-lookup"><span data-stu-id="eb250-108">Policy type</span></span>       | <span data-ttu-id="eb250-109">说明</span><span class="sxs-lookup"><span data-stu-id="eb250-109">Description</span></span> | <span data-ttu-id="eb250-110">示例</span><span class="sxs-lookup"><span data-stu-id="eb250-110">Examples</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="eb250-111">activityBasedTimeoutPolicies</span><span class="sxs-lookup"><span data-stu-id="eb250-111">activityBasedTimeoutPolicies</span></span>](activityBasedTimeoutPolicy.md)| <span data-ttu-id="eb250-112">表示在一段时间不活动后控制 web 会话的自动注销的策略，适用于支持基于活动的超时功能的应用程序。</span><span class="sxs-lookup"><span data-stu-id="eb250-112">Represents a policy that controls automatic sign-out for web sessions after a period of inactivity, for applications that support activity-based timeout functionality.</span></span>| <span data-ttu-id="eb250-113">将 Azure 门户配置为使非活动超时为15分钟。</span><span class="sxs-lookup"><span data-stu-id="eb250-113">Configure the Azure portal to have an inactivity timeout of 15 minutes.</span></span> |
|[<span data-ttu-id="eb250-114">homeRealmDiscoveryPolicies</span><span class="sxs-lookup"><span data-stu-id="eb250-114">homeRealmDiscoveryPolicies</span></span>](homeRealmDiscoveryPolicy.md)| <span data-ttu-id="eb250-115">表示用于控制联盟用户的 Azure Active Directory 身份验证行为的策略，尤其适用于联合域中的自动加速和用户身份验证限制。</span><span class="sxs-lookup"><span data-stu-id="eb250-115">Represents a policy to control Azure Active Directory authentication behavior for federated users, in particular for auto-acceleration and user authentication restrictions in federated domains.</span></span>| <span data-ttu-id="eb250-116">将所有用户配置为跳过 "主页领域发现"，并将其直接路由到 ADFS 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="eb250-116">Configure all users to skip home realm discovery and be routed directly to ADFS for authentication.</span></span> |
|[<span data-ttu-id="eb250-117">tokenLifetimePolicies</span><span class="sxs-lookup"><span data-stu-id="eb250-117">tokenLifetimePolicies</span></span>](tokenlifetimepolicy.md)|<span data-ttu-id="eb250-118">表示用于访问受保护的资源的访问令牌的生存期持续时间。</span><span class="sxs-lookup"><span data-stu-id="eb250-118">Represents the lifetime duration of access tokens used to access protected resources.</span></span>| <span data-ttu-id="eb250-119">配置一个具有短于默认令牌生存期的特别敏感的应用程序。</span><span class="sxs-lookup"><span data-stu-id="eb250-119">Configure a particularly sensitive application with a shorter than default token lifetime.</span></span>|
|[<span data-ttu-id="eb250-120">tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="eb250-120">tokenIssuancePolicy</span></span>](tokenIssuancePolicy.md)|<span data-ttu-id="eb250-121">表示指定由 Azure AD 颁发的 SAML 令牌的特征的策略。</span><span class="sxs-lookup"><span data-stu-id="eb250-121">Represents the policy to specify the characteristics of SAML tokens issued by Azure AD.</span></span>| <span data-ttu-id="eb250-122">配置用于发出 SAML 令牌的签名算法或 SAML 令牌版本。</span><span class="sxs-lookup"><span data-stu-id="eb250-122">Configure the signing algorithm or SAML token version to be used to issue the SAML token.</span></span>

## <a name="next-steps"></a><span data-ttu-id="eb250-123">后续步骤</span><span class="sxs-lookup"><span data-stu-id="eb250-123">Next steps</span></span>

* <span data-ttu-id="eb250-124">查看上面列出的不同策略资源类型及其各种方法。</span><span class="sxs-lookup"><span data-stu-id="eb250-124">Review the different policy resouce types listed above and their various methods.</span></span>
* <span data-ttu-id="eb250-125">请尝试 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中的 API。</span><span class="sxs-lookup"><span data-stu-id="eb250-125">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
