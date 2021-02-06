---
title: 使用 Azure AD 标识保护 API
description: 可以使用 Microsoft Graph 查询 Identity Protection API，以接收有关 Azure AD Identity Protection 检测到的风险的信息。
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 712aa53234f8917fec334c52234db8155f1e913e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129385"
---
# <a name="use-the-azure-ad-identity-protection-api"></a><span data-ttu-id="9b01a-103">使用 Azure AD 标识保护 API</span><span class="sxs-lookup"><span data-stu-id="9b01a-103">Use the Azure AD identity protection API</span></span>

<span data-ttu-id="9b01a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b01a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b01a-105">身份保护是一种工具，允许组织发现、调查和修正其环境中基于标识的风险。</span><span class="sxs-lookup"><span data-stu-id="9b01a-105">Identity Protection is a tool that allows organizations to discover, investigate, and remediate identity-based risks in their environment.</span></span> <span data-ttu-id="9b01a-106">可以使用以下 Microsoft Graph API 查询 Identity Protection 检测到的风险：</span><span class="sxs-lookup"><span data-stu-id="9b01a-106">You can use the following Microsoft Graph APIs to query risks detected by Identity Protection:</span></span> 

* <span data-ttu-id="9b01a-107">[riskDetection](riskdetection.md) - 在 Microsoft Graph 中查询用户和登录链接风险检测列表，以及检测相关信息。</span><span class="sxs-lookup"><span data-stu-id="9b01a-107">[riskDetection](riskdetection.md) - Query Microsoft Graph for a list of both user and sign-in linked risk detections and associated information about the detection.</span></span> <span data-ttu-id="9b01a-108">Azure AD Identity Protection 中的风险检测包括任何与目录中的用户帐户相关的已识别可疑操作。</span><span class="sxs-lookup"><span data-stu-id="9b01a-108">Risk detections in Azure AD Identity Protection include any identified suspicious actions related to user accounts in the directory.</span></span>

* <span data-ttu-id="9b01a-109">[riskyUsers](riskyuser.md) - 查询 Microsoft Graph，获取标识保护检测到有风险的用户的信息。</span><span class="sxs-lookup"><span data-stu-id="9b01a-109">[riskyUsers](riskyuser.md) - Query Microsoft Graph for information about users that Identity Protection detected as risky.</span></span> <span data-ttu-id="9b01a-110">用户风险表示给定标识或帐户受到威胁的可能性。</span><span class="sxs-lookup"><span data-stu-id="9b01a-110">User risk represents the probability that a given identity or account is compromised.</span></span> <span data-ttu-id="9b01a-111">这些风险使用 Microsoft 的内部和外部威胁情报源（包括安全研究人员、法律专业人员、Microsoft 的安全团队和其他受信任来源）脱机计算。</span><span class="sxs-lookup"><span data-stu-id="9b01a-111">These risks are calculated offline using Microsoft’s internal and external threat intelligence sources, including security researchers, law enforcement professionals, security teams at Microsoft, and other trusted sources.</span></span>

* <span data-ttu-id="9b01a-112">[signIn](signin.md) - 查询 Microsoft Graph，获取与风险状态、详细信息和级别相关的特定属性的 Azure AD 登录信息。</span><span class="sxs-lookup"><span data-stu-id="9b01a-112">[signIn](signin.md) - Query Microsoft Graph for information about Azure AD sign-ins with specific properties related to risk state, detail, and level.</span></span> <span data-ttu-id="9b01a-113">登录风险表示给定身份验证请求未由标识所有者授权的概率。</span><span class="sxs-lookup"><span data-stu-id="9b01a-113">A sign-in risk represents the probability that a given authentication request isn’t authorized by the identity owner.</span></span> <span data-ttu-id="9b01a-114">可以使用 Microsoft 的内部和外部威胁情报源（包括安全研究人员、法律专业人员、Microsoft 的安全团队和其他受信任来源）实时或脱机计算这些风险。</span><span class="sxs-lookup"><span data-stu-id="9b01a-114">These risks can be calculated in real-time or calculated offline using Microsoft’s internal and external threat intelligence sources, including security researchers, law enforcement professionals, security teams at Microsoft, and other trusted sources.</span></span>

* <span data-ttu-id="9b01a-115">[identityRiskEvents](identityriskevent.md) - 查询 Microsoft Graph，获取风险检测和相关信息的列表。</span><span class="sxs-lookup"><span data-stu-id="9b01a-115">[identityRiskEvents](identityriskevent.md) - Query Microsoft Graph for a list of risk detections and associated information.</span></span> <span data-ttu-id="9b01a-116">此 API 已弃用;我们建议你改为使用 **riskDetections。**</span><span class="sxs-lookup"><span data-stu-id="9b01a-116">This API is deprecated; we recommend that you use **riskDetections** instead.</span></span>

>[!CAUTION]
><span data-ttu-id="9b01a-117">**identityRiskEvents** API 已弃用，将在 2020 年 1 月 10 日停止返回数据。</span><span class="sxs-lookup"><span data-stu-id="9b01a-117">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="9b01a-118">有关详细信息，请参阅 [IdentityRiskEvents API 的弃用](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/)。</span><span class="sxs-lookup"><span data-stu-id="9b01a-118">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

## <a name="see-also"></a><span data-ttu-id="9b01a-119">另请参阅</span><span class="sxs-lookup"><span data-stu-id="9b01a-119">See also</span></span>

* [<span data-ttu-id="9b01a-120">关于 Azure Active Directory Identity Protection</span><span class="sxs-lookup"><span data-stu-id="9b01a-120">About Azure Active Directory Identity Protection</span></span>](/azure/active-directory/identity-protection/overview-identity-protection)
* [<span data-ttu-id="9b01a-121">Azure Active Directory 标识保护和 Microsoft Graph 入门</span><span class="sxs-lookup"><span data-stu-id="9b01a-121">Get started with Azure Active Directory identity protection and Microsoft Graph</span></span>](/azure/active-directory/identity-protection/howto-identity-protection-graph-api)
