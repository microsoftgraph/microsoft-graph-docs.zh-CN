---
title: 活动报告 API 概述
description: 使用 Microsoft Graph 中的活动报告 API 访问 Azure Active Directory 创建的报告，跟踪租户中的用户活动。
localization_priority: Priority
author: besiler
ms.prod: identity-and-access-reports
doc_type: conceptualPageType
ms.openlocfilehash: 28d09cfe7dcb78480e02e5a2a23893495eb6655f
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546208"
---
# <a name="activity-reports-api-overview"></a><span data-ttu-id="a1f4f-103">活动报告 API 概述</span><span class="sxs-lookup"><span data-stu-id="a1f4f-103">Activity reports API overview</span></span>

<span data-ttu-id="a1f4f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1f4f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a1f4f-105">Azure Active Directory (Azure AD) 可跟踪用户活动和创建报告，以帮助你了解用户如何访问和使用 Azure AD 服务。</span><span class="sxs-lookup"><span data-stu-id="a1f4f-105">Azure Active Directory (Azure AD) tracks user activity and creates reports that help you understand how your users access and use Azure AD services.</span></span> <span data-ttu-id="a1f4f-106">使用 Microsoft Graph API for Azure AD 分析这些报告中的数据，并根据组织的特定需求创建自定义解决方案。</span><span class="sxs-lookup"><span data-stu-id="a1f4f-106">Use the Microsoft Graph API for Azure AD to analyze the data in these reports and to create custom solutions tailored to your organization's specific needs.</span></span>

<span data-ttu-id="a1f4f-107">这些活动报告的可用性受 Azure AD 的数据保留策略管理。</span><span class="sxs-lookup"><span data-stu-id="a1f4f-107">The availability of these activity reports is governed by the Azure AD data retention policies.</span></span> <span data-ttu-id="a1f4f-108">有关详细信息，请参阅 [数据保留策略](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data)。</span><span class="sxs-lookup"><span data-stu-id="a1f4f-108">For more information, see [data retention policies](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data).</span></span>

## <a name="what-are-azure-ad-activity-logs"></a><span data-ttu-id="a1f4f-109">什么是 Azure AD 活动日志？</span><span class="sxs-lookup"><span data-stu-id="a1f4f-109">What are Azure AD activity logs?</span></span>

<span data-ttu-id="a1f4f-110">Azure AD 提供以下三种类型的活动报告：</span><span class="sxs-lookup"><span data-stu-id="a1f4f-110">Azure AD provides the following types of activity reports:</span></span>

- <span data-ttu-id="a1f4f-111">目录审核</span><span class="sxs-lookup"><span data-stu-id="a1f4f-111">Directory audits</span></span>
- <span data-ttu-id="a1f4f-112">登录</span><span class="sxs-lookup"><span data-stu-id="a1f4f-112">Sign-ins</span></span>

### <a name="directory-audits"></a><span data-ttu-id="a1f4f-113">目录审核</span><span class="sxs-lookup"><span data-stu-id="a1f4f-113">Directory audits</span></span>

<span data-ttu-id="a1f4f-114">借助目录审核报告，你可以获取租户中执行的每项任务的历史记录。</span><span class="sxs-lookup"><span data-stu-id="a1f4f-114">The directory audit report provides you with access to the history of every task performed in your tenant.</span></span> <span data-ttu-id="a1f4f-115">目录审核报告为你提供了系统合规活动的记录。</span><span class="sxs-lookup"><span data-stu-id="a1f4f-115">The directory audit report provides you with records of system activities for compliance.</span></span> <span data-ttu-id="a1f4f-116">除此之外，提供的数据还可让你了解常见情景，例如：</span><span class="sxs-lookup"><span data-stu-id="a1f4f-116">Amongst others, the provided data enables you to address common scenarios such as:</span></span>

- <span data-ttu-id="a1f4f-117">谁向管理员组授予了访问目录用户的权限？</span><span class="sxs-lookup"><span data-stu-id="a1f4f-117">Who granted admin group access to a directory user?</span></span>
- <span data-ttu-id="a1f4f-118">哪些用户正在登录最近购买的应用程序？</span><span class="sxs-lookup"><span data-stu-id="a1f4f-118">Which users are signing in to a recently acquired app?</span></span>
- <span data-ttu-id="a1f4f-119">在目录中进行了多少次密码重置？</span><span class="sxs-lookup"><span data-stu-id="a1f4f-119">How many passwords resets were made within the directory?</span></span>

### <a name="sign-ins"></a><span data-ttu-id="a1f4f-120">登录</span><span class="sxs-lookup"><span data-stu-id="a1f4f-120">Sign-ins</span></span>

<span data-ttu-id="a1f4f-121">登录活动报告可帮助你确定负责执行目录审核所报告的任务的人员。</span><span class="sxs-lookup"><span data-stu-id="a1f4f-121">The sign-ins report helps you determine who performed the tasks reported by directory audits.</span></span> <span data-ttu-id="a1f4f-122">登录报告可帮助你回答如下问题：</span><span class="sxs-lookup"><span data-stu-id="a1f4f-122">The sign-ins report helps you answer questions like:</span></span>

- <span data-ttu-id="a1f4f-123">用户的登录模式是什么？</span><span class="sxs-lookup"><span data-stu-id="a1f4f-123">What is the sign in pattern of a user?</span></span>
- <span data-ttu-id="a1f4f-124">上周有多少用户进行了登录？</span><span class="sxs-lookup"><span data-stu-id="a1f4f-124">How many users have signed in during the last week?</span></span>
- <span data-ttu-id="a1f4f-125">这些登录的状态如何？</span><span class="sxs-lookup"><span data-stu-id="a1f4f-125">What's the status of these sign-ins?</span></span>

## <a name="what-can-i-do-with-audit-log-apis-in-microsoft-graph"></a><span data-ttu-id="a1f4f-126">可以使用 Microsoft Graph 中的审核日志 API 做什么？</span><span class="sxs-lookup"><span data-stu-id="a1f4f-126">What can I do with audit log APIs in Microsoft Graph?</span></span>

<span data-ttu-id="a1f4f-127">以下是处理审核日志数据的常见请求：</span><span class="sxs-lookup"><span data-stu-id="a1f4f-127">The following are popular requests for working with audit log data:</span></span>

<span data-ttu-id="a1f4f-128">Operation</span><span class="sxs-lookup"><span data-stu-id="a1f4f-128">Operation</span></span> | <span data-ttu-id="a1f4f-129">URL</span><span class="sxs-lookup"><span data-stu-id="a1f4f-129">URL</span></span>
:----------|:----
<span data-ttu-id="a1f4f-130">获取租户用户活动</span><span class="sxs-lookup"><span data-stu-id="a1f4f-130">GET tenant user activities</span></span> | [<span data-ttu-id="a1f4f-131">GET https://graph.microsoft.com/v1.0/auditLogs/directoryAudits</span><span class="sxs-lookup"><span data-stu-id="a1f4f-131">GET https://graph.microsoft.com/v1.0/auditLogs/directoryAudits</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=v1.0)
<span data-ttu-id="a1f4f-132">获取租户用户登录信息</span><span class="sxs-lookup"><span data-stu-id="a1f4f-132">GET tenant user sign-ins</span></span> | [<span data-ttu-id="a1f4f-133">GET https://graph.microsoft.com/v1.0/auditLogs/signIns</span><span class="sxs-lookup"><span data-stu-id="a1f4f-133">GET https://graph.microsoft.com/v1.0/auditLogs/signIns</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=v1.0)

## <a name="what-licenses-do-i-need"></a><span data-ttu-id="a1f4f-134">需要哪些许可证？</span><span class="sxs-lookup"><span data-stu-id="a1f4f-134">What licenses do I need?</span></span>

<span data-ttu-id="a1f4f-135">活动报告适用于已获得许可的功能。</span><span class="sxs-lookup"><span data-stu-id="a1f4f-135">Activity reports are available for features that you've licensed.</span></span> <span data-ttu-id="a1f4f-136">如果你拥有特定功能的许可证，则还可以访问报告。</span><span class="sxs-lookup"><span data-stu-id="a1f4f-136">If you have a license for a specific feature, you also have access to the reports.</span></span>

<span data-ttu-id="a1f4f-137">例如，你需要 Azure AD Premium P1 许可证才能访问自助密码审核报告。</span><span class="sxs-lookup"><span data-stu-id="a1f4f-137">For example, you need an Azure AD Premium P1 license to access self-service password audit reports.</span></span>  <span data-ttu-id="a1f4f-138">若要了解详细信息，请参阅 [Azure AD 许可](https://azure.microsoft.com/pricing/details/active-directory/)。</span><span class="sxs-lookup"><span data-stu-id="a1f4f-138">To learn more, see [Azure AD licensing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

<span data-ttu-id="a1f4f-139">登录报告需要 Azure AD Premium 许可证。</span><span class="sxs-lookup"><span data-stu-id="a1f4f-139">Sign-in reports require an Azure AD Premium license.</span></span>

<span data-ttu-id="a1f4f-140">若要了解详细信息，请参阅 [Azure AD 定价](https://azure.microsoft.com/pricing/details/active-directory/)。</span><span class="sxs-lookup"><span data-stu-id="a1f4f-140">To learn more, see [Azure AD pricing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

## <a name="next-steps"></a><span data-ttu-id="a1f4f-141">后续步骤</span><span class="sxs-lookup"><span data-stu-id="a1f4f-141">Next Steps</span></span>

- <span data-ttu-id="a1f4f-142">[注册你的应用程序](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)以满足报告先决条件。</span><span class="sxs-lookup"><span data-stu-id="a1f4f-142">[Register your app](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to satisfy report prerequisites.</span></span> 
- <span data-ttu-id="a1f4f-143">了解[审核日志](/azure/active-directory/active-directory-reporting-api-audit-samples)和[登录示例](/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples)。</span><span class="sxs-lookup"><span data-stu-id="a1f4f-143">Learn from [audit log](/azure/active-directory/active-directory-reporting-api-audit-samples) and [sign-in samples](/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span></span>  
- <span data-ttu-id="a1f4f-144">审查 [directoryAudit](directoryaudit.md) 资源和操作。</span><span class="sxs-lookup"><span data-stu-id="a1f4f-144">Review [directoryAudit](directoryaudit.md) resource and actions.</span></span>
- <span data-ttu-id="a1f4f-145">审查 [signIn](signin.md) 资源和操作。</span><span class="sxs-lookup"><span data-stu-id="a1f4f-145">Review [signIn](signin.md) resource and actions.</span></span> 
<!--
{
  "type": "#page.annotation",
  "suppressions": [
  ]
}
-->
