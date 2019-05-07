---
title: 查看应用程序身份验证库更改
description: 介绍如何更新身份验证库使用, 以便将应用从 Azure Active Directory (Azure AD) API 应用迁移到 Microsoft Graph API。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 77604945064565f1387553b22a26a0fa871c998d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630263"
---
# <a name="review-app-authentication-library-changes"></a><span data-ttu-id="561fa-103">查看应用程序身份验证库更改</span><span class="sxs-lookup"><span data-stu-id="561fa-103">Review app authentication library changes</span></span>

<span data-ttu-id="561fa-104">本文是*第3步: 查看迁移应用程序的应用程序详细信息的第3步: 查看*该[过程](migrate-azure-ad-graph-planning-checklist.md)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="561fa-104">This article is part of *step 3: review app details* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="561fa-105">大多数应用使用身份验证库来 aquire 和管理访问令牌以调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="561fa-105">Most apps use an authentication library to aquire and manage access tokens to call Microsoft Graph.</span></span>  <span data-ttu-id="561fa-106">Microsoft 提供了两个身份验证库:</span><span class="sxs-lookup"><span data-stu-id="561fa-106">Microsoft offers two authentication libraries:</span></span>

- <span data-ttu-id="561fa-107">[Azure Active Directory 身份验证库](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries)ADAL</span><span class="sxs-lookup"><span data-stu-id="561fa-107">[Azure Active Directory authentication library](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL)</span></span>
- <span data-ttu-id="561fa-108">[Microsoft 身份验证库](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries)MSAL</span><span class="sxs-lookup"><span data-stu-id="561fa-108">[Microsoft authentication library](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) (MSAL)</span></span>

## <a name="updating-adal"></a><span data-ttu-id="561fa-109">更新 ADAL</span><span class="sxs-lookup"><span data-stu-id="561fa-109">Updating ADAL</span></span>

<span data-ttu-id="561fa-110">如果你的应用当前使用 ADAL, 请使用两阶段迁移方法:</span><span class="sxs-lookup"><span data-stu-id="561fa-110">If your app currently uses ADAL, use a two-stage migration approach:</span></span>

1. <span data-ttu-id="561fa-111">更新您的应用程序以获取 Microsoft Graph 的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="561fa-111">Update your app to acquire access tokens for Microsoft Graph.</span></span> <span data-ttu-id="561fa-112">继续使用 ADAL 执行此步骤。</span><span class="sxs-lookup"><span data-stu-id="561fa-112">Continue to use ADAL for this step.</span></span> <span data-ttu-id="561fa-113">更新**resourceURL**, 其中包含表示资源 web API 的 URI, 从:</span><span class="sxs-lookup"><span data-stu-id="561fa-113">Update the **resourceURL**, which holds the URI representing the resource web API, from:</span></span>

    `https://graph.windows.net`  

    <span data-ttu-id="561fa-114">自：</span><span class="sxs-lookup"><span data-stu-id="561fa-114">To:</span></span>  

    `https://graph.microsoft.com`

    <span data-ttu-id="561fa-115">在此更改之后, 新获取的令牌具有相同的作用域, 但访问令牌的访问群体现在是 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="561fa-115">Newly acquired tokens have the same scopes after this change, but the audience of the access tokens is now Microsoft Graph.</span></span>  

    <span data-ttu-id="561fa-116">更新**resourceURL**和已验证的功能后, 发布临时更新以获取用户的 up 和 runnning。</span><span class="sxs-lookup"><span data-stu-id="561fa-116">Once you've updated **resourceURL** and verified functionality, release an interim update to get your users up and runnning.</span></span>

1.  <span data-ttu-id="561fa-117">接下来, 开始将应用程序迁移到使用 MSAL, 这是受支持的库, 以供将来使用。</span><span class="sxs-lookup"><span data-stu-id="561fa-117">Next, begin work migrating your app to use MSAL, which is the supported library to use moving forward.</span></span>

## <a name="migrating-to-msal"></a><span data-ttu-id="561fa-118">迁移到 MSAL</span><span class="sxs-lookup"><span data-stu-id="561fa-118">Migrating to MSAL</span></span>

<span data-ttu-id="561fa-119">MSAL 提供了多个优于 ADAL 的优势, 包括增量许可、更丰富的单一登录体验、对个人 Microsoft 帐户的支持、使用基于标准的协议等。</span><span class="sxs-lookup"><span data-stu-id="561fa-119">MSAL provides multiple benefits over ADAL, including incremental consent, richer single sign-on experiences, support for personal Microsoft accounts, use of standards-based protocols and so on.</span></span>  

<span data-ttu-id="561fa-120">当您将应用程序切换到 MSAL 时, 您需要进行一些更改, 包括在令牌 acquistion 请求中设置**scope**参数:</span><span class="sxs-lookup"><span data-stu-id="561fa-120">When you switch your app over to MSAL, you'll need to make a few changes, including setting the **scopes** parameter in the token acquistion request:</span></span>

``` csharp
var scopes = new string[] { "https://graph.microsoft.com/.default" };
```

<span data-ttu-id="561fa-121">上面的表达式将权限范围请求限制为在 Azure 门户中的应用程序注册过程中配置的请求, 并将现有用户保存为不得不再次同意您的应用程序。</span><span class="sxs-lookup"><span data-stu-id="561fa-121">The expression above limits the permission scopes request to those configured during application registration in the Azure Portal, and saves your existing users from having to consent to your app again.</span></span>

<span data-ttu-id="561fa-122">请参阅[将 ADAL 迁移到 MSAL](https://aka.ms/adal-net-to-msal-net) , 以在过程中提供直接和广泛的帮助, 包括故障排除和帮助常见错误。</span><span class="sxs-lookup"><span data-stu-id="561fa-122">See [Migrating ADAL to MSAL](https://aka.ms/adal-net-to-msal-net) for direct and extensive help with the process, including troubleshooting and help with common errors.</span></span>

<span data-ttu-id="561fa-123">迁移到 MSAL 后, 您可以动态请求其他作用域, 并且在下次使用您的应用程序时, 系统会提示用户提供增量许可。</span><span class="sxs-lookup"><span data-stu-id="561fa-123">Once you've migrated to MSAL, you can request additional scopes dynamically, and users are prompted to provide incremental consent the next time they use your app.</span></span>

## <a name="next-steps"></a><span data-ttu-id="561fa-124">后续步骤</span><span class="sxs-lookup"><span data-stu-id="561fa-124">Next Steps</span></span>

- <span data-ttu-id="561fa-125">了解 Azure AD Graph 和 Microsoft Graph 之间的[.net 客户端库](migrate-azure-ad-graph-client-libraries.md)差异。</span><span class="sxs-lookup"><span data-stu-id="561fa-125">Learn [.NET client library](migrate-azure-ad-graph-client-libraries.md) differences between Azure AD Graph and Microsoft Graph.</span></span>
- <span data-ttu-id="561fa-126">探索[如何将 ADAL 迁移到 MSAL](https://aka.ms/adal-net-to-msal-net) , 以获取有关迁移到 MSAL 的更深入的帮助。</span><span class="sxs-lookup"><span data-stu-id="561fa-126">Explore [Migrating ADAL to MSAL](https://aka.ms/adal-net-to-msal-net) for more in-depth help on migrating to MSAL.</span></span>
- <span data-ttu-id="561fa-127">浏览[Microsoft Graph](/graph/overview)概念和实践。</span><span class="sxs-lookup"><span data-stu-id="561fa-127">Explore [Microsoft Graph](/graph/overview) concepts and practices.</span></span>
- <span data-ttu-id="561fa-128">使用[Graph 浏览器](https://aka.ms/ge)试用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="561fa-128">Use [Graph Explorer](https://aka.ms/ge) to experiment with Microsoft Graph.</span></span>
