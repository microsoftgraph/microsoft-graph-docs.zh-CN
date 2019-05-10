---
title: Azure AD 审核日志 API 概述
description: Azure Active Directory (Azure AD) 可跟踪用户活动和登录指标并创建审核日志报告，以帮助你了解用户如何访问和使用 Azure AD 服务。
localization_priority: Priority
author: dhanyahk
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4df05291b4ce06312f4797b5f89ae49d74246ed5
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629318"
---
# <a name="azure-ad-audit-log-api-overview"></a><span data-ttu-id="f0acc-103">Azure AD 审核日志 API 概述</span><span class="sxs-lookup"><span data-stu-id="f0acc-103">Azure AD audit log API overview</span></span>

<span data-ttu-id="f0acc-104">Azure Active Directory (Azure AD) 可跟踪用户活动和登录指标并创建审核日志报告，以帮助你了解用户如何访问和使用 Azure AD 服务。</span><span class="sxs-lookup"><span data-stu-id="f0acc-104">Azure Active Directory (Azure AD) tracks user activity and sign-in metrics and creates audit log reports that help you understand how your users access and leverage Azure AD services.</span></span> <span data-ttu-id="f0acc-105">使用 Microsoft Graph API for Azure AD 分析这些报告的基础数据，并根据组织的特定需求创建自定义解决方案。</span><span class="sxs-lookup"><span data-stu-id="f0acc-105">Use the Microsoft Graph API for Azure AD to analyze the data underlying these reports and to create custom solutions tailored to your organization's specific needs.</span></span>

## <a name="what-are-azure-ad-activity-logs"></a><span data-ttu-id="f0acc-106">什么是 Azure AD 活动日志？</span><span class="sxs-lookup"><span data-stu-id="f0acc-106">What are Azure AD activity logs?</span></span>

<span data-ttu-id="f0acc-107">Azure AD 提供了两种类型的活动日志：</span><span class="sxs-lookup"><span data-stu-id="f0acc-107">Azure AD provides two types of activity logs:</span></span>

- <span data-ttu-id="f0acc-108">审核日志</span><span class="sxs-lookup"><span data-stu-id="f0acc-108">audit logs</span></span>
- <span data-ttu-id="f0acc-109">登录日志</span><span class="sxs-lookup"><span data-stu-id="f0acc-109">sign-in logs</span></span>

### <a name="audit-logs"></a><span data-ttu-id="f0acc-110">审核日志</span><span class="sxs-lookup"><span data-stu-id="f0acc-110">Audit logs</span></span>

<span data-ttu-id="f0acc-111">通过审核日志活动报告，你可以访问在租户中执行的每项任务的历史记录。</span><span class="sxs-lookup"><span data-stu-id="f0acc-111">The audit logs activity report provides you with access to the history of every task performed in your tenant.</span></span> <span data-ttu-id="f0acc-112">审核日志报告为你提供了系统合规活动的记录。</span><span class="sxs-lookup"><span data-stu-id="f0acc-112">The audit logs report provides you with records of system activities for compliance.</span></span> <span data-ttu-id="f0acc-113">除此之外，提供的数据还可让你了解常见情景，例如：</span><span class="sxs-lookup"><span data-stu-id="f0acc-113">Amongst others, the provided data enables you to address common scenarios such as:</span></span>

- <span data-ttu-id="f0acc-114">谁向管理员组授予了访问目录用户的权限？</span><span class="sxs-lookup"><span data-stu-id="f0acc-114">Who granted admin group access to a directory user?</span></span>
- <span data-ttu-id="f0acc-115">哪些用户正在登录最近购买的应用程序？</span><span class="sxs-lookup"><span data-stu-id="f0acc-115">Which users are signing in to a recently acquired app?</span></span>
- <span data-ttu-id="f0acc-116">在目录中进行了多少次密码重置？</span><span class="sxs-lookup"><span data-stu-id="f0acc-116">How many passwords resets were made within the directory?</span></span>

### <a name="sign-in-logs"></a><span data-ttu-id="f0acc-117">登录日志</span><span class="sxs-lookup"><span data-stu-id="f0acc-117">sign-in logs</span></span>

<span data-ttu-id="f0acc-118">登录活动报告可帮助你确定负责执行审核日志报告所报告的任务的人员。</span><span class="sxs-lookup"><span data-stu-id="f0acc-118">The sign-ins activity report helps you determine who performed the tasks reported by audit log reports.</span></span> <span data-ttu-id="f0acc-119">登录活动报告可帮助你回答如下问题：</span><span class="sxs-lookup"><span data-stu-id="f0acc-119">The sign-ins activity report helps you answer questions like:</span></span>

- <span data-ttu-id="f0acc-120">用户的登录模式是什么？</span><span class="sxs-lookup"><span data-stu-id="f0acc-120">What is the sign in pattern of a user?</span></span>
- <span data-ttu-id="f0acc-121">上周有多少用户进行了登录？</span><span class="sxs-lookup"><span data-stu-id="f0acc-121">How many users have signed in during the last week?</span></span>
- <span data-ttu-id="f0acc-122">这些登录的状态如何？</span><span class="sxs-lookup"><span data-stu-id="f0acc-122">What's the status of these sign-ins?</span></span>

## <a name="what-can-i-do-with-audit-log-apis-in-microsoft-graph"></a><span data-ttu-id="f0acc-123">可以使用 Microsoft Graph 中的审核日志 API 做什么？</span><span class="sxs-lookup"><span data-stu-id="f0acc-123">What can I do with audit log APIs in Microsoft Graph?</span></span>

<span data-ttu-id="f0acc-124">以下是处理审核日志数据的常见请求：</span><span class="sxs-lookup"><span data-stu-id="f0acc-124">Here are popular requests for working with audit log data:</span></span>

<span data-ttu-id="f0acc-125">Operation</span><span class="sxs-lookup"><span data-stu-id="f0acc-125">Operation</span></span> | <span data-ttu-id="f0acc-126">URL</span><span class="sxs-lookup"><span data-stu-id="f0acc-126">URL</span></span>
:----------|:----
<span data-ttu-id="f0acc-127">获取租户用户活动</span><span class="sxs-lookup"><span data-stu-id="f0acc-127">GET tenant user activities</span></span> | [<span data-ttu-id="f0acc-128">GET https://graph.microsoft.com/v1.0/auditLogs/directoryAudits</span><span class="sxs-lookup"><span data-stu-id="f0acc-128">Gethttps://graph.microsoft.com/v1.0/auditLogs/directoryAudits</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=v1.0)
<span data-ttu-id="f0acc-129">获取租户用户登录信息</span><span class="sxs-lookup"><span data-stu-id="f0acc-129">GET tenant user sign-ins</span></span> | [<span data-ttu-id="f0acc-130">GET https://graph.microsoft.com/v1.0/auditLogs/signIns</span><span class="sxs-lookup"><span data-stu-id="f0acc-130">Gethttps://graph.microsoft.com/v1.0/auditLogs/signIns</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=v1.0)

## <a name="what-licenses-do-i-need"></a><span data-ttu-id="f0acc-131">需要哪些许可证？</span><span class="sxs-lookup"><span data-stu-id="f0acc-131">What licenses do I need?</span></span>

<span data-ttu-id="f0acc-132">审核日志报告适用于已获得许可的功能。</span><span class="sxs-lookup"><span data-stu-id="f0acc-132">Audit log reports are available for features that you've licensed.</span></span>  <span data-ttu-id="f0acc-133">如果你拥有特定功能的许可证，则还可以访问其审核日志。</span><span class="sxs-lookup"><span data-stu-id="f0acc-133">If you have a license for a specific feature, you also have access to its audit logs.</span></span>

<span data-ttu-id="f0acc-134">例如，你需要 Azure AD Premium P1 许可证才能访问自助密码审核报告。</span><span class="sxs-lookup"><span data-stu-id="f0acc-134">For example, you need an Azure AD Premium P1 license to access self-service password audit reports.</span></span>  <span data-ttu-id="f0acc-135">若要了解详细信息，请参阅 [Azure AD 许可](https://azure.microsoft.com/pricing/details/active-directory/)。</span><span class="sxs-lookup"><span data-stu-id="f0acc-135">To learn more, see [Azure AD licensing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

<span data-ttu-id="f0acc-136">登录报告需要 Azure AD Premium 许可证。</span><span class="sxs-lookup"><span data-stu-id="f0acc-136">Sign-in reports require an Azure AD Premium license.</span></span>

<span data-ttu-id="f0acc-137">若要了解详细信息，请参阅 [Azure AD 定价](https://azure.microsoft.com/pricing/details/active-directory/)。</span><span class="sxs-lookup"><span data-stu-id="f0acc-137">To learn more, see [Azure AD pricing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

## <a name="next-steps"></a><span data-ttu-id="f0acc-138">后续步骤</span><span class="sxs-lookup"><span data-stu-id="f0acc-138">Next Steps</span></span>

- <span data-ttu-id="f0acc-139">[注册你的应用程序](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)以满足审核日志先决条件。</span><span class="sxs-lookup"><span data-stu-id="f0acc-139">[Register your app](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to satisfy audit log prerequisites.</span></span> 
- <span data-ttu-id="f0acc-140">了解[审核日志](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples)和[登录示例](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples)。</span><span class="sxs-lookup"><span data-stu-id="f0acc-140">Learn from [audit log](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples) and [sign-in samples](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span></span>  
- <span data-ttu-id="f0acc-141">审查 [directoryAudit](directoryaudit.md) 资源和操作。</span><span class="sxs-lookup"><span data-stu-id="f0acc-141">Review [directoryAudit](directoryaudit.md) resource and actions.</span></span>
- <span data-ttu-id="f0acc-142">审查 [signIn](signin.md) 资源和操作。</span><span class="sxs-lookup"><span data-stu-id="f0acc-142">Review [signIn](signin.md) resource and actions.</span></span> 
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/azure-ad-auditlog-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
