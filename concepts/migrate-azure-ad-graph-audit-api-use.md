---
title: 检查 Azure AD Graph API 应用使用情况
description: 介绍如何审核 Azure Active Directory (Azure AD) API 以将应用迁移到 Microsoft Graph API。
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: e7e21f03cdfd8ce3d45f0201d15ec489c7322530
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760691"
---
# <a name="examine-azure-ad-graph-apis-app-usage"></a><span data-ttu-id="123c2-103">检查 Azure AD Graph API 应用使用情况</span><span class="sxs-lookup"><span data-stu-id="123c2-103">Examine Azure AD Graph APIs app usage</span></span>

<span data-ttu-id="123c2-104">这是迁移应用 [过程的第](migrate-azure-ad-graph-planning-checklist.md)2 步。</span><span class="sxs-lookup"><span data-stu-id="123c2-104">This is step 2 of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="123c2-105">在计划迁移到 Microsoft Graph 时，请花时间查看现有应用程序并编录你当前使用的 Azure AD Graph API。</span><span class="sxs-lookup"><span data-stu-id="123c2-105">While planning your migration to Microsoft Graph, take time to review your existing application and to catalog the Azure AD Graph APIs you're currently using.</span></span>

<span data-ttu-id="123c2-106">将列表与已知差异进行比较。</span><span class="sxs-lookup"><span data-stu-id="123c2-106">Compare your list to the known differences.</span></span>  <span data-ttu-id="123c2-107">这有助于确定迁移应用所需的特定更改。</span><span class="sxs-lookup"><span data-stu-id="123c2-107">This helps identify specific changes you'll need to make to migrate your app.</span></span>  <span data-ttu-id="123c2-108">其中包括使用编辑器的搜索和替换功能轻松解决的简单更改，或者可能需要更多分析的更复杂的更新。</span><span class="sxs-lookup"><span data-stu-id="123c2-108">These include simple changes easily resolved using an editor's search-and-replace features or more complicated updates that might require more analysis.</span></span>

<span data-ttu-id="123c2-109">Microsoft Graph 支持 Azure AD 图形的许多相同特性和功能。</span><span class="sxs-lookup"><span data-stu-id="123c2-109">Microsoft Graph supports many of the same features and capabilities of Azure AD graph.</span></span>  <span data-ttu-id="123c2-110">有一些关键区别：</span><span class="sxs-lookup"><span data-stu-id="123c2-110">There are a few key differences:</span></span>

- [<span data-ttu-id="123c2-111">请求差异</span><span class="sxs-lookup"><span data-stu-id="123c2-111">Request differences</span></span>](migrate-azure-ad-graph-request-differences.md)
- [<span data-ttu-id="123c2-112">功能差异</span><span class="sxs-lookup"><span data-stu-id="123c2-112">Feature differences</span></span>](migrate-azure-ad-graph-feature-differences.md)
- [<span data-ttu-id="123c2-113">资源类型差异</span><span class="sxs-lookup"><span data-stu-id="123c2-113">Resource type differences</span></span>](migrate-azure-ad-graph-resource-differences.md)
- [<span data-ttu-id="123c2-114">属性差异</span><span class="sxs-lookup"><span data-stu-id="123c2-114">Property differences</span></span>](migrate-azure-ad-graph-property-differences.md)
- [<span data-ttu-id="123c2-115">方法差异</span><span class="sxs-lookup"><span data-stu-id="123c2-115">Method differences</span></span>](migrate-azure-ad-graph-method-differences.md)

<span data-ttu-id="123c2-116">你还希望验证应用使用的功能所需的权限。</span><span class="sxs-lookup"><span data-stu-id="123c2-116">You'll also want to verify the permissions required for the features your app is using.</span></span>  <span data-ttu-id="123c2-117">在某些情况下，可以使用更精细的权限。</span><span class="sxs-lookup"><span data-stu-id="123c2-117">In some cases, more granular permissions are available.</span></span>

<span data-ttu-id="123c2-118">若要了解详细信息，请参阅[权限](permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="123c2-118">To learn more, see [Permissions](permissions-reference.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="123c2-119">后续步骤</span><span class="sxs-lookup"><span data-stu-id="123c2-119">Next Steps</span></span>

- <span data-ttu-id="123c2-120">了解 [Azure](migrate-azure-ad-graph-app-registration.md) AD Graph 和 Microsoft Graph 之间的应用注册、权限和许可差异。</span><span class="sxs-lookup"><span data-stu-id="123c2-120">Learn about [app registration, permissions and consent differences](migrate-azure-ad-graph-app-registration.md) between Azure AD Graph and Microsoft Graph.</span></span>
- <span data-ttu-id="123c2-121">再次查看 [检查](migrate-azure-ad-graph-planning-checklist.md) 表。</span><span class="sxs-lookup"><span data-stu-id="123c2-121">Review the [checklist](migrate-azure-ad-graph-planning-checklist.md) again.</span></span>

