# <a name="sharepoint-sites-and-content-api-overview"></a><span data-ttu-id="b44cc-101">SharePoint 网站和内容 API 概述</span><span class="sxs-lookup"><span data-stu-id="b44cc-101">SharePoint sites and content API overview</span></span>

<span data-ttu-id="b44cc-102">SharePoint 是移动且智能的内部网。</span><span class="sxs-lookup"><span data-stu-id="b44cc-102">SharePoint is your mobile, intelligent intranet.</span></span> <span data-ttu-id="b44cc-103">借助 SharePoint，用户可以共享和管理内容、知识和应用程序，以增强团队合作、查找信息并在整个组织内进行协作。</span><span class="sxs-lookup"><span data-stu-id="b44cc-103">With SharePoint, users can share and manage content, knowledge, and applications to empower teamwork, find information, and collaborate across an organization.</span></span> <span data-ttu-id="b44cc-104">你可以在 Microsoft Graph 中使用 SharePoint REST API，将解决方案与 SharePoint 网站和内容进行集成。</span><span class="sxs-lookup"><span data-stu-id="b44cc-104">You can use the SharePoint REST API in Microsoft Graph to integrate your solutions with SharePoint sites and content.</span></span>

## <a name="why-integrate-with-sharepoint-sites-and-content"></a><span data-ttu-id="b44cc-105">为什么与 SharePoint 网站和内容集成？</span><span class="sxs-lookup"><span data-stu-id="b44cc-105">Why integrate with SharePoint sites and content?</span></span>

<span data-ttu-id="b44cc-106">SharePoint 网站可增强团队的协作和沟通。</span><span class="sxs-lookup"><span data-stu-id="b44cc-106">SharePoint sites power team collaboration and communication.</span></span> <span data-ttu-id="b44cc-107">Office 365 组、Microsoft Teams 和门户均基于 SharePoint，因此，可以使用 Microsoft Graph 来访问数据，而无需考虑数据存储在何处。</span><span class="sxs-lookup"><span data-stu-id="b44cc-107">Office 365 groups, Microsoft Teams, and portals are all based on SharePoint, so you can use Microsoft Graph to access data no matter where it's kept.</span></span> <span data-ttu-id="b44cc-108">在 Microsoft Graph 中使用 SharePoint API 可访问：</span><span class="sxs-lookup"><span data-stu-id="b44cc-108">Use the SharePoint API in Microsoft Graph to access:</span></span>

- <span data-ttu-id="b44cc-109">存储用户与其同事协作内容的团队网站。</span><span class="sxs-lookup"><span data-stu-id="b44cc-109">Team sites that store the content that users collaborate on with their coworkers.</span></span>
- <span data-ttu-id="b44cc-110">用户发布要在整个组织中共享的丰富内容页的通信网站和门户。</span><span class="sxs-lookup"><span data-stu-id="b44cc-110">Communication sites and portals where users publish rich content pages to share across the organization.</span></span>

### <a name="unleash-your-data-with-sharepoint-lists"></a><span data-ttu-id="b44cc-111">借助 SharePoint 列表充分使用数据</span><span class="sxs-lookup"><span data-stu-id="b44cc-111">Unleash your data with SharePoint lists</span></span>

<span data-ttu-id="b44cc-112">[列表][list]是 SharePoint 中数据存储的基础。</span><span class="sxs-lookup"><span data-stu-id="b44cc-112">[Lists][list] are the foundation for data storage in SharePoint.</span></span>
<span data-ttu-id="b44cc-113">[创建列表][create]以存储各种不同的业务数据，从简单的客户联系人列表到前端具有 PowerApps 的自定义业务应用程序。</span><span class="sxs-lookup"><span data-stu-id="b44cc-113">[Create lists][create] to store a variety of business data, from a simple customer contact list to a custom business application, fronted with PowerApps.</span></span>
<span data-ttu-id="b44cc-114">使用[列][]定义架构时，SharePoint 可以保护数据的完整性，并启用丰富的索引、查询和搜索功能。</span><span class="sxs-lookup"><span data-stu-id="b44cc-114">When you use [columns][] to define your schema, SharePoint can protect the integrity of your data as well as enable  rich indexing, querying, and search capabilities.</span></span>

### <a name="bring-the-power-of-lists-to-your-teams-files"></a><span data-ttu-id="b44cc-115">将列表的强大功能引入团队文件中</span><span class="sxs-lookup"><span data-stu-id="b44cc-115">Bring the power of lists to your team's files</span></span>

<span data-ttu-id="b44cc-116">SharePoint 将文件存储在名为文档库的特殊[列表类型][]中。</span><span class="sxs-lookup"><span data-stu-id="b44cc-116">SharePoint stores files in a special [list type][] called a document library.</span></span>
<span data-ttu-id="b44cc-117">可以使用 [OneDrive API][] 将库用作[驱动器][]，或使用 SharePoint API 将库用作[列表][]。</span><span class="sxs-lookup"><span data-stu-id="b44cc-117">You can use the [OneDrive API][] to work with a library as a [drive][], or the SharePoint API to work with it as a [list][].</span></span>
<span data-ttu-id="b44cc-118">就像常规列表一样，可以扩展文档库的架构以通过自定义列来支持业务需求。</span><span class="sxs-lookup"><span data-stu-id="b44cc-118">Just like a regular list, you can extend the schema of a Document Library to support your business needs with custom columns.</span></span>

### <a name="light-up-your-app-with-your-users-sharepoint-intranet-data"></a><span data-ttu-id="b44cc-119">通过用户的 SharePoint 内部网数据使应用更强大</span><span class="sxs-lookup"><span data-stu-id="b44cc-119">Light up your app with your users' SharePoint intranet data</span></span>

<span data-ttu-id="b44cc-120">使用 Microsoft Graph，可以在应用中显示用户最重要的数据。</span><span class="sxs-lookup"><span data-stu-id="b44cc-120">With Microsoft Graph, you can surface your users' most important data within your app.</span></span>
<span data-ttu-id="b44cc-121">通过[查询][]存储用户数据的列表来使数据保持最新。</span><span class="sxs-lookup"><span data-stu-id="b44cc-121">Keep things fresh by [querying][] the list that stores your users' data.</span></span>
<span data-ttu-id="b44cc-122">为应用[创建][]自己的列表，并允许用户在其他 SharePoint 体验中访问你的数据，或使数据处于隐藏状态。</span><span class="sxs-lookup"><span data-stu-id="b44cc-122">[Create][] your own lists for your app and let users access your data in other SharePoint experiences, or keep things hidden.</span></span>

### <a name="use-microsoft-graph-to-extend-sharepoint"></a><span data-ttu-id="b44cc-123">使用 Microsoft Graph 扩展 SharePoint</span><span class="sxs-lookup"><span data-stu-id="b44cc-123">Use Microsoft Graph to extend SharePoint</span></span>

<span data-ttu-id="b44cc-124">作为平台，SharePoint 提供一些用于扩展和集成的模型：</span><span class="sxs-lookup"><span data-stu-id="b44cc-124">As a platform, SharePoint provides several models for extension and integration:</span></span>

- <span data-ttu-id="b44cc-125">[SharePoint Framework][] 提供了一种方法，使用可托管于 SharePoint 页面上的客户端技术和开源代码工具生成 Web 部件。</span><span class="sxs-lookup"><span data-stu-id="b44cc-125">The [SharePoint Framework][] provides a way to build web parts using client-side technologies and open source tooling that can be hosted on SharePoint pages.</span></span>
- <span data-ttu-id="b44cc-126">[SharePoint 外接程序][]是可添加到 SharePoint 网站而无需在服务器上运行自定义代码的自包含扩展。</span><span class="sxs-lookup"><span data-stu-id="b44cc-126">[SharePoint Add-ins][] are self-contained extensions that can be added to a SharePoint site without the need for custom code to run on the server.</span></span>

<span data-ttu-id="b44cc-127">当应用在 SharePoint 页面内运行时，可以使用 Microsoft Graph 轻松访问整个 Office 365 中的数据。</span><span class="sxs-lookup"><span data-stu-id="b44cc-127">When your app runs within a SharePoint page, you can easily use Microsoft Graph to access data across Office 365.</span></span>

<span data-ttu-id="b44cc-128">若要了解这些模型的详细信息，请访问 [SharePoint 开发人员中心][]或 [SharePoint 开发人员文档][]。</span><span class="sxs-lookup"><span data-stu-id="b44cc-128">To learn about these models in more detail, visit the [SharePoint Dev Center][] or the [SharePoint Developer Docs][].</span></span>

## <a name="next-steps"></a><span data-ttu-id="b44cc-129">后续步骤</span><span class="sxs-lookup"><span data-stu-id="b44cc-129">Next steps</span></span>

<span data-ttu-id="b44cc-130">通过了解关于[使用网站][SharePoint]的更多信息来开始在 Microsoft Graph 中使用 SharePoint。</span><span class="sxs-lookup"><span data-stu-id="b44cc-130">Get started with SharePoint in Microsoft Graph by learning more about [working with sites][SharePoint].</span></span>

[列表]: ../api-reference/v1.0/resources/list.md
[list]: ../api-reference/v1.0/resources/list.md
[列]: ../api-reference/v1.0/resources/columndefinition.md
[columns]: ../api-reference/v1.0/resources/columndefinition.md
[列表类型]: ../api-reference/v1.0/resources/listinfo.md
[List Type]: ../api-reference/v1.0/resources/listinfo.md
[创建]: ../api-reference/v1.0/api/list_create.md
[Create]: ../api-reference/v1.0/api/list_create.md.
[查询]: ../api-reference/v1.0/api/listitem_get.md
[querying]: ../api-reference/v1.0/api/listitem_get.md
[驱动器]: ../api-reference/v1.0/resources/drive.md
[drive]: ../api-reference/v1.0/resources/drive.md
<span data-ttu-id="b44cc-137">
  [OneDrive API]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/onedrive</span><span class="sxs-lookup"><span data-stu-id="b44cc-137">[onedrive api]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/onedrive</span></span>
[SharePoint Framework]: https://docs.microsoft.com/sharepoint/dev/spfx/sharepoint-framework-overview
[SharePoint 外接程序]: https://docs.microsoft.com/sharepoint/dev/sp-add-ins/sharepoint-add-ins
[SharePoint Add-ins]: https://docs.microsoft.com/sharepoint/dev/sp-add-ins/sharepoint-add-ins
[SharePoint 开发人员中心]: https://developer.microsoft.com/sharepoint
[SharePoint Dev Center]: https://developer.microsoft.com/sharepoint
[SharePoint 开发人员文档]: http://aka.ms/spdev-docs
[SharePoint Developer Docs]: http://aka.ms/spdev-docs
[SharePoint]: https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/sharepoint
