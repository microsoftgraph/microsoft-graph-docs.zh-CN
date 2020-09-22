---
title: 活动报告 API 概述
description: 使用 Microsoft Graph 中的活动报告 API 访问 Azure Active Directory 创建的报告，跟踪租户中的用户活动。
localization_priority: Priority
author: khotz
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: cfb622200b5437390c6617c8bd599409fa90925f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091871"
---
# <a name="activity-reports-api-overview"></a><span data-ttu-id="81f1d-103">活动报告 API 概述</span><span class="sxs-lookup"><span data-stu-id="81f1d-103">Activity reports API overview</span></span>

<span data-ttu-id="81f1d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81f1d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="81f1d-105">Azure Active Directory (Azure AD) 可跟踪用户活动和创建报告，以帮助你了解用户如何访问和使用 Azure AD 服务。</span><span class="sxs-lookup"><span data-stu-id="81f1d-105">Azure Active Directory (Azure AD) tracks user activity and creates reports that help you understand how your users access and use Azure AD services.</span></span> <span data-ttu-id="81f1d-106">使用 Microsoft Graph API for Azure AD 分析这些报告中的数据，并根据组织的特定需求创建自定义解决方案。</span><span class="sxs-lookup"><span data-stu-id="81f1d-106">Use the Microsoft Graph API for Azure AD to analyze the data in these reports and to create custom solutions tailored to your organization's specific needs.</span></span>

## <a name="what-are-azure-ad-activity-logs"></a><span data-ttu-id="81f1d-107">什么是 Azure AD 活动日志？</span><span class="sxs-lookup"><span data-stu-id="81f1d-107">What are Azure AD activity logs?</span></span>

<span data-ttu-id="81f1d-108">Azure AD 提供以下三种类型的活动报告：</span><span class="sxs-lookup"><span data-stu-id="81f1d-108">Azure AD provides three types of activity reports:</span></span>

- <span data-ttu-id="81f1d-109">审核日志</span><span class="sxs-lookup"><span data-stu-id="81f1d-109">audit logs</span></span>
- <span data-ttu-id="81f1d-110">登录日志</span><span class="sxs-lookup"><span data-stu-id="81f1d-110">sign-in logs</span></span>

### <a name="directory-audits"></a><span data-ttu-id="81f1d-111">目录审核</span><span class="sxs-lookup"><span data-stu-id="81f1d-111">Directory audits</span></span>

<span data-ttu-id="81f1d-112">借助目录审核报告，你可以获取租户中执行的每项任务的历史记录。</span><span class="sxs-lookup"><span data-stu-id="81f1d-112">The directory audit report provides you with access to the history of every task performed in your tenant.</span></span> <span data-ttu-id="81f1d-113">目录审核报告为你提供了系统合规活动的记录。</span><span class="sxs-lookup"><span data-stu-id="81f1d-113">The directory audit report provides you with records of system activities for compliance.</span></span> <span data-ttu-id="81f1d-114">除此之外，提供的数据还可让你了解常见情景，例如：</span><span class="sxs-lookup"><span data-stu-id="81f1d-114">Amongst others, the provided data enables you to address common scenarios such as:</span></span>

- <span data-ttu-id="81f1d-115">谁向管理员组授予了访问目录用户的权限？</span><span class="sxs-lookup"><span data-stu-id="81f1d-115">Who granted admin group access to a directory user?</span></span>
- <span data-ttu-id="81f1d-116">哪些用户正在登录最近购买的应用程序？</span><span class="sxs-lookup"><span data-stu-id="81f1d-116">Which users are signing in to a recently acquired app?</span></span>
- <span data-ttu-id="81f1d-117">在目录中进行了多少次密码重置？</span><span class="sxs-lookup"><span data-stu-id="81f1d-117">How many passwords resets were made within the directory?</span></span>

### <a name="sign-ins"></a><span data-ttu-id="81f1d-118">登录</span><span class="sxs-lookup"><span data-stu-id="81f1d-118">Sign-ins</span></span>

<span data-ttu-id="81f1d-119">登录活动报告可帮助你确定负责执行目录审核所报告的任务的人员。</span><span class="sxs-lookup"><span data-stu-id="81f1d-119">The sign-ins report helps you determine who performed the tasks reported by directory audits.</span></span> <span data-ttu-id="81f1d-120">登录报告可帮助你回答如下问题：</span><span class="sxs-lookup"><span data-stu-id="81f1d-120">The sign-ins report helps you answer questions like:</span></span>

- <span data-ttu-id="81f1d-121">用户的登录模式是什么？</span><span class="sxs-lookup"><span data-stu-id="81f1d-121">What is the sign in pattern of a user?</span></span>
- <span data-ttu-id="81f1d-122">上周有多少用户进行了登录？</span><span class="sxs-lookup"><span data-stu-id="81f1d-122">How many users have signed in during the last week?</span></span>
- <span data-ttu-id="81f1d-123">这些登录的状态如何？</span><span class="sxs-lookup"><span data-stu-id="81f1d-123">What's the status of these sign-ins?</span></span>

## <a name="what-can-i-do-with-audit-log-apis-in-microsoft-graph"></a><span data-ttu-id="81f1d-124">可以使用 Microsoft Graph 中的审核日志 API 做什么？</span><span class="sxs-lookup"><span data-stu-id="81f1d-124">What can I do with audit log APIs in Microsoft Graph?</span></span>

<span data-ttu-id="81f1d-125">以下是处理审核日志数据的常见请求：</span><span class="sxs-lookup"><span data-stu-id="81f1d-125">The following are popular requests for working with audit log data:</span></span>

<span data-ttu-id="81f1d-126">Operation</span><span class="sxs-lookup"><span data-stu-id="81f1d-126">Operation</span></span> | <span data-ttu-id="81f1d-127">URL</span><span class="sxs-lookup"><span data-stu-id="81f1d-127">URL</span></span>
:----------|:----
<span data-ttu-id="81f1d-128">获取租户用户活动</span><span class="sxs-lookup"><span data-stu-id="81f1d-128">GET tenant user activities</span></span> | [<span data-ttu-id="81f1d-129">GET https://graph.microsoft.com/v1.0/auditLogs/directoryAudits</span><span class="sxs-lookup"><span data-stu-id="81f1d-129">GET https://graph.microsoft.com/v1.0/auditLogs/directoryAudits</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=v1.0)
<span data-ttu-id="81f1d-130">获取租户用户登录信息</span><span class="sxs-lookup"><span data-stu-id="81f1d-130">GET tenant user sign-ins</span></span> | [<span data-ttu-id="81f1d-131">GET https://graph.microsoft.com/v1.0/auditLogs/signIns</span><span class="sxs-lookup"><span data-stu-id="81f1d-131">GET https://graph.microsoft.com/v1.0/auditLogs/signIns</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=v1.0)

## <a name="what-licenses-do-i-need"></a><span data-ttu-id="81f1d-132">需要哪些许可证？</span><span class="sxs-lookup"><span data-stu-id="81f1d-132">What licenses do I need?</span></span>

<span data-ttu-id="81f1d-133">活动报告适用于已获得许可的功能。</span><span class="sxs-lookup"><span data-stu-id="81f1d-133">Activity reports are available for features that you've licensed.</span></span> <span data-ttu-id="81f1d-134">如果你拥有特定功能的许可证，则还可以访问报告。</span><span class="sxs-lookup"><span data-stu-id="81f1d-134">If you have a license for a specific feature, you also have access to the reports.</span></span>

<span data-ttu-id="81f1d-135">例如，你需要 Azure AD Premium P1 许可证才能访问自助密码审核报告。</span><span class="sxs-lookup"><span data-stu-id="81f1d-135">For example, you need an Azure AD Premium P1 license to access self-service password audit reports.</span></span>  <span data-ttu-id="81f1d-136">若要了解详细信息，请参阅 [Azure AD 许可](https://azure.microsoft.com/pricing/details/active-directory/)。</span><span class="sxs-lookup"><span data-stu-id="81f1d-136">To learn more, see [Azure AD licensing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

<span data-ttu-id="81f1d-137">登录报告需要 Azure AD Premium 许可证。</span><span class="sxs-lookup"><span data-stu-id="81f1d-137">Sign-in reports require an Azure AD Premium license.</span></span>

<span data-ttu-id="81f1d-138">若要了解详细信息，请参阅 [Azure AD 定价](https://azure.microsoft.com/pricing/details/active-directory/)。</span><span class="sxs-lookup"><span data-stu-id="81f1d-138">To learn more, see [Azure AD pricing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

## <a name="next-steps"></a><span data-ttu-id="81f1d-139">后续步骤</span><span class="sxs-lookup"><span data-stu-id="81f1d-139">Next Steps</span></span>

- <span data-ttu-id="81f1d-140">[注册你的应用程序](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)以满足报告先决条件。</span><span class="sxs-lookup"><span data-stu-id="81f1d-140">[Register your app](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to satisfy report prerequisites.</span></span> 
- <span data-ttu-id="81f1d-141">了解[审核日志](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples)和[登录示例](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples)。</span><span class="sxs-lookup"><span data-stu-id="81f1d-141">Learn from [audit log](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples) and [sign-in samples](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span></span>  
- <span data-ttu-id="81f1d-142">审查 [directoryAudit](directoryaudit.md) 资源和操作。</span><span class="sxs-lookup"><span data-stu-id="81f1d-142">Review [directoryAudit](directoryaudit.md) resource and actions.</span></span>
- <span data-ttu-id="81f1d-143">审查 [signIn](signin.md) 资源和操作。</span><span class="sxs-lookup"><span data-stu-id="81f1d-143">Review [signIn](signin.md) resource and actions.</span></span> 
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/azure-ad-auditlog-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

