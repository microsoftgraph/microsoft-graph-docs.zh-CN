---
title: 使用 Microsoft Graph 安全 API
description: Microsoft Graph 安全 API 提供统一的接口和集成使用经 Microsoft 和生态系统的合作伙伴的安全解决方案的架构。 这使客户能够简化安全性操作和更好地防御增加网络威胁。 Microsoft Graph 安全 API 可以作为联盟的安全聚合服务，用于向所有 onboarded 安全提供程序获取聚合的响应提交查询。 使用 Microsoft Graph 安全 API 来构建应用程序的：
ms.openlocfilehash: b675ecd66081aec29f2727a394a91d9e2ee5fd5b
ms.sourcegitcommit: 4aebfaefc23e02a98b2fec35958cd2110020f15f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/06/2018
ms.locfileid: "27184516"
---
# <a name="use-the-microsoft-graph-security-api"></a><span data-ttu-id="4988e-106">使用 Microsoft Graph 安全 API</span><span class="sxs-lookup"><span data-stu-id="4988e-106">Use the Microsoft Graph Security API</span></span>

<span data-ttu-id="4988e-107">Microsoft Graph 安全 API 提供统一的接口和集成使用经 Microsoft 和生态系统的合作伙伴的安全解决方案的架构。</span><span class="sxs-lookup"><span data-stu-id="4988e-107">The Microsoft Graph Security API provides a unified interface and schema to integrate with security solutions from Microsoft and ecosystem partners.</span></span> <span data-ttu-id="4988e-108">这使客户能够简化安全性操作和更好地防御增加网络威胁。</span><span class="sxs-lookup"><span data-stu-id="4988e-108">This empowers customers to streamline security operations and better defend against increasing cyber threats.</span></span> <span data-ttu-id="4988e-109">Microsoft Graph 安全 API 可以作为联盟的安全聚合服务，用于向所有 onboarded 安全提供程序获取聚合的响应提交查询。</span><span class="sxs-lookup"><span data-stu-id="4988e-109">The Microsoft Graph Security API can be used as a federated security aggregation service to submit queries to all onboarded security providers to get aggregated responses.</span></span> <span data-ttu-id="4988e-110">使用 Microsoft Graph 安全 API 来构建应用程序的：</span><span class="sxs-lookup"><span data-stu-id="4988e-110">Use Microsoft Graph Security API to build applications that:</span></span>

- <span data-ttu-id="4988e-111">合并和关联多个来源的安全警告</span><span class="sxs-lookup"><span data-stu-id="4988e-111">Consolidate and correlate security alerts from multiple sources</span></span>
- <span data-ttu-id="4988e-112">解除锁定上下文数据来告知调查</span><span class="sxs-lookup"><span data-stu-id="4988e-112">Unlock contextual data to inform investigations</span></span>
- <span data-ttu-id="4988e-113">自动化安全操作以提高效率</span><span class="sxs-lookup"><span data-stu-id="4988e-113">Automate security operations for greater efficiency</span></span>
- <span data-ttu-id="4988e-114">提供的可见性安全数据，以启用主动风险管理</span><span class="sxs-lookup"><span data-stu-id="4988e-114">Provide visibility into security data to enable proactive risk management</span></span>

<span data-ttu-id="4988e-115">Microsoft Graph 安全 API 包括以下主要实体。</span><span class="sxs-lookup"><span data-stu-id="4988e-115">The Microsoft Graph Security API includes the following key entities.</span></span>

## <a name="alerts"></a><span data-ttu-id="4988e-116">警报</span><span class="sxs-lookup"><span data-stu-id="4988e-116">Alerts</span></span>

<span data-ttu-id="4988e-117">通知是潜在客户的租户的 Microsoft 或合作伙伴的安全解决方案已经确定并标记的操作或通知中的安全问题。</span><span class="sxs-lookup"><span data-stu-id="4988e-117">Alerts are potential security issues within a customer's tenant that Microsoft or partner security solutions have identified and are flagged for action or notification.</span></span> <span data-ttu-id="4988e-118">与 Microsoft Graph 安全[警报](alert.md)实体，您可以统一并简化跨所有集成的解决方案的安全问题。</span><span class="sxs-lookup"><span data-stu-id="4988e-118">With the Microsoft Graph Security [alerts](alert.md) entity, you can unify and streamline security  issues across all integrated solutions.</span></span> <span data-ttu-id="4988e-119">这还允许应用程序关联的通知和上下文改进威胁保护和响应。</span><span class="sxs-lookup"><span data-stu-id="4988e-119">This also enables applications to correlate alerts and context to improve threat protection and response.</span></span> <span data-ttu-id="4988e-120">通过减少调查时间和时间的事件的分辨率，这些解锁安全运营效率。</span><span class="sxs-lookup"><span data-stu-id="4988e-120">These unlock security operational efficiencies by reducing investigation time and time to resolution for incidents.</span></span> <span data-ttu-id="4988e-121">使用通知更新功能中，可以跨不同安全产品和服务与 Microsoft Graph 安全 API 通过更新[通知](alert.md)实体集成同步特定警报的状态。</span><span class="sxs-lookup"><span data-stu-id="4988e-121">With the alert update capability, you can sync the status of specific alerts across different security products and services that are integrated with the Microsoft Graph Security API by updating your [alerts](alert.md) entity.</span></span>

<span data-ttu-id="4988e-122">Microsoft Graph 安全集成解决方案将收到来自下列安全提供程序的通知：</span><span class="sxs-lookup"><span data-stu-id="4988e-122">Microsoft Graph Security-integrated solutions will receive alerts from the following security providers:</span></span>

- [<span data-ttu-id="4988e-123">Azure 安全中心</span><span class="sxs-lookup"><span data-stu-id="4988e-123">Azure Security Center</span></span>](https://docs.microsoft.com/azure/security-center/security-center-alerts-type)
- [<span data-ttu-id="4988e-124">Azure Active Directory 标识保护</span><span class="sxs-lookup"><span data-stu-id="4988e-124">Azure Active Directory Identity Protection</span></span>](https://docs.microsoft.com/azure/active-directory/identity-protection/playbook)
- [<span data-ttu-id="4988e-125">Microsoft 云应用程序安全性</span><span class="sxs-lookup"><span data-stu-id="4988e-125">Microsoft Cloud Application Security</span></span>](https://docs.microsoft.com/cloud-app-security/monitor-alerts )
- [<span data-ttu-id="4988e-126">Windows Defender 高级威胁保护</span><span class="sxs-lookup"><span data-stu-id="4988e-126">Windows Defender Advanced Threat Protection</span></span>](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/attack-simulations-windows-defender-advanced-threat-protection)
- <span data-ttu-id="4988e-127">[Azure 信息保护](https://docs.microsoft.com/azure/information-protection/faqs#i-see-azure-information-protection-is-listed-as-a-security-provider-for-microsoft-graph-securityhow-does-this-work-and-what-alerts-will-i-receive)**（预览）**</span><span class="sxs-lookup"><span data-stu-id="4988e-127">[Azure Information Protection](https://docs.microsoft.com/azure/information-protection/faqs#i-see-azure-information-protection-is-listed-as-a-security-provider-for-microsoft-graph-securityhow-does-this-work-and-what-alerts-will-i-receive) **(preview)**</span></span>
- <span data-ttu-id="4988e-128">Microsoft Intune **（专用预览）**</span><span class="sxs-lookup"><span data-stu-id="4988e-128">Microsoft Intune **(private preview)**</span></span>
- <span data-ttu-id="4988e-129">Office 365 **（即将推出）**</span><span class="sxs-lookup"><span data-stu-id="4988e-129">Office 365 **(coming soon)**</span></span>
- <span data-ttu-id="4988e-130">Azure 高级威胁保护 **（即将推出）**</span><span class="sxs-lookup"><span data-stu-id="4988e-130">Azure Advanced Threat Protection **(coming soon)**</span></span>
- <span data-ttu-id="4988e-131">合作伙伴解决方案，如帕洛阿尔托市网络应用程序框架</span><span class="sxs-lookup"><span data-stu-id="4988e-131">Partner solutions, such as Palo Alto Networks App Framework</span></span>

> <span data-ttu-id="4988e-132">**注意：** 新的提供程序持续是加入到 Microsoft Graph Security 生态系统。</span><span class="sxs-lookup"><span data-stu-id="4988e-132">**Note:** New providers are continuously onboarding to the Microsoft Graph Security ecosystem.</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="4988e-133">常见用例</span><span class="sxs-lookup"><span data-stu-id="4988e-133">Common use cases</span></span>

<span data-ttu-id="4988e-134">下面是一些有关使用 Microsoft Graph 安全 API 的最常用请求：</span><span class="sxs-lookup"><span data-stu-id="4988e-134">The following are some of the most popular requests for working with the Microsoft Graph Security API:</span></span>

| <span data-ttu-id="4988e-135">**用例**</span><span class="sxs-lookup"><span data-stu-id="4988e-135">**Use cases**</span></span>   | <span data-ttu-id="4988e-136">**REST 资源**</span><span class="sxs-lookup"><span data-stu-id="4988e-136">**REST resources**</span></span> | <span data-ttu-id="4988e-137">**尝试在图资源管理器**</span><span class="sxs-lookup"><span data-stu-id="4988e-137">**Try it in Graph Explorer**</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="4988e-138">列出警报</span><span class="sxs-lookup"><span data-stu-id="4988e-138">List alerts</span></span> | [<span data-ttu-id="4988e-139">列出警报</span><span class="sxs-lookup"><span data-stu-id="4988e-139">List alerts</span></span>](../api/alert-list.md) | [https://graph.microsoft.com/v1.0/security/alerts](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com) |
| <span data-ttu-id="4988e-140">更新通知</span><span class="sxs-lookup"><span data-stu-id="4988e-140">Update alerts</span></span> | [<span data-ttu-id="4988e-141">更新警报</span><span class="sxs-lookup"><span data-stu-id="4988e-141">Update alert</span></span>](../api/alert-update.md) | [https://graph.microsoft.com/v1.0/security/alerts/{alert-id}](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts/{alert-id}&method=PATCH&version=v1.0&GraphUrl=https://graph.microsoft.com) |

<span data-ttu-id="4988e-142">您可以使用 Microsoft Graph [webhooks](/graph/webhooks)订阅和接收有关 Microsoft Graph Security 实体更新通知。</span><span class="sxs-lookup"><span data-stu-id="4988e-142">You can use Microsoft Graph [webhooks](/graph/webhooks) to subscribe to and receive notifications about updates to Microsoft Graph Security entities.</span></span>

## <a name="resources"></a><span data-ttu-id="4988e-143">资源</span><span class="sxs-lookup"><span data-stu-id="4988e-143">Resources</span></span>

<span data-ttu-id="4988e-144">代码并参与到这些 Microsoft Graph 安全 API 示例：</span><span class="sxs-lookup"><span data-stu-id="4988e-144">Code and contribute to these Microsoft Graph Security API samples:</span></span>

- [<span data-ttu-id="4988e-145">ASP.NET (C#) 示例</span><span class="sxs-lookup"><span data-stu-id="4988e-145">ASP.NET (C#) sample</span></span>](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [<span data-ttu-id="4988e-146">Python 示例</span><span class="sxs-lookup"><span data-stu-id="4988e-146">Python sample</span></span>](https://github.com/microsoftgraph/python-security-rest-sample)
- [<span data-ttu-id="4988e-147">Node.js (JavaScript) 示例</span><span class="sxs-lookup"><span data-stu-id="4988e-147">Node.js (JavaScript) sample</span></span>](https://github.com/microsoftgraph/nodejs-security-sample)

<span data-ttu-id="4988e-148">社区的使用：</span><span class="sxs-lookup"><span data-stu-id="4988e-148">Engage with the community:</span></span>

- [<span data-ttu-id="4988e-149">加入技术社区</span><span class="sxs-lookup"><span data-stu-id="4988e-149">Join the tech community</span></span>](https://aka.ms/graphsecuritycommunity)
- [<span data-ttu-id="4988e-150">讨论在 StackOverflow 上</span><span class="sxs-lookup"><span data-stu-id="4988e-150">Discuss on StackOverflow</span></span>](https://stackoverflow.com/questions/tagged/microsoft-graph-security)

## <a name="next-steps"></a><span data-ttu-id="4988e-151">后续步骤</span><span class="sxs-lookup"><span data-stu-id="4988e-151">Next steps</span></span>

<span data-ttu-id="4988e-152">您可以使用不同的安全解决方案来自 Microsoft 和合作伙伴进行新的方法可以打开 Microsoft Graph 安全 API。</span><span class="sxs-lookup"><span data-stu-id="4988e-152">The Microsoft Graph Security API can open up new ways for you to engage with different security solutions from Microsoft and partners.</span></span> <span data-ttu-id="4988e-153">按照以下步骤开始：</span><span class="sxs-lookup"><span data-stu-id="4988e-153">Follow these steps to get started:</span></span>

- <span data-ttu-id="4988e-154">向下钻取到[通知](alert.md)。</span><span class="sxs-lookup"><span data-stu-id="4988e-154">Drill down into [alerts](alert.md).</span></span>
- <span data-ttu-id="4988e-155">尝试 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中的 API。</span><span class="sxs-lookup"><span data-stu-id="4988e-155">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span> <span data-ttu-id="4988e-156">下**的示例查询**，选择**显示更多示例**，并设置为**上**的安全类别。</span><span class="sxs-lookup"><span data-stu-id="4988e-156">Under **Sample Queries**, choose **show more samples** and set the Security category to **on**.</span></span>
- <span data-ttu-id="4988e-157">尝试在实体更改[订阅和接收通知](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="4988e-157">Try [subscribing to and receiving notifications](/graph/webhooks) on entity changes.</span></span>

<span data-ttu-id="4988e-p106">需要更多灵感？请参阅[我们的一些合作伙伴如何使用 Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners)。</span><span class="sxs-lookup"><span data-stu-id="4988e-p106">Need more ideas? See [how some of our partners are using Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).</span></span>
