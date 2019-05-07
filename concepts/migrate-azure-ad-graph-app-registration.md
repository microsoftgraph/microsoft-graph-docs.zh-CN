---
title: 查看应用注册、权限和同意迁移问题
description: 介绍从 Azure Active Directory (Azure AD) 到 Microsoft Graph API 的应用注册、权限和同意迁移。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 54e187fcf35f030413aa98a6cb0e34649532a8b4
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630277"
---
# <a name="review-app-registration-permissions-and-consent"></a><span data-ttu-id="8112b-103">查看应用注册、权限和同意</span><span class="sxs-lookup"><span data-stu-id="8112b-103">Review app registration, permissions, and consent</span></span>

<span data-ttu-id="8112b-104">本文是*第3步: 查看迁移应用程序的应用程序详细信息的第3步: 查看*该[过程](migrate-azure-ad-graph-planning-checklist.md)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="8112b-104">This article is part of *step 3: review app details* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="8112b-105">对于任何应用程序更新, 有三个要考虑的方面:</span><span class="sxs-lookup"><span data-stu-id="8112b-105">For any app update, there are three areas to consider:</span></span>

- <span data-ttu-id="8112b-106">**应用注册**: 您可以继续在应用程序代码中使用现有`appId`的应用注册 ()。</span><span class="sxs-lookup"><span data-stu-id="8112b-106">**App registration**: You can continue to use your existing app registration (`appId`) in your application code.</span></span>  

    <span data-ttu-id="8112b-107">您无\*\*\*\* 需重新注册您的应用程序即可迁移到 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="8112b-107">You do **not** have to re-register your app to migrate to Microsoft Graph.</span></span> <span data-ttu-id="8112b-108">只需更新代码, 对其进行大量测试, 然后再部署更新。</span><span class="sxs-lookup"><span data-stu-id="8112b-108">Simply update the code, test heavily, and then deploy your update.</span></span>  

- <span data-ttu-id="8112b-109">**权限**: 您可以继续为您的应用程序使用现有配置的权限。</span><span class="sxs-lookup"><span data-stu-id="8112b-109">**Permissions**: You can continue to use the existing configured permissions for your app.</span></span> <span data-ttu-id="8112b-110">您无需请求新的权限, 因为 Azure AD Graph 权限与 Microsoft Graph 共享。</span><span class="sxs-lookup"><span data-stu-id="8112b-110">You do not have to request new permissions because Azure AD Graph permissions are shared with Microsoft Graph.</span></span>

    <span data-ttu-id="8112b-111">例如, 如果现有的应用程序具有_User。 all_和_Group。 read。 all_权限, 这些权限也被隐式授予为 Microsoft Graph 的更新的应用程序。</span><span class="sxs-lookup"><span data-stu-id="8112b-111">For example, if your existing app has _User.Read.All_ and _Group.Read.All_ permissions, those permissions are implicitly granted to your updated app for Microsoft Graph as well.</span></span>

    <span data-ttu-id="8112b-112">如果您的更新还 incudes 使用不适用于 Azure AD Graph 的功能或功能, 则您可能需要请求这些新功能的权限。</span><span class="sxs-lookup"><span data-stu-id="8112b-112">If your update also incudes the use of features or capabilities that aren't available to Azure AD Graph, you'll likely need to request permissions for these new features.</span></span> <span data-ttu-id="8112b-113">如果是这种情况, 您可以切换应用程序以使用 MSAL 和 v2 终结点, 并动态请求其他/增量许可。</span><span class="sxs-lookup"><span data-stu-id="8112b-113">If that's the case, you can switch your app to use MSAL and the v2 endpoint, and request additional/incremental consent dynamically.</span></span> <span data-ttu-id="8112b-114">在[审阅应用程序身份验证库更改](/graph/migrate-azure-ad-graph-authentication-library)中查找有关切换到 MSAL 的更多详细信息。</span><span class="sxs-lookup"><span data-stu-id="8112b-114">Find more details about switching to MSAL in [review app authentication library changes](/graph/migrate-azure-ad-graph-authentication-library).</span></span>

- <span data-ttu-id="8112b-115">**同意**: 最终用户可以继续使用您的应用程序, 而无需再次向您授予许可。</span><span class="sxs-lookup"><span data-stu-id="8112b-115">**Consent**: End-users can continue using your app without being asked to grant consent again.</span></span>

    <span data-ttu-id="8112b-116">已向你的应用程序授予访问其数据的同意的用户可以继续使用你的应用程序以使用 Microsoft Graph, 而不要求再次同意。</span><span class="sxs-lookup"><span data-stu-id="8112b-116">Users who have already granted consent to your app to access their data can continue to use your app after it's been updated to use Microsoft Graph, without being asked to consent again.</span></span>

<span data-ttu-id="8112b-117">简单迁移项目在这些领域中不应遇到任何问题。</span><span class="sxs-lookup"><span data-stu-id="8112b-117">Simple migration projects should experience no issues in these areas.</span></span>

<span data-ttu-id="8112b-118">但是, 如果您使用新的功能、服务或添加其他功能, 则可能需要新权限, 并且可能需要最终用户同意。</span><span class="sxs-lookup"><span data-stu-id="8112b-118">However, if you use new features, services, or add additional capabilities, you may need new permissions and end-user consent may be required.</span></span>  <span data-ttu-id="8112b-119">在这种情况下, 会在刷新令牌时请求同意。</span><span class="sxs-lookup"><span data-stu-id="8112b-119">In such cases, consent is requested when tokens are refreshed.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8112b-120">后续步骤</span><span class="sxs-lookup"><span data-stu-id="8112b-120">Next Steps</span></span>

- <span data-ttu-id="8112b-121">了解 Azure AD Graph 和 Microsoft Graph 之间的[身份验证库](migrate-azure-ad-graph-authentication-library.md)差异。</span><span class="sxs-lookup"><span data-stu-id="8112b-121">Learn [authentication library](migrate-azure-ad-graph-authentication-library.md) differences between Azure AD Graph and Microsoft Graph.</span></span>
- <span data-ttu-id="8112b-122">浏览[Microsoft Graph](/graph/overview)概念和实践。</span><span class="sxs-lookup"><span data-stu-id="8112b-122">Explore [Microsoft Graph](/graph/overview) concepts and practices.</span></span>
- <span data-ttu-id="8112b-123">使用[Graph 浏览器](https://aka.ms/ge)试用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="8112b-123">Use [Graph Explorer](https://aka.ms/ge) to experiment with Microsoft Graph.</span></span>
