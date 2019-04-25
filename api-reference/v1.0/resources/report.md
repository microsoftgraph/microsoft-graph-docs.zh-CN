---
title: 在 Microsoft Graph 中使用 Office 365 使用情况报表
description: 通过 Microsoft Graph，可以访问 Office 365 使用情况报表资源，了解企业用户的 Office 365 服务使用情况。 例如，可以发现大量使用服务且要达到配额的用户，也可以发现可能完全不需要 Office 365 许可证的用户。
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c786d2a6c26a667f44037e1bcb2834dee757ae94
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579301"
---
# <a name="working-with-office-365-usage-reports-in-microsoft-graph"></a><span data-ttu-id="10e90-104">在 Microsoft Graph 中使用 Office 365 使用情况报表</span><span class="sxs-lookup"><span data-stu-id="10e90-104">Working with Office 365 usage reports in Microsoft Graph</span></span>

<span data-ttu-id="10e90-105">通过 Microsoft Graph，可以访问 Office 365 使用情况报表资源，了解企业用户的 Office 365 服务使用情况。</span><span class="sxs-lookup"><span data-stu-id="10e90-105">With Microsoft Graph, you can access Office 365 usage reports resources to get the information about how people in your business are using Office 365 services.</span></span> <span data-ttu-id="10e90-106">例如，可以发现大量使用服务且要达到配额的用户，也可以发现可能完全不需要 Office 365 许可证的用户。</span><span class="sxs-lookup"><span data-stu-id="10e90-106">For example, you can identify who is using a service a lot and reaching quotas, or who may not need an Office 365 license at all.</span></span>

## <a name="authorization"></a><span data-ttu-id="10e90-107">授权</span><span class="sxs-lookup"><span data-stu-id="10e90-107">Authorization</span></span>

<span data-ttu-id="10e90-108">Microsoft Graph 通过权限控制对资源的访问。</span><span class="sxs-lookup"><span data-stu-id="10e90-108">Microsoft Graph controls access to resources via permissions.</span></span> <span data-ttu-id="10e90-109">必须指定访问报表资源所需的权限。</span><span class="sxs-lookup"><span data-stu-id="10e90-109">You must specify the permissions you need in order to access Reports resources.</span></span> <span data-ttu-id="10e90-110">通常是在 Azure Active Directory (Azure AD) 门户中指定权限。</span><span class="sxs-lookup"><span data-stu-id="10e90-110">Typically, you specify permissions in the Azure Active Directory (Azure AD) portal.</span></span> <span data-ttu-id="10e90-111">有关详细信息，请参阅 [Microsoft Graph 权限参考](/graph/permissions-reference)和[报表权限](/graph/permissions-reference#reports-permissions)。</span><span class="sxs-lookup"><span data-stu-id="10e90-111">For more information, see [Microsoft Graph permissions reference](/graph/permissions-reference) and [Reports permissions](/graph/permissions-reference#reports-permissions).</span></span>

## <a name="next-steps"></a><span data-ttu-id="10e90-112">后续步骤</span><span class="sxs-lookup"><span data-stu-id="10e90-112">Next steps</span></span>

<span data-ttu-id="10e90-113">借助报表资源和 API，可以通过新方式使用 Microsoft Graph 与用户进行交互，并管理他们的用户体验。</span><span class="sxs-lookup"><span data-stu-id="10e90-113">Reports resources and APIs can open up new ways for you to engage with users and manage their experiences with Microsoft Graph.</span></span> <span data-ttu-id="10e90-114">若要了解详细信息：</span><span class="sxs-lookup"><span data-stu-id="10e90-114">To learn more:</span></span>

- <span data-ttu-id="10e90-115">深入了解对方案最有帮助的资源的方法和属性。</span><span class="sxs-lookup"><span data-stu-id="10e90-115">Drill down on the methods and properties of the resources most helpful to your scenario.</span></span>
- <span data-ttu-id="10e90-116">尝试在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中调用 API。</span><span class="sxs-lookup"><span data-stu-id="10e90-116">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

<span data-ttu-id="10e90-p105">需要更多灵感？请参阅[我们的一些合作伙伴如何使用 Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners)。</span><span class="sxs-lookup"><span data-stu-id="10e90-p105">Need more ideas? See [how some of our partners are using Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).</span></span>
