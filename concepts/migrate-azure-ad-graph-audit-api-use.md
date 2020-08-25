---
title: 检查 Azure AD Graph Api 应用程序使用情况
description: 介绍如何审核 Azure Active Directory (Azure AD) Api，以将应用程序迁移到 Microsoft Graph API。
author: dkershaw10
localization_priority: Normal
ms.prod: azure-active-directory
ms.openlocfilehash: 405c68d1e0f88af33caa7b5f4c083bd1acdec82d
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46872962"
---
# <a name="examine-azure-ad-graph-apis-app-usage"></a><span data-ttu-id="16e7b-103">检查 Azure AD Graph Api 应用程序使用情况</span><span class="sxs-lookup"><span data-stu-id="16e7b-103">Examine Azure AD Graph APIs app usage</span></span>

<span data-ttu-id="16e7b-104">这是 [迁移应用程序过程](migrate-azure-ad-graph-planning-checklist.md)的步骤2。</span><span class="sxs-lookup"><span data-stu-id="16e7b-104">This is step 2 of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="16e7b-105">在规划到 Microsoft Graph 的迁移时，请花时间查看现有应用程序，并对您当前使用的 Azure AD Graph Api 进行编目。</span><span class="sxs-lookup"><span data-stu-id="16e7b-105">While planning your migration to Microsoft Graph, take time to review your existing application and to catalog the Azure AD Graph APIs you're currently using.</span></span>

<span data-ttu-id="16e7b-106">将您的列表与已知的区别进行比较。</span><span class="sxs-lookup"><span data-stu-id="16e7b-106">Compare your list to the known differences.</span></span>  <span data-ttu-id="16e7b-107">这有助于确定迁移应用程序所需的特定更改。</span><span class="sxs-lookup"><span data-stu-id="16e7b-107">This helps identify specific changes you'll need to make to migrate your app.</span></span>  <span data-ttu-id="16e7b-108">其中包括使用编辑器的搜索和替换功能或更多可能需要更多分析的更复杂的更新轻松解析的简单更改。</span><span class="sxs-lookup"><span data-stu-id="16e7b-108">These include simple changes easily resolved using an editor's search-and-replace features or more complicated updates that might require more analysis.</span></span>

<span data-ttu-id="16e7b-109">Microsoft Graph 支持 Azure AD Graph 的许多相同特性和功能。</span><span class="sxs-lookup"><span data-stu-id="16e7b-109">Microsoft Graph supports many of the same features and capabilities of Azure AD graph.</span></span>  <span data-ttu-id="16e7b-110">有几个关键区别：</span><span class="sxs-lookup"><span data-stu-id="16e7b-110">There are a few key differences:</span></span>

- [<span data-ttu-id="16e7b-111">请求差异</span><span class="sxs-lookup"><span data-stu-id="16e7b-111">Request differences</span></span>](migrate-azure-ad-graph-request-differences.md)
- [<span data-ttu-id="16e7b-112">功能差异</span><span class="sxs-lookup"><span data-stu-id="16e7b-112">Feature differences</span></span>](migrate-azure-ad-graph-feature-differences.md)
- [<span data-ttu-id="16e7b-113">资源类型差异</span><span class="sxs-lookup"><span data-stu-id="16e7b-113">Resource type differences</span></span>](migrate-azure-ad-graph-resource-differences.md)
- [<span data-ttu-id="16e7b-114">属性差异</span><span class="sxs-lookup"><span data-stu-id="16e7b-114">Property differences</span></span>](migrate-azure-ad-graph-property-differences.md)
- [<span data-ttu-id="16e7b-115">方法差异</span><span class="sxs-lookup"><span data-stu-id="16e7b-115">Method differences</span></span>](migrate-azure-ad-graph-method-differences.md)

<span data-ttu-id="16e7b-116">您还需要验证您的应用程序所使用的功能所需的权限。</span><span class="sxs-lookup"><span data-stu-id="16e7b-116">You'll also want to verify the permissions required for the features your app is using.</span></span>  <span data-ttu-id="16e7b-117">在某些情况下，可以使用更精细的权限。</span><span class="sxs-lookup"><span data-stu-id="16e7b-117">In some cases, more granular permissions are available.</span></span>

<span data-ttu-id="16e7b-118">若要了解详细信息，请参阅[权限](permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="16e7b-118">To learn more, see [Permissions](permissions-reference.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="16e7b-119">后续步骤</span><span class="sxs-lookup"><span data-stu-id="16e7b-119">Next Steps</span></span>

- <span data-ttu-id="16e7b-120">了解 Azure AD Graph 与 Microsoft Graph 之间 [的应用注册、权限和同意差异](migrate-azure-ad-graph-app-registration.md) 。</span><span class="sxs-lookup"><span data-stu-id="16e7b-120">Learn about [app registration, permissions and consent differences](migrate-azure-ad-graph-app-registration.md) between Azure AD Graph and Microsoft Graph.</span></span>
- <span data-ttu-id="16e7b-121">再次查看 [检查表](migrate-azure-ad-graph-planning-checklist.md) 。</span><span class="sxs-lookup"><span data-stu-id="16e7b-121">Review the [checklist](migrate-azure-ad-graph-planning-checklist.md) again.</span></span>

