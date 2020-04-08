---
title: 使用 Azure AD 标识保护 Api （预览）
description: 您可以使用 Microsoft Graph 来查询标识保护 Api，以接收 Azure AD Identity Protection 检测到的风险的相关信息。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 43fbfb8f0645d4d7d9a58135f2cd6fe986c62643
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181734"
---
# <a name="use-the-azure-ad-identity-protection-api-preview"></a><span data-ttu-id="99a89-103">使用 Azure AD 标识保护 API （预览）</span><span class="sxs-lookup"><span data-stu-id="99a89-103">Use the Azure AD identity protection API (preview)</span></span>

<span data-ttu-id="99a89-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99a89-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99a89-105">标识保护是一种工具，使组织能够在其环境中发现、调查和修正基于标识的风险。</span><span class="sxs-lookup"><span data-stu-id="99a89-105">Identity Protection is a tool that allows organizations to discover, investigate, and remediate identity-based risks in their environment.</span></span> <span data-ttu-id="99a89-106">您可以使用以下 Microsoft Graph Api 来查询由身份保护检测到的风险：</span><span class="sxs-lookup"><span data-stu-id="99a89-106">You can use the following Microsoft Graph APIs to query risks detected by Identity Protection:</span></span> 

* <span data-ttu-id="99a89-107">[riskDetection](riskdetection.md) -查询 Microsoft Graph，以获取用户和登录相关的风险检测以及有关检测的相关信息的列表。</span><span class="sxs-lookup"><span data-stu-id="99a89-107">[riskDetection](riskdetection.md) - Query Microsoft Graph for a list of both user and sign-in linked risk detections and associated information about the detection.</span></span> <span data-ttu-id="99a89-108">Azure AD 标识保护中的风险检测包括与目录中的用户帐户相关的任何已确定的可疑操作。</span><span class="sxs-lookup"><span data-stu-id="99a89-108">Risk detections in Azure AD Identity Protection include any identified suspicious actions related to user accounts in the directory.</span></span>

* <span data-ttu-id="99a89-109">[riskyUsers](riskyuser.md) -查询 Microsoft Graph，以获取标识保护检测为有风险的用户的信息。</span><span class="sxs-lookup"><span data-stu-id="99a89-109">[riskyUsers](riskyuser.md) - Query Microsoft Graph for information about users that Identity Protection detected as risky.</span></span> <span data-ttu-id="99a89-110">用户风险表示给定标识或帐户受到危害的可能性。</span><span class="sxs-lookup"><span data-stu-id="99a89-110">User risk represents the probability that a given identity or account is compromised.</span></span> <span data-ttu-id="99a89-111">这些风险是使用 Microsoft 的内部和外部威胁智能源（包括安全研究人员、执法人员、Microsoft 安全团队以及其他受信任的来源）进行脱机计算的。</span><span class="sxs-lookup"><span data-stu-id="99a89-111">These risks are calculated offline using Microsoft’s internal and external threat intelligence sources, including security researchers, law enforcement professionals, security teams at Microsoft, and other trusted sources.</span></span>

* <span data-ttu-id="99a89-112">[登录](signin.md)查询 Microsoft Graph，以获取有关具有与风险状态、详细信息和级别相关的特定属性的 Azure AD 登录信息。</span><span class="sxs-lookup"><span data-stu-id="99a89-112">[signIn](signin.md) - Query Microsoft Graph for information about Azure AD sign-ins with specific properties related to risk state, detail, and level.</span></span> <span data-ttu-id="99a89-113">登录风险表示标识所有者未授权给定的身份验证请求的可能性。</span><span class="sxs-lookup"><span data-stu-id="99a89-113">A sign-in risk represents the probability that a given authentication request isn’t authorized by the identity owner.</span></span> <span data-ttu-id="99a89-114">可以使用 Microsoft 的内部和外部威胁智能来源实时计算或计算这些风险，包括安全研究人员、执法人员、Microsoft 安全团队以及其他受信任的来源。</span><span class="sxs-lookup"><span data-stu-id="99a89-114">These risks can be calculated in real-time or calculated offline using Microsoft’s internal and external threat intelligence sources, including security researchers, law enforcement professionals, security teams at Microsoft, and other trusted sources.</span></span>

* <span data-ttu-id="99a89-115">[identityRiskEvents](identityriskevent.md) -查询 Microsoft Graph 以获取风险检测和相关信息的列表。</span><span class="sxs-lookup"><span data-stu-id="99a89-115">[identityRiskEvents](identityriskevent.md) - Query Microsoft Graph for a list of risk detections and associated information.</span></span> <span data-ttu-id="99a89-116">此 API 已弃用;我们建议您改为使用**riskDetections** 。</span><span class="sxs-lookup"><span data-stu-id="99a89-116">This API is deprecated; we recommend that you use **riskDetections** instead.</span></span>

>[!NOTE]
><span data-ttu-id="99a89-117">**IdentityRiskEvents** API 已弃用，并将停止返回2020年1月10日的数据。</span><span class="sxs-lookup"><span data-stu-id="99a89-117">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="99a89-118">有关详细信息，请参阅[弃用的 IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/)。</span><span class="sxs-lookup"><span data-stu-id="99a89-118">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

## <a name="see-also"></a><span data-ttu-id="99a89-119">另请参阅</span><span class="sxs-lookup"><span data-stu-id="99a89-119">See also</span></span>

* [<span data-ttu-id="99a89-120">关于 Azure Active Directory 标识保护</span><span class="sxs-lookup"><span data-stu-id="99a89-120">About Azure Active Directory Identity Protection</span></span>](https://docs.microsoft.com/azure/active-directory/identity-protection/overview-identity-protection)
* [<span data-ttu-id="99a89-121">Azure Active Directory 标识保护和 Microsoft Graph 入门</span><span class="sxs-lookup"><span data-stu-id="99a89-121">Get started with Azure Active Directory identity protection and Microsoft Graph</span></span>](https://docs.microsoft.com/azure/active-directory/identity-protection/howto-identity-protection-graph-api)
