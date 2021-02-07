---
title: 标识保护 API
description: identityProtectionRoot 资源类型
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 344dc8073ee33d028943c803eb560f94a4ecdc86
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129742"
---
# <a name="identityprotectionroot-resource-type"></a><span data-ttu-id="4b658-103">identityProtectionRoot 资源类型</span><span class="sxs-lookup"><span data-stu-id="4b658-103">identityProtectionRoot resource type</span></span>

<span data-ttu-id="4b658-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b658-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4b658-105">身份保护是一种工具，允许组织发现、调查和修正其环境中基于标识的风险。</span><span class="sxs-lookup"><span data-stu-id="4b658-105">Identity Protection is a tool that allows organizations to discover, investigate, and remediate identity-based risks in their environment.</span></span> <span data-ttu-id="4b658-106">可以使用以下 Microsoft Graph API 查询 Identity Protection 检测到的风险：</span><span class="sxs-lookup"><span data-stu-id="4b658-106">You can use the following Microsoft Graph APIs to query risks detected by Identity Protection:</span></span> 

* <span data-ttu-id="4b658-107">[riskDetection](riskdetection.md) - 在 Microsoft Graph 中查询用户和登录链接风险检测列表，以及检测相关信息。</span><span class="sxs-lookup"><span data-stu-id="4b658-107">[riskDetection](riskdetection.md) - Query Microsoft Graph for a list of both user and sign-in linked risk detections and associated information about the detection.</span></span> <span data-ttu-id="4b658-108">Azure AD Identity Protection 中的风险检测包括任何与目录中的用户帐户相关的已识别可疑操作。</span><span class="sxs-lookup"><span data-stu-id="4b658-108">Risk detections in Azure AD Identity Protection include any identified suspicious actions related to user accounts in the directory.</span></span>

* <span data-ttu-id="4b658-109">[riskyUsers](riskyuser.md) - 查询 Microsoft Graph，获取标识保护检测到有风险的用户的信息。</span><span class="sxs-lookup"><span data-stu-id="4b658-109">[riskyUsers](riskyuser.md) - Query Microsoft Graph for information about users that Identity Protection detected as risky.</span></span> <span data-ttu-id="4b658-110">用户风险表示给定标识或帐户受到威胁的可能性。</span><span class="sxs-lookup"><span data-stu-id="4b658-110">User risk represents the probability that a given identity or account is compromised.</span></span> <span data-ttu-id="4b658-111">这些风险使用 Microsoft 的内部和外部威胁情报源（包括安全研究人员、法律专业人员、Microsoft 的安全团队和其他受信任来源）脱机计算。</span><span class="sxs-lookup"><span data-stu-id="4b658-111">These risks are calculated offline using Microsoft’s internal and external threat intelligence sources, including security researchers, law enforcement professionals, security teams at Microsoft, and other trusted sources.</span></span>

* <span data-ttu-id="4b658-112">[signIn](signin.md) - 查询 Microsoft Graph，获取与风险状态、详细信息和级别相关的特定属性的 Azure AD 登录信息。</span><span class="sxs-lookup"><span data-stu-id="4b658-112">[signIn](signin.md) - Query Microsoft Graph for information about Azure AD sign-ins with specific properties related to risk state, detail, and level.</span></span> <span data-ttu-id="4b658-113">登录风险表示给定身份验证请求未由标识所有者授权的概率。</span><span class="sxs-lookup"><span data-stu-id="4b658-113">A sign-in risk represents the probability that a given authentication request isn’t authorized by the identity owner.</span></span> <span data-ttu-id="4b658-114">可以使用 Microsoft 的内部和外部威胁情报源（包括安全研究人员、法律专业人员、Microsoft 的安全团队和其他受信任来源）实时或脱机计算这些风险。</span><span class="sxs-lookup"><span data-stu-id="4b658-114">These risks can be calculated in real-time or calculated offline using Microsoft’s internal and external threat intelligence sources, including security researchers, law enforcement professionals, security teams at Microsoft, and other trusted sources.</span></span>

## <a name="what-can-i-do-with-identity-protection-apis-in-microsoft-graph"></a><span data-ttu-id="4b658-115">使用 Microsoft Graph 中的标识保护 API 可以做什么？</span><span class="sxs-lookup"><span data-stu-id="4b658-115">What can I do with Identity Protection APIs in Microsoft Graph?</span></span>

<span data-ttu-id="4b658-116">以下是处理审核日志数据的常见请求：</span><span class="sxs-lookup"><span data-stu-id="4b658-116">The following are popular requests for working with audit log data:</span></span>

<span data-ttu-id="4b658-117">Operation</span><span class="sxs-lookup"><span data-stu-id="4b658-117">Operation</span></span> | <span data-ttu-id="4b658-118">URL</span><span class="sxs-lookup"><span data-stu-id="4b658-118">URL</span></span>
:----------|:----
<span data-ttu-id="4b658-119">获取有风险的用户</span><span class="sxs-lookup"><span data-stu-id="4b658-119">GET risky users</span></span> | [<span data-ttu-id="4b658-120">GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers</span><span class="sxs-lookup"><span data-stu-id="4b658-120">GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskyUsers&version=v1.0)
<span data-ttu-id="4b658-121">获取风险检测</span><span class="sxs-lookup"><span data-stu-id="4b658-121">GET risk detections</span></span> | [<span data-ttu-id="4b658-122">GET https://graph.microsoft.com/v1.0/identityProtection/riskDetections</span><span class="sxs-lookup"><span data-stu-id="4b658-122">GET https://graph.microsoft.com/v1.0/identityProtection/riskDetections</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskDetections&version=v1.0)
<span data-ttu-id="4b658-123">获取用户的风险历史记录</span><span class="sxs-lookup"><span data-stu-id="4b658-123">GET a user's risk history</span></span> | [<span data-ttu-id="4b658-124">GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/{riskyUserId}/history</span><span class="sxs-lookup"><span data-stu-id="4b658-124">GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/{riskyUserId}/history</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskyUsers/{riskyUserId}/history&version=v1.0)
<span data-ttu-id="4b658-125">确认用户遭到入侵</span><span class="sxs-lookup"><span data-stu-id="4b658-125">CONFIRM a user as compromised</span></span> | [<span data-ttu-id="4b658-126">发布 https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/confirmCompromised</span><span class="sxs-lookup"><span data-stu-id="4b658-126">POST https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/confirmCompromised</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=/identityProtection/riskyUsers/confirmCompromised&version=v1.0)
<span data-ttu-id="4b658-127">消除有风险的用户</span><span class="sxs-lookup"><span data-stu-id="4b658-127">DISMISS a risky user</span></span> | [<span data-ttu-id="4b658-128">发布 https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/dismiss</span><span class="sxs-lookup"><span data-stu-id="4b658-128">POST https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/dismiss</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=/identityProtection/riskyUsers/dismiss&version=v1.0)

## <a name="what-licenses-do-i-need"></a><span data-ttu-id="4b658-129">需要哪些许可证？</span><span class="sxs-lookup"><span data-stu-id="4b658-129">What licenses do I need?</span></span>

<span data-ttu-id="4b658-130">Azure AD Identity Protection 是一项高级功能。</span><span class="sxs-lookup"><span data-stu-id="4b658-130">Azure AD Identity Protection is a premium feature.</span></span> <span data-ttu-id="4b658-131">你需要 Azure AD Premium P1 或 P2 许可证才能访问 riskDetection API (注意：P1 许可证会收到有限的风险) 。</span><span class="sxs-lookup"><span data-stu-id="4b658-131">You need an Azure AD Premium P1 or P2 license to access the riskDetection API (note: P1 licenses receive limited risk information).</span></span> <span data-ttu-id="4b658-132">riskyUsers API 仅适用于 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="4b658-132">The riskyUsers API is only available to Azure AD Premium P2 licenses only.</span></span>

## <a name="see-also"></a><span data-ttu-id="4b658-133">另请参阅</span><span class="sxs-lookup"><span data-stu-id="4b658-133">See also</span></span>

* [<span data-ttu-id="4b658-134">关于 Azure Active Directory Identity Protection</span><span class="sxs-lookup"><span data-stu-id="4b658-134">About Azure Active Directory Identity Protection</span></span>](/azure/active-directory/identity-protection/overview-identity-protection)
* [<span data-ttu-id="4b658-135">Azure Active Directory 标识保护和 Microsoft Graph 入门</span><span class="sxs-lookup"><span data-stu-id="4b658-135">Get started with Azure Active Directory identity protection and Microsoft Graph</span></span>](/azure/active-directory/identity-protection/howto-identity-protection-graph-api)
