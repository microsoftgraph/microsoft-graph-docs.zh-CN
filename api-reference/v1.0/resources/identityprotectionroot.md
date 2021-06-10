---
title: 标识保护 API
description: identityProtectionRoot 资源类型
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: d4eee47b1503b8c37eb0551817725b966d492866
ms.sourcegitcommit: 9eeb056f311044aaa40654cdb3ae5ae61f1c4d04
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/09/2021
ms.locfileid: "52854122"
---
# <a name="identityprotectionroot-resource-type"></a><span data-ttu-id="deba7-103">identityProtectionRoot 资源类型</span><span class="sxs-lookup"><span data-stu-id="deba7-103">identityProtectionRoot resource type</span></span>

<span data-ttu-id="deba7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="deba7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="deba7-105">标识保护是一种工具，允许组织发现、调查和修正其环境中基于标识的风险。</span><span class="sxs-lookup"><span data-stu-id="deba7-105">Identity Protection is a tool that allows organizations to discover, investigate, and remediate identity-based risks in their environment.</span></span> <span data-ttu-id="deba7-106">可以使用以下 Microsoft Graph API 查询 Identity Protection 检测到的风险：</span><span class="sxs-lookup"><span data-stu-id="deba7-106">You can use the following Microsoft Graph APIs to query risks detected by Identity Protection:</span></span> 

* <span data-ttu-id="deba7-107">[riskDetection](riskdetection.md) - Graph Microsoft 查询用户和登录链接风险检测的列表，以及有关检测的相关信息。</span><span class="sxs-lookup"><span data-stu-id="deba7-107">[riskDetection](riskdetection.md) - Query Microsoft Graph for a list of both user and sign-in linked risk detections and associated information about the detection.</span></span> <span data-ttu-id="deba7-108">Azure AD Identity Protection 中的风险检测包括任何与目录中的用户帐户相关的已识别可疑操作。</span><span class="sxs-lookup"><span data-stu-id="deba7-108">Risk detections in Azure AD Identity Protection include any identified suspicious actions related to user accounts in the directory.</span></span>

* <span data-ttu-id="deba7-109">[riskyUsers](riskyuser.md) - 查询 Microsoft Graph，获取标识保护检测到有风险的用户的信息。</span><span class="sxs-lookup"><span data-stu-id="deba7-109">[riskyUsers](riskyuser.md) - Query Microsoft Graph for information about users that Identity Protection detected as risky.</span></span> <span data-ttu-id="deba7-110">用户风险表示给定标识或帐户受到威胁的可能性。</span><span class="sxs-lookup"><span data-stu-id="deba7-110">User risk represents the probability that a given identity or account is compromised.</span></span> <span data-ttu-id="deba7-111">这些风险使用 Microsoft 的内部和外部威胁情报源（包括安全研究人员、执法机构、Microsoft 的安全团队和其他受信任来源）脱机计算。</span><span class="sxs-lookup"><span data-stu-id="deba7-111">These risks are calculated offline using Microsoft’s internal and external threat intelligence sources, including security researchers, law enforcement professionals, security teams at Microsoft, and other trusted sources.</span></span>

* <span data-ttu-id="deba7-112">[signIn](signin.md) - 查询 Microsoft Graph，获取与风险状态、详细信息和级别相关的特定属性的 Azure AD 登录信息。</span><span class="sxs-lookup"><span data-stu-id="deba7-112">[signIn](signin.md) - Query Microsoft Graph for information about Azure AD sign-ins with specific properties related to risk state, detail, and level.</span></span> <span data-ttu-id="deba7-113">登录风险表示给定身份验证请求未由标识所有者授权的概率。</span><span class="sxs-lookup"><span data-stu-id="deba7-113">A sign-in risk represents the probability that a given authentication request isn’t authorized by the identity owner.</span></span> <span data-ttu-id="deba7-114">可以使用 Microsoft 的内部和外部威胁情报源（包括安全研究人员、执法机构、Microsoft 的安全团队和其他受信任来源）实时计算或脱机计算这些风险。</span><span class="sxs-lookup"><span data-stu-id="deba7-114">These risks can be calculated in real-time or calculated offline using Microsoft’s internal and external threat intelligence sources, including security researchers, law enforcement professionals, security teams at Microsoft, and other trusted sources.</span></span>

## <a name="what-can-i-do-with-identity-protection-apis-in-microsoft-graph"></a><span data-ttu-id="deba7-115">在 Microsoft 服务中，可以使用标识保护 API Graph？</span><span class="sxs-lookup"><span data-stu-id="deba7-115">What can I do with Identity Protection APIs in Microsoft Graph?</span></span>

<span data-ttu-id="deba7-116">以下是处理审核日志数据的常见请求：</span><span class="sxs-lookup"><span data-stu-id="deba7-116">The following are popular requests for working with audit log data:</span></span>

<span data-ttu-id="deba7-117">Operation</span><span class="sxs-lookup"><span data-stu-id="deba7-117">Operation</span></span> | <span data-ttu-id="deba7-118">URL</span><span class="sxs-lookup"><span data-stu-id="deba7-118">URL</span></span>
:----------|:----
<span data-ttu-id="deba7-119">获取有风险的用户</span><span class="sxs-lookup"><span data-stu-id="deba7-119">GET risky users</span></span> | [<span data-ttu-id="deba7-120">GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers</span><span class="sxs-lookup"><span data-stu-id="deba7-120">GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskyUsers&version=v1.0)
<span data-ttu-id="deba7-121">获取风险检测</span><span class="sxs-lookup"><span data-stu-id="deba7-121">GET risk detections</span></span> | [<span data-ttu-id="deba7-122">GET https://graph.microsoft.com/v1.0/identityProtection/riskDetections</span><span class="sxs-lookup"><span data-stu-id="deba7-122">GET https://graph.microsoft.com/v1.0/identityProtection/riskDetections</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskDetections&version=v1.0)
<span data-ttu-id="deba7-123">获取用户的风险历史记录</span><span class="sxs-lookup"><span data-stu-id="deba7-123">GET a user's risk history</span></span> | [<span data-ttu-id="deba7-124">GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/{riskyUserId}/history</span><span class="sxs-lookup"><span data-stu-id="deba7-124">GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/{riskyUserId}/history</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskyUsers/{riskyUserId}/history&version=v1.0)
<span data-ttu-id="deba7-125">确认用户受到威胁</span><span class="sxs-lookup"><span data-stu-id="deba7-125">CONFIRM a user as compromised</span></span> | [<span data-ttu-id="deba7-126">发布 https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/confirmCompromised</span><span class="sxs-lookup"><span data-stu-id="deba7-126">POST https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/confirmCompromised</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=/identityProtection/riskyUsers/confirmCompromised&version=v1.0)
<span data-ttu-id="deba7-127">消除有风险的用户</span><span class="sxs-lookup"><span data-stu-id="deba7-127">DISMISS a risky user</span></span> | [<span data-ttu-id="deba7-128">发布 https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/dismiss</span><span class="sxs-lookup"><span data-stu-id="deba7-128">POST https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/dismiss</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=/identityProtection/riskyUsers/dismiss&version=v1.0)

<span data-ttu-id="deba7-129">有关特定指南和其他信息，请参阅使用 Microsoft Graph [API 识别和修正风险](/graph/tutorial-riskdetection-api)。</span><span class="sxs-lookup"><span data-stu-id="deba7-129">For specific guidance and additional information, see [Identify and remediate risks using Microsoft Graph APIs](/graph/tutorial-riskdetection-api).</span></span>

## <a name="what-licenses-do-i-need"></a><span data-ttu-id="deba7-130">需要哪些许可证？</span><span class="sxs-lookup"><span data-stu-id="deba7-130">What licenses do I need?</span></span>

<span data-ttu-id="deba7-131">Azure AD Identity Protection 是一项高级功能。</span><span class="sxs-lookup"><span data-stu-id="deba7-131">Azure AD Identity Protection is a premium feature.</span></span> <span data-ttu-id="deba7-132">你需要 Azure AD 高级版 P1 或 P2 许可证才能访问 riskDetection API (注意： P1 许可证会收到有限的) 。</span><span class="sxs-lookup"><span data-stu-id="deba7-132">You need an Azure AD Premium P1 or P2 license to access the riskDetection API (note: P1 licenses receive limited risk information).</span></span> <span data-ttu-id="deba7-133">riskyUsers API 仅适用于 Azure AD 高级版 P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="deba7-133">The riskyUsers API is only available to Azure AD Premium P2 licenses only.</span></span>

## <a name="see-also"></a><span data-ttu-id="deba7-134">另请参阅</span><span class="sxs-lookup"><span data-stu-id="deba7-134">See also</span></span>

* [<span data-ttu-id="deba7-135">关于 Azure Active Directory Identity Protection</span><span class="sxs-lookup"><span data-stu-id="deba7-135">About Azure Active Directory Identity Protection</span></span>](/azure/active-directory/identity-protection/overview-identity-protection)
* [<span data-ttu-id="deba7-136">开始使用 microsoft Azure Active Directory 和 Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="deba7-136">Get started with Azure Active Directory identity protection and Microsoft Graph</span></span>](/azure/active-directory/identity-protection/howto-identity-protection-graph-api)
