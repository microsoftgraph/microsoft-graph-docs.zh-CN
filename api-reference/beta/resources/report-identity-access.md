---
title: 身份和访问权限报告 API 概述
description: 访问身份和访问权限报告，了解企业中的员工如何使用 Azure Active Directory 租户中的应用。
localization_priority: Priority
ms.prod: microsoft-identity-platform
author: besiler
doc_type: conceptualPageType
ms.openlocfilehash: 0414b0d8bd94ae5fe44f5913dea33c366377ec2d
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523729"
---
# <a name="identity-and-access-reports-api-overview"></a><span data-ttu-id="6996d-103">身份和访问权限报告 API 概述</span><span class="sxs-lookup"><span data-stu-id="6996d-103">Identity and access reports API overview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6996d-104">借助 Microsoft Graph，你可以通过访问身份和访问权限报告，获取有关企业中的员工如何使用 Azure Active Directory (AD) 租户中的应用的信息。</span><span class="sxs-lookup"><span data-stu-id="6996d-104">With Microsoft Graph, you can use access identity and access reports to get information about how people in your business are using applications in your Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="authorization"></a><span data-ttu-id="6996d-105">授权</span><span class="sxs-lookup"><span data-stu-id="6996d-105">Authorization</span></span>

<span data-ttu-id="6996d-106">Microsoft Graph 通过权限控制对资源的访问。</span><span class="sxs-lookup"><span data-stu-id="6996d-106">Microsoft Graph controls access to resources using permissions.</span></span> <span data-ttu-id="6996d-107">必须指定访问报告资源所需的权限。</span><span class="sxs-lookup"><span data-stu-id="6996d-107">You must specify the permissions you need in order to access reports resources.</span></span> <span data-ttu-id="6996d-108">有关详细信息，请参阅 [Microsoft Graph 权限参考](/graph/permissions-reference)和[报表权限](/graph/permissions-reference#reports-permissions)。</span><span class="sxs-lookup"><span data-stu-id="6996d-108">For more information, see [Microsoft Graph permissions reference](/graph/permissions-reference) and [Reports permissions](/graph/permissions-reference#reports-permissions).</span></span>

## <a name="what-are-identity-and-access-reports"></a><span data-ttu-id="6996d-109">什么是身份和访问权限报告？</span><span class="sxs-lookup"><span data-stu-id="6996d-109">What are identity and access reports?</span></span>

<span data-ttu-id="6996d-110">以下身份和访问权限报告可帮助你了解租户中的应用程序活动：</span><span class="sxs-lookup"><span data-stu-id="6996d-110">The following identity and access reports are available to help you understand application activity in your tenant:</span></span>

- <span data-ttu-id="6996d-111">AD FS 应用程序活动</span><span class="sxs-lookup"><span data-stu-id="6996d-111">AD FS application activity</span></span>
- <span data-ttu-id="6996d-112">应用程序登录</span><span class="sxs-lookup"><span data-stu-id="6996d-112">Application sign-in</span></span>
- <span data-ttu-id="6996d-113">注册和使用情况</span><span class="sxs-lookup"><span data-stu-id="6996d-113">Registration and usage</span></span>

### <a name="ad-fs-application-activity"></a><span data-ttu-id="6996d-114">AD FS 应用程序活动</span><span class="sxs-lookup"><span data-stu-id="6996d-114">AD FS application activity</span></span>

<span data-ttu-id="6996d-115">AD FS 应用程序活动报告可提供与使用 Active Directory 联合身份验证服务（以下简称“AD FS”）配置的依赖方相关的信息、其聚合的使用情况，以及是否可以将信赖方配置迁移到 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="6996d-115">The AD FS application activity report provides information about how a relying party is configured with Active Directory Federation Services (AD FS), its aggregated usage, and whether the relying party configuration can be migrated to Azure Active Directory.</span></span> <span data-ttu-id="6996d-116">有关详细信息，请参阅 [relyingPartyDetailedSummary](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta) 资源。</span><span class="sxs-lookup"><span data-stu-id="6996d-116">For more information, see the [relyingPartyDetailedSummary](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta) resource.</span></span>

### <a name="application-sign-in"></a><span data-ttu-id="6996d-117">应用程序登录</span><span class="sxs-lookup"><span data-stu-id="6996d-117">Application sign-in</span></span>

<span data-ttu-id="6996d-118">使用摘要报告或提供登录详细信息（例如，登录次数以及在登录过程中是否发生任何错误）的报告，评估应用程序登录使用情况。</span><span class="sxs-lookup"><span data-stu-id="6996d-118">Evaluate the usage of application sign-ins in your tenant using either a summary report or a report that provides details of sign-ins, such as the number of sign-ins and whether any errors occured during sign-in.</span></span> <span data-ttu-id="6996d-119">有关详细信息，请参阅 [applicationSignInSummary](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta) 资源。</span><span class="sxs-lookup"><span data-stu-id="6996d-119">For more information, see the [applicationSignInSummary](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta) resource.</span></span>

### <a name="registration-and-usage"></a><span data-ttu-id="6996d-120">注册和使用情况</span><span class="sxs-lookup"><span data-stu-id="6996d-120">Registration and usage</span></span>

<span data-ttu-id="6996d-121">更好地了解组织中的用户如何使用 Azure AD 功能，如自助密码重置和多重身份验证 (MFA)。</span><span class="sxs-lookup"><span data-stu-id="6996d-121">Get a better understanding of how users in your organization use Azure AD capabilities, such as self-service password rest and multi-factor authentication (MFA).</span></span> <span data-ttu-id="6996d-122">你可以确定对组织而言最有效的身份验证方法、最终用户遇到的错误类型，以及帮助最终用户接受使用自动密码重置和 MFA 所需要的市场活动。</span><span class="sxs-lookup"><span data-stu-id="6996d-122">You can determine which authentication methods are more successful for your organization, what types of errors end users are running into, and what campaign you need to run to help your end users adopt the use of self-service password rest and MFA.</span></span> <span data-ttu-id="6996d-123">有关详细信息，请参阅[身份验证方法使用情况 API](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta)。</span><span class="sxs-lookup"><span data-stu-id="6996d-123">For more information, see the [authentication methods usage report API](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta).</span></span>

## <a name="next-steps"></a><span data-ttu-id="6996d-124">后续步骤</span><span class="sxs-lookup"><span data-stu-id="6996d-124">Next steps</span></span>

<span data-ttu-id="6996d-125">借助报表资源和 API，可以通过新方式使用 Microsoft Graph 与用户进行交互，并管理他们的用户体验。</span><span class="sxs-lookup"><span data-stu-id="6996d-125">Reports resources and APIs can open up new ways for you to engage with users and manage their experiences with Microsoft Graph.</span></span> <span data-ttu-id="6996d-126">若要了解详细信息：</span><span class="sxs-lookup"><span data-stu-id="6996d-126">To learn more:</span></span>

- <span data-ttu-id="6996d-127">深入了解对方案最有帮助的资源的方法和属性。</span><span class="sxs-lookup"><span data-stu-id="6996d-127">Drill down on the methods and properties of the resources most helpful to your scenario.</span></span>
- <span data-ttu-id="6996d-128">在 [Graph 资源管理器](https://developer.microsoft.com/graph/graph-explorer)中试用 API。</span><span class="sxs-lookup"><span data-stu-id="6996d-128">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>


