---
title: 将 Azure AD Graph 应用迁移到 Microsoft Graph
description: 介绍如何将 Azure Active Directory （Azure AD） API 应用迁移到 Microsoft Graph API。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4a759516ad5852f0ef73aaacd87d0c8d85d9a0a1
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896439"
---
# <a name="migrate-azure-ad-graph-apps-to-microsoft-graph"></a><span data-ttu-id="d35b0-103">将 Azure AD Graph 应用迁移到 Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d35b0-103">Migrate Azure AD Graph apps to Microsoft Graph</span></span>

<span data-ttu-id="d35b0-104">Microsoft Graph 完全替换 Azure Active Directory （Azure AD）图形。</span><span class="sxs-lookup"><span data-stu-id="d35b0-104">Microsoft Graph is fully replacing Azure Active Directory (Azure AD) Graph.</span></span> <span data-ttu-id="d35b0-105">对于大多数生产应用程序，Microsoft Graph 可能已经完全支持 Azure AD 场景。</span><span class="sxs-lookup"><span data-stu-id="d35b0-105">For most production apps, Microsoft Graph can already fully support Azure AD scenarios.</span></span> <span data-ttu-id="d35b0-106">你现在应开始将 Azure AD Graph 应用移动到 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="d35b0-106">You should start moving your Azure AD Graph apps to Microsoft Graph now.</span></span>

<span data-ttu-id="d35b0-107">此外，Microsoft Graph 支持许多新的 Azure AD 数据集和功能，这些功能在 Azure AD Graph 中不可用。</span><span class="sxs-lookup"><span data-stu-id="d35b0-107">In addition, Microsoft Graph supports many new Azure AD datasets and features that are not available in Azure AD Graph.</span></span> <span data-ttu-id="d35b0-108">切换到 Microsoft Graph 以利用这些新的 Api，这一切都通过一个单终结点，包括：</span><span class="sxs-lookup"><span data-stu-id="d35b0-108">Switch to Microsoft Graph to take advantage of these new APIs, all through one single endpoint, including:</span></span>

- [<span data-ttu-id="d35b0-109">Microsoft 365 组管理</span><span class="sxs-lookup"><span data-stu-id="d35b0-109">Microsoft 365 group management</span></span>](/graph/office365-groups-concept-overview)
- [<span data-ttu-id="d35b0-110">外部用户邀请</span><span class="sxs-lookup"><span data-stu-id="d35b0-110">External user invitations</span></span>](/graph/api/resources/invitation?view=graph-rest-1.0)
- <span data-ttu-id="d35b0-111">能够在删除[用户和 Microsoft 365 组](/graph/api/resources/directory?view=graph-rest-1.0)之后对其进行还原</span><span class="sxs-lookup"><span data-stu-id="d35b0-111">The ability to [restore users and Microsoft 365 groups](/graph/api/resources/directory?view=graph-rest-1.0) after they've been deleted</span></span>
- [<span data-ttu-id="d35b0-112">用户和组上的 Webhook 通知</span><span class="sxs-lookup"><span data-stu-id="d35b0-112">Webhook notifications on users and groups</span></span>](/graph/webhooks?toc=./ref/toc.json&view=graph-rest-1.0)
- <span data-ttu-id="d35b0-113">身份管理功能，如：</span><span class="sxs-lookup"><span data-stu-id="d35b0-113">Identity governance features such as:</span></span>
  - <span data-ttu-id="d35b0-114">[特权标识管理](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta)（PIM）仅在需要时和在有限时间段内将用户提升到特权角色</span><span class="sxs-lookup"><span data-stu-id="d35b0-114">[Privileged identity management](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta) (PIM) to elevate users to privileged roles only when needed and for a limited time period</span></span>
  - <span data-ttu-id="d35b0-115">[对用户](/graph/api/resources/accessreviews-root?view=graph-rest-beta)访问权限证明的一次性或定期访问审核</span><span class="sxs-lookup"><span data-stu-id="d35b0-115">[Access reviews](/graph/api/resources/accessreviews-root?view=graph-rest-beta) for one-time or recurring access reviews for attestation of user's access rights</span></span>
  - <span data-ttu-id="d35b0-116">帮助组织提供有关法律或合规性要求的信息（如免责声明通知）[的使用条款](/graph/api/resources/accessreviews-root?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="d35b0-116">[Terms-of-use](/graph/api/resources/accessreviews-root?view=graph-rest-beta) to enable organizations to present information for legal or compliance requirements, like disclaimer notices</span></span>
- <span data-ttu-id="d35b0-117">安全功能，如：</span><span class="sxs-lookup"><span data-stu-id="d35b0-117">Security features such as:</span></span>
  - [<span data-ttu-id="d35b0-118">身份风险事件</span><span class="sxs-lookup"><span data-stu-id="d35b0-118">Identity risk events</span></span>](/graph/api/resources/identityriskevent?view=graph-rest-beta)
  - [<span data-ttu-id="d35b0-119">风险用户</span><span class="sxs-lookup"><span data-stu-id="d35b0-119">Risky users</span></span>](/graph/api/resources/riskyuser?view=graph-rest-beta)
- <span data-ttu-id="d35b0-120">可在更多平台和语言中使用的[客户端库和示例](/graph/)。</span><span class="sxs-lookup"><span data-stu-id="d35b0-120">[Client libraries and samples](/graph/) available on many more platforms and languages.</span></span> <span data-ttu-id="d35b0-121">Microsoft Graph Sdk 提供了一个可发现接口，可在透明地处理令牌获取、重试处理（由于错误和限制、安全重定向处理以及模型序列化和反序列化）而轻松访问数据。</span><span class="sxs-lookup"><span data-stu-id="d35b0-121">The Microsoft Graph SDKs provide a discoverable interface to easily access your data while transparently handling token acquisition, retry handling due to errors and throttling, secure redirect handling and model serialization and deserialization.</span></span>

<span data-ttu-id="d35b0-122">与 Azure Active Directory 相比，Microsoft Graph 提供了更多的服务访问权限。</span><span class="sxs-lookup"><span data-stu-id="d35b0-122">Microsoft Graph offers access to many more services than just Azure Active Directory.</span></span> <span data-ttu-id="d35b0-123">这也是[Microsoft 365 服务的 API 网关](/graph/)。</span><span class="sxs-lookup"><span data-stu-id="d35b0-123">It's the [API gateway to Microsoft 365 services too](/graph/).</span></span>

<span data-ttu-id="d35b0-124">本节中的其余文章将帮助你将应用从 Azure AD Graph 移动到 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="d35b0-124">The rest of the articles in this section help you move your app from Azure AD Graph to Microsoft Graph.</span></span> <span data-ttu-id="d35b0-125">你会发现：</span><span class="sxs-lookup"><span data-stu-id="d35b0-125">You'll find:</span></span>

- <span data-ttu-id="d35b0-126">帮助您进行规划的检查表。</span><span class="sxs-lookup"><span data-stu-id="d35b0-126">A checklist to help you plan.</span></span>
- <span data-ttu-id="d35b0-127">描述 Api 之间的特定差异的指南。</span><span class="sxs-lookup"><span data-stu-id="d35b0-127">Guidance describing specific differences between the APIs.</span></span>
- <span data-ttu-id="d35b0-128">指向说明特定差异的其他资源和示例的链接。</span><span class="sxs-lookup"><span data-stu-id="d35b0-128">Links to additional resources and examples to illustrate specific differences.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d35b0-129">后续步骤</span><span class="sxs-lookup"><span data-stu-id="d35b0-129">Next Steps</span></span>

- <span data-ttu-id="d35b0-130">浏览[应用程序迁移清单](migrate-azure-ad-graph-planning-checklist.md)以帮助您规划移动。</span><span class="sxs-lookup"><span data-stu-id="d35b0-130">Walk through the [app migration checklist](migrate-azure-ad-graph-planning-checklist.md) to help you plan the move.</span></span>
- <span data-ttu-id="d35b0-131">浏览[Microsoft Graph](/graph/overview)概念和实践。</span><span class="sxs-lookup"><span data-stu-id="d35b0-131">Explore [Microsoft Graph](/graph/overview) concepts and practices.</span></span>
- <span data-ttu-id="d35b0-132">使用[Graph 浏览器](https://aka.ms/ge)试用 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="d35b0-132">Use [Graph Explorer](https://aka.ms/ge) to experiment with Microsoft Graph.</span></span>
- <span data-ttu-id="d35b0-133">若要了解有关进度更新和时间线的详细信息，请参阅[Microsoft Graph 或 AZURE AD Graph](https://developer.microsoft.com/graph/blogs/microsoft-graph-or-azure-ad-graph/)。</span><span class="sxs-lookup"><span data-stu-id="d35b0-133">To learn more about progress updates and timelines, see [Microsoft Graph or the Azure AD Graph](https://developer.microsoft.com/graph/blogs/microsoft-graph-or-azure-ad-graph/).</span></span>
