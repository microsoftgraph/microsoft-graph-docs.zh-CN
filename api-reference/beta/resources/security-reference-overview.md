---
title: 使用 Microsoft Graph API 进行安全威胁检测和保护（预览）
description: 安全威胁的复杂程度不断提升，从而影响了全球经济。 损坏通常会在组织甚至发现之前很长时间完成。 您可以使用 Microsoft Graph 构建或扩展安全解决方案，这些解决方案可从多个源中整合和关联安全警报、检测尝试危害用户标识的威胁、解锁上下文数据以通知调查，并实现自动化安全操作以提高效率。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: conceptualPageType
ms.openlocfilehash: f5980cb2db52a5c418d69b8c786a5b6f51123e3b
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870108"
---
# <a name="use-the-microsoft-graph-api-for-security-threat-detection-and-protection-preview"></a><span data-ttu-id="298e8-105">使用 Microsoft Graph API 进行安全威胁检测和保护（预览）</span><span class="sxs-lookup"><span data-stu-id="298e8-105">Use the Microsoft Graph API for security threat detection and protection (preview)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="298e8-106">安全威胁的复杂程度不断提升，从而影响了全球经济。</span><span class="sxs-lookup"><span data-stu-id="298e8-106">The sophistication of security threats continues to escalate, affecting the global economy.</span></span> <span data-ttu-id="298e8-107">损坏通常会在组织甚至发现之前很长时间完成。</span><span class="sxs-lookup"><span data-stu-id="298e8-107">Damage is often done long before organizations even discover it.</span></span> <span data-ttu-id="298e8-108">您可以使用 Microsoft Graph 构建或扩展安全解决方案，这些解决方案可从多个源中整合和关联安全警报、检测尝试危害用户标识的威胁、解锁上下文数据以通知调查，并实现自动化安全操作以提高效率。</span><span class="sxs-lookup"><span data-stu-id="298e8-108">You can use Microsoft Graph to build or extend security solutions that consolidate and correlate security alerts from multiple sources, detect threats that attempt to compromise user identity, unlock contextual data to inform investigations, and automate security operations for greater efficiency.</span></span>

<span data-ttu-id="298e8-109">智能安全图形将来自世界各地的 Microsoft、安全运营中心和合作伙伴的安全智能组合在一起，构成集成安全解决方案生态系统。</span><span class="sxs-lookup"><span data-stu-id="298e8-109">Intelligent Security Graph brings together security intelligence from within Microsoft, security operations centers, and partners from around the world to form an ecosystem of integrated security solutions.</span></span> <span data-ttu-id="298e8-110">通过使用机器学习、行为监控和云规模，智能安全图形可以更好地对威胁进行快速和全面的保护、检测和响应。</span><span class="sxs-lookup"><span data-stu-id="298e8-110">Using machine learning, behavioral monitoring, and the scale of the cloud, the Intelligent Security Graph can better protect, detect, and respond to threats quickly and comprehensively.</span></span> <span data-ttu-id="298e8-111">[安全 API](security-api-overview.md)将您连接到[智能安全图形](https://www.microsoft.com/en-us/security/intelligence-security-api)，为您提供可操作且具有整体的解决方案。</span><span class="sxs-lookup"><span data-stu-id="298e8-111">The [security API](security-api-overview.md) connects you to the [Intelligent Security Graph](https://www.microsoft.com/en-us/security/intelligence-security-api), empowering you with solutions that are actionable and holistic.</span></span>

<span data-ttu-id="298e8-112">[Identity protection 风险事件 API](identityprotection-root.md)为 Azure AD Premium P1 和 P2 客户提供了轻松访问，以查询[标识保护所进行的风险检测](/azure/active-directory/active-directory-identityprotection-graph-getting-started)并在 SIEM 系统和安全应用程序中使用这些事件。</span><span class="sxs-lookup"><span data-stu-id="298e8-112">The [identity protection risk events API](identityprotection-root.md) gives easy access for Azure AD Premium P1 and P2 customers to query [risk detections made by Identity Protection](/azure/active-directory/active-directory-identityprotection-graph-getting-started) and use those events in SIEM systems and security applications.</span></span>

## <a name="see-also"></a><span data-ttu-id="298e8-113">另请参阅</span><span class="sxs-lookup"><span data-stu-id="298e8-113">See also</span></span>

- [<span data-ttu-id="298e8-114">为什么要使用安全 API？</span><span class="sxs-lookup"><span data-stu-id="298e8-114">Why use the security API?</span></span>](/graph/security-concept-overview#why-use-the-security-api-and-connect-with-microsoft-intelligent-security-graph)
- [<span data-ttu-id="298e8-115">使用安全 API 与智能安全图形集成</span><span class="sxs-lookup"><span data-stu-id="298e8-115">Use the security API to integrate with Intelligent Security Graph</span></span>](security-api-overview.md)
- [<span data-ttu-id="298e8-116">为什么要使用 Azure AD 来保护组织中的身份？</span><span class="sxs-lookup"><span data-stu-id="298e8-116">Why use Azure AD to protect identities in your organization?</span></span>](/graph/security-concept-overview#why-use-azure-ad-to-protect-identities-in-your-organization)
- [<span data-ttu-id="298e8-117">使用 Azure AD 标识保护 API</span><span class="sxs-lookup"><span data-stu-id="298e8-117">Use the Azure AD Identity Protection API</span></span>](identityprotection-root.md)
