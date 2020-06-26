---
title: 标识保护 Api
description: identityProtectionRoot 资源类型
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d7b31b0a27ca96333087d55b3666f97eefdd70b9
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898049"
---
# <a name="identityprotectionroot-resource-type"></a><span data-ttu-id="8c69f-103">identityProtectionRoot 资源类型</span><span class="sxs-lookup"><span data-stu-id="8c69f-103">identityProtectionRoot resource type</span></span>

<span data-ttu-id="8c69f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c69f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8c69f-105">标识保护是一种工具，使组织能够在其环境中发现、调查和修正基于标识的风险。</span><span class="sxs-lookup"><span data-stu-id="8c69f-105">Identity Protection is a tool that allows organizations to discover, investigate, and remediate identity-based risks in their environment.</span></span> <span data-ttu-id="8c69f-106">您可以使用以下 Microsoft Graph Api 来查询由身份保护检测到的风险：</span><span class="sxs-lookup"><span data-stu-id="8c69f-106">You can use the following Microsoft Graph APIs to query risks detected by Identity Protection:</span></span> 

* <span data-ttu-id="8c69f-107">[riskDetection](riskdetection.md) -查询 Microsoft Graph，以获取用户和登录相关的风险检测以及有关检测的相关信息的列表。</span><span class="sxs-lookup"><span data-stu-id="8c69f-107">[riskDetection](riskdetection.md) - Query Microsoft Graph for a list of both user and sign-in linked risk detections and associated information about the detection.</span></span> <span data-ttu-id="8c69f-108">Azure AD 标识保护中的风险检测包括与目录中的用户帐户相关的任何已确定的可疑操作。</span><span class="sxs-lookup"><span data-stu-id="8c69f-108">Risk detections in Azure AD Identity Protection include any identified suspicious actions related to user accounts in the directory.</span></span>

* <span data-ttu-id="8c69f-109">[riskyUsers](riskyuser.md) -查询 Microsoft Graph，以获取标识保护检测为有风险的用户的信息。</span><span class="sxs-lookup"><span data-stu-id="8c69f-109">[riskyUsers](riskyuser.md) - Query Microsoft Graph for information about users that Identity Protection detected as risky.</span></span> <span data-ttu-id="8c69f-110">用户风险表示给定标识或帐户受到危害的可能性。</span><span class="sxs-lookup"><span data-stu-id="8c69f-110">User risk represents the probability that a given identity or account is compromised.</span></span> <span data-ttu-id="8c69f-111">这些风险是使用 Microsoft 的内部和外部威胁智能源（包括安全研究人员、执法人员、Microsoft 安全团队以及其他受信任的来源）进行脱机计算的。</span><span class="sxs-lookup"><span data-stu-id="8c69f-111">These risks are calculated offline using Microsoft’s internal and external threat intelligence sources, including security researchers, law enforcement professionals, security teams at Microsoft, and other trusted sources.</span></span>

* <span data-ttu-id="8c69f-112">[登录](signin.md)查询 Microsoft Graph，以获取有关具有与风险状态、详细信息和级别相关的特定属性的 Azure AD 登录信息。</span><span class="sxs-lookup"><span data-stu-id="8c69f-112">[signIn](signin.md) - Query Microsoft Graph for information about Azure AD sign-ins with specific properties related to risk state, detail, and level.</span></span> <span data-ttu-id="8c69f-113">登录风险表示标识所有者未授权给定的身份验证请求的可能性。</span><span class="sxs-lookup"><span data-stu-id="8c69f-113">A sign-in risk represents the probability that a given authentication request isn’t authorized by the identity owner.</span></span> <span data-ttu-id="8c69f-114">可以使用 Microsoft 的内部和外部威胁智能来源实时计算或计算这些风险，包括安全研究人员、执法人员、Microsoft 安全团队以及其他受信任的来源。</span><span class="sxs-lookup"><span data-stu-id="8c69f-114">These risks can be calculated in real-time or calculated offline using Microsoft’s internal and external threat intelligence sources, including security researchers, law enforcement professionals, security teams at Microsoft, and other trusted sources.</span></span>

## <a name="what-can-i-do-with-identity-protection-apis-in-microsoft-graph"></a><span data-ttu-id="8c69f-115">在 Microsoft Graph 中，我可以对身份保护 Api 执行哪些操作？</span><span class="sxs-lookup"><span data-stu-id="8c69f-115">What can I do with Identity Protection APIs in Microsoft Graph?</span></span>

<span data-ttu-id="8c69f-116">以下是处理审核日志数据的常见请求：</span><span class="sxs-lookup"><span data-stu-id="8c69f-116">The following are popular requests for working with audit log data:</span></span>

<span data-ttu-id="8c69f-117">Operation</span><span class="sxs-lookup"><span data-stu-id="8c69f-117">Operation</span></span> | <span data-ttu-id="8c69f-118">URL</span><span class="sxs-lookup"><span data-stu-id="8c69f-118">URL</span></span>
:----------|:----
<span data-ttu-id="8c69f-119">获取有风险的用户</span><span class="sxs-lookup"><span data-stu-id="8c69f-119">GET risky users</span></span> | [<span data-ttu-id="8c69f-120">GET https://graph.microsoft.com/v1.0/identityProtection/riskyUser</span><span class="sxs-lookup"><span data-stu-id="8c69f-120">GET https://graph.microsoft.com/v1.0/identityProtection/riskyUser</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskyUsers&version=v1.0)
<span data-ttu-id="8c69f-121">获取风险检测</span><span class="sxs-lookup"><span data-stu-id="8c69f-121">GET risk detections</span></span> | [<span data-ttu-id="8c69f-122">GET https://graph.microsoft.com/v1.0/identityProtection/riskDetections</span><span class="sxs-lookup"><span data-stu-id="8c69f-122">GET https://graph.microsoft.com/v1.0/identityProtection/riskDetections</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskDetections&version=v1.0)
<span data-ttu-id="8c69f-123">获取用户的风险历史记录</span><span class="sxs-lookup"><span data-stu-id="8c69f-123">GET a user's risk history</span></span> | [<span data-ttu-id="8c69f-124">GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/{riskyUserId}/history</span><span class="sxs-lookup"><span data-stu-id="8c69f-124">GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/{riskyUserId}/history</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskyUsers/{riskyUserId}/history&version=v1.0)
<span data-ttu-id="8c69f-125">确认用户是否受到威胁</span><span class="sxs-lookup"><span data-stu-id="8c69f-125">CONFIRM a user as compromised</span></span> | [<span data-ttu-id="8c69f-126">发布https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/confirmCompromised</span><span class="sxs-lookup"><span data-stu-id="8c69f-126">POST https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/confirmCompromised</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=/identityProtection/riskyUsers/confirmCompromised&version=v1.0)
<span data-ttu-id="8c69f-127">消除有风险的用户</span><span class="sxs-lookup"><span data-stu-id="8c69f-127">DISMISS a risky user</span></span> | [<span data-ttu-id="8c69f-128">发布https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/dismiss</span><span class="sxs-lookup"><span data-stu-id="8c69f-128">POST https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/dismiss</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=/identityProtection/riskyUsers/dismiss&version=v1.0)

## <a name="what-licenses-do-i-need"></a><span data-ttu-id="8c69f-129">需要哪些许可证？</span><span class="sxs-lookup"><span data-stu-id="8c69f-129">What licenses do I need?</span></span>

<span data-ttu-id="8c69f-130">Azure AD Identity Protection 是一项高级功能。</span><span class="sxs-lookup"><span data-stu-id="8c69f-130">Azure AD Identity Protection is a premium feature.</span></span> <span data-ttu-id="8c69f-131">您需要使用 Azure AD 高级 P1 或 P2 许可证来访问 riskDetection API （注意： P1 许可证收到有限的风险信息）。</span><span class="sxs-lookup"><span data-stu-id="8c69f-131">You need an Azure AD Premium P1 or P2 license to access the riskDetection API (note: P1 licenses receive limited risk information).</span></span> <span data-ttu-id="8c69f-132">RiskyUsers API 仅适用于 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="8c69f-132">The riskyUsers API is only available to Azure AD Premium P2 licenses only.</span></span>

## <a name="see-also"></a><span data-ttu-id="8c69f-133">另请参阅</span><span class="sxs-lookup"><span data-stu-id="8c69f-133">See also</span></span>

* [<span data-ttu-id="8c69f-134">关于 Azure Active Directory 标识保护</span><span class="sxs-lookup"><span data-stu-id="8c69f-134">About Azure Active Directory Identity Protection</span></span>](https://docs.microsoft.com/azure/active-directory/identity-protection/overview-identity-protection)
* [<span data-ttu-id="8c69f-135">Azure Active Directory 标识保护和 Microsoft Graph 入门</span><span class="sxs-lookup"><span data-stu-id="8c69f-135">Get started with Azure Active Directory identity protection and Microsoft Graph</span></span>](https://docs.microsoft.com/azure/active-directory/identity-protection/howto-identity-protection-graph-api)


