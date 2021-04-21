---
title: 组的访问评审 API 概述
description: 组的访问评审 API 允许你以编程方式查看对组的访问权限
author: FaithOmbongi
localization_priority: Normal
ms.prod: governance
ms.openlocfilehash: a009ac515024cbd04159138434e5408536671aaf
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51922049"
---
# <a name="overview-of-the-access-reviews-api-for-groups"></a><span data-ttu-id="abd1c-103">组的访问评审 API 概述</span><span class="sxs-lookup"><span data-stu-id="abd1c-103">Overview of the access reviews API for groups</span></span>

<span data-ttu-id="abd1c-104">Microsoft Graph [中的组的访问](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) 评审 API 允许你以编程方式查看对组的访问权限。</span><span class="sxs-lookup"><span data-stu-id="abd1c-104">The [access reviews API for groups](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) in Microsoft Graph allows you to programmatically review access to your groups.</span></span> <span data-ttu-id="abd1c-105">这包括：</span><span class="sxs-lookup"><span data-stu-id="abd1c-105">This includes:</span></span>
+ <span data-ttu-id="abd1c-106">创建、读取、更新和删除访问评审、访问评审设置和计划。</span><span class="sxs-lookup"><span data-stu-id="abd1c-106">Creating, reading, updating, and deleting access reviews, access review settings, and schedules.</span></span>
+ <span data-ttu-id="abd1c-107">调查过去的访问评审和审阅者做出的决策，包括 Azure AD 自动执行的步骤。</span><span class="sxs-lookup"><span data-stu-id="abd1c-107">Investigating past access reviews and the decisions taken by reviewers, including the steps Azure AD took automatically.</span></span>

## <a name="scope-of-use"></a><span data-ttu-id="abd1c-108">使用范围</span><span class="sxs-lookup"><span data-stu-id="abd1c-108">Scope of use</span></span>

<span data-ttu-id="abd1c-109">访问评审 API 既支持委托上下文又支持应用程序上下文。</span><span class="sxs-lookup"><span data-stu-id="abd1c-109">The access reviews APIs support both delegated and application contexts.</span></span> <span data-ttu-id="abd1c-110">在委派 (上下文中) ，应用程序代表用户调用访问评审 API。</span><span class="sxs-lookup"><span data-stu-id="abd1c-110">In a user (delegated) context, an application calls the access reviews API on behalf of a user.</span></span> <span data-ttu-id="abd1c-111">典型方案包括：</span><span class="sxs-lookup"><span data-stu-id="abd1c-111">Typical scenarios include:</span></span>
+ <span data-ttu-id="abd1c-112">使用脚本创建、读取或更新访问评审的管理员。</span><span class="sxs-lookup"><span data-stu-id="abd1c-112">An administrator using a script to create, read, or update an access review.</span></span>
+ <span data-ttu-id="abd1c-113">使用应用或脚本为自己拥有的资源创建访问评审的资源所有者。</span><span class="sxs-lookup"><span data-stu-id="abd1c-113">A resource owner using an app or a script to create an access review for a resource they own.</span></span>
+ <span data-ttu-id="abd1c-114">管理员会自动收集一个或多个访问评审的所有决策。</span><span class="sxs-lookup"><span data-stu-id="abd1c-114">An administrator automatically collecting all decisions for one or more access reviews.</span></span>
  
<span data-ttu-id="abd1c-115">若要在用户环境中授权 (委派) ，请参阅代表 [用户获取访问权限](/graph/auth-v2-user)。</span><span class="sxs-lookup"><span data-stu-id="abd1c-115">To authorize your app in a user (delegated) context, see [get access on behalf of a user](/graph/auth-v2-user).</span></span>

<span data-ttu-id="abd1c-116">在应用程序上下文中，应用程序在没有登录用户的情况下调用访问评审 API。</span><span class="sxs-lookup"><span data-stu-id="abd1c-116">In an application context, an application calls the access reviews API without a signed-in user present.</span></span> <span data-ttu-id="abd1c-117">典型方案是安排的后台脚本定期收集所有访问评审的决策。</span><span class="sxs-lookup"><span data-stu-id="abd1c-117">A typical scenario is a scheduled background script regularly collecting decisions for all access reviews.</span></span> <span data-ttu-id="abd1c-118">若要在此上下文中授权你的应用，请参阅 [在没有用户的情况下获取访问权限](/graph/auth-v2-service)。</span><span class="sxs-lookup"><span data-stu-id="abd1c-118">To authorize your app in this context, see [get access without a user](/graph/auth-v2-service).</span></span>

## <a name="building-blocks-of-an-access-review"></a><span data-ttu-id="abd1c-119">访问评审的构建基块</span><span class="sxs-lookup"><span data-stu-id="abd1c-119">Building blocks of an access review</span></span>

<span data-ttu-id="abd1c-120">访问评审按逻辑进行构建，并包含以下构建基块：</span><span class="sxs-lookup"><span data-stu-id="abd1c-120">Access reviews are structured logically and are comprised of these building blocks:</span></span>
+ <span data-ttu-id="abd1c-121">**访问评审计划定义** - 包含访问评审及其实例设置的逻辑蓝图。</span><span class="sxs-lookup"><span data-stu-id="abd1c-121">**Access reviews schedule definitions** -  The logical blueprint that contains the settings of an access review and its instances.</span></span>
+ <span data-ttu-id="abd1c-122">**访问评审实例** - 表示具有作用域、审阅者和状态的审阅活动。</span><span class="sxs-lookup"><span data-stu-id="abd1c-122">**Access review instance** - Represents a review activity that has a scope, reviewers, and a status.</span></span> <span data-ttu-id="abd1c-123">访问评审定义可以具有多个实例，就像定期审阅中一样。</span><span class="sxs-lookup"><span data-stu-id="abd1c-123">An access review definition may have multiple instances as is the case in recurring reviews.</span></span> <span data-ttu-id="abd1c-124">一次评审只有一个实例。</span><span class="sxs-lookup"><span data-stu-id="abd1c-124">One-off reviews have exactly one instance.</span></span>
+ <span data-ttu-id="abd1c-125">**记录用于审阅的决策项** - 表示审阅者对实例做出的决定，包括时间戳和决策理由。</span><span class="sxs-lookup"><span data-stu-id="abd1c-125">**Decision items recorded for a review** - Represent a decision a reviewer made on an instance, including the time stamp and justification for the decision.</span></span> <span data-ttu-id="abd1c-126">每个审阅实例具有与所审阅用户数一样多的决策。</span><span class="sxs-lookup"><span data-stu-id="abd1c-126">Each review instance has as many decisions as the number of users under review.</span></span> <span data-ttu-id="abd1c-127">如果没有做出任何决策，即审阅者尚未对审阅做出响应，则实例将没有决策对象。</span><span class="sxs-lookup"><span data-stu-id="abd1c-127">If there are no decisions taken, that is, reviewers haven’t responded to the review, there will be no decision objects for the instance.</span></span>

## <a name="next-steps"></a><span data-ttu-id="abd1c-128">后续步骤</span><span class="sxs-lookup"><span data-stu-id="abd1c-128">Next steps</span></span>

<span data-ttu-id="abd1c-129">请尝试以下教程来管理访问评审：</span><span class="sxs-lookup"><span data-stu-id="abd1c-129">Try out the following tutorials to manage access reviews:</span></span>

+ [<span data-ttu-id="abd1c-130">使用组的访问评审 API 查看对安全组的访问权限</span><span class="sxs-lookup"><span data-stu-id="abd1c-130">Use access reviews API for groups to review access to your security groups</span></span>](tutorial-accessreviews-securitygroup.md)
+ [<span data-ttu-id="abd1c-131">使用组的访问评审 API 查看对具有来宾用户的所有 Microsoft 365 组的访问权限</span><span class="sxs-lookup"><span data-stu-id="abd1c-131">Use access reviews API for groups to review access to all your Microsoft 365 groups with guest users</span></span>](tutorial-accessreviews-M365group.md)

## <a name="see-also"></a><span data-ttu-id="abd1c-132">另请参阅</span><span class="sxs-lookup"><span data-stu-id="abd1c-132">See also</span></span>

+ [<span data-ttu-id="abd1c-133">规划 Azure Active Directory 访问评审部署</span><span class="sxs-lookup"><span data-stu-id="abd1c-133">Planning Azure Active Directory Access Reviews deployment</span></span>](/azure/active-directory/governance/deploy-access-reviews)
+ [<span data-ttu-id="abd1c-134">创建对应用程序应用程序的组&评审</span><span class="sxs-lookup"><span data-stu-id="abd1c-134">Create an access review of groups & applications</span></span>](/azure/active-directory/governance/create-access-review)
+ [<span data-ttu-id="abd1c-135">代表用户获取访问权限</span><span class="sxs-lookup"><span data-stu-id="abd1c-135">Get access on behalf of a user</span></span>](/graph/auth-v2-user)
+ [<span data-ttu-id="abd1c-136">不代表用户获取访问权限</span><span class="sxs-lookup"><span data-stu-id="abd1c-136">Get access without a user</span></span>](/graph/auth-v2-service)
