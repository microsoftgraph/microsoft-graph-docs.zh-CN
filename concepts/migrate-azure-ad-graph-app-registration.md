---
title: 查看应用注册、权限和同意迁移问题
description: 介绍应用注册、权限和许可从 Azure Active Directory (Azure AD) Microsoft Graph API。
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: 1ba0ad7c7b0826dae7c5d971f7580784447ec708
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760698"
---
# <a name="review-app-registration-permissions-and-consent"></a><span data-ttu-id="cc7b7-103">查看应用注册、权限和许可</span><span class="sxs-lookup"><span data-stu-id="cc7b7-103">Review app registration, permissions, and consent</span></span>

<span data-ttu-id="cc7b7-104">本文是步骤 *3：查看应用程序迁移*[过程的详细信息的一部分](migrate-azure-ad-graph-planning-checklist.md)。</span><span class="sxs-lookup"><span data-stu-id="cc7b7-104">This article is part of *step 3: review app details* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="cc7b7-105">对于任何应用更新，有三个方面需要考虑：</span><span class="sxs-lookup"><span data-stu-id="cc7b7-105">For any app update, there are three areas to consider:</span></span>

- <span data-ttu-id="cc7b7-106">**应用注册**：可以在应用程序代码中继续使用现有 () `appId` 注册帐户。</span><span class="sxs-lookup"><span data-stu-id="cc7b7-106">**App registration**: You can continue to use your existing app registration (`appId`) in your application code.</span></span>  

    <span data-ttu-id="cc7b7-107">你 **不需要** 重新注册应用以迁移到 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="cc7b7-107">You do **not** have to re-register your app to migrate to Microsoft Graph.</span></span> <span data-ttu-id="cc7b7-108">只需更新代码，进行大量测试，然后部署更新。</span><span class="sxs-lookup"><span data-stu-id="cc7b7-108">Simply update the code, test heavily, and then deploy your update.</span></span>  

- <span data-ttu-id="cc7b7-109">**权限**：应该将配置的权限更改为等效的 Microsoft Graph 权限。</span><span class="sxs-lookup"><span data-stu-id="cc7b7-109">**Permissions**: You should change your configured permissions to the equivalent Microsoft Graph permissions.</span></span> <span data-ttu-id="cc7b7-110">为 Azure AD Graph 授予的委派权限也会隐式视为为 Microsoft Graph 授予。</span><span class="sxs-lookup"><span data-stu-id="cc7b7-110">Delegated permissions which were granted for Azure AD Graph will be implicitly considered granted for Microsoft Graph also.</span></span> <span data-ttu-id="cc7b7-111">需要再次 (应用程序) 应用程序角色的应用程序权限。</span><span class="sxs-lookup"><span data-stu-id="cc7b7-111">Application permissions (app roles) will need to be granted again.</span></span>

    <span data-ttu-id="cc7b7-112">如果你的更新还表明使用了对 Azure AD Graph 不可用的特性或功能，你可能需要请求获取这些新功能的权限。</span><span class="sxs-lookup"><span data-stu-id="cc7b7-112">If your update also incudes the use of features or capabilities that aren't available to Azure AD Graph, you'll likely need to request permissions for these new features.</span></span> <span data-ttu-id="cc7b7-113">如果是这样，你可以将应用切换为使用 MSAL 和 v2 终结点，并动态请求其他/增量同意。</span><span class="sxs-lookup"><span data-stu-id="cc7b7-113">If that's the case, you can switch your app to use MSAL and the v2 endpoint, and request additional/incremental consent dynamically.</span></span> <span data-ttu-id="cc7b7-114">查看应用身份验证库更改，查找有关切换到 MSAL [的更多详细信息](./migrate-azure-ad-graph-authentication-library.md)。</span><span class="sxs-lookup"><span data-stu-id="cc7b7-114">Find more details about switching to MSAL in [review app authentication library changes](./migrate-azure-ad-graph-authentication-library.md).</span></span>

- <span data-ttu-id="cc7b7-115">**同意**：已授予委派权限 (或已由管理员) 授予同意的最终用户无需再次授予同意即可继续使用你的应用。</span><span class="sxs-lookup"><span data-stu-id="cc7b7-115">**Consent**: End-users who have already granted consent for delegated permissions (or for whom consent has already been granted by an admin) can continue using your app without being asked to grant consent again.</span></span>

    <span data-ttu-id="cc7b7-116">已同意你的应用访问其数据的用户可以在应用更新为使用 Microsoft Graph 后继续使用它，无需再次请求同意。</span><span class="sxs-lookup"><span data-stu-id="cc7b7-116">Users who have already granted consent to your app to access their data can continue to use your app after it's been updated to use Microsoft Graph, without being asked to consent again.</span></span> <span data-ttu-id="cc7b7-117">将提示新用户征得同意。</span><span class="sxs-lookup"><span data-stu-id="cc7b7-117">New users will be prompted for consent.</span></span>

<span data-ttu-id="cc7b7-118">简单迁移项目应不会在这些方面遇到任何问题。</span><span class="sxs-lookup"><span data-stu-id="cc7b7-118">Simple migration projects should experience no issues in these areas.</span></span>

<span data-ttu-id="cc7b7-119">但是，如果您使用新功能、服务或添加其他功能，您可能需要新的权限，并且可能需要最终用户同意。</span><span class="sxs-lookup"><span data-stu-id="cc7b7-119">However, if you use new features, services, or add additional capabilities, you may need new permissions and end-user consent may be required.</span></span>  <span data-ttu-id="cc7b7-120">在这种情况下，刷新令牌时将请求同意。</span><span class="sxs-lookup"><span data-stu-id="cc7b7-120">In such cases, consent is requested when tokens are refreshed.</span></span>

## <a name="next-steps"></a><span data-ttu-id="cc7b7-121">后续步骤</span><span class="sxs-lookup"><span data-stu-id="cc7b7-121">Next Steps</span></span>

- <span data-ttu-id="cc7b7-122">了解 [Azure](migrate-azure-ad-graph-authentication-library.md) AD Graph 和 Microsoft Graph 之间的身份验证库差异。</span><span class="sxs-lookup"><span data-stu-id="cc7b7-122">Learn [authentication library](migrate-azure-ad-graph-authentication-library.md) differences between Azure AD Graph and Microsoft Graph.</span></span>
- <span data-ttu-id="cc7b7-123">再次查看 [检查](migrate-azure-ad-graph-planning-checklist.md) 表。</span><span class="sxs-lookup"><span data-stu-id="cc7b7-123">Review the [checklist](migrate-azure-ad-graph-planning-checklist.md) again.</span></span>
