---
title: Azure AD 审核日志 API 概述
description: Azure Active Directory (Azure AD) 可跟踪用户活动和登录指标并创建审核日志报告，以帮助你了解用户如何访问和使用 Azure AD 服务。
localization_priority: Priority
author: kholtz
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: f2841b950096ca43f72f387a50a39b632e53ab62
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2020
ms.locfileid: "43124215"
---
# <a name="azure-ad-audit-log-api-overview"></a><span data-ttu-id="573aa-103">Azure AD 审核日志 API 概述</span><span class="sxs-lookup"><span data-stu-id="573aa-103">Azure AD audit log API overview</span></span>

<span data-ttu-id="573aa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="573aa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="573aa-105">Azure Active Directory (Azure AD) 可跟踪用户活动和登录指标并创建审核日志报告，以帮助你了解用户如何访问和使用 Azure AD 服务。</span><span class="sxs-lookup"><span data-stu-id="573aa-105">Azure Active Directory (Azure AD) tracks user activity and sign-in metrics and creates audit log reports that help you understand how your users access and use Azure AD services.</span></span> <span data-ttu-id="573aa-106">使用 Microsoft Graph API for Azure AD 分析这些报告的基础数据，并根据组织的特定需求创建自定义解决方案。</span><span class="sxs-lookup"><span data-stu-id="573aa-106">Use the Microsoft Graph API for Azure AD to analyze the data underlying these reports and to create custom solutions tailored to your organization's specific needs.</span></span>

## <a name="what-are-azure-ad-activity-logs"></a><span data-ttu-id="573aa-107">什么是 Azure AD 活动日志？</span><span class="sxs-lookup"><span data-stu-id="573aa-107">What are Azure AD activity logs?</span></span>

<span data-ttu-id="573aa-108">Azure AD 提供了两种类型的活动日志：</span><span class="sxs-lookup"><span data-stu-id="573aa-108">Azure AD provides two types of activity logs:</span></span>

- <span data-ttu-id="573aa-109">审核日志</span><span class="sxs-lookup"><span data-stu-id="573aa-109">audit logs</span></span>
- <span data-ttu-id="573aa-110">登录日志</span><span class="sxs-lookup"><span data-stu-id="573aa-110">sign-in logs</span></span>

### <a name="audit-logs"></a><span data-ttu-id="573aa-111">审核日志</span><span class="sxs-lookup"><span data-stu-id="573aa-111">Audit logs</span></span>

<span data-ttu-id="573aa-112">通过审核日志活动报告，你可以访问在租户中执行的每项任务的历史记录。</span><span class="sxs-lookup"><span data-stu-id="573aa-112">The audit logs activity report provides you with access to the history of every task performed in your tenant.</span></span> <span data-ttu-id="573aa-113">审核日志报告为你提供了系统合规活动的记录。</span><span class="sxs-lookup"><span data-stu-id="573aa-113">The audit logs report provides you with records of system activities for compliance.</span></span> <span data-ttu-id="573aa-114">除此之外，提供的数据还可让你了解常见情景，例如：</span><span class="sxs-lookup"><span data-stu-id="573aa-114">Amongst others, the provided data enables you to address common scenarios such as:</span></span>

- <span data-ttu-id="573aa-115">谁向管理员组授予了访问目录用户的权限？</span><span class="sxs-lookup"><span data-stu-id="573aa-115">Who granted admin group access to a directory user?</span></span>
- <span data-ttu-id="573aa-116">哪些用户正在登录最近购买的应用程序？</span><span class="sxs-lookup"><span data-stu-id="573aa-116">Which users are signing in to a recently acquired app?</span></span>
- <span data-ttu-id="573aa-117">在目录中进行了多少次密码重置？</span><span class="sxs-lookup"><span data-stu-id="573aa-117">How many passwords resets were made within the directory?</span></span>

### <a name="sign-in-logs"></a><span data-ttu-id="573aa-118">登录日志</span><span class="sxs-lookup"><span data-stu-id="573aa-118">Sign-in logs</span></span>

<span data-ttu-id="573aa-119">登录活动报告可帮助你确定负责执行审核日志报告所报告的任务的人员。</span><span class="sxs-lookup"><span data-stu-id="573aa-119">The sign-ins activity report helps you determine who performed the tasks reported by audit log reports.</span></span> <span data-ttu-id="573aa-120">登录活动报告可帮助你回答如下问题：</span><span class="sxs-lookup"><span data-stu-id="573aa-120">The sign-ins activity report helps you answer questions like:</span></span>

- <span data-ttu-id="573aa-121">用户的登录模式是什么？</span><span class="sxs-lookup"><span data-stu-id="573aa-121">What is the sign in pattern of a user?</span></span>
- <span data-ttu-id="573aa-122">上周有多少用户进行了登录？</span><span class="sxs-lookup"><span data-stu-id="573aa-122">How many users have signed in during the last week?</span></span>
- <span data-ttu-id="573aa-123">这些登录的状态如何？</span><span class="sxs-lookup"><span data-stu-id="573aa-123">What's the status of these sign-ins?</span></span>

## <a name="what-can-i-do-with-audit-log-apis-in-microsoft-graph"></a><span data-ttu-id="573aa-124">可以使用 Microsoft Graph 中的审核日志 API 做什么？</span><span class="sxs-lookup"><span data-stu-id="573aa-124">What can I do with audit log APIs in Microsoft Graph?</span></span>

<span data-ttu-id="573aa-125">以下是处理审核日志数据的常见请求：</span><span class="sxs-lookup"><span data-stu-id="573aa-125">The following are popular requests for working with audit log data:</span></span>

<span data-ttu-id="573aa-126">Operation</span><span class="sxs-lookup"><span data-stu-id="573aa-126">Operation</span></span> | <span data-ttu-id="573aa-127">URL</span><span class="sxs-lookup"><span data-stu-id="573aa-127">URL</span></span>
:----------|:----
<span data-ttu-id="573aa-128">获取租户用户活动</span><span class="sxs-lookup"><span data-stu-id="573aa-128">GET tenant user activities</span></span> | [<span data-ttu-id="573aa-129">GET https://graph.microsoft.com/v1.0/auditLogs/directoryAudits</span><span class="sxs-lookup"><span data-stu-id="573aa-129">GET https://graph.microsoft.com/v1.0/auditLogs/directoryAudits</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=v1.0)
<span data-ttu-id="573aa-130">获取租户用户登录信息</span><span class="sxs-lookup"><span data-stu-id="573aa-130">GET tenant user sign-ins</span></span> | [<span data-ttu-id="573aa-131">GET https://graph.microsoft.com/v1.0/auditLogs/signIns</span><span class="sxs-lookup"><span data-stu-id="573aa-131">GET https://graph.microsoft.com/v1.0/auditLogs/signIns</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=v1.0)

## <a name="what-licenses-do-i-need"></a><span data-ttu-id="573aa-132">需要哪些许可证？</span><span class="sxs-lookup"><span data-stu-id="573aa-132">What licenses do I need?</span></span>

<span data-ttu-id="573aa-133">审核日志报告适用于已获得许可的功能。</span><span class="sxs-lookup"><span data-stu-id="573aa-133">Audit log reports are available for features that you've licensed.</span></span>  <span data-ttu-id="573aa-134">如果你拥有特定功能的许可证，则还可以访问其审核日志。</span><span class="sxs-lookup"><span data-stu-id="573aa-134">If you have a license for a specific feature, you also have access to its audit logs.</span></span>

<span data-ttu-id="573aa-135">例如，你需要 Azure AD Premium P1 许可证才能访问自助密码审核报告。</span><span class="sxs-lookup"><span data-stu-id="573aa-135">For example, you need an Azure AD Premium P1 license to access self-service password audit reports.</span></span>  <span data-ttu-id="573aa-136">若要了解详细信息，请参阅 [Azure AD 许可](https://azure.microsoft.com/pricing/details/active-directory/)。</span><span class="sxs-lookup"><span data-stu-id="573aa-136">To learn more, see [Azure AD licensing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

<span data-ttu-id="573aa-137">登录报告需要 Azure AD Premium 许可证。</span><span class="sxs-lookup"><span data-stu-id="573aa-137">Sign-in reports require an Azure AD Premium license.</span></span>

<span data-ttu-id="573aa-138">若要了解详细信息，请参阅 [Azure AD 定价](https://azure.microsoft.com/pricing/details/active-directory/)。</span><span class="sxs-lookup"><span data-stu-id="573aa-138">To learn more, see [Azure AD pricing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

## <a name="next-steps"></a><span data-ttu-id="573aa-139">后续步骤</span><span class="sxs-lookup"><span data-stu-id="573aa-139">Next Steps</span></span>

- <span data-ttu-id="573aa-140">[注册你的应用程序](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)以满足审核日志先决条件。</span><span class="sxs-lookup"><span data-stu-id="573aa-140">[Register your app](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to satisfy audit log prerequisites.</span></span> 
- <span data-ttu-id="573aa-141">了解[审核日志](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples)和[登录示例](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples)。</span><span class="sxs-lookup"><span data-stu-id="573aa-141">Learn from [audit log](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples) and [sign-in samples](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span></span>  
- <span data-ttu-id="573aa-142">审查 [directoryAudit](directoryaudit.md) 资源和操作。</span><span class="sxs-lookup"><span data-stu-id="573aa-142">Review [directoryAudit](directoryaudit.md) resource and actions.</span></span>
- <span data-ttu-id="573aa-143">审查 [signIn](signin.md) 资源和操作。</span><span class="sxs-lookup"><span data-stu-id="573aa-143">Review [signIn](signin.md) resource and actions.</span></span> 
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/azure-ad-auditlog-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
