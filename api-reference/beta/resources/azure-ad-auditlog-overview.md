---
title: Azure AD 审核日志 API 概述
description: Azure Active Directory (Azure AD) 跟踪用户活动和登录指标，并创建审核日志报告可帮助您了解您的用户如何访问和利用 Azure AD 服务。 若要分析的数据，这些报告和创建组织的特定需要的自定义解决方案，请使用 Azure AD Microsoft Graph API。
ms.openlocfilehash: b25e9820d4f6df0c6a38fc9784a37ce8a82ceeb1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042924"
---
# <a name="azure-ad-audit-log-api-overview"></a><span data-ttu-id="93f12-104">Azure AD 审核日志 API 概述</span><span class="sxs-lookup"><span data-stu-id="93f12-104">Azure AD audit log API overview</span></span>

> <span data-ttu-id="93f12-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="93f12-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="93f12-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="93f12-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="93f12-107">Azure Active Directory (Azure AD) 跟踪用户活动和登录指标，并创建审核日志报告可帮助您了解您的用户如何访问和利用 Azure AD 服务。</span><span class="sxs-lookup"><span data-stu-id="93f12-107">Azure Active Directory (Azure AD) tracks user activity and sign-in metrics and creates audit log reports that help you understand how your users access and leverage Azure AD services.</span></span> <span data-ttu-id="93f12-108">若要分析的数据，这些报告和创建组织的特定需要的自定义解决方案，请使用 Azure AD Microsoft Graph API。</span><span class="sxs-lookup"><span data-stu-id="93f12-108">Use the Microsoft Graph API for Azure AD to analyze the data underlying these reports and to create custom solutions tailored to your organization's specific needs.</span></span>

## <a name="what-are-azure-ad-activity-logs"></a><span data-ttu-id="93f12-109">什么是 Azure AD 活动日志？</span><span class="sxs-lookup"><span data-stu-id="93f12-109">What are Azure AD activity logs?</span></span>

<span data-ttu-id="93f12-110">Azure AD 提供了两种类型的活动日志：</span><span class="sxs-lookup"><span data-stu-id="93f12-110">Azure AD provides two types of activity logs:</span></span>

- <span data-ttu-id="93f12-111">审核日志</span><span class="sxs-lookup"><span data-stu-id="93f12-111">audit logs</span></span> 
- <span data-ttu-id="93f12-112">登录日志</span><span class="sxs-lookup"><span data-stu-id="93f12-112">sign-in logs</span></span>

### <a name="audit-logs"></a><span data-ttu-id="93f12-113">审核日志</span><span class="sxs-lookup"><span data-stu-id="93f12-113">Audit logs</span></span>

<span data-ttu-id="93f12-114">审核日志活动报告提供有权访问您的租户中执行每个任务的历史记录。</span><span class="sxs-lookup"><span data-stu-id="93f12-114">The audit logs activity report provides you with access to the history of every task performed in your tenant.</span></span> <span data-ttu-id="93f12-115">审核日志报告为您提供的合规性系统活动记录。</span><span class="sxs-lookup"><span data-stu-id="93f12-115">The audit logs report provides you with records of system activities for compliance.</span></span> <span data-ttu-id="93f12-116">在其他中提供的数据使您能够解决常见方案，如：</span><span class="sxs-lookup"><span data-stu-id="93f12-116">Amongst others, the provided data enables you to address common scenarios such as:</span></span>

- <span data-ttu-id="93f12-117">谁将管理组的访问权限授予目录用户？</span><span class="sxs-lookup"><span data-stu-id="93f12-117">Who granted admin group access to a directory user?</span></span>

- <span data-ttu-id="93f12-118">哪些用户登录到的最近收购的应用程序？</span><span class="sxs-lookup"><span data-stu-id="93f12-118">Which users are signing in to a recently acquired app?</span></span>

- <span data-ttu-id="93f12-119">在目录内进行多少密码重置？</span><span class="sxs-lookup"><span data-stu-id="93f12-119">How many passwords resets were made within the directory?</span></span>

### <a name="sign-in-logs"></a><span data-ttu-id="93f12-120">登录日志</span><span class="sxs-lookup"><span data-stu-id="93f12-120">Sign in logs</span></span>

<span data-ttu-id="93f12-121">登录活动报告可帮助您确定用户执行的任务报告的审核日志报告。</span><span class="sxs-lookup"><span data-stu-id="93f12-121">The sign-ins activity report helps you determine who performed the tasks reported by audit log reports.</span></span> <span data-ttu-id="93f12-122">登录活动报告可帮助您回答以下问题：</span><span class="sxs-lookup"><span data-stu-id="93f12-122">The sign-ins activity report helps you answer questions like:</span></span>

- <span data-ttu-id="93f12-123">什么是用户的模式登录？</span><span class="sxs-lookup"><span data-stu-id="93f12-123">What is the sign in pattern of a user?</span></span>
- <span data-ttu-id="93f12-124">多少用户登录过程的最后一个星期中？</span><span class="sxs-lookup"><span data-stu-id="93f12-124">How many users have signed in during the last week?</span></span>
- <span data-ttu-id="93f12-125">这些登录的状态是什么？</span><span class="sxs-lookup"><span data-stu-id="93f12-125">What's the status of these sign-ins?</span></span>

## <a name="what-can-i-do-with-audit-log-apis-in-microsoft-graph"></a><span data-ttu-id="93f12-126">使用审核日志在 Microsoft Graph 中的 Api 可以做什么？</span><span class="sxs-lookup"><span data-stu-id="93f12-126">What can I do with audit log APIs in Microsoft Graph?</span></span>

<span data-ttu-id="93f12-127">下面是使用审核日志数据的常用请求：</span><span class="sxs-lookup"><span data-stu-id="93f12-127">Here are popular requests for working with audit log data:</span></span>

<span data-ttu-id="93f12-128">操作</span><span class="sxs-lookup"><span data-stu-id="93f12-128">Operation</span></span> | <span data-ttu-id="93f12-129">URL</span><span class="sxs-lookup"><span data-stu-id="93f12-129">URL</span></span>
:----------|:----
<span data-ttu-id="93f12-130">获取用户活动的租户</span><span class="sxs-lookup"><span data-stu-id="93f12-130">GET tenant user activities</span></span> | [https://graph.microsoft.com/beta/auditLogs/directoryAudits](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=beta)
<span data-ttu-id="93f12-131">获取用户登录的租户</span><span class="sxs-lookup"><span data-stu-id="93f12-131">GET tenant user sign-ins</span></span> | [https://graph.microsoft.com/beta/auditLogs/signIns](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=beta)

## <a name="what-licenses-do-i-need"></a><span data-ttu-id="93f12-132">是否需要哪些许可证？</span><span class="sxs-lookup"><span data-stu-id="93f12-132">What licenses do I need?</span></span>

<span data-ttu-id="93f12-133">审核日志报告是可用于已许可的功能。</span><span class="sxs-lookup"><span data-stu-id="93f12-133">Audit log reports are available for features that you've licensed.</span></span>  <span data-ttu-id="93f12-134">如果您有特定功能的许可证，还可以访问其审核日志。</span><span class="sxs-lookup"><span data-stu-id="93f12-134">If you have a license for a specific feature, you also have access to its audit logs.</span></span>

<span data-ttu-id="93f12-135">例如，您需要访问自助服务密码审核报告的 Azure AD Premium P1 许可证。</span><span class="sxs-lookup"><span data-stu-id="93f12-135">For example, you need an Azure AD Premium P1 license to access self-service password audit reports.</span></span>  <span data-ttu-id="93f12-136">若要了解详细信息，请参阅[Azure AD 许可](https://azure.microsoft.com/pricing/details/active-directory/)。</span><span class="sxs-lookup"><span data-stu-id="93f12-136">To learn more, see [Azure AD licensing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

<span data-ttu-id="93f12-137">登录报告需要的 Azure AD Premium 许可证。</span><span class="sxs-lookup"><span data-stu-id="93f12-137">Sign-in reports require an Azure AD Premium license.</span></span>

<span data-ttu-id="93f12-138">若要了解详细信息，请参阅[Azure AD 定价](https://azure.microsoft.com/pricing/details/active-directory/)。</span><span class="sxs-lookup"><span data-stu-id="93f12-138">To learn more, see [Azure AD pricing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

## <a name="next-steps"></a><span data-ttu-id="93f12-139">后续步骤</span><span class="sxs-lookup"><span data-stu-id="93f12-139">Next Steps</span></span>

- <span data-ttu-id="93f12-140">[注册应用程序](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)，以满足审核日志必备组件。</span><span class="sxs-lookup"><span data-stu-id="93f12-140">[Register your app](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to satisfy audit log prerequisites.</span></span> 
- <span data-ttu-id="93f12-141">了解从[审核日志](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples)和[登录项示例](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples)。</span><span class="sxs-lookup"><span data-stu-id="93f12-141">Learn from [audit log](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples) and [sign-in samples](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span></span>  
- <span data-ttu-id="93f12-142">查看[directoryAudit](directoryaudit.md)资源和操作。</span><span class="sxs-lookup"><span data-stu-id="93f12-142">Review [directoryAudit](directoryaudit.md) resource and actions.</span></span>
- <span data-ttu-id="93f12-143">查看[次数](signin.md)资源和操作。</span><span class="sxs-lookup"><span data-stu-id="93f12-143">Review [signIn](signin.md) resource and actions.</span></span> 