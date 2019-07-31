---
title: Azure AD 审核日志 API 概述
description: Azure Active Directory (Azure AD) 可跟踪用户活动和登录指标并创建审核日志报告，以帮助你了解用户如何访问和使用 Azure AD 服务。 使用 Microsoft Graph API for Azure AD 分析这些报告的基础数据，并根据组织的特定需求创建自定义解决方案。
localization_priority: Priority
doc_type: conceptualPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 9d739cbe711ad175e485ecb3d9d12173718a1b75
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974237"
---
# <a name="azure-ad-audit-log-api-overview"></a><span data-ttu-id="6bd14-104">Azure AD 审核日志 API 概述</span><span class="sxs-lookup"><span data-stu-id="6bd14-104">Azure AD audit log API overview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6bd14-105">Azure Active Directory (Azure AD) 可跟踪用户活动和登录指标并创建审核日志报告，以帮助你了解用户如何访问和使用 Azure AD 服务。</span><span class="sxs-lookup"><span data-stu-id="6bd14-105">Azure Active Directory (Azure AD) tracks user activity and sign-in metrics and creates audit log reports that help you understand how your users access and use Azure AD services.</span></span> <span data-ttu-id="6bd14-106">使用 Microsoft Graph API for Azure AD 分析这些报告的基础数据，并根据组织的特定需求创建自定义解决方案。</span><span class="sxs-lookup"><span data-stu-id="6bd14-106">Use the Microsoft Graph API for Azure AD to analyze the data underlying these reports and to create custom solutions tailored to your organization's specific needs.</span></span>

## <a name="what-are-azure-ad-activity-logs"></a><span data-ttu-id="6bd14-107">什么是 Azure AD 活动日志？</span><span class="sxs-lookup"><span data-stu-id="6bd14-107">What are Azure AD activity logs?</span></span>

<span data-ttu-id="6bd14-108">Azure AD 提供了三种类型的活动日志：</span><span class="sxs-lookup"><span data-stu-id="6bd14-108">Azure AD provides two types of activity logs:</span></span>

- <span data-ttu-id="6bd14-109">审核日志</span><span class="sxs-lookup"><span data-stu-id="6bd14-109">Audit logs</span></span> 
- <span data-ttu-id="6bd14-110">登录日志</span><span class="sxs-lookup"><span data-stu-id="6bd14-110">Sign-in logs</span></span>
- <span data-ttu-id="6bd14-111">预配日志</span><span class="sxs-lookup"><span data-stu-id="6bd14-111">Provisioning logs</span></span>

### <a name="audit-logs"></a><span data-ttu-id="6bd14-112">审核日志</span><span class="sxs-lookup"><span data-stu-id="6bd14-112">Audit logs</span></span>

<span data-ttu-id="6bd14-113">通过审核日志活动报告，你可以访问在租户中执行的每项任务的历史记录。</span><span class="sxs-lookup"><span data-stu-id="6bd14-113">The audit logs activity report provides you with access to the history of every task performed in your tenant.</span></span> <span data-ttu-id="6bd14-114">审核日志报告为你提供了系统合规活动的记录。</span><span class="sxs-lookup"><span data-stu-id="6bd14-114">The audit logs report provides you with records of system activities for compliance.</span></span> <span data-ttu-id="6bd14-115">除此之外，提供的数据还可让你了解常见情景，例如：</span><span class="sxs-lookup"><span data-stu-id="6bd14-115">Amongst others, the provided data enables you to address common scenarios such as:</span></span>

- <span data-ttu-id="6bd14-116">谁向管理员组授予了访问目录用户的权限？</span><span class="sxs-lookup"><span data-stu-id="6bd14-116">Who granted admin group access to a directory user?</span></span>

- <span data-ttu-id="6bd14-117">哪些用户正在登录最近购买的应用程序？</span><span class="sxs-lookup"><span data-stu-id="6bd14-117">Which users are signing in to a recently acquired app?</span></span>

- <span data-ttu-id="6bd14-118">在目录中进行了多少次密码重置？</span><span class="sxs-lookup"><span data-stu-id="6bd14-118">How many passwords resets were made within the directory?</span></span>

### <a name="sign-in-logs"></a><span data-ttu-id="6bd14-119">登录日志</span><span class="sxs-lookup"><span data-stu-id="6bd14-119">Sign-in logs</span></span>

<span data-ttu-id="6bd14-120">登录活动报告可帮助你确定负责执行审核日志报告所报告的任务的人员。</span><span class="sxs-lookup"><span data-stu-id="6bd14-120">The sign-ins activity report helps you determine who performed the tasks reported by audit log reports.</span></span> <span data-ttu-id="6bd14-121">登录活动报告可帮助你回答如下问题：</span><span class="sxs-lookup"><span data-stu-id="6bd14-121">The sign-ins activity report helps you answer questions like:</span></span>

- <span data-ttu-id="6bd14-122">用户的登录模式是什么？</span><span class="sxs-lookup"><span data-stu-id="6bd14-122">What is the sign in pattern of a user?</span></span>
- <span data-ttu-id="6bd14-123">上周有多少用户进行了登录？</span><span class="sxs-lookup"><span data-stu-id="6bd14-123">How many users have signed in during the last week?</span></span>
- <span data-ttu-id="6bd14-124">这些登录的状态如何？</span><span class="sxs-lookup"><span data-stu-id="6bd14-124">What's the status of these sign-ins?</span></span>

### <a name="provisioning-logs"></a><span data-ttu-id="6bd14-125">预配日志</span><span class="sxs-lookup"><span data-stu-id="6bd14-125">Provisioning logs</span></span>
<span data-ttu-id="6bd14-126">预配日志可帮助你查看 Azure AD 预配服务执行的所有操作。</span><span class="sxs-lookup"><span data-stu-id="6bd14-126">The provisioning logs help you see all the actions performed by the Azure AD provisioning service.</span></span> <span data-ttu-id="6bd14-127">预配日志可帮助你了解以下情况：</span><span class="sxs-lookup"><span data-stu-id="6bd14-127">The provisioning logs help you answer questions like:</span></span>

- <span data-ttu-id="6bd14-128">在 ServiceNow 中成功创建了哪些组？</span><span class="sxs-lookup"><span data-stu-id="6bd14-128">What groups were successfully created in ServiceNow?</span></span>
- <span data-ttu-id="6bd14-129">从 Amazon Web 服务导入了哪些角色？</span><span class="sxs-lookup"><span data-stu-id="6bd14-129">What roles were imported from Amazon Web Services?</span></span>
- <span data-ttu-id="6bd14-130">哪些用户从 Workday 创建失败？</span><span class="sxs-lookup"><span data-stu-id="6bd14-130">What users were unsuccessfully created from Workday?</span></span>

## <a name="what-can-i-do-with-audit-log-apis-in-microsoft-graph"></a><span data-ttu-id="6bd14-131">可以使用 Microsoft Graph 中的审核日志 API 做什么？</span><span class="sxs-lookup"><span data-stu-id="6bd14-131">What can I do with audit log APIs in Microsoft Graph?</span></span>

<span data-ttu-id="6bd14-132">以下是处理审核日志数据的常见请求：</span><span class="sxs-lookup"><span data-stu-id="6bd14-132">Here are popular requests for working with audit log data:</span></span>

<span data-ttu-id="6bd14-133">操作</span><span class="sxs-lookup"><span data-stu-id="6bd14-133">Operation</span></span> | <span data-ttu-id="6bd14-134">URL</span><span class="sxs-lookup"><span data-stu-id="6bd14-134">URL</span></span>
:----------|:----
<span data-ttu-id="6bd14-135">获取租户用户活动</span><span class="sxs-lookup"><span data-stu-id="6bd14-135">GET tenant user activities</span></span> | [https://graph.microsoft.com/beta/auditLogs/directoryAudits](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=beta)
<span data-ttu-id="6bd14-136">获取租户用户登录信息</span><span class="sxs-lookup"><span data-stu-id="6bd14-136">GET tenant user sign-ins</span></span> | [https://graph.microsoft.com/beta/auditLogs/signIns](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=beta)
<span data-ttu-id="6bd14-137">获取预配日志</span><span class="sxs-lookup"><span data-stu-id="6bd14-137">GET provisioning logs</span></span> | [https://graph.microsoft.com/beta/auditLogs/directoryProvisioning](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryProvisioning&version=beta)

## <a name="what-licenses-do-i-need"></a><span data-ttu-id="6bd14-138">需要哪些许可证？</span><span class="sxs-lookup"><span data-stu-id="6bd14-138">What licenses do I need?</span></span>

<span data-ttu-id="6bd14-139">审核日志报告适用于已获得许可的功能。</span><span class="sxs-lookup"><span data-stu-id="6bd14-139">Audit log reports are available for features that you've licensed.</span></span>  <span data-ttu-id="6bd14-140">如果你拥有特定功能的许可证，则还可以访问其审核日志。</span><span class="sxs-lookup"><span data-stu-id="6bd14-140">If you have a license for a specific feature, you also have access to its audit logs.</span></span>

<span data-ttu-id="6bd14-141">例如，你需要 Azure AD Premium P1 许可证才能访问自助密码审核报告。</span><span class="sxs-lookup"><span data-stu-id="6bd14-141">For example, you need an Azure AD Premium P1 license to access self-service password audit reports.</span></span>  <span data-ttu-id="6bd14-142">若要了解详细信息，请参阅 [Azure AD 许可](https://azure.microsoft.com/pricing/details/active-directory/)。</span><span class="sxs-lookup"><span data-stu-id="6bd14-142">To learn more, see [Azure AD licensing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

<span data-ttu-id="6bd14-143">登录报告需要 Azure AD Premium 许可证。</span><span class="sxs-lookup"><span data-stu-id="6bd14-143">Sign-in reports require an Azure AD Premium license.</span></span>

<span data-ttu-id="6bd14-144">若要了解详细信息，请参阅 [Azure AD 定价](https://azure.microsoft.com/pricing/details/active-directory/)。</span><span class="sxs-lookup"><span data-stu-id="6bd14-144">To learn more, see [Azure AD pricing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

## <a name="next-steps"></a><span data-ttu-id="6bd14-145">后续步骤</span><span class="sxs-lookup"><span data-stu-id="6bd14-145">Next steps</span></span>

- <span data-ttu-id="6bd14-146">[注册你的应用程序](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)以满足审核日志先决条件。</span><span class="sxs-lookup"><span data-stu-id="6bd14-146">[Register your app](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to satisfy audit log prerequisites.</span></span> 
- <span data-ttu-id="6bd14-147">了解[审核日志](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples)和[登录示例](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples)。</span><span class="sxs-lookup"><span data-stu-id="6bd14-147">Learn from [audit log](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples) and [sign-in samples](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span></span>  
- <span data-ttu-id="6bd14-148">审查 [directoryAudit](directoryaudit.md) 资源和操作。</span><span class="sxs-lookup"><span data-stu-id="6bd14-148">Review [directoryAudit](directoryaudit.md) resource and actions.</span></span>
- <span data-ttu-id="6bd14-149">审查 [signIn](signin.md) 资源和操作。</span><span class="sxs-lookup"><span data-stu-id="6bd14-149">Review [signIn](signin.md) resource and actions.</span></span> 
- <span data-ttu-id="6bd14-150">审查 [provisioningObjectSummary](provisioningobjectsummary.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="6bd14-150">Review the [provisioningObjectSummary](provisioningobjectsummary.md) resource.</span></span>
