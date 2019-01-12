---
title: SharePoint 网站和内容 API 概述
description: SharePoint 是移动且智能的内部网。 借助 SharePoint，用户可以共享和管理内容、知识和应用程序，以增强团队合作、查找信息并在整个组织内进行协作。 你可以在 Microsoft Graph 中使用 SharePoint REST API，将解决方案与 SharePoint 网站和内容进行集成。
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 7f703854112643afc11cf82b32b6b9247f0bca39
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965269"
---
# <a name="sharepoint-sites-and-content-api-overview"></a><span data-ttu-id="d6380-105">SharePoint 网站和内容 API 概述</span><span class="sxs-lookup"><span data-stu-id="d6380-105">SharePoint sites and content API overview</span></span>

<span data-ttu-id="d6380-106">SharePoint 是移动且智能的内部网。</span><span class="sxs-lookup"><span data-stu-id="d6380-106">SharePoint is your mobile, intelligent intranet.</span></span> <span data-ttu-id="d6380-107">借助 SharePoint，用户可以共享和管理内容、知识和应用程序，以增强团队合作、查找信息并在整个组织内进行协作。</span><span class="sxs-lookup"><span data-stu-id="d6380-107">With SharePoint, users can share and manage content, knowledge, and applications to empower teamwork, find information, and collaborate across an organization.</span></span> <span data-ttu-id="d6380-108">你可以在 Microsoft Graph 中使用 SharePoint REST API，将解决方案与 SharePoint 网站和内容进行集成。</span><span class="sxs-lookup"><span data-stu-id="d6380-108">You can use the SharePoint REST API in Microsoft Graph to integrate your solutions with SharePoint sites and content.</span></span>

## <a name="why-integrate-with-sharepoint-sites-and-content"></a><span data-ttu-id="d6380-109">为什么与 SharePoint 网站和内容集成？</span><span class="sxs-lookup"><span data-stu-id="d6380-109">Why integrate with SharePoint sites and content?</span></span>

<span data-ttu-id="d6380-110">SharePoint 网站可增强团队的协作和沟通。</span><span class="sxs-lookup"><span data-stu-id="d6380-110">SharePoint sites power team collaboration and communication.</span></span> <span data-ttu-id="d6380-111">Office 365 组、Microsoft Teams 和门户均基于 SharePoint，因此，可以使用 Microsoft Graph 来访问数据，而无需考虑数据存储在何处。</span><span class="sxs-lookup"><span data-stu-id="d6380-111">Office 365 groups, Microsoft Teams, and portals are all based on SharePoint, so you can use Microsoft Graph to access data no matter where it's kept.</span></span> <span data-ttu-id="d6380-112">在 Microsoft Graph 中使用 SharePoint API 可访问：</span><span class="sxs-lookup"><span data-stu-id="d6380-112">Use the SharePoint API in Microsoft Graph to access:</span></span>

- <span data-ttu-id="d6380-113">存储用户与其同事协作内容的团队网站。</span><span class="sxs-lookup"><span data-stu-id="d6380-113">Team sites that store the content that users collaborate on with their coworkers.</span></span>
- <span data-ttu-id="d6380-114">用户发布要在整个组织中共享的丰富内容页的通信网站和门户。</span><span class="sxs-lookup"><span data-stu-id="d6380-114">Communication sites and portals where users publish rich content pages to share across the organization.</span></span>

### <a name="unleash-your-data-with-sharepoint-lists"></a><span data-ttu-id="d6380-115">借助 SharePoint 列表充分使用数据</span><span class="sxs-lookup"><span data-stu-id="d6380-115">Unleash your data with SharePoint lists</span></span>

<span data-ttu-id="d6380-116">[列表][list]是 SharePoint 中数据存储的基础。</span><span class="sxs-lookup"><span data-stu-id="d6380-116">[Lists][list] are the foundation for data storage in SharePoint.</span></span>
<span data-ttu-id="d6380-117">[创建列表][create]以存储各种不同的业务数据，从简单的客户联系人列表到前端具有 PowerApps 的自定义业务应用程序。</span><span class="sxs-lookup"><span data-stu-id="d6380-117">[Create lists][create] to store a variety of business data, from a simple customer contact list to a custom business application, fronted with PowerApps.</span></span>
<span data-ttu-id="d6380-118">使用[列][]定义架构时，SharePoint 可以保护数据的完整性，并启用丰富的索引、查询和搜索功能。</span><span class="sxs-lookup"><span data-stu-id="d6380-118">When you use [columns][] to define your schema, SharePoint can protect the integrity of your data as well as enable  rich indexing, querying, and search capabilities.</span></span>

### <a name="bring-the-power-of-lists-to-your-teams-files"></a><span data-ttu-id="d6380-119">将列表的强大功能引入团队文件中</span><span class="sxs-lookup"><span data-stu-id="d6380-119">Bring the power of lists to your team's files</span></span>

<span data-ttu-id="d6380-120">SharePoint 将文件存储在名为文档库的特殊[列表类型][]中。</span><span class="sxs-lookup"><span data-stu-id="d6380-120">SharePoint stores files in a special [list type][] called a document library.</span></span>
<span data-ttu-id="d6380-121">可以使用 [OneDrive API][] 将库用作[驱动器][]，或使用 SharePoint API 将库用作[列表][]。</span><span class="sxs-lookup"><span data-stu-id="d6380-121">You can use the [OneDrive API][] to work with a library as a [drive][], or the SharePoint API to work with it as a [list][].</span></span>
<span data-ttu-id="d6380-122">就像常规列表一样，可以扩展文档库的架构以通过自定义列来支持业务需求。</span><span class="sxs-lookup"><span data-stu-id="d6380-122">Just like a regular list, you can extend the schema of a Document Library to support your business needs with custom columns.</span></span>

### <a name="light-up-your-app-with-your-users-sharepoint-intranet-data"></a><span data-ttu-id="d6380-123">通过用户的 SharePoint 内部网数据使应用更强大</span><span class="sxs-lookup"><span data-stu-id="d6380-123">Light up your app with your users' SharePoint intranet data</span></span>

<span data-ttu-id="d6380-124">使用 Microsoft Graph，可以在应用中显示用户最重要的数据。</span><span class="sxs-lookup"><span data-stu-id="d6380-124">With Microsoft Graph, you can surface your users' most important data within your app.</span></span>
<span data-ttu-id="d6380-125">通过[查询][]存储用户数据的列表来使数据保持最新。</span><span class="sxs-lookup"><span data-stu-id="d6380-125">Keep things fresh by [querying][] the list that stores your users' data.</span></span>
<span data-ttu-id="d6380-126">为应用[创建][]自己的列表，并允许用户在其他 SharePoint 体验中访问你的数据，或使数据处于隐藏状态。</span><span class="sxs-lookup"><span data-stu-id="d6380-126">[Create][] your own lists for your app and let users access your data in other SharePoint experiences, or keep things hidden.</span></span>

### <a name="use-microsoft-graph-to-extend-sharepoint"></a><span data-ttu-id="d6380-127">使用 Microsoft Graph 扩展 SharePoint</span><span class="sxs-lookup"><span data-stu-id="d6380-127">Use Microsoft Graph to extend SharePoint</span></span>

<span data-ttu-id="d6380-128">作为平台，SharePoint 提供一些用于扩展和集成的模型：</span><span class="sxs-lookup"><span data-stu-id="d6380-128">As a platform, SharePoint provides several models for extension and integration:</span></span>

- <span data-ttu-id="d6380-129">[SharePoint Framework][] 提供了一种方法，使用可托管于 SharePoint 页面上的客户端技术和开源代码工具生成 Web 部件。</span><span class="sxs-lookup"><span data-stu-id="d6380-129">The [SharePoint Framework][] provides a way to build web parts using client-side technologies and open source tooling that can be hosted on SharePoint pages.</span></span>
- <span data-ttu-id="d6380-130">[SharePoint 外接程序][]是可添加到 SharePoint 网站而无需在服务器上运行自定义代码的自包含扩展。</span><span class="sxs-lookup"><span data-stu-id="d6380-130">[SharePoint Add-ins][] are self-contained extensions that can be added to a SharePoint site without the need for custom code to run on the server.</span></span>

<span data-ttu-id="d6380-131">当应用在 SharePoint 页面内运行时，可以使用 Microsoft Graph 轻松访问整个 Office 365 中的数据。</span><span class="sxs-lookup"><span data-stu-id="d6380-131">When your app runs within a SharePoint page, you can easily use Microsoft Graph to access data across Office 365.</span></span>

<span data-ttu-id="d6380-132">若要详细了解这些模型，请访问 [SharePoint 开发人员中心][]或 [SharePoint 开发人员文档][]。</span><span class="sxs-lookup"><span data-stu-id="d6380-132">To learn about these models in more detail, visit the [SharePoint Dev Center][] or the [SharePoint Developer Docs][].</span></span>

## <a name="api-reference"></a><span data-ttu-id="d6380-133">API 参考</span><span class="sxs-lookup"><span data-stu-id="d6380-133">API reference</span></span>
<span data-ttu-id="d6380-134">在查找此服务的 API 参考？</span><span class="sxs-lookup"><span data-stu-id="d6380-134">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="d6380-135">Microsoft Graph v1.0 中的 SharePoint API</span><span class="sxs-lookup"><span data-stu-id="d6380-135">SharePoint API in Microsoft Graph v1.0</span></span>](/graph/api/resources/sharepoint?view=graph-rest-1.0)
- [<span data-ttu-id="d6380-136">Microsoft Graph beta 中的 SharePoint API</span><span class="sxs-lookup"><span data-stu-id="d6380-136">SharePoint API in Microsoft Graph beta</span></span>](/graph/api/resources/sharepoint?view=graph-rest-beta)

## <a name="next-steps"></a><span data-ttu-id="d6380-137">后续步骤</span><span class="sxs-lookup"><span data-stu-id="d6380-137">Next steps</span></span>

<span data-ttu-id="d6380-138">通过了解关于[使用网站][SharePoint]的更多信息来开始在 Microsoft Graph 中使用 SharePoint。</span><span class="sxs-lookup"><span data-stu-id="d6380-138">Get started with SharePoint in Microsoft Graph by learning more about [working with sites][SharePoint].</span></span>

[列表]: /graph/api/resources/list?view=graph-rest-1.0
[list]: /graph/api/resources/list?view=graph-rest-1.0
[列]: /graph/api/resources/columndefinition?view=graph-rest-1.0
[columns]: /graph/api/resources/columndefinition?view=graph-rest-1.0
[列表类型]: /graph/api/resources/listinfo?view=graph-rest-1.0
[list type]: /graph/api/resources/listinfo?view=graph-rest-1.0
[创建]: /graph/api/list-create?view=graph-rest-1.0
[create]: /graph/api/list-create?view=graph-rest-1.0
[查询]: /graph/api/listitem-get?view=graph-rest-1.0
[querying]: /graph/api/listitem-get?view=graph-rest-1.0
[驱动器]: /graph/api/resources/drive?view=graph-rest-1.0
[drive]: /graph/api/resources/drive?view=graph-rest-1.0
[OneDrive API]: /graph/api/resources/onedrive?view=graph-rest-1.0
[SharePoint Framework]: https://docs.microsoft.com/sharepoint/dev/spfx/sharepoint-framework-overview
[SharePoint 外接程序]: https://docs.microsoft.com/sharepoint/dev/sp-add-ins/sharepoint-add-ins
[SharePoint Add-ins]: https://docs.microsoft.com/sharepoint/dev/sp-add-ins/sharepoint-add-ins
[SharePoint 开发人员中心]: https://developer.microsoft.com/sharepoint
[SharePoint Dev Center]: https://developer.microsoft.com/sharepoint
[SharePoint 开发人员文档]: https://aka.ms/spdev-docs
[SharePoint Developer Docs]: https://aka.ms/spdev-docs
[SharePoint]: /graph/api/resources/sharepoint?view=graph-rest-1.0
