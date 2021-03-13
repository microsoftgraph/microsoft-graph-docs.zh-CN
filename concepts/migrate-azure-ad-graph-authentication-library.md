---
title: 查看应用身份验证库更改
description: 介绍如何更新身份验证库使用，以将应用从 Azure Active Directory (Azure AD) API 迁移到 Microsoft Graph API。
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: ef49c6a3448dd63a7c933bb40748f218d6fd2db0
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760684"
---
# <a name="review-app-authentication-library-changes"></a><span data-ttu-id="17bef-103">查看应用身份验证库更改</span><span class="sxs-lookup"><span data-stu-id="17bef-103">Review app authentication library changes</span></span>

<span data-ttu-id="17bef-104">本文是步骤 *3：查看应用程序迁移*[过程的详细信息的一部分](migrate-azure-ad-graph-planning-checklist.md)。</span><span class="sxs-lookup"><span data-stu-id="17bef-104">This article is part of *step 3: review app details* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="17bef-105">大多数应用使用身份验证库获取和管理访问令牌以调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="17bef-105">Most apps use an authentication library to acquire and manage access tokens to call Microsoft Graph.</span></span>  <span data-ttu-id="17bef-106">Microsoft 提供两个身份验证库：</span><span class="sxs-lookup"><span data-stu-id="17bef-106">Microsoft offers two authentication libraries:</span></span>

- <span data-ttu-id="17bef-107">[Azure Active Directory 身份验证库 (](/azure/active-directory/develop/active-directory-authentication-libraries) ADAL) </span><span class="sxs-lookup"><span data-stu-id="17bef-107">[Azure Active Directory authentication library](/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL)</span></span>
- <span data-ttu-id="17bef-108">[MICROSOFT 身份验证库](/azure/active-directory/develop/reference-v2-libraries) (MSAL) </span><span class="sxs-lookup"><span data-stu-id="17bef-108">[Microsoft authentication library](/azure/active-directory/develop/reference-v2-libraries) (MSAL)</span></span>

## <a name="updating-adal"></a><span data-ttu-id="17bef-109">更新 ADAL</span><span class="sxs-lookup"><span data-stu-id="17bef-109">Updating ADAL</span></span>

<span data-ttu-id="17bef-110">如果你的应用当前使用 ADAL，请使用两阶段迁移方法：</span><span class="sxs-lookup"><span data-stu-id="17bef-110">If your app currently uses ADAL, use a two-stage migration approach:</span></span>

1. <span data-ttu-id="17bef-111">更新应用以获取 Microsoft Graph 的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="17bef-111">Update your app to acquire access tokens for Microsoft Graph.</span></span> <span data-ttu-id="17bef-112">继续使用 ADAL 执行此步骤。</span><span class="sxs-lookup"><span data-stu-id="17bef-112">Continue to use ADAL for this step.</span></span> <span data-ttu-id="17bef-113">更新 **resourceURL**，其中保存了表示资源 Web API 的 URI，网址为：</span><span class="sxs-lookup"><span data-stu-id="17bef-113">Update the **resourceURL**, which holds the URI representing the resource web API, from:</span></span>

    `https://graph.windows.net`  

    <span data-ttu-id="17bef-114">自：</span><span class="sxs-lookup"><span data-stu-id="17bef-114">To:</span></span>  

    `https://graph.microsoft.com`

    <span data-ttu-id="17bef-115">在此更改后，新获取的令牌具有相同的作用域，但访问令牌的访问群体现在为 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="17bef-115">Newly acquired tokens have the same scopes after this change, but the audience of the access tokens is now Microsoft Graph.</span></span>  

    <span data-ttu-id="17bef-116">更新 **resourceURL** 和验证功能后，发布临时更新，让用户启动并运行。</span><span class="sxs-lookup"><span data-stu-id="17bef-116">Once you've updated **resourceURL** and verified functionality, release an interim update to get your users up and runnning.</span></span>

1.  <span data-ttu-id="17bef-117">接下来，开始迁移应用以使用 MSAL，这是一个受支持的库，可继续操作，现已弃用 ADAL。</span><span class="sxs-lookup"><span data-stu-id="17bef-117">Next, begin work migrating your app to use MSAL, which is the supported library to use moving forward, now that ADAL is deprecated.</span></span>

## <a name="migrating-to-msal"></a><span data-ttu-id="17bef-118">迁移到 MSAL</span><span class="sxs-lookup"><span data-stu-id="17bef-118">Migrating to MSAL</span></span>

<span data-ttu-id="17bef-119">与 ADAL 相比，MSAL 提供了多个优势，包括增量同意、更丰富的单一登录体验、个人 Microsoft 帐户支持、使用基于标准的协议等。</span><span class="sxs-lookup"><span data-stu-id="17bef-119">MSAL provides multiple benefits over ADAL, including incremental consent, richer single sign-on experiences, support for personal Microsoft accounts, use of standards-based protocols and so on.</span></span>  

<span data-ttu-id="17bef-120">在将应用切换到 MSAL 时，你需要进行一些更改，包括在令牌获取请求中设置 **scopes** 参数：</span><span class="sxs-lookup"><span data-stu-id="17bef-120">When you switch your app over to MSAL, you'll need to make a few changes, including setting the **scopes** parameter in the token acquisition request:</span></span>

``` csharp
var scopes = new string[] { "https://graph.microsoft.com/.default" };
```

<span data-ttu-id="17bef-121">上述表达式将权限范围请求限定为在 Azure 门户中注册应用程序期间配置的权限范围请求，并节省现有用户再次同意应用的权限范围。</span><span class="sxs-lookup"><span data-stu-id="17bef-121">The expression above limits the permission scopes request to those configured during application registration in the Azure Portal, and saves your existing users from having to consent to your app again.</span></span>

<span data-ttu-id="17bef-122">有关 [此过程的直接和广泛](https://aka.ms/adal-net-to-msal-net) 帮助，包括常见错误的疑难解答和帮助，请参阅将 ADAL 迁移到 MSAL。</span><span class="sxs-lookup"><span data-stu-id="17bef-122">See [Migrating ADAL to MSAL](https://aka.ms/adal-net-to-msal-net) for direct and extensive help with the process, including troubleshooting and help with common errors.</span></span>

<span data-ttu-id="17bef-123">迁移到 MSAL 后，可以动态请求其他范围，并且用户下次使用你的应用时将提示他们提供增量同意。</span><span class="sxs-lookup"><span data-stu-id="17bef-123">Once you've migrated to MSAL, you can request additional scopes dynamically, and users are prompted to provide incremental consent the next time they use your app.</span></span>

## <a name="next-steps"></a><span data-ttu-id="17bef-124">后续步骤</span><span class="sxs-lookup"><span data-stu-id="17bef-124">Next Steps</span></span>

- <span data-ttu-id="17bef-125">了解 Azure AD Graph 和 Microsoft Graph 之间的 [.NET](migrate-azure-ad-graph-client-libraries.md) 客户端库差异。</span><span class="sxs-lookup"><span data-stu-id="17bef-125">Learn [.NET client library](migrate-azure-ad-graph-client-libraries.md) differences between Azure AD Graph and Microsoft Graph.</span></span>
- <span data-ttu-id="17bef-126">再次查看 [检查](migrate-azure-ad-graph-planning-checklist.md) 表。</span><span class="sxs-lookup"><span data-stu-id="17bef-126">Review the [checklist](migrate-azure-ad-graph-planning-checklist.md) again.</span></span>