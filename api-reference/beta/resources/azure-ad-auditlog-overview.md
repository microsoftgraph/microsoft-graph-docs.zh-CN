---
title: 活动报告 API 概述
description: 使用 Microsoft Graph 中的活动报告 API 访问 Azure Active Directory 创建的报告，跟踪租户中的用户活动。
localization_priority: Priority
doc_type: conceptualPageType
ms.prod: microsoft-identity-platform
author: besiler
ms.openlocfilehash: 2c3bd3533a871fabe338b960c0af14ff8ad1fa5d
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597410"
---
# <a name="activity-reports-api-overview"></a><span data-ttu-id="74003-103">活动报告 API 概述</span><span class="sxs-lookup"><span data-stu-id="74003-103">Activity reports API overview</span></span>

<span data-ttu-id="74003-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74003-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74003-105">Azure Active Directory (Azure AD) 可跟踪用户活动和创建报告，以帮助你了解用户如何访问和使用 Azure AD 服务。</span><span class="sxs-lookup"><span data-stu-id="74003-105">Azure Active Directory (Azure AD) tracks user activity and creates reports that help you understand how your users access and use Azure AD services.</span></span> <span data-ttu-id="74003-106">使用 Microsoft Graph API for Azure AD 分析这些报告中的数据，并根据组织的特定需求创建自定义解决方案。</span><span class="sxs-lookup"><span data-stu-id="74003-106">Use the Microsoft Graph API for Azure AD to analyze the data in these reports and to create custom solutions tailored to your organization's specific needs.</span></span>

<span data-ttu-id="74003-107">这些活动报告的可用性受 Azure AD 的数据保留策略管理。</span><span class="sxs-lookup"><span data-stu-id="74003-107">The availability of these activity reports is governed by the Azure AD data retention policies.</span></span> <span data-ttu-id="74003-108">有关详细信息，请参阅 [数据保留策略](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data)。</span><span class="sxs-lookup"><span data-stu-id="74003-108">For more information, see [data retention policies](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data).</span></span>

## <a name="what-are-activity-reports"></a><span data-ttu-id="74003-109">什么是活动报告？</span><span class="sxs-lookup"><span data-stu-id="74003-109">What are activity reports?</span></span>

<span data-ttu-id="74003-110">Azure AD 提供以下三种类型的活动报告：</span><span class="sxs-lookup"><span data-stu-id="74003-110">Azure AD provides three types of activity reports:</span></span>

- <span data-ttu-id="74003-111">目录审核</span><span class="sxs-lookup"><span data-stu-id="74003-111">Directory audits</span></span> 
- <span data-ttu-id="74003-112">登录</span><span class="sxs-lookup"><span data-stu-id="74003-112">Sign-ins</span></span>
- <span data-ttu-id="74003-113">预配</span><span class="sxs-lookup"><span data-stu-id="74003-113">Provisioning</span></span>

### <a name="directory-audits"></a><span data-ttu-id="74003-114">目录审核</span><span class="sxs-lookup"><span data-stu-id="74003-114">Directory audits</span></span>

<span data-ttu-id="74003-115">借助目录审核报告，你可以获取租户中执行的每项任务的历史记录。</span><span class="sxs-lookup"><span data-stu-id="74003-115">The directory audit report provides you with access to the history of every task performed in your tenant.</span></span> <span data-ttu-id="74003-116">目录审核报告为你提供了系统合规活动的记录。</span><span class="sxs-lookup"><span data-stu-id="74003-116">The directory audit report provides you with records of system activities for compliance.</span></span> <span data-ttu-id="74003-117">除此之外，提供的数据还可让你了解常见情景，例如：</span><span class="sxs-lookup"><span data-stu-id="74003-117">Amongst others, the provided data enables you to address common scenarios such as:</span></span>

- <span data-ttu-id="74003-118">谁向管理员组授予了访问目录用户的权限？</span><span class="sxs-lookup"><span data-stu-id="74003-118">Who granted admin group access to a directory user?</span></span>
- <span data-ttu-id="74003-119">哪些用户正在登录最近购买的应用程序？</span><span class="sxs-lookup"><span data-stu-id="74003-119">Which users are signing in to a recently acquired app?</span></span>
- <span data-ttu-id="74003-120">在目录中进行了多少次密码重置？</span><span class="sxs-lookup"><span data-stu-id="74003-120">How many passwords resets were made within the directory?</span></span>

### <a name="sign-ins"></a><span data-ttu-id="74003-121">登录</span><span class="sxs-lookup"><span data-stu-id="74003-121">Sign-ins</span></span>

<span data-ttu-id="74003-122">登录活动报告可帮助你确定负责执行目录审核所报告的任务的人员。</span><span class="sxs-lookup"><span data-stu-id="74003-122">The sign-ins report helps you determine who performed the tasks reported by directory audits.</span></span> <span data-ttu-id="74003-123">登录报告可帮助你回答如下问题：</span><span class="sxs-lookup"><span data-stu-id="74003-123">The sign-ins report helps you answer questions like:</span></span>

- <span data-ttu-id="74003-124">用户的登录模式是什么？</span><span class="sxs-lookup"><span data-stu-id="74003-124">What is the sign in pattern of a user?</span></span>
- <span data-ttu-id="74003-125">上周有多少用户进行了登录？</span><span class="sxs-lookup"><span data-stu-id="74003-125">How many users have signed in during the last week?</span></span>
- <span data-ttu-id="74003-126">这些登录的状态如何？</span><span class="sxs-lookup"><span data-stu-id="74003-126">What's the status of these sign-ins?</span></span>

### <a name="provisioning"></a><span data-ttu-id="74003-127">预配</span><span class="sxs-lookup"><span data-stu-id="74003-127">Provisioning</span></span>

<span data-ttu-id="74003-128">预配报告可帮助你查看 Azure AD 预配服务执行的所有操作。</span><span class="sxs-lookup"><span data-stu-id="74003-128">The provisioning report helps you see all the actions performed by the Azure AD provisioning service.</span></span> <span data-ttu-id="74003-129">预配报告可帮助你了解以下情况：</span><span class="sxs-lookup"><span data-stu-id="74003-129">The provisioning report helps you answer questions like:</span></span>

- <span data-ttu-id="74003-130">在 ServiceNow 中成功创建了哪些组？</span><span class="sxs-lookup"><span data-stu-id="74003-130">What groups were successfully created in ServiceNow?</span></span>
- <span data-ttu-id="74003-131">从 Amazon Web 服务导入了哪些角色？</span><span class="sxs-lookup"><span data-stu-id="74003-131">What roles were imported from Amazon Web Services?</span></span>
- <span data-ttu-id="74003-132">哪些用户从 Workday 创建失败？</span><span class="sxs-lookup"><span data-stu-id="74003-132">What users were unsuccessfully created from Workday?</span></span>

## <a name="what-can-i-do-with-activity-reports-in-microsoft-graph"></a><span data-ttu-id="74003-133">可以使用 Microsoft Graph 中的活动报告做什么？</span><span class="sxs-lookup"><span data-stu-id="74003-133">What can I do with activity reports in Microsoft Graph?</span></span>

<span data-ttu-id="74003-134">以下是处理报告数据的常见请求：</span><span class="sxs-lookup"><span data-stu-id="74003-134">Here are popular requests for working with report data:</span></span>

<span data-ttu-id="74003-135">操作</span><span class="sxs-lookup"><span data-stu-id="74003-135">Operation</span></span> | <span data-ttu-id="74003-136">URL</span><span class="sxs-lookup"><span data-stu-id="74003-136">URL</span></span>
:----------|:----
<span data-ttu-id="74003-137">获取租户用户活动</span><span class="sxs-lookup"><span data-stu-id="74003-137">GET tenant user activities</span></span> | [https://graph.microsoft.com/beta/auditLogs/directoryAudits](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=beta)
<span data-ttu-id="74003-138">获取租户用户登录信息</span><span class="sxs-lookup"><span data-stu-id="74003-138">GET tenant user sign-ins</span></span> | [https://graph.microsoft.com/beta/auditLogs/signIns](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=beta)
<span data-ttu-id="74003-139">获取预配日志</span><span class="sxs-lookup"><span data-stu-id="74003-139">GET provisioning logs</span></span> | [https://graph.microsoft.com/beta/auditLogs/provisioning](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/Provisioning&version=beta)

## <a name="what-licenses-do-i-need"></a><span data-ttu-id="74003-140">需要哪些许可证？</span><span class="sxs-lookup"><span data-stu-id="74003-140">What licenses do I need?</span></span>

<span data-ttu-id="74003-141">活动报告适用于已获得许可的功能。</span><span class="sxs-lookup"><span data-stu-id="74003-141">Activity reports are available for features that you've licensed.</span></span> <span data-ttu-id="74003-142">如果你拥有特定功能的许可证，则还可以访问报告。</span><span class="sxs-lookup"><span data-stu-id="74003-142">If you have a license for a specific feature, you also have access to the reports.</span></span>

<span data-ttu-id="74003-143">例如，你需要 Azure AD Premium P1 许可证才能访问自助密码审核报告。</span><span class="sxs-lookup"><span data-stu-id="74003-143">For example, you need an Azure AD Premium P1 license to access self-service password audit reports.</span></span>  <span data-ttu-id="74003-144">若要了解详细信息，请参阅 [Azure AD 许可](https://azure.microsoft.com/pricing/details/active-directory/)。</span><span class="sxs-lookup"><span data-stu-id="74003-144">To learn more, see [Azure AD licensing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

<span data-ttu-id="74003-145">登录报告需要 Azure AD Premium 许可证。</span><span class="sxs-lookup"><span data-stu-id="74003-145">Sign-in reports require an Azure AD Premium license.</span></span>

<span data-ttu-id="74003-146">若要了解详细信息，请参阅 [Azure AD 定价](https://azure.microsoft.com/pricing/details/active-directory/)。</span><span class="sxs-lookup"><span data-stu-id="74003-146">To learn more, see [Azure AD pricing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

## <a name="next-steps"></a><span data-ttu-id="74003-147">后续步骤</span><span class="sxs-lookup"><span data-stu-id="74003-147">Next steps</span></span>

- <span data-ttu-id="74003-148">[注册你的应用程序](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)以满足报告先决条件。</span><span class="sxs-lookup"><span data-stu-id="74003-148">[Register your app](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to satisfy report prerequisites.</span></span> 
- <span data-ttu-id="74003-149">了解[审核日志](/azure/active-directory/active-directory-reporting-api-audit-samples)和[登录示例](/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples)。</span><span class="sxs-lookup"><span data-stu-id="74003-149">Learn from [audit log](/azure/active-directory/active-directory-reporting-api-audit-samples) and [sign-in samples](/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span></span>  
- <span data-ttu-id="74003-150">审查 [directoryAudit](directoryaudit.md) 资源和操作。</span><span class="sxs-lookup"><span data-stu-id="74003-150">Review the [directoryAudit](directoryaudit.md) resource and actions.</span></span>
- <span data-ttu-id="74003-151">审查 [signIn](signin.md) 资源和操作。</span><span class="sxs-lookup"><span data-stu-id="74003-151">Review the [signIn](signin.md) resource and actions.</span></span> 
- <span data-ttu-id="74003-152">审查 [provisioningObjectSummary](provisioningobjectsummary.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="74003-152">Review the [provisioningObjectSummary](provisioningobjectsummary.md) resource.</span></span>