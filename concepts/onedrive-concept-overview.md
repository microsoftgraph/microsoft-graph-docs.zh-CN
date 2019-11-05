---
title: OneDrive 文件存储 API 概述
description: OneDrive 是 Office 365 的文件中心。
localization_priority: Priority
ms.prod: onedrive
ms.custom: scenarios:getting-started
ms.openlocfilehash: b0b548880d788e6b8d98596e06f0071e7bdc3a8e
ms.sourcegitcommit: b1e1f614299f668453916bd85761ef7b6c8d6eff
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37969345"
---
# <a name="onedrive-file-storage-api-overview"></a><span data-ttu-id="dc952-103">OneDrive 文件存储 API 概述</span><span class="sxs-lookup"><span data-stu-id="dc952-103">OneDrive file storage API overview</span></span>

<span data-ttu-id="dc952-104">OneDrive 是 Office 365 的文件中心。</span><span class="sxs-lookup"><span data-stu-id="dc952-104">OneDrive is the files hub in Office 365.</span></span>
<span data-ttu-id="dc952-105">人们会在各种各样的环境中使用文件，如 Microsoft Teams、组、SharePoint 等。</span><span class="sxs-lookup"><span data-stu-id="dc952-105">People work with files in a variety of contexts, like Microsoft Teams, groups, SharePoint, and more.</span></span>
<span data-ttu-id="dc952-106">通过 OneDrive，用户可以访问这些文件而不管它们存储在什么位置，而通过 Microsoft Graph，则可以使用单个 API 来使用它们。</span><span class="sxs-lookup"><span data-stu-id="dc952-106">With OneDrive, users can access these files no matter where they are stored, and with Microsoft Graph, you can use a single API to work with them.</span></span>

<span data-ttu-id="dc952-107">Office 365 中的文件存储在[驱动器][Drive API]中。</span><span class="sxs-lookup"><span data-stu-id="dc952-107">Files in Office 365 are stored in [drives][Drive API].</span></span>
<span data-ttu-id="dc952-108">用户可以在其个人驱动器 (OneDrive) 或 [SharePoint][] 文档库支持的共享驱动器中存储文件。</span><span class="sxs-lookup"><span data-stu-id="dc952-108">Users can store files in a personal drive - their OneDrive - or in a shared drive powered by a [SharePoint][] document library.</span></span>
<span data-ttu-id="dc952-109">但是 OneDrive 的灵活性可使用户以最佳的方式进行协作。</span><span class="sxs-lookup"><span data-stu-id="dc952-109">OneDrive's flexibility lets users collaborate however it works best for them.</span></span>
<span data-ttu-id="dc952-110">用户可以共享文件链接、将文件复制或移动到团队驱动器，甚至可以将 OneDrive 文件附加到 Outlook 中的邮件消息。</span><span class="sxs-lookup"><span data-stu-id="dc952-110">Users can share links to files, copy or move files to team drives, or even attach OneDrive files to mail messages in Outlook.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/vG-hQxFHCAE]

## <a name="why-integrate-with-onedrive-file-storage-in-the-cloud"></a><span data-ttu-id="dc952-111">为什么与云中的 OneDrive 文件存储集成？</span><span class="sxs-lookup"><span data-stu-id="dc952-111">Why integrate with OneDrive file storage in the cloud?</span></span>

### <a name="tap-into-an-ecosystem-with-billions-of-files"></a><span data-ttu-id="dc952-112">利用一个包含数十亿个文件的生态系统</span><span class="sxs-lookup"><span data-stu-id="dc952-112">Tap into an ecosystem with billions of files</span></span>

<span data-ttu-id="dc952-113">OneDrive 用户可从任何设备以联机或脱机方式访问他们的文件，并与其组织内外人员共享文件。</span><span class="sxs-lookup"><span data-stu-id="dc952-113">OneDrive users can access their files from any device, online or offline, and share files with people inside or outside their organization.</span></span>
<span data-ttu-id="dc952-114">OneDrive 可以在 Word、Excel 和 PowerPoint 等熟悉的应用中实现实时共同创作功能。</span><span class="sxs-lookup"><span data-stu-id="dc952-114">OneDrive enables real-time coauthoring in familiar apps like Word, Excel, and PowerPoint.</span></span>
<span data-ttu-id="dc952-115">通过 Microsoft Graph 提供支持的数百种格式、视频流、分析等丰富的缩略图呈现文件。</span><span class="sxs-lookup"><span data-stu-id="dc952-115">Files light up with rich thumbnails for hundreds of formats, video streaming, analytics, and more, powered by Microsoft Graph.</span></span>
<span data-ttu-id="dc952-116">OneDrive 中的数据受到客户信任的高级加密、合规性和安全性功能的保护。</span><span class="sxs-lookup"><span data-stu-id="dc952-116">Data in OneDrive is protected with advanced encryption, compliance, and security features that customers trust.</span></span>

<span data-ttu-id="dc952-117">有超过 5 亿的设备运行 OneDrive 应用，超过 85% 的财富 500 强企业使用 OneDrive for Business，通过将应用与 OneDrive 集成，你可以与数以百万计的消费者、学生和商业用户建立联系，并与每天都在其中工作的客户进行互动。</span><span class="sxs-lookup"><span data-stu-id="dc952-117">With over 500 million devices running the OneDrive app and over 85% of the Fortune 500 using OneDrive for Business, by integrating your app with OneDrive, you can connect with millions of consumers, students, and business users and engage with customers where they already do their work every day.</span></span>

### <a name="store-your-apps-files-in-a-powerful-cloud"></a><span data-ttu-id="dc952-118">将应用文件存储在功能强大的云中</span><span class="sxs-lookup"><span data-stu-id="dc952-118">Store your app's files in a powerful cloud</span></span>

<span data-ttu-id="dc952-119">当你将文件存储在 OneDrive 中时，应用可以利用 Microsoft 云的功能，且你的用户可以在任何地方访问他们的文件。</span><span class="sxs-lookup"><span data-stu-id="dc952-119">When you store your files in OneDrive, your app can take advantage of the features of the Microsoft cloud and your users can access their files anywhere.</span></span>
<span data-ttu-id="dc952-120">通过[文件选择器][] SDK，可以使用 OneDrive 用户熟悉的相同体验，快速打开、下载、保存或共享存储在 OneDrive 中的文件。</span><span class="sxs-lookup"><span data-stu-id="dc952-120">Use the [file picker][] SDK to quickly open, download, save, or share files stored in OneDrive from within your own app, using the same experience OneDrive users are familiar with.</span></span>
<span data-ttu-id="dc952-121">从选取器 SDK 中直接获取关于选定文件的信息，或者直接使用 Microsoft Graph API 与文件进行更深入的交互。</span><span class="sxs-lookup"><span data-stu-id="dc952-121">Get information about selected files directly from the picker SDK, or use Microsoft Graph APIs directly to interact more deeply with files.</span></span>
<span data-ttu-id="dc952-122">使用[][]“特殊文件夹”将文件存储在 OneDrive 上的已知位置，如 `Documents` 和 `Camera Roll`，或者为你的应用提供其自己的个人文件夹。</span><span class="sxs-lookup"><span data-stu-id="dc952-122">Use [special folders][] to store files in well-known locations on OneDrive, like `Documents` and `Camera Roll`, or give your app its own personal folder.</span></span>

### <a name="bring-your-app-straight-to-users-within-onedrive"></a><span data-ttu-id="dc952-123">在 OneDrive 中直接向用户提供你的应用</span><span class="sxs-lookup"><span data-stu-id="dc952-123">Bring your app straight to users within OneDrive</span></span>

<span data-ttu-id="dc952-124">OneDrive 客户可以直接在 OneDrive 中使用或启动你的应用，以打开、编辑或预览文件。</span><span class="sxs-lookup"><span data-stu-id="dc952-124">OneDrive customers can use or launch your app directly from within OneDrive to open, edit, or preview files.</span></span>
<span data-ttu-id="dc952-125">使用 OneDrive 的[文件处理程序][]扩展，为你自己的自定义文件扩展名提供图标和预览，将你的应用添加到“新建”\*\*\*\* 按钮，甚至可以将你自己的自定义操作添加到菜单栏以启动应用。</span><span class="sxs-lookup"><span data-stu-id="dc952-125">Use OneDrive's [file handler][] extensions to provide icons and previews for your own custom file extensions, add your app to the **New** button or even add your own custom actions to the menu bar to launch your app.</span></span>

### <a name="work-with-content-in-formats-your-app-understands"></a><span data-ttu-id="dc952-126">使用应用理解的格式来处理内容</span><span class="sxs-lookup"><span data-stu-id="dc952-126">Work with content in formats your app understands</span></span>

<span data-ttu-id="dc952-127">应用可以以最方便的格式获取文件内容。</span><span class="sxs-lookup"><span data-stu-id="dc952-127">Your app can get file content in the format that is most convenient for you.</span></span>
<span data-ttu-id="dc952-128">应用可以显示数百种不同文件格式的自定义大小的“缩略图”[][]。</span><span class="sxs-lookup"><span data-stu-id="dc952-128">Your app can display custom-sized [thumbnails][] for hundreds of different file formats.</span></span>
<span data-ttu-id="dc952-129">你可以下载各种不同“格式”[][]的文件，如 PDF。</span><span class="sxs-lookup"><span data-stu-id="dc952-129">You can download files in a variety of alternative [formats][], like PDF.</span></span>
<span data-ttu-id="dc952-130">甚至可以在应用中使用[][]预览 API (beta) 嵌入的 OneDrive 文件预览程序。</span><span class="sxs-lookup"><span data-stu-id="dc952-130">You can even embed the OneDrive file previewers within your app by using the [preview][] API (beta).</span></span>

### <a name="work-with-file-content-and-metadata-without-downloading-the-binary"></a><span data-ttu-id="dc952-131">在不下载二进制文件的情况下使用文件内容和元数据</span><span class="sxs-lookup"><span data-stu-id="dc952-131">Work with file content and metadata without downloading the binary</span></span>

<span data-ttu-id="dc952-132">使用 Microsoft Graph，可以通过 REST API 访问丰富的内容，而无需下载二进制文件。</span><span class="sxs-lookup"><span data-stu-id="dc952-132">With Microsoft Graph, you can access rich content through REST APIs without having to download the binary.</span></span>
<span data-ttu-id="dc952-133">在[][]“照片”、[][]“音频”和[][]“视频”文件中探索提取的元数据。</span><span class="sxs-lookup"><span data-stu-id="dc952-133">Explore extracted metadata from [photo][], [audio][], and [video][] files.</span></span>
<span data-ttu-id="dc952-134">使用 Excel API[][] 可直接使用存储在 Excel 工作簿中的原始数据。</span><span class="sxs-lookup"><span data-stu-id="dc952-134">Use the [Excel API][] to work directly with the raw data stored in an Excel workbook.</span></span>
<span data-ttu-id="dc952-135">使用[][]注释 API 可访问 OneNote 笔记本内容。</span><span class="sxs-lookup"><span data-stu-id="dc952-135">Use the [Notes API][] to access the contents of OneNote notebooks.</span></span>

### <a name="react-to-file-changes"></a><span data-ttu-id="dc952-136">对文件更改做出反应</span><span class="sxs-lookup"><span data-stu-id="dc952-136">React to file changes</span></span>

<span data-ttu-id="dc952-137">通过 webhooks[][]，当文件发生更改时你将收到通知，以此可以快速做出响应。</span><span class="sxs-lookup"><span data-stu-id="dc952-137">With [webhooks][], your app can get notified when files change so you can quickly react.</span></span>
<span data-ttu-id="dc952-138">[delta API][] 可用于查看自上次应用与云同步以来发生的更改。</span><span class="sxs-lookup"><span data-stu-id="dc952-138">Use the [delta API][] to see what changed since the last time your app synchronized with the cloud.</span></span>

## <a name="api-reference"></a><span data-ttu-id="dc952-139">API 参考</span><span class="sxs-lookup"><span data-stu-id="dc952-139">API reference</span></span>
<span data-ttu-id="dc952-140">在查找此服务的 API 参考？</span><span class="sxs-lookup"><span data-stu-id="dc952-140">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="dc952-141">Microsoft Graph v1.0 中的 OneDrive 文件存储 API</span><span class="sxs-lookup"><span data-stu-id="dc952-141">OneDrive file storage API in Microsoft Graph v1.0</span></span>](/graph/api/resources/onedrive?view=graph-rest-1.0)
- [<span data-ttu-id="dc952-142">Microsoft Graph beta 中的 OneDrive 文件存储 API</span><span class="sxs-lookup"><span data-stu-id="dc952-142">OneDrive file storage API in Microsoft Graph beta</span></span>](/graph/api/resources/onedrive?view=graph-rest-beta)

## <a name="next-steps"></a><span data-ttu-id="dc952-143">后续步骤</span><span class="sxs-lookup"><span data-stu-id="dc952-143">Next steps</span></span>

<span data-ttu-id="dc952-144">详细了解如何在 Microsoft Graph v1.0 中[使用 OneDrive API][Drive API]。</span><span class="sxs-lookup"><span data-stu-id="dc952-144">Find out more about [using the OneDrive API][Drive API] in Microsoft Graph v1.0.</span></span>

[SharePoint]: sharepoint-concept-overview.md
[文件选取器]: https://dev.onedrive.com/sdk/js-v72/js-picker-overview.htm
[file picker]: https://dev.onedrive.com/sdk/js-v72/js-picker-overview.htm
[文件处理程序]: https://docs.microsoft.com/onedrive/developer/file-handlers
[file handler]: https://docs.microsoft.com/onedrive/developer/file-handlers
[特殊文件夹]: /graph/api/drive-get-specialfolder?view=graph-rest-1.0
[special folders]: /graph/api/drive-get-specialfolder?view=graph-rest-1.0
[注释 API]: integrate-with-onenote.md
[Notes API]: integrate-with-onenote.md
[Excel API]: /graph/api/resources/excel?view=graph-rest-1.0
[REST API]: /graph/api/resources/onedrive?view=graph-rest-1.0
[增量 API]: /graph/api/driveitem-delta?view=graph-rest-1.0
[delta API]: /graph/api/driveitem-delta?view=graph-rest-1.0
[视频]: /graph/api/resources/video?view=graph-rest-1.0
[video]: /graph/api/resources/video?view=graph-rest-1.0
[照片]: /graph/api/resources/photo?view=graph-rest-1.0
[photo]: /graph/api/resources/photo?view=graph-rest-1.0
[音频]: /graph/api/resources/audio?view=graph-rest-1.0
[audio]: /graph/api/resources/audio?view=graph-rest-1.0
[格式]: /graph/api/driveitem-get-content-format?view=graph-rest-1.0
[formats]: /graph/api/driveitem-get-content-format?view=graph-rest-1.0
[缩略图]: /graph/api/driveitem-list-thumbnails?view=graph-rest-1.0
[thumbnails]: /graph/api/driveitem-list-thumbnails?view=graph-rest-1.0
[预览]: /graph/api/driveitem-preview?view=graph-rest-beta
[preview]: /graph/api/driveitem-preview?view=graph-rest-beta
[webhooks]: /graph/api/resources/webhooks?view=graph-rest-1.0
[Drive API]: /graph/api/resources/onedrive?view=graph-rest-1.0
