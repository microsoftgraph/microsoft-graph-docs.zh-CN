---
title: Microsoft Graph 连接器概述
description: Microsoft Graph 连接器概述
author: mecampos
localization_priority: Priority
doc_type: conceptualPageType
ms.prod: search
ms.openlocfilehash: 3c4e358ed8d0d769aa88aa7100acb113fe2caa9a
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645715"
---
# <a name="microsoft-graph-connectors-overview"></a><span data-ttu-id="8998c-103">Microsoft Graph 连接器概述</span><span class="sxs-lookup"><span data-stu-id="8998c-103">Microsoft Graph connectors overview</span></span>

<span data-ttu-id="8998c-104">[Microsoft 365](https://www.microsoft.com/microsoft-365) 是一套完整的智能解决方案，可让用户和组织获得创新生产力体验和丰富见解，从而提高效率、促进业务增长。</span><span class="sxs-lookup"><span data-stu-id="8998c-104">[Microsoft 365](https://www.microsoft.com/microsoft-365) is a complete, intelligent solution that empowers users and organizations with innovative productivity experiences and rich insights to increase efficiency and drive business growth.</span></span> <span data-ttu-id="8998c-105">Microsoft Graph 是支持这些智能体验的数据平台，Microsoft Graph API 提供此数据和智能的访问权限。</span><span class="sxs-lookup"><span data-stu-id="8998c-105">Microsoft Graph is the data fabric that powers these intelligent experiences, and the Microsoft Graph API provides access to this data and intelligence.</span></span>

<span data-ttu-id="8998c-106">尽管大多数信息工作者在生产力应用程序（如 [Microsoft 365](https://www.microsoft.com/microsoft-365)）上花费大量时间，但他们也需要一种方法将环境与企业应用程序以及他们使用的其他本地和 SaaS 云软件和服务集成。</span><span class="sxs-lookup"><span data-stu-id="8998c-106">Although most information workers spend much of their work time within productivity applications such as [Microsoft 365](https://www.microsoft.com/microsoft-365), they also need a way to integrate that environment with the enterprise applications and other on-premises and SaaS cloud software and services they use.</span></span> <span data-ttu-id="8998c-107">例如，企业资源计划 （ERP） 应用程序、客户资源管理 （CRM） 应用程序、Intranet 应用程序、Wiki、博客和社交网络网站。</span><span class="sxs-lookup"><span data-stu-id="8998c-107">For example, enterprise resource planning (ERP) applications, customer resource management (CRM) applications, intranet applications, wikis, blogs, and social networking sites.</span></span>

<span data-ttu-id="8998c-108">Microsoft Graph 连接器提供了一种简单直观的方法，可将外部服务中的内容引入 Microsoft Graph，为 Microsoft 365 智能体验提供支持，如 Microsoft Search（当前 GA）以及即将推出许多如 Viva 主题等。</span><span class="sxs-lookup"><span data-stu-id="8998c-108">Microsoft Graph connectors offer a simple and intuitive way to bring content from external services into Microsoft Graph, enabling external data to power Microsoft 365 intelligent experiences like Microsoft Search (currently GA) and many more coming soon like Viva Topics.</span></span>

<span data-ttu-id="8998c-109">现在，使用 Microsoft Graph 连接器，你引入组织的数据可能出现在 Microsoft 搜索结果中。</span><span class="sxs-lookup"><span data-stu-id="8998c-109">Today, with Microsoft Graph connectors, the data you bring in from your organization can appear in Microsoft Search results.</span></span> <span data-ttu-id="8998c-110">此功能扩展了 Microsoft 365 生产力应用中可搜索的内容源类型以及 Microsoft 更广泛的数据源。</span><span class="sxs-lookup"><span data-stu-id="8998c-110">This feature expands the types of content sources that are searchable in your Microsoft 365 productivity apps and the broader Microsoft ecosystem.</span></span> <span data-ttu-id="8998c-111">不久将，连接器将支持许多其他 Microsoft 365 智能体验。</span><span class="sxs-lookup"><span data-stu-id="8998c-111">Soon, connectors will power many other Microsoft 365 intelligent experiences.</span></span>
<span data-ttu-id="8998c-112">下图提供了 Microsoft Graph 连接线高级概述。</span><span class="sxs-lookup"><span data-stu-id="8998c-112">The following diagram provides a high-level overview of Microsoft Graph connectors.</span></span>

<!---Insert image reference here --->
<!---       ![Select the Microsoft Graph permissions](./images/application-saml-sso-configure-api/set-permissions.png) --->
<span data-ttu-id="8998c-113">![图像显示正使用连接线将数据引入 Microsoft Graph](./images/connectors-images/overview.png)</span><span class="sxs-lookup"><span data-stu-id="8998c-113">![Image showing connectors being used to bring data into Microsoft Graph](./images/connectors-images/overview.png)</span></span>

## <a name="build-your-own-custom-connector"></a><span data-ttu-id="8998c-114">构建自己的自定义连接器</span><span class="sxs-lookup"><span data-stu-id="8998c-114">Build your own custom connector</span></span>

<span data-ttu-id="8998c-115">Microsoft 和合作伙伴当前提供的 100 多个连接器可用于连接到热门的 Microsoft 和非 Microsoft 服务。</span><span class="sxs-lookup"><span data-stu-id="8998c-115">The 100+ connectors currently available from Microsoft and partners enable you to connect to popular Microsoft and non-Microsoft services.</span></span> <span data-ttu-id="8998c-116">现有连接器的示例包括 Azure 服务、Box、ServiceNow、SalesForce、Google 服务、MediaWiki 等。</span><span class="sxs-lookup"><span data-stu-id="8998c-116">Examples of existing connectors include Azure services, Box, ServiceNow, SalesForce, Google services, MediaWiki, and more.</span></span>

<span data-ttu-id="8998c-117">若要详细了解现有的 Microsoft Graph 连接器，请访问 [Microsoft Graph 连接器库](/microsoftsearch/connectors-gallery)。</span><span class="sxs-lookup"><span data-stu-id="8998c-117">To learn more about the existing Microsoft Graph connectors, visit the [Microsoft Graph connectors gallery](/microsoftsearch/connectors-gallery).</span></span>

<span data-ttu-id="8998c-118">尽管这些连接器有助于连接到流行的服务，但您可能希望与现有[连接器库](/microsoftsearch/connectors-gallery)中未提供的服务进行集成。</span><span class="sxs-lookup"><span data-stu-id="8998c-118">While these connectors help connect to popular services, you may want to integrate with services that aren't available in the existing [connectors gallery](/microsoftsearch/connectors-gallery).</span></span> <span data-ttu-id="8998c-119">您可以使用 Microsoft Graph connectors API 构建自定义连接器，将外部数据引入 Microsoft 365 体验，包括 Microsoft Search、Viva 主题等（即将推出）。</span><span class="sxs-lookup"><span data-stu-id="8998c-119">You can use the Microsoft Graph connectors API to build custom connectors to bring your external data into Microsoft 365 experiences, including Microsoft Search, Viva Topics and more (coming soon), within your organization.</span></span>

## <a name="get-started-with-custom-graph-connectors"></a><span data-ttu-id="8998c-120">自定义图形连接线入门：</span><span class="sxs-lookup"><span data-stu-id="8998c-120">Get started with custom Graph connectors:</span></span>
* [<span data-ttu-id="8998c-121">使用连接器 API</span><span class="sxs-lookup"><span data-stu-id="8998c-121">Working with the connectors API</span></span>](connecting-external-content-connectors-api-overview.md)
* [<span data-ttu-id="8998c-122">将 Postman 与 Microsoft Graph 连接器 API 一并使用</span><span class="sxs-lookup"><span data-stu-id="8998c-122">Use Postman with the Microsoft Graph connectors API</span></span>](connecting-external-content-connectors-api-postman.md)
<!---**(Articles coming next)**
* [Build your first custom connector with Microsoft Graph]()
--->

