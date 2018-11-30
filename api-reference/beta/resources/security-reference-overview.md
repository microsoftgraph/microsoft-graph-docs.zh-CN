---
title: 使用 Microsoft Graph API 进行安全威胁检测和保护 （预览）
description: 安全威胁的复杂程度继续升级，全球经济影响。 通常损害长之前组织甚至发现。 您可以使用 Microsoft Graph 建立或扩展的合并和关联多个来源的安全警告、 检测尝试损害用户标识和 unlock 上下文数据来告知调查，并自动给出的威胁的安全解决方案安全性操作以提高效率。
ms.openlocfilehash: 48cfbc2ea2bfb0ce47e77d3d37e971c0a19b9158
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045220"
---
# <a name="use-the-microsoft-graph-api-for-security-threat-detection-and-protection-preview"></a><span data-ttu-id="a29e2-105">使用 Microsoft Graph API 进行安全威胁检测和保护 （预览）</span><span class="sxs-lookup"><span data-stu-id="a29e2-105">Use the Microsoft Graph API for security threat detection and protection (preview)</span></span>

> <span data-ttu-id="a29e2-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a29e2-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a29e2-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a29e2-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a29e2-108">安全威胁的复杂程度继续升级，全球经济影响。</span><span class="sxs-lookup"><span data-stu-id="a29e2-108">The sophistication of security threats continues to escalate, affecting the global economy.</span></span> <span data-ttu-id="a29e2-109">通常损害长之前组织甚至发现。</span><span class="sxs-lookup"><span data-stu-id="a29e2-109">Damage is often done long before organizations even discover it.</span></span> <span data-ttu-id="a29e2-110">您可以使用 Microsoft Graph 建立或扩展的合并和关联多个来源的安全警告、 检测尝试损害用户标识和 unlock 上下文数据来告知调查，并自动给出的威胁的安全解决方案安全性操作以提高效率。</span><span class="sxs-lookup"><span data-stu-id="a29e2-110">You can use Microsoft Graph to build or extend security solutions that consolidate and correlate security alerts from multiple sources, detect threats that attempt to compromise user identity, unlock contextual data to inform investigations, and automate security operations for greater efficiency.</span></span>

<span data-ttu-id="a29e2-111">智能安全图汇集了从 Microsoft、 安全操作中心和来自合作伙伴中的安全智能周围全球的表单的集成的安全性解决方案生态系统。</span><span class="sxs-lookup"><span data-stu-id="a29e2-111">Intelligent Security Graph brings together security intelligence from within Microsoft, security operations centers, and partners from around the world to form an ecosystem of integrated security solutions.</span></span> <span data-ttu-id="a29e2-112">使用机器学习、 行为监控设备以及云中的小数位数，智能安全图可以更好地保护、 检测和快速地全面响应威胁。</span><span class="sxs-lookup"><span data-stu-id="a29e2-112">Using machine learning, behavioral monitoring, and the scale of the cloud, the Intelligent Security Graph can better protect, detect, and respond to threats quickly and comprehensively.</span></span> <span data-ttu-id="a29e2-113">[安全 API](security-api-overview.md)将您连接到[智能安全图](https://www.microsoft.com/en-us/security/intelligence-security-api)，为您进行全面的可操作的解决方案。</span><span class="sxs-lookup"><span data-stu-id="a29e2-113">The [security API](security-api-overview.md) connects you to the [Intelligent Security Graph](https://www.microsoft.com/en-us/security/intelligence-security-api), empowering you with solutions that are actionable and holistic.</span></span>

<span data-ttu-id="a29e2-114">[标识保护风险事件 API](identityprotection-root.md) ，为 Azure AD Premium P1 和 P2 客户查询[风险检测所做的标识保护](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection-graph-getting-started)和 SIEM 系统和安全应用程序中使用这些事件的轻松访问。</span><span class="sxs-lookup"><span data-stu-id="a29e2-114">The [identity protection risk events API](identityprotection-root.md) gives easy access for Azure AD Premium P1 and P2 customers to query [risk detections made by Identity Protection](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection-graph-getting-started) and use those events in SIEM systems and security applications.</span></span>

## <a name="see-also"></a><span data-ttu-id="a29e2-115">另请参阅</span><span class="sxs-lookup"><span data-stu-id="a29e2-115">See also</span></span>

- [<span data-ttu-id="a29e2-116">为什么使用安全 API？</span><span class="sxs-lookup"><span data-stu-id="a29e2-116">Why use the security API?</span></span>](/graph/security-concept-overview#why-use-the-security-api-and-connect-with-microsoft-intelligent-security-graph)
- [<span data-ttu-id="a29e2-117">使用安全 API 与智能安全图集成</span><span class="sxs-lookup"><span data-stu-id="a29e2-117">Use the security API to integrate with Intelligent Security Graph</span></span>](security-api-overview.md)
- [<span data-ttu-id="a29e2-118">为什么要使用 Azure AD 来保护组织中的身份信息？</span><span class="sxs-lookup"><span data-stu-id="a29e2-118">Why use Azure AD to protect identities in your organization?</span></span>](/graph/security-concept-overview#why-use-azure-ad-to-protect-identities-in-your-organization)
- [<span data-ttu-id="a29e2-119">使用 Azure AD Identity Protection</span><span class="sxs-lookup"><span data-stu-id="a29e2-119">Use the Azure AD Identity Protection API</span></span>](identityprotection-root.md)
