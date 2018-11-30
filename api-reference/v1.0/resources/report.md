---
title: 在 Microsoft Graph 中使用 Office 365 使用情况报表
description: 通过 Microsoft Graph，可以访问 Office 365 使用情况报表资源，了解企业用户的 Office 365 服务使用情况。 例如，可以发现大量使用服务且要达到配额的用户，也可以发现可能完全不需要 Office 365 许可证的用户。
ms.openlocfilehash: cc125f5b6ffd171014bca724c5a611c5454e8186
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011432"
---
# <a name="working-with-office-365-usage-reports-in-microsoft-graph"></a><span data-ttu-id="74d1e-104">在 Microsoft Graph 中使用 Office 365 使用情况报表</span><span class="sxs-lookup"><span data-stu-id="74d1e-104">Working with Office 365 usage reports in Microsoft Graph</span></span>

<span data-ttu-id="74d1e-105">通过 Microsoft Graph，可以访问 Office 365 使用情况报表资源，了解企业用户的 Office 365 服务使用情况。</span><span class="sxs-lookup"><span data-stu-id="74d1e-105">With Microsoft Graph, you can access Office 365 usage reports resources to get the information about how people in your business are using Office 365 services.</span></span> <span data-ttu-id="74d1e-106">例如，可以发现大量使用服务且要达到配额的用户，也可以发现可能完全不需要 Office 365 许可证的用户。</span><span class="sxs-lookup"><span data-stu-id="74d1e-106">For example, you can identify who is using a service a lot and reaching quotas, or who may not need an Office 365 license at all.</span></span>

## <a name="authorization"></a><span data-ttu-id="74d1e-107">授权</span><span class="sxs-lookup"><span data-stu-id="74d1e-107">Authorization</span></span>

<span data-ttu-id="74d1e-108">Microsoft Graph 通过权限控制对资源的访问。</span><span class="sxs-lookup"><span data-stu-id="74d1e-108">Microsoft Graph controls access to resources via permissions.</span></span> <span data-ttu-id="74d1e-109">必须指定访问报表资源所需的权限。</span><span class="sxs-lookup"><span data-stu-id="74d1e-109">You must specify the permissions you need in order to access Reports resources.</span></span> <span data-ttu-id="74d1e-110">通常是在 Azure Active Directory (Azure AD) 门户中指定权限。</span><span class="sxs-lookup"><span data-stu-id="74d1e-110">Typically, you specify permissions in the Azure Active Directory (Azure AD) portal.</span></span> <span data-ttu-id="74d1e-111">有关详细信息，请参阅 [Microsoft Graph 权限参考](/graph/permissions-reference)和[报表权限](/graph/permissions-reference#reports-permissions)。</span><span class="sxs-lookup"><span data-stu-id="74d1e-111">For more information, see [Microsoft Graph permissions reference](/graph/permissions-reference) and [Reports permissions](/graph/permissions-reference#reports-permissions).</span></span>

## <a name="next-steps"></a><span data-ttu-id="74d1e-112">后续步骤</span><span class="sxs-lookup"><span data-stu-id="74d1e-112">Next steps</span></span>

<span data-ttu-id="74d1e-113">借助报表资源和 API，可以通过新方式使用 Microsoft Graph 与用户进行交互，并管理他们的用户体验。</span><span class="sxs-lookup"><span data-stu-id="74d1e-113">Reports resources and APIs can open up new ways for you to engage with users and manage their experiences with Microsoft Graph.</span></span> <span data-ttu-id="74d1e-114">若要了解详细信息：</span><span class="sxs-lookup"><span data-stu-id="74d1e-114">To learn more:</span></span>

- <span data-ttu-id="74d1e-115">深入了解对方案最有帮助的资源的方法和属性。</span><span class="sxs-lookup"><span data-stu-id="74d1e-115">Drill down on the methods and properties of the resources most helpful to your scenario.</span></span>
- <span data-ttu-id="74d1e-116">尝试 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中的 API。</span><span class="sxs-lookup"><span data-stu-id="74d1e-116">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

<span data-ttu-id="74d1e-p105">需要更多灵感？请参阅[我们的一些合作伙伴如何使用 Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners)。</span><span class="sxs-lookup"><span data-stu-id="74d1e-p105">Need more ideas? See [how some of our partners are using Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).</span></span>