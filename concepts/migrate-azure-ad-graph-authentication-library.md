---
title: 查看应用程序身份验证库更改
description: 介绍如何更新身份验证库使用，以便将应用从 Azure Active Directory (Azure AD) API 应用迁移到 Microsoft Graph API。
author: dkershaw10
localization_priority: Normal
ms.prod: azure-active-directory
ms.openlocfilehash: 35fc2b5c1ad1d7aebc790b93a31ba8d1924b8bc1
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2020
ms.locfileid: "48289020"
---
# <a name="review-app-authentication-library-changes"></a><span data-ttu-id="c9b55-103">查看应用程序身份验证库更改</span><span class="sxs-lookup"><span data-stu-id="c9b55-103">Review app authentication library changes</span></span>

<span data-ttu-id="c9b55-104">本文是 *第3步：查看迁移应用程序的应用程序详细信息的第3步：查看* 该 [过程](migrate-azure-ad-graph-planning-checklist.md)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="c9b55-104">This article is part of *step 3: review app details* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="c9b55-105">大多数应用使用身份验证库来获取和管理访问令牌，以调用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="c9b55-105">Most apps use an authentication library to acquire and manage access tokens to call Microsoft Graph.</span></span>  <span data-ttu-id="c9b55-106">Microsoft 提供了两个身份验证库：</span><span class="sxs-lookup"><span data-stu-id="c9b55-106">Microsoft offers two authentication libraries:</span></span>

- <span data-ttu-id="c9b55-107">[Azure Active Directory 身份验证库](/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL) </span><span class="sxs-lookup"><span data-stu-id="c9b55-107">[Azure Active Directory authentication library](/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL)</span></span>
- <span data-ttu-id="c9b55-108">[Microsoft 身份验证库](/azure/active-directory/develop/reference-v2-libraries) (MSAL) </span><span class="sxs-lookup"><span data-stu-id="c9b55-108">[Microsoft authentication library](/azure/active-directory/develop/reference-v2-libraries) (MSAL)</span></span>

## <a name="updating-adal"></a><span data-ttu-id="c9b55-109">更新 ADAL</span><span class="sxs-lookup"><span data-stu-id="c9b55-109">Updating ADAL</span></span>

<span data-ttu-id="c9b55-110">如果你的应用当前使用 ADAL，请使用两阶段迁移方法：</span><span class="sxs-lookup"><span data-stu-id="c9b55-110">If your app currently uses ADAL, use a two-stage migration approach:</span></span>

1. <span data-ttu-id="c9b55-111">更新您的应用程序以获取 Microsoft Graph 的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="c9b55-111">Update your app to acquire access tokens for Microsoft Graph.</span></span> <span data-ttu-id="c9b55-112">继续使用 ADAL 执行此步骤。</span><span class="sxs-lookup"><span data-stu-id="c9b55-112">Continue to use ADAL for this step.</span></span> <span data-ttu-id="c9b55-113">更新 **resourceURL**，其中包含表示资源 web API 的 URI，从：</span><span class="sxs-lookup"><span data-stu-id="c9b55-113">Update the **resourceURL**, which holds the URI representing the resource web API, from:</span></span>

    `https://graph.windows.net`  

    <span data-ttu-id="c9b55-114">自：</span><span class="sxs-lookup"><span data-stu-id="c9b55-114">To:</span></span>  

    `https://graph.microsoft.com`

    <span data-ttu-id="c9b55-115">在此更改之后，新获取的令牌具有相同的作用域，但访问令牌的访问群体现在是 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="c9b55-115">Newly acquired tokens have the same scopes after this change, but the audience of the access tokens is now Microsoft Graph.</span></span>  

    <span data-ttu-id="c9b55-116">更新 **resourceURL** 和已验证的功能后，发布临时更新以获取用户的 up 和 runnning。</span><span class="sxs-lookup"><span data-stu-id="c9b55-116">Once you've updated **resourceURL** and verified functionality, release an interim update to get your users up and runnning.</span></span>

1.  <span data-ttu-id="c9b55-117">接下来，开始将应用程序迁移到使用 MSAL （即，支持的库可供将来使用），现在将 ADAL 弃用。</span><span class="sxs-lookup"><span data-stu-id="c9b55-117">Next, begin work migrating your app to use MSAL, which is the supported library to use moving forward, now that ADAL is deprecated.</span></span>

## <a name="migrating-to-msal"></a><span data-ttu-id="c9b55-118">迁移到 MSAL</span><span class="sxs-lookup"><span data-stu-id="c9b55-118">Migrating to MSAL</span></span>

<span data-ttu-id="c9b55-119">MSAL 提供了多个优于 ADAL 的优势，包括增量许可、更丰富的单一登录体验、对个人 Microsoft 帐户的支持、使用基于标准的协议等。</span><span class="sxs-lookup"><span data-stu-id="c9b55-119">MSAL provides multiple benefits over ADAL, including incremental consent, richer single sign-on experiences, support for personal Microsoft accounts, use of standards-based protocols and so on.</span></span>  

<span data-ttu-id="c9b55-120">当您将应用程序切换到 MSAL 时，您需要进行一些更改，包括在令牌 acquistion 请求中设置 **scope** 参数：</span><span class="sxs-lookup"><span data-stu-id="c9b55-120">When you switch your app over to MSAL, you'll need to make a few changes, including setting the **scopes** parameter in the token acquistion request:</span></span>

``` csharp
var scopes = new string[] { "https://graph.microsoft.com/.default" };
```

<span data-ttu-id="c9b55-121">上面的表达式将权限范围请求限制为在 Azure 门户中的应用程序注册过程中配置的请求，并将现有用户保存为不得不再次同意您的应用程序。</span><span class="sxs-lookup"><span data-stu-id="c9b55-121">The expression above limits the permission scopes request to those configured during application registration in the Azure Portal, and saves your existing users from having to consent to your app again.</span></span>

<span data-ttu-id="c9b55-122">请参阅 [将 ADAL 迁移到 MSAL](https://aka.ms/adal-net-to-msal-net) ，以在过程中提供直接和广泛的帮助，包括故障排除和帮助常见错误。</span><span class="sxs-lookup"><span data-stu-id="c9b55-122">See [Migrating ADAL to MSAL](https://aka.ms/adal-net-to-msal-net) for direct and extensive help with the process, including troubleshooting and help with common errors.</span></span>

<span data-ttu-id="c9b55-123">迁移到 MSAL 后，您可以动态请求其他作用域，并且在下次使用您的应用程序时，系统会提示用户提供增量许可。</span><span class="sxs-lookup"><span data-stu-id="c9b55-123">Once you've migrated to MSAL, you can request additional scopes dynamically, and users are prompted to provide incremental consent the next time they use your app.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c9b55-124">后续步骤</span><span class="sxs-lookup"><span data-stu-id="c9b55-124">Next Steps</span></span>

- <span data-ttu-id="c9b55-125">了解 Azure AD Graph 和 Microsoft Graph 之间的 [.net 客户端库](migrate-azure-ad-graph-client-libraries.md) 差异。</span><span class="sxs-lookup"><span data-stu-id="c9b55-125">Learn [.NET client library](migrate-azure-ad-graph-client-libraries.md) differences between Azure AD Graph and Microsoft Graph.</span></span>
- <span data-ttu-id="c9b55-126">再次查看 [检查表](migrate-azure-ad-graph-planning-checklist.md) 。</span><span class="sxs-lookup"><span data-stu-id="c9b55-126">Review the [checklist](migrate-azure-ad-graph-planning-checklist.md) again.</span></span>