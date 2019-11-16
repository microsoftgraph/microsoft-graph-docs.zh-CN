---
title: Azure AD 和 Microsoft Graph 之间的方法差异
description: 介绍 Azure Active Directory （Azure AD） Graph API 和 Microsoft Graph API （REST）之间的方法差异。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 00649e4f55a8bfcfd5354d2a75793447e3686109
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/15/2019
ms.locfileid: "38656527"
---
# <a name="method-differences-between-azure-ad-and-microsoft-graph"></a><span data-ttu-id="2d70c-103">Azure AD 和 Microsoft Graph 之间的方法差异</span><span class="sxs-lookup"><span data-stu-id="2d70c-103">Method differences between Azure AD and Microsoft Graph</span></span>

<span data-ttu-id="2d70c-104">本文是*第1步：查看*[迁移应用程序](migrate-azure-ad-graph-planning-checklist.md)的 API 差异的过程的一部分。</span><span class="sxs-lookup"><span data-stu-id="2d70c-104">This article is part of *step 1: review API differences* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="2d70c-105">许多 Azure AD Graph 方法也已更改。</span><span class="sxs-lookup"><span data-stu-id="2d70c-105">A handful of Azure AD Graph methods have also changed.</span></span>  <span data-ttu-id="2d70c-106">如果**未**在此列表中显示方法，则该方法在 Microsoft Graph 的 v1.0[版本](/graph/api/overview?view=graph-rest-1.0)中可用，与 Azure AD Graph 中的名称完全相同。</span><span class="sxs-lookup"><span data-stu-id="2d70c-106">If a method is **not** shown in this list, it is already available in the [v1.0 version](/graph/api/overview?view=graph-rest-1.0) of Microsoft Graph, with exactly the same name as in Azure AD Graph.</span></span>

|<span data-ttu-id="2d70c-107">Azure AD Graph</span><span class="sxs-lookup"><span data-stu-id="2d70c-107">Azure AD Graph</span></span> <br><span data-ttu-id="2d70c-108">（v. 1.6）方法</span><span class="sxs-lookup"><span data-stu-id="2d70c-108">(v1.6) method</span></span> |<span data-ttu-id="2d70c-109">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2d70c-109">Microsoft Graph</span></span><br><span data-ttu-id="2d70c-110">（资源/方法）</span><span class="sxs-lookup"><span data-stu-id="2d70c-110">(resource/method)</span></span>|<span data-ttu-id="2d70c-111">备注</span><span class="sxs-lookup"><span data-stu-id="2d70c-111">Comments</span></span>|
|---|---|---|
| <span data-ttu-id="2d70c-112">getAvailableExtensionProperties</span><span class="sxs-lookup"><span data-stu-id="2d70c-112">getAvailableExtensionProperties</span></span> | <span data-ttu-id="2d70c-113">beta 版-_不可用_</span><span class="sxs-lookup"><span data-stu-id="2d70c-113">beta - _Not available_</span></span> <br> <span data-ttu-id="2d70c-114">v1.0-不可_用_</span><span class="sxs-lookup"><span data-stu-id="2d70c-114">v1.0 - _Not available_</span></span> |  |
| <span data-ttu-id="2d70c-115">getObjectsByObjectId</span><span class="sxs-lookup"><span data-stu-id="2d70c-115">getObjectsByObjectId</span></span> | <span data-ttu-id="2d70c-116">&nbsp;-beta&nbsp;目录/getByIds</span><span class="sxs-lookup"><span data-stu-id="2d70c-116">beta&nbsp;-&nbsp;directory/getByIds</span></span> <br> <span data-ttu-id="2d70c-117">v1.0-directory/getByIds</span><span class="sxs-lookup"><span data-stu-id="2d70c-117">v1.0 - directory/getByIds</span></span> | |
| <span data-ttu-id="2d70c-118">invalidateAllRefreshTokens</span><span class="sxs-lookup"><span data-stu-id="2d70c-118">invalidateAllRefreshTokens</span></span> | <span data-ttu-id="2d70c-119">beta-revokeSignInSessions</span><span class="sxs-lookup"><span data-stu-id="2d70c-119">beta - revokeSignInSessions</span></span> <br> <span data-ttu-id="2d70c-120">v1.0-revokeSignInSessions</span><span class="sxs-lookup"><span data-stu-id="2d70c-120">v1.0 - revokeSignInSessions</span></span> | |
| <span data-ttu-id="2d70c-121">isMemberOf</span><span class="sxs-lookup"><span data-stu-id="2d70c-121">isMemberOf</span></span> | <span data-ttu-id="2d70c-122">beta-_未计划_</span><span class="sxs-lookup"><span data-stu-id="2d70c-122">beta - _Not planned_</span></span> <br> <span data-ttu-id="2d70c-123">v1.0-_未计划_</span><span class="sxs-lookup"><span data-stu-id="2d70c-123">v1.0 - _Not planned_</span></span> | <span data-ttu-id="2d70c-124">请改用 checkMemberGroups。</span><span class="sxs-lookup"><span data-stu-id="2d70c-124">Use checkMemberGroups instead.</span></span> |
| <span data-ttu-id="2d70c-125">restore</span><span class="sxs-lookup"><span data-stu-id="2d70c-125">restore</span></span> | <span data-ttu-id="2d70c-126">&nbsp;-beta&nbsp;还原&nbsp;（应用程序&nbsp;、用户&nbsp;和&nbsp;组）</span><span class="sxs-lookup"><span data-stu-id="2d70c-126">beta&nbsp;-&nbsp;restore&nbsp;(applications,&nbsp;users,&nbsp;and&nbsp;groups)</span></span><br> <span data-ttu-id="2d70c-127">&nbsp;-1.0&nbsp;版还原&nbsp;（用户&nbsp;和&nbsp;组）</span><span class="sxs-lookup"><span data-stu-id="2d70c-127">v1.0&nbsp;-&nbsp;restore&nbsp;(users&nbsp;and&nbsp;groups)</span></span> | <span data-ttu-id="2d70c-128">您还可以查看已删除的应用程序、用户和组，并永久删除它们。</span><span class="sxs-lookup"><span data-stu-id="2d70c-128">You can also view deleted applications, users, and groups and permanently delete them.</span></span> |

## <a name="next-steps"></a><span data-ttu-id="2d70c-129">后续步骤</span><span class="sxs-lookup"><span data-stu-id="2d70c-129">Next Steps</span></span>

- <span data-ttu-id="2d70c-130">了解如何在 Azure AD Graph 和 Microsoft Graph 之间检查您的应用程序中的[API 差异](migrate-azure-ad-graph-audit-api-use.md)。</span><span class="sxs-lookup"><span data-stu-id="2d70c-130">Learn how to [examine API differences](migrate-azure-ad-graph-audit-api-use.md) in your app between Azure AD Graph and Microsoft graph.</span></span>
- <span data-ttu-id="2d70c-131">浏览[Microsoft Graph](/graph/overview)概念和实践。</span><span class="sxs-lookup"><span data-stu-id="2d70c-131">Explore [Microsoft Graph](/graph/overview) concepts and practices.</span></span>
- <span data-ttu-id="2d70c-132">使用[Graph 浏览器](https://aka.ms/ge)试用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="2d70c-132">Use [Graph Explorer](https://aka.ms/ge) to experiment with Microsoft Graph.</span></span>
