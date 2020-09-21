---
title: 在 Microsoft Graph 中使用 Microsoft 365 的使用情况报表
description: 通过 Microsoft Graph，可以访问 Microsoft 365 的使用情况报表资源，以获取企业用户的 Microsoft 365 服务使用情况。 例如，可以发现大量使用服务且即将达到配额的用户，也可以发现可能完全不需要 Microsoft 365 许可证的用户。
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 3213daeabebe655810736715c1c24bb34a20ff53
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47967308"
---
# <a name="working-with-microsoft-365-usage-reports-in-microsoft-graph"></a><span data-ttu-id="52c49-104">在 Microsoft Graph 中使用 Microsoft 365 的使用情况报表</span><span class="sxs-lookup"><span data-stu-id="52c49-104">Working with Microsoft 365 usage reports in Microsoft Graph</span></span>

<span data-ttu-id="52c49-105">通过 Microsoft Graph，可以访问 Microsoft 365 的使用情况报表资源，以获取企业用户的 Microsoft 365 服务使用情况。</span><span class="sxs-lookup"><span data-stu-id="52c49-105">With Microsoft Graph, you can access Microsoft 365 usage reports resources to get the information about how people in your business are using Microsoft 365 services.</span></span> <span data-ttu-id="52c49-106">例如，可以发现大量使用服务且即将达到配额的用户，也可以发现可能完全不需要 Microsoft 365 许可证的用户。</span><span class="sxs-lookup"><span data-stu-id="52c49-106">For example, you can identify who is using a service a lot and reaching quotas, or who may not need a Microsoft 365 license at all.</span></span>

## <a name="authorization"></a><span data-ttu-id="52c49-107">Authorization</span><span class="sxs-lookup"><span data-stu-id="52c49-107">Authorization</span></span>

<span data-ttu-id="52c49-108">Microsoft Graph 通过权限控制对资源的访问。</span><span class="sxs-lookup"><span data-stu-id="52c49-108">Microsoft Graph controls access to resources via permissions.</span></span> <span data-ttu-id="52c49-109">必须指定访问报表资源所需的权限。</span><span class="sxs-lookup"><span data-stu-id="52c49-109">You must specify the permissions you need in order to access Reports resources.</span></span> <span data-ttu-id="52c49-110">通常是在 Azure Active Directory (Azure AD) 门户中指定权限。</span><span class="sxs-lookup"><span data-stu-id="52c49-110">Typically, you specify permissions in the Azure Active Directory (Azure AD) portal.</span></span> <span data-ttu-id="52c49-111">有关详细信息，请参阅 [Microsoft Graph 权限参考](/graph/permissions-reference)和[报表权限](/graph/permissions-reference#reports-permissions)。</span><span class="sxs-lookup"><span data-stu-id="52c49-111">For more information, see [Microsoft Graph permissions reference](/graph/permissions-reference) and [Reports permissions](/graph/permissions-reference#reports-permissions).</span></span>

## <a name="whats-new"></a><span data-ttu-id="52c49-112">最近更新</span><span class="sxs-lookup"><span data-stu-id="52c49-112">What's new</span></span>
<span data-ttu-id="52c49-113">了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。</span><span class="sxs-lookup"><span data-stu-id="52c49-113">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>

## <a name="next-steps"></a><span data-ttu-id="52c49-114">后续步骤</span><span class="sxs-lookup"><span data-stu-id="52c49-114">Next steps</span></span>

<span data-ttu-id="52c49-115">借助报表资源和 API，可以通过新方式使用 Microsoft Graph 与用户进行交互，并管理他们的用户体验。</span><span class="sxs-lookup"><span data-stu-id="52c49-115">Reports resources and APIs can open up new ways for you to engage with users and manage their experiences with Microsoft Graph.</span></span> <span data-ttu-id="52c49-116">若要了解详细信息：</span><span class="sxs-lookup"><span data-stu-id="52c49-116">To learn more:</span></span>

- <span data-ttu-id="52c49-117">深入了解对方案最有帮助的资源的方法和属性。</span><span class="sxs-lookup"><span data-stu-id="52c49-117">Drill down on the methods and properties of the resources most helpful to your scenario.</span></span>
- <span data-ttu-id="52c49-118">尝试在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中调用 API。</span><span class="sxs-lookup"><span data-stu-id="52c49-118">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

<span data-ttu-id="52c49-p105">需要更多灵感？请参阅[我们的一些合作伙伴如何使用 Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners)。</span><span class="sxs-lookup"><span data-stu-id="52c49-p105">Need more ideas? See [how some of our partners are using Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).</span></span>

