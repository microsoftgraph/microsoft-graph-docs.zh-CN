---
title: 查看应用注册、权限和同意迁移问题
description: 介绍从 Azure Active Directory (Azure AD) 到 Microsoft Graph API 的应用注册、权限和许可迁移。
author: dkershaw10
localization_priority: Normal
ms.prod: azure-active-directory
ms.openlocfilehash: f7508296ff7fc4e78f5d39f777390057d2570109
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46872969"
---
# <a name="review-app-registration-permissions-and-consent"></a><span data-ttu-id="52579-103">查看应用注册、权限和同意</span><span class="sxs-lookup"><span data-stu-id="52579-103">Review app registration, permissions, and consent</span></span>

<span data-ttu-id="52579-104">本文是 *第3步：查看迁移应用程序的应用程序详细信息的第3步：查看* 该 [过程](migrate-azure-ad-graph-planning-checklist.md)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="52579-104">This article is part of *step 3: review app details* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="52579-105">对于任何应用程序更新，有三个要考虑的方面：</span><span class="sxs-lookup"><span data-stu-id="52579-105">For any app update, there are three areas to consider:</span></span>

- <span data-ttu-id="52579-106">**应用注册**：您可以继续 `appId` 在应用程序代码中使用现有的应用注册 () 。</span><span class="sxs-lookup"><span data-stu-id="52579-106">**App registration**: You can continue to use your existing app registration (`appId`) in your application code.</span></span>  

    <span data-ttu-id="52579-107">您无 **需重新** 注册您的应用程序即可迁移到 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="52579-107">You do **not** have to re-register your app to migrate to Microsoft Graph.</span></span> <span data-ttu-id="52579-108">只需更新代码，对其进行大量测试，然后再部署更新。</span><span class="sxs-lookup"><span data-stu-id="52579-108">Simply update the code, test heavily, and then deploy your update.</span></span>  

- <span data-ttu-id="52579-109">**权限**：您可以继续为您的应用程序使用现有配置的权限。</span><span class="sxs-lookup"><span data-stu-id="52579-109">**Permissions**: You can continue to use the existing configured permissions for your app.</span></span> <span data-ttu-id="52579-110">您无需请求新的权限，因为 Azure AD Graph 权限与 Microsoft Graph 共享。</span><span class="sxs-lookup"><span data-stu-id="52579-110">You do not have to request new permissions because Azure AD Graph permissions are shared with Microsoft Graph.</span></span>

    <span data-ttu-id="52579-111">例如，如果现有的应用程序具有 _User. all_ 和 _Group。 read. all_ 权限，这些权限也被隐式授予为 Microsoft Graph 的更新的应用程序。</span><span class="sxs-lookup"><span data-stu-id="52579-111">For example, if your existing app has _User.Read.All_ and _Group.Read.All_ permissions, those permissions are implicitly granted to your updated app for Microsoft Graph as well.</span></span>

    <span data-ttu-id="52579-112">如果您的更新还 incudes 使用不适用于 Azure AD Graph 的功能或功能，则您可能需要请求这些新功能的权限。</span><span class="sxs-lookup"><span data-stu-id="52579-112">If your update also incudes the use of features or capabilities that aren't available to Azure AD Graph, you'll likely need to request permissions for these new features.</span></span> <span data-ttu-id="52579-113">如果是这种情况，您可以切换应用程序以使用 MSAL 和 v2 终结点，并动态请求其他/增量许可。</span><span class="sxs-lookup"><span data-stu-id="52579-113">If that's the case, you can switch your app to use MSAL and the v2 endpoint, and request additional/incremental consent dynamically.</span></span> <span data-ttu-id="52579-114">在 [审阅应用程序身份验证库更改](/graph/migrate-azure-ad-graph-authentication-library)中查找有关切换到 MSAL 的更多详细信息。</span><span class="sxs-lookup"><span data-stu-id="52579-114">Find more details about switching to MSAL in [review app authentication library changes](/graph/migrate-azure-ad-graph-authentication-library).</span></span>

- <span data-ttu-id="52579-115">**同意**：最终用户可以继续使用您的应用程序，而无需再次向您授予许可。</span><span class="sxs-lookup"><span data-stu-id="52579-115">**Consent**: End-users can continue using your app without being asked to grant consent again.</span></span>

    <span data-ttu-id="52579-116">已向你的应用程序授予访问其数据的同意的用户可以继续使用你的应用程序以使用 Microsoft Graph，而不要求再次同意。</span><span class="sxs-lookup"><span data-stu-id="52579-116">Users who have already granted consent to your app to access their data can continue to use your app after it's been updated to use Microsoft Graph, without being asked to consent again.</span></span>

<span data-ttu-id="52579-117">简单迁移项目在这些领域中不应遇到任何问题。</span><span class="sxs-lookup"><span data-stu-id="52579-117">Simple migration projects should experience no issues in these areas.</span></span>

<span data-ttu-id="52579-118">但是，如果您使用新的功能、服务或添加其他功能，则可能需要新权限，并且可能需要最终用户同意。</span><span class="sxs-lookup"><span data-stu-id="52579-118">However, if you use new features, services, or add additional capabilities, you may need new permissions and end-user consent may be required.</span></span>  <span data-ttu-id="52579-119">在这种情况下，会在刷新令牌时请求同意。</span><span class="sxs-lookup"><span data-stu-id="52579-119">In such cases, consent is requested when tokens are refreshed.</span></span>

## <a name="next-steps"></a><span data-ttu-id="52579-120">后续步骤</span><span class="sxs-lookup"><span data-stu-id="52579-120">Next Steps</span></span>

- <span data-ttu-id="52579-121">了解 Azure AD Graph 和 Microsoft Graph 之间的 [身份验证库](migrate-azure-ad-graph-authentication-library.md) 差异。</span><span class="sxs-lookup"><span data-stu-id="52579-121">Learn [authentication library](migrate-azure-ad-graph-authentication-library.md) differences between Azure AD Graph and Microsoft Graph.</span></span>
- <span data-ttu-id="52579-122">再次查看 [检查表](migrate-azure-ad-graph-planning-checklist.md) 。</span><span class="sxs-lookup"><span data-stu-id="52579-122">Review the [checklist](migrate-azure-ad-graph-planning-checklist.md) again.</span></span>
