---
title: 使用 Microsoft Graph 安全性 API
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Priority
author: preetikr
ms.prod: security
ms.openlocfilehash: 042c63cfee833a1f9c7493a9e35a6bbb8eb2fbaa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511826"
---
# <a name="use-the-microsoft-graph-security-api"></a><span data-ttu-id="6d464-104">使用 Microsoft Graph 安全性 API</span><span class="sxs-lookup"><span data-stu-id="6d464-104">Use the Microsoft Graph Security API</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d464-105">Microsoft Graph 安全性 API 提供了统一的界面的架构，用于与 Microsoft 和生态系统合作伙伴的安全性解决方案集成。</span><span class="sxs-lookup"><span data-stu-id="6d464-105">The Microsoft Graph Security API provides a unified interface and schema to integrate with security solutions from Microsoft and ecosystem partners.</span></span> <span data-ttu-id="6d464-106">这使客户能够简化安全性操作和更好地抵御日益增多的网络威胁。</span><span class="sxs-lookup"><span data-stu-id="6d464-106">This empowers customers to streamline security operations and better defend against increasing cyber threats.</span></span> <span data-ttu-id="6d464-107">Microsoft Graph 安全性 API 可用作联合安全聚合服务，向所有已启用的安全提供程序提交查询，以获得聚合响应。</span><span class="sxs-lookup"><span data-stu-id="6d464-107">The Microsoft Graph Security API can be used as a federated security aggregation service to submit queries to all onboarded security providers to get aggregated responses.</span></span> <span data-ttu-id="6d464-108">使用 Microsoft Graph 安全性 API 构建应用程序，以：</span><span class="sxs-lookup"><span data-stu-id="6d464-108">Use Microsoft Graph Security API to build applications that:</span></span>

- <span data-ttu-id="6d464-109">合并和关联多个来源的安全警报</span><span class="sxs-lookup"><span data-stu-id="6d464-109">Consolidate and correlate security alerts from multiple sources</span></span>
- <span data-ttu-id="6d464-110">解锁上下文数据，以提供调查信息</span><span class="sxs-lookup"><span data-stu-id="6d464-110">Unlock contextual data to inform investigations</span></span>
- <span data-ttu-id="6d464-111">自动执行安全性操作，以提高效率</span><span class="sxs-lookup"><span data-stu-id="6d464-111">Automate security operations for greater efficiency</span></span>
- <span data-ttu-id="6d464-112">提供安全性数据可见性，实现主动风险管理</span><span class="sxs-lookup"><span data-stu-id="6d464-112">Provide visibility into security data to enable proactive risk management</span></span>

<span data-ttu-id="6d464-113">Microsoft Graph 安全性 API 包括以下关键实体。</span><span class="sxs-lookup"><span data-stu-id="6d464-113">The Microsoft Graph Security API includes the following key entities.</span></span>

## <a name="alerts"></a><span data-ttu-id="6d464-114">警报</span><span class="sxs-lookup"><span data-stu-id="6d464-114">Alerts</span></span>

<span data-ttu-id="6d464-115">警报表示 Microsoft 或合作伙伴安全解决方已标识客户组合内存在潜在的安全问题，用于提醒用户采取操作或通知用户。</span><span class="sxs-lookup"><span data-stu-id="6d464-115">Alerts are potential security issues within a customer's tenant that Microsoft or partner security solutions have identified and are flagged for action or notification.</span></span> <span data-ttu-id="6d464-116">利用 Microsoft Graph 安全性[警报](alert.md)实体，可以统一和简化所有集成解决方案中的安全问题。</span><span class="sxs-lookup"><span data-stu-id="6d464-116">With the Microsoft Graph Security [alerts](alert.md) entity, you can unify and streamline security  issues across all integrated solutions.</span></span> <span data-ttu-id="6d464-117">此外，这还可以使应用程序关联警报和上下文，以提升威胁防护和响应。</span><span class="sxs-lookup"><span data-stu-id="6d464-117">This also enables applications to correlate alerts and context to improve threat protection and response.</span></span> <span data-ttu-id="6d464-118">这些警报可以缩短调查时间和解决事故的时间。</span><span class="sxs-lookup"><span data-stu-id="6d464-118">These unlock security operational efficiencies by reducing investigation time and time to resolution for incidents.</span></span> <span data-ttu-id="6d464-119">利用警报更新功能，你可以更新[警报](alert.md)实体，从而同步与 Microsoft Graph 安全性 API 集成的不同安全产品和服务中的特定警报状态。</span><span class="sxs-lookup"><span data-stu-id="6d464-119">With the alert update capability, you can sync the status of specific alerts across different security products and services that are integrated with the Microsoft Graph Security API by updating your [alerts](alert.md) entity.</span></span>

<span data-ttu-id="6d464-120">Microsoft Graph 安全集成解决方案将收到来自以下安全提供程序的警报：</span><span class="sxs-lookup"><span data-stu-id="6d464-120">Microsoft Graph Security-integrated solutions will receive alerts from the following security providers:</span></span>

- [<span data-ttu-id="6d464-121">Azure 安全中心</span><span class="sxs-lookup"><span data-stu-id="6d464-121">Azure Security Center</span></span>](https://docs.microsoft.com/azure/security-center/security-center-alerts-type)
- [<span data-ttu-id="6d464-122">Azure Active Directory Identity Protection</span><span class="sxs-lookup"><span data-stu-id="6d464-122">Azure Active Directory Identity Protection</span></span>](https://docs.microsoft.com/azure/active-directory/identity-protection/playbook)
- [<span data-ttu-id="6d464-123">Microsoft Cloud App Security</span><span class="sxs-lookup"><span data-stu-id="6d464-123">Microsoft Cloud Application Security</span></span>](https://docs.microsoft.com/cloud-app-security/monitor-alerts )
- [<span data-ttu-id="6d464-124">Windows Defender 高级威胁防护</span><span class="sxs-lookup"><span data-stu-id="6d464-124">Windows Defender Advanced Threat Protection</span></span>](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/attack-simulations-windows-defender-advanced-threat-protection)
- <span data-ttu-id="6d464-125">[Azure 信息保护](https://docs.microsoft.com/azure/information-protection/faqs#i-see-azure-information-protection-is-listed-as-a-security-provider-for-microsoft-graph-securityhow-does-this-work-and-what-alerts-will-i-receive)**（预览版）**</span><span class="sxs-lookup"><span data-stu-id="6d464-125">[Azure Information Protection](https://docs.microsoft.com/azure/information-protection/faqs#i-see-azure-information-protection-is-listed-as-a-security-provider-for-microsoft-graph-securityhow-does-this-work-and-what-alerts-will-i-receive) **(preview)**</span></span>
- <span data-ttu-id="6d464-126">Microsoft Intune **（个人预览版）**</span><span class="sxs-lookup"><span data-stu-id="6d464-126">Microsoft Intune **(private preview)**</span></span>
- <span data-ttu-id="6d464-127">Office 365 **（即将推出）**</span><span class="sxs-lookup"><span data-stu-id="6d464-127">Office 365 **(coming soon)**</span></span>
- <span data-ttu-id="6d464-128">Azure 高级威胁防护 **（即将推出）**</span><span class="sxs-lookup"><span data-stu-id="6d464-128">Azure Advanced Threat Protection **(coming soon)**</span></span>
- <span data-ttu-id="6d464-129">合作伙伴解决方案，例如 Palo Alto 网络应用程序框架</span><span class="sxs-lookup"><span data-stu-id="6d464-129">Partner solutions, such as Palo Alto Networks App Framework</span></span>

> <span data-ttu-id="6d464-130">**注释：** 新提供程序将会不断加入 Microsoft Graph 安全生态系统。</span><span class="sxs-lookup"><span data-stu-id="6d464-130">**Note:** New providers are continuously onboarding to the Microsoft Graph Security ecosystem.</span></span>

## <a name="secure-score-preview"></a><span data-ttu-id="6d464-131">安全功能分数（预览版）</span><span class="sxs-lookup"><span data-stu-id="6d464-131">Secure Score (preview)</span></span>

<span data-ttu-id="6d464-132">[Microsoft 安全功能分数](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Office-365-Secure-Score-is-now-Microsoft-Secure-Score/ba-p/182358)是一款安全分析解决方案，可让你了解安全项目组合以及如何改进这些组合。</span><span class="sxs-lookup"><span data-stu-id="6d464-132">[Microsoft Secure Score](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Office-365-Secure-Score-is-now-Microsoft-Secure-Score/ba-p/182358) is a security analytics solution that gives you visibility into your security portfolio and how to improve it.</span></span> <span data-ttu-id="6d464-133">只需一个分数，你就可以更好地了解已采取了哪些措施来降低 Microsoft 解决方案中的风险。</span><span class="sxs-lookup"><span data-stu-id="6d464-133">With a single score, you can better understand what you have done to reduce your risk in Microsoft solutions.</span></span> <span data-ttu-id="6d464-134">此外，你还可以将你的分数与其他组织比较，以了解你的分数趋势。</span><span class="sxs-lookup"><span data-stu-id="6d464-134">You can also compare your score with other organizations and see how your score has been trending over time.</span></span> <span data-ttu-id="6d464-135">Microsoft Graph 安全性 [secureScore](securescores.md) 和 [secureScoreControlProfiles](securescorecontrolprofiles.md) 实体可以帮助你实现组织的安全性与生产力需求之间的平衡，同时支持相应的安全功能混合。</span><span class="sxs-lookup"><span data-stu-id="6d464-135">The Microsoft Graph Security [secureScore](securescores.md) and [secureScoreControlProfiles](securescorecontrolprofiles.md) entities help you balance your organization's security and productivity needs while enabling the appropriate mix of security features.</span></span> <span data-ttu-id="6d464-136">你也可以计划采取安全功能之后的分数。</span><span class="sxs-lookup"><span data-stu-id="6d464-136">You can also project what your score would be after you adopt security features.</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="6d464-137">常见用例</span><span class="sxs-lookup"><span data-stu-id="6d464-137">Common use cases</span></span>

<span data-ttu-id="6d464-138">以下是使用 Microsoft Graph 安全性 API 的一些热门的请求。</span><span class="sxs-lookup"><span data-stu-id="6d464-138">The following are some of the most popular requests for working with the Microsoft Graph Security API.</span></span>

| <span data-ttu-id="6d464-139">**用例**</span><span class="sxs-lookup"><span data-stu-id="6d464-139">**Use cases**</span></span>   | <span data-ttu-id="6d464-140">**REST 资源**</span><span class="sxs-lookup"><span data-stu-id="6d464-140">**REST resources**</span></span> | <span data-ttu-id="6d464-141">**在 Graph 浏览器中试调用**</span><span class="sxs-lookup"><span data-stu-id="6d464-141">**Try it in Graph Explorer**</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="6d464-142">列出警报</span><span class="sxs-lookup"><span data-stu-id="6d464-142">List alerts</span></span> | [<span data-ttu-id="6d464-143">List alerts</span><span class="sxs-lookup"><span data-stu-id="6d464-143">List alerts</span></span>](../api/alert-list.md) | [https://graph.microsoft.com/beta/security/alerts](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts&method=GET&version=beta&GraphUrl=https://graph.microsoft.com) |
| <span data-ttu-id="6d464-144">更新警报</span><span class="sxs-lookup"><span data-stu-id="6d464-144">Update alerts</span></span> | [<span data-ttu-id="6d464-145">Update alert</span><span class="sxs-lookup"><span data-stu-id="6d464-145">Update alert</span></span>](../api/alert-update.md) | [https://graph.microsoft.com/beta/security/alerts/{alert-id}](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts/{alert-id}&method=PATCH&version=beta&GraphUrl=https://graph.microsoft.com) |
|<span data-ttu-id="6d464-146">列出安全功能分数</span><span class="sxs-lookup"><span data-stu-id="6d464-146">List secure scores</span></span>|<span data-ttu-id="6d464-147">[List secureScores](../api/securescores-list.md)（预览版）</span><span class="sxs-lookup"><span data-stu-id="6d464-147">[List secureScores](../api/securescores-list.md) (preview)</span></span>|[https://graph.microsoft.com/beta/security/secureScores](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScores&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|<span data-ttu-id="6d464-148">列出安全功能控制配置文件</span><span class="sxs-lookup"><span data-stu-id="6d464-148">List secure score control profiles</span></span>|<span data-ttu-id="6d464-149">[List secureScoreControlProfiles](../api/securescorecontrolprofiles-list.md)（预览版）</span><span class="sxs-lookup"><span data-stu-id="6d464-149">[List secureScoreControlProfiles](../api/securescorecontrolprofiles-list.md) (preview)</span></span>|[https://graph.microsoft.com/beta/security/secureScoreControlProfiles](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|<span data-ttu-id="6d464-150">更新安全功能控制配置文件</span><span class="sxs-lookup"><span data-stu-id="6d464-150">Update secure score control profiles</span></span>|<span data-ttu-id="6d464-151">[Update secureScoreControlProfiles](../api/securescorecontrolprofiles-update.md)（预览）</span><span class="sxs-lookup"><span data-stu-id="6d464-151">[Update secureScoreControlProfiles](../api/securescorecontrolprofiles-update.md) (preview)</span></span>|[https://graph.microsoft.com/beta/security/secureScoreControlProfiles/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles/{id}&method=PATCH&version=beta&GraphUrl=https://graph.microsoft.com)|

<span data-ttu-id="6d464-152">可以使用 Microsoft Graph [webhooks](/graph/webhooks) 订阅和接收与 Microsoft Graph 安全性实体相关的通知。</span><span class="sxs-lookup"><span data-stu-id="6d464-152">You can use Microsoft Graph [webhooks](/graph/webhooks) to subscribe to and receive notifications about updates to Microsoft Graph Security entities.</span></span>

## <a name="next-steps"></a><span data-ttu-id="6d464-153">后续步骤</span><span class="sxs-lookup"><span data-stu-id="6d464-153">Next steps</span></span>

<span data-ttu-id="6d464-154">Microsoft Graph 安全性 API 可以为你提供使用 Microsoft 和合作伙伴的不同安全解决方案的新方式。</span><span class="sxs-lookup"><span data-stu-id="6d464-154">The Microsoft Graph Security API can open up new ways for you to engage with different security solutions from Microsoft and partners.</span></span> <span data-ttu-id="6d464-155">请按照以下步骤开始操作：</span><span class="sxs-lookup"><span data-stu-id="6d464-155">Follow these steps to get started:</span></span>

- <span data-ttu-id="6d464-156">向下钻取到 [alerts](alert.md)、[secureScore](securescores.md)（预览版）和 [secureScoreControlProfiles](securescorecontrolprofiles.md)（预览版）。</span><span class="sxs-lookup"><span data-stu-id="6d464-156">Drill down into [alerts](alert.md), [secureScore](securescores.md) (Preview), and [secureScoreControlProfiles](securescorecontrolprofiles.md) (Preview).</span></span>
- <span data-ttu-id="6d464-157">尝试在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中调用 API。</span><span class="sxs-lookup"><span data-stu-id="6d464-157">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span> <span data-ttu-id="6d464-158">在“**示例查询**”中，选择“**显示更多示例**”并将“安全类别”设为“**开启**”。</span><span class="sxs-lookup"><span data-stu-id="6d464-158">Under **Sample Queries**, choose **show more samples** and set the Security category to **on**.</span></span>
- <span data-ttu-id="6d464-159">请尝试[订阅和接收实体变更通知](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="6d464-159">Try [subscribing to and receiving notifications](/graph/webhooks) on entity changes.</span></span>

<span data-ttu-id="6d464-p107">需要更多灵感？请参阅[我们的一些合作伙伴如何使用 Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners)。</span><span class="sxs-lookup"><span data-stu-id="6d464-p107">Need more ideas? See [how some of our partners are using Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).</span></span>

## <a name="see-also"></a><span data-ttu-id="6d464-162">另请参阅</span><span class="sxs-lookup"><span data-stu-id="6d464-162">See also</span></span>

<span data-ttu-id="6d464-163">Microsoft Graph 安全性 API 示例代码及参与 API：</span><span class="sxs-lookup"><span data-stu-id="6d464-163">Code and contribute to these Microsoft Graph Security API samples:</span></span>

- [<span data-ttu-id="6d464-164">ASP.NET (C#) 示例</span><span class="sxs-lookup"><span data-stu-id="6d464-164">ASP.NET (C#) sample</span></span>](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [<span data-ttu-id="6d464-165">Python 示例</span><span class="sxs-lookup"><span data-stu-id="6d464-165">Python sample</span></span>](https://github.com/microsoftgraph/python-security-rest-sample)
- [<span data-ttu-id="6d464-166">Node.js (JavaScript) 示例</span><span class="sxs-lookup"><span data-stu-id="6d464-166">Node.js (JavaScript) sample</span></span>](https://github.com/microsoftgraph/nodejs-security-sample)

<span data-ttu-id="6d464-167">与社区互动：</span><span class="sxs-lookup"><span data-stu-id="6d464-167">Engage with the community:</span></span>

- [<span data-ttu-id="6d464-168">加入技术社区</span><span class="sxs-lookup"><span data-stu-id="6d464-168">Join the tech community</span></span>](https://aka.ms/graphsecuritycommunity)
- [<span data-ttu-id="6d464-169">在 StackOverflow 上讨论</span><span class="sxs-lookup"><span data-stu-id="6d464-169">Discuss on StackOverflow</span></span>](https://stackoverflow.com/questions/tagged/microsoft-graph-security)
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/security-api-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
