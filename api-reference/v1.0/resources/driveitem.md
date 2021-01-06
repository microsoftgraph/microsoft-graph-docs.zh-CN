---
author: JeremyKelley
title: DriveItem 资源类型
description: 项目是 OneDrive API 中的主数据模型。 每项都是一个项目。
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f4fc16e311a696c10076588023945064f76ee3dc
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49752774"
---
# <a name="driveitem-resource-type"></a><span data-ttu-id="dcb37-104">DriveItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="dcb37-104">driveItem resource type</span></span>

<span data-ttu-id="dcb37-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dcb37-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dcb37-106">**driveItem** 资源代表文件、文件夹或存储在驱动器中的 其他项。</span><span class="sxs-lookup"><span data-stu-id="dcb37-106">The **driveItem** resource represents a file, folder, or other item stored in a drive.</span></span>

<span data-ttu-id="dcb37-107">OneDrive 和 SharePoint 中的所有文件系统对象将作为 **driveItem** 资源返回。</span><span class="sxs-lookup"><span data-stu-id="dcb37-107">All file system objects in OneDrive and SharePoint are returned as **driveItem** resources.</span></span> <span data-ttu-id="dcb37-108">SharePoint 文档库中的项目可以表示为 [listItem][] 或 **driveItem** 资源。</span><span class="sxs-lookup"><span data-stu-id="dcb37-108">Items in SharePoint document libraries can be represented as [listItem][] or **driveItem** resources.</span></span>

<span data-ttu-id="dcb37-109">**driveItem** 资源的寻址方式主要有两种：</span><span class="sxs-lookup"><span data-stu-id="dcb37-109">There are two primary ways of addressing a **driveItem** resource:</span></span>

* <span data-ttu-id="dcb37-110">通过 **driveItem** 唯一标识符使用 `drive/items/{item-id}` 的方式</span><span class="sxs-lookup"><span data-stu-id="dcb37-110">By the **driveItem** unique identifier using `drive/items/{item-id}`</span></span>
* <span data-ttu-id="dcb37-111">通过使用文件系统路径 `/drive/root:/path/to/file` 的方式</span><span class="sxs-lookup"><span data-stu-id="dcb37-111">By file system path using `/drive/root:/path/to/file`</span></span>

<span data-ttu-id="dcb37-112">**DriveItem** 资源具有多个建模为属性的 Facet，用于提供 driveItem 的标识和功能相关数据。</span><span class="sxs-lookup"><span data-stu-id="dcb37-112">**driveItem** resources have facets modeled as properties that provide data about the driveItem's identities and capabilities.</span></span>
<span data-ttu-id="dcb37-113">例如：</span><span class="sxs-lookup"><span data-stu-id="dcb37-113">For example:</span></span>

* <span data-ttu-id="dcb37-114">文件夹具有 [**folder facet**][folder]</span><span class="sxs-lookup"><span data-stu-id="dcb37-114">Folders have a [**folder facet**][folder]</span></span>
* <span data-ttu-id="dcb37-115">文件具有 [**file facet**][file]。</span><span class="sxs-lookup"><span data-stu-id="dcb37-115">Files have a [**file facet**][file].</span></span>
* <span data-ttu-id="dcb37-116">除了 file facet 之外，图像还具有 [**image facet**][image]。</span><span class="sxs-lookup"><span data-stu-id="dcb37-116">Images have an [**image facet**][image] in addition to their file facet.</span></span>
* <span data-ttu-id="dcb37-117">使用照相机拍摄的图像（照片）具有 [**photo facet**][photo]，用于将项标识为照片，并提供照片的拍摄时间和拍摄所用设备等属性。</span><span class="sxs-lookup"><span data-stu-id="dcb37-117">Images taken with a camera (photos) have a [**photo facet**][photo] that identifies the item as a photo and provides the properties of when the photo was taken and with what device.</span></span>

<span data-ttu-id="dcb37-118">具有 **文件夹** Facet 的项目充当项目的容器，因此具有指向文件夹下的 **driveItems** 集合的 `children` 引用。</span><span class="sxs-lookup"><span data-stu-id="dcb37-118">Items with the **folder** facet act as containers of items and therefore have a `children` reference pointing to a collection of **driveItems** under the folder.</span></span>

><span data-ttu-id="dcb37-119">**注意：** 在 OneDrive for Business 或 SharePoint 文档库中，如果 **driveItem** 具有 [folder][] Facet，则不返回 **cTag** 属性。</span><span class="sxs-lookup"><span data-stu-id="dcb37-119">**Note:** In OneDrive for Business or SharePoint document libraries, the **cTag** property is not returned, if the **driveItem** has a [folder][] facet.</span></span>

## <a name="properties"></a><span data-ttu-id="dcb37-120">属性</span><span class="sxs-lookup"><span data-stu-id="dcb37-120">Properties</span></span>

| <span data-ttu-id="dcb37-121">属性</span><span class="sxs-lookup"><span data-stu-id="dcb37-121">Property</span></span>             | <span data-ttu-id="dcb37-122">类型</span><span class="sxs-lookup"><span data-stu-id="dcb37-122">Type</span></span>               | <span data-ttu-id="dcb37-123">说明</span><span class="sxs-lookup"><span data-stu-id="dcb37-123">Description</span></span>
|:---------------------|:-------------------|:---------------------------------
| <span data-ttu-id="dcb37-124">audio</span><span class="sxs-lookup"><span data-stu-id="dcb37-124">audio</span></span>                | <span data-ttu-id="dcb37-125">[audio][]</span><span class="sxs-lookup"><span data-stu-id="dcb37-125">[audio][]</span></span>          | <span data-ttu-id="dcb37-p104">音频元数据（如果此项是一个音频文件）。只读。</span><span class="sxs-lookup"><span data-stu-id="dcb37-p104">Audio metadata, if the item is an audio file. Read-only.</span></span>
| <span data-ttu-id="dcb37-128">content</span><span class="sxs-lookup"><span data-stu-id="dcb37-128">content</span></span>              | <span data-ttu-id="dcb37-129">流</span><span class="sxs-lookup"><span data-stu-id="dcb37-129">Stream</span></span>             | <span data-ttu-id="dcb37-130">内容流（如果此项表示一个文件）。</span><span class="sxs-lookup"><span data-stu-id="dcb37-130">The content stream, if the item represents a file.</span></span>
| <span data-ttu-id="dcb37-131">createdBy</span><span class="sxs-lookup"><span data-stu-id="dcb37-131">createdBy</span></span>            | <span data-ttu-id="dcb37-132">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="dcb37-132">[identitySet][]</span></span>    | <span data-ttu-id="dcb37-p105">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="dcb37-p105">Identity of the user, device, and application which created the item. Read-only.</span></span>
| <span data-ttu-id="dcb37-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dcb37-135">createdDateTime</span></span>      | <span data-ttu-id="dcb37-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dcb37-136">DateTimeOffset</span></span>     | <span data-ttu-id="dcb37-p106">创建项的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="dcb37-p106">Date and time of item creation. Read-only.</span></span>
| <span data-ttu-id="dcb37-139">cTag</span><span class="sxs-lookup"><span data-stu-id="dcb37-139">cTag</span></span>                 | <span data-ttu-id="dcb37-140">String</span><span class="sxs-lookup"><span data-stu-id="dcb37-140">String</span></span>             | <span data-ttu-id="dcb37-p107">项目内容的 eTag。如果只有元数据更改，此 eTag 不会更改。**注意** 如果项目是文件夹，则不返回此属性。只读。</span><span class="sxs-lookup"><span data-stu-id="dcb37-p107">An eTag for the content of the item. This eTag is not changed if only the metadata is changed. **Note** This property is not returned if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="dcb37-145">deleted</span><span class="sxs-lookup"><span data-stu-id="dcb37-145">deleted</span></span>              | <span data-ttu-id="dcb37-146">[deleted][]</span><span class="sxs-lookup"><span data-stu-id="dcb37-146">[deleted][]</span></span>        | <span data-ttu-id="dcb37-p108">有关项目删除状态的信息。只读。</span><span class="sxs-lookup"><span data-stu-id="dcb37-p108">Information about the deleted state of the item. Read-only.</span></span>
| <span data-ttu-id="dcb37-149">description</span><span class="sxs-lookup"><span data-stu-id="dcb37-149">description</span></span>          | <span data-ttu-id="dcb37-150">字符串</span><span class="sxs-lookup"><span data-stu-id="dcb37-150">String</span></span>             | <span data-ttu-id="dcb37-p109">提供项的用户可见的说明。读写。仅在 OneDrive 个人版上</span><span class="sxs-lookup"><span data-stu-id="dcb37-p109">Provides a user-visible description of the item. Read-write. Only on OneDrive Personal</span></span>
| <span data-ttu-id="dcb37-154">eTag</span><span class="sxs-lookup"><span data-stu-id="dcb37-154">eTag</span></span>                 | <span data-ttu-id="dcb37-155">String</span><span class="sxs-lookup"><span data-stu-id="dcb37-155">String</span></span>             | <span data-ttu-id="dcb37-p110">整个项目（元数据和内容）的 eTag。只读。</span><span class="sxs-lookup"><span data-stu-id="dcb37-p110">eTag for the entire item (metadata + content). Read-only.</span></span>
| <span data-ttu-id="dcb37-158">file</span><span class="sxs-lookup"><span data-stu-id="dcb37-158">file</span></span>                 | <span data-ttu-id="dcb37-159">[file][]</span><span class="sxs-lookup"><span data-stu-id="dcb37-159">[file][]</span></span>           | <span data-ttu-id="dcb37-p111">文件元数据（如果此项是一个文件）。只读。</span><span class="sxs-lookup"><span data-stu-id="dcb37-p111">File metadata, if the item is a file. Read-only.</span></span>
| <span data-ttu-id="dcb37-162">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="dcb37-162">fileSystemInfo</span></span>       | <span data-ttu-id="dcb37-163">[fileSystemInfo][]</span><span class="sxs-lookup"><span data-stu-id="dcb37-163">[fileSystemInfo][]</span></span> | <span data-ttu-id="dcb37-p112">客户端上的文件系统信息。读写。</span><span class="sxs-lookup"><span data-stu-id="dcb37-p112">File system information on client. Read-write.</span></span>
| <span data-ttu-id="dcb37-166">folder</span><span class="sxs-lookup"><span data-stu-id="dcb37-166">folder</span></span>               | <span data-ttu-id="dcb37-167">[folder][]</span><span class="sxs-lookup"><span data-stu-id="dcb37-167">[folder][]</span></span>         | <span data-ttu-id="dcb37-p113">文件夹元数据（如果此项是一个文件夹）。只读。</span><span class="sxs-lookup"><span data-stu-id="dcb37-p113">Folder metadata, if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="dcb37-170">id</span><span class="sxs-lookup"><span data-stu-id="dcb37-170">id</span></span>                   | <span data-ttu-id="dcb37-171">String</span><span class="sxs-lookup"><span data-stu-id="dcb37-171">String</span></span>             | <span data-ttu-id="dcb37-p114">项在驱动器中的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="dcb37-p114">The unique identifier of the item within the Drive. Read-only.</span></span>
| <span data-ttu-id="dcb37-174">image</span><span class="sxs-lookup"><span data-stu-id="dcb37-174">image</span></span>                | <span data-ttu-id="dcb37-175">[image][]</span><span class="sxs-lookup"><span data-stu-id="dcb37-175">[image][]</span></span>          | <span data-ttu-id="dcb37-p115">图像元数据（如果此项是一个图像）。只读。</span><span class="sxs-lookup"><span data-stu-id="dcb37-p115">Image metadata, if the item is an image. Read-only.</span></span>
| <span data-ttu-id="dcb37-178">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="dcb37-178">lastModifiedBy</span></span>       | <span data-ttu-id="dcb37-179">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="dcb37-179">[identitySet][]</span></span>    | <span data-ttu-id="dcb37-p116">上次修改项目的用户、设备和应用程序的标识。只读。</span><span class="sxs-lookup"><span data-stu-id="dcb37-p116">Identity of the user, device, and application which last modified the item. Read-only.</span></span>
| <span data-ttu-id="dcb37-182">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dcb37-182">lastModifiedDateTime</span></span> | <span data-ttu-id="dcb37-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dcb37-183">DateTimeOffset</span></span>     | <span data-ttu-id="dcb37-p117">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="dcb37-p117">Date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="dcb37-186">location</span><span class="sxs-lookup"><span data-stu-id="dcb37-186">location</span></span>             | <span data-ttu-id="dcb37-187">[geoCoordinates][]</span><span class="sxs-lookup"><span data-stu-id="dcb37-187">[geoCoordinates][]</span></span> | <span data-ttu-id="dcb37-p118">位置元数据（如果此项包含位置数据）。只读。</span><span class="sxs-lookup"><span data-stu-id="dcb37-p118">Location metadata, if the item has location data. Read-only.</span></span>
| <span data-ttu-id="dcb37-190">name</span><span class="sxs-lookup"><span data-stu-id="dcb37-190">name</span></span>                 | <span data-ttu-id="dcb37-191">String</span><span class="sxs-lookup"><span data-stu-id="dcb37-191">String</span></span>             | <span data-ttu-id="dcb37-p119">项目名称（文件名和扩展名）。读写。</span><span class="sxs-lookup"><span data-stu-id="dcb37-p119">The name of the item (filename and extension). Read-write.</span></span>
| <span data-ttu-id="dcb37-194">package</span><span class="sxs-lookup"><span data-stu-id="dcb37-194">package</span></span>              | <span data-ttu-id="dcb37-195">[package][]</span><span class="sxs-lookup"><span data-stu-id="dcb37-195">[package][]</span></span>        | <span data-ttu-id="dcb37-p120">如果存在，则表示此项是一个包，而不是文件夹或文件。包被视为某些上下文中的文件和其他上下文中的文件夹。只读。</span><span class="sxs-lookup"><span data-stu-id="dcb37-p120">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span>
| <span data-ttu-id="dcb37-199">parentReference</span><span class="sxs-lookup"><span data-stu-id="dcb37-199">parentReference</span></span>      | <span data-ttu-id="dcb37-200">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="dcb37-200">[itemReference][]</span></span>  | <span data-ttu-id="dcb37-p121">父信息（如果此项具有父级）。读写。</span><span class="sxs-lookup"><span data-stu-id="dcb37-p121">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="dcb37-203">pendingOperations</span><span class="sxs-lookup"><span data-stu-id="dcb37-203">pendingOperations</span></span>    | <span data-ttu-id="dcb37-204">[pendingOperations][]</span><span class="sxs-lookup"><span data-stu-id="dcb37-204">[pendingOperations][]</span></span> | <span data-ttu-id="dcb37-205">如果存在，则表示可能影响 driveItem 状态的一个或多个操作正在等待完成。</span><span class="sxs-lookup"><span data-stu-id="dcb37-205">If present, indicates that one or more operations that might affect the state of the driveItem are pending completion.</span></span> <span data-ttu-id="dcb37-206">只读。</span><span class="sxs-lookup"><span data-stu-id="dcb37-206">Read-only.</span></span>
| <span data-ttu-id="dcb37-207">photo</span><span class="sxs-lookup"><span data-stu-id="dcb37-207">photo</span></span>                | <span data-ttu-id="dcb37-208">[照片][]</span><span class="sxs-lookup"><span data-stu-id="dcb37-208">[photo][]</span></span>          | <span data-ttu-id="dcb37-p123">照片元数据（如果此项包含照片）。只读。</span><span class="sxs-lookup"><span data-stu-id="dcb37-p123">Photo metadata, if the item is a photo. Read-only.</span></span>
| <span data-ttu-id="dcb37-211">publication</span><span class="sxs-lookup"><span data-stu-id="dcb37-211">publication</span></span>          | <span data-ttu-id="dcb37-212">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="dcb37-212">[publicationFacet][]</span></span> | <span data-ttu-id="dcb37-213">在支持此类操作的位置提供有关某个项目的已发布或签出状态信息。</span><span class="sxs-lookup"><span data-stu-id="dcb37-213">Provides information about the published or checked-out state of an item, in locations that support such actions.</span></span> <span data-ttu-id="dcb37-214">默认情况下，不会返回此属性。</span><span class="sxs-lookup"><span data-stu-id="dcb37-214">This property is not returned by default.</span></span> <span data-ttu-id="dcb37-215">只读。</span><span class="sxs-lookup"><span data-stu-id="dcb37-215">Read-only.</span></span> |
| <span data-ttu-id="dcb37-216">remoteItem</span><span class="sxs-lookup"><span data-stu-id="dcb37-216">remoteItem</span></span>           | <span data-ttu-id="dcb37-217">[remoteItem][]</span><span class="sxs-lookup"><span data-stu-id="dcb37-217">[remoteItem][]</span></span>     | <span data-ttu-id="dcb37-p125">远程项目数据（如果此项是从驱动器共享的项目，而不是被访问的项目）。只读。</span><span class="sxs-lookup"><span data-stu-id="dcb37-p125">Remote item data, if the item is shared from a drive other than the one being accessed. Read-only.</span></span>
| <span data-ttu-id="dcb37-220">root</span><span class="sxs-lookup"><span data-stu-id="dcb37-220">root</span></span>                 | <span data-ttu-id="dcb37-221">[root][]</span><span class="sxs-lookup"><span data-stu-id="dcb37-221">[root][]</span></span>           | <span data-ttu-id="dcb37-222">如果此属性为非 NULL，则表明 driveItem 是驱动器中最上面的 driveItem。</span><span class="sxs-lookup"><span data-stu-id="dcb37-222">If this property is non-null, it indicates that the driveItem is the top-most driveItem in the drive.</span></span>
| <span data-ttu-id="dcb37-223">searchResult</span><span class="sxs-lookup"><span data-stu-id="dcb37-223">searchResult</span></span>         | <span data-ttu-id="dcb37-224">[searchResult][]</span><span class="sxs-lookup"><span data-stu-id="dcb37-224">[searchResult][]</span></span>   | <span data-ttu-id="dcb37-p126">搜索元数据（如果此项目来自搜索结果）。只读。</span><span class="sxs-lookup"><span data-stu-id="dcb37-p126">Search metadata, if the item is from a search result. Read-only.</span></span>
| <span data-ttu-id="dcb37-227">shared</span><span class="sxs-lookup"><span data-stu-id="dcb37-227">shared</span></span>               | <span data-ttu-id="dcb37-228">[shared][]</span><span class="sxs-lookup"><span data-stu-id="dcb37-228">[shared][]</span></span>         | <span data-ttu-id="dcb37-p127">表示此项已与他人共享，并提供有关项目共享状态的信息。只读。</span><span class="sxs-lookup"><span data-stu-id="dcb37-p127">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>
| <span data-ttu-id="dcb37-231">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="dcb37-231">sharepointIds</span></span>        | <span data-ttu-id="dcb37-232">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="dcb37-232">[sharepointIds][]</span></span>  | <span data-ttu-id="dcb37-p128">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="dcb37-p128">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="dcb37-235">size</span><span class="sxs-lookup"><span data-stu-id="dcb37-235">size</span></span>                 | <span data-ttu-id="dcb37-236">Int64</span><span class="sxs-lookup"><span data-stu-id="dcb37-236">Int64</span></span>              | <span data-ttu-id="dcb37-p129">项目大小，以字节为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="dcb37-p129">Size of the item in bytes. Read-only.</span></span>
| <span data-ttu-id="dcb37-239">specialFolder</span><span class="sxs-lookup"><span data-stu-id="dcb37-239">specialFolder</span></span>        | <span data-ttu-id="dcb37-240">[specialFolder][]</span><span class="sxs-lookup"><span data-stu-id="dcb37-240">[specialFolder][]</span></span>  | <span data-ttu-id="dcb37-p130">如果当前项同时也是一个特殊的文件夹，则返回此 facet。只读。</span><span class="sxs-lookup"><span data-stu-id="dcb37-p130">If the current item is also available as a special folder, this facet is returned. Read-only.</span></span>
| <span data-ttu-id="dcb37-243">video</span><span class="sxs-lookup"><span data-stu-id="dcb37-243">video</span></span>                | <span data-ttu-id="dcb37-244">[video][]</span><span class="sxs-lookup"><span data-stu-id="dcb37-244">[video][]</span></span>          | <span data-ttu-id="dcb37-p131">视频元数据（如果此项是一个视频）。只读。</span><span class="sxs-lookup"><span data-stu-id="dcb37-p131">Video metadata, if the item is a video. Read-only.</span></span>
| <span data-ttu-id="dcb37-247">WebDavUrl</span><span class="sxs-lookup"><span data-stu-id="dcb37-247">webDavUrl</span></span>            | <span data-ttu-id="dcb37-248">String</span><span class="sxs-lookup"><span data-stu-id="dcb37-248">String</span></span>             | <span data-ttu-id="dcb37-249">项的可兼容 WebDAV 的 URL。</span><span class="sxs-lookup"><span data-stu-id="dcb37-249">WebDAV compatible URL for the item.</span></span>
| <span data-ttu-id="dcb37-250">WebUrl</span><span class="sxs-lookup"><span data-stu-id="dcb37-250">webUrl</span></span>               | <span data-ttu-id="dcb37-251">String</span><span class="sxs-lookup"><span data-stu-id="dcb37-251">String</span></span>             | <span data-ttu-id="dcb37-p132">在浏览器中显示此资源的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="dcb37-p132">URL that displays the resource in the browser. Read-only.</span></span>

><span data-ttu-id="dcb37-p133">**注意：** ETag 和 cTag 属性在容器（文件夹）中以不同的方式工作。更改任意文件夹后代的内容或元数据时，也会修改 CTag 值。除了从后代派生的属性（例如 **childCount** 或 **lastModifiedDateTime**），仅在更改文件夹的属性时修改 eTag 值。</span><span class="sxs-lookup"><span data-stu-id="dcb37-p133">**Note:** The eTag and cTag properties work differently on containers (folders). The cTag value is modified when content or metadata of any descendant of the folder is changed. The eTag value is only modified when the folder's properties are changed, except for properties that are derived from descendants (like **childCount** or **lastModifiedDateTime**).</span></span>

## <a name="relationships"></a><span data-ttu-id="dcb37-257">关系</span><span class="sxs-lookup"><span data-stu-id="dcb37-257">Relationships</span></span>

| <span data-ttu-id="dcb37-258">关系</span><span class="sxs-lookup"><span data-stu-id="dcb37-258">Relationship</span></span>       | <span data-ttu-id="dcb37-259">类型</span><span class="sxs-lookup"><span data-stu-id="dcb37-259">Type</span></span>                        | <span data-ttu-id="dcb37-260">说明</span><span class="sxs-lookup"><span data-stu-id="dcb37-260">Description</span></span>
|:-------------------|:----------------------------|:--------------------------
| <span data-ttu-id="dcb37-261">activities</span><span class="sxs-lookup"><span data-stu-id="dcb37-261">activities</span></span>         | <span data-ttu-id="dcb37-262">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="dcb37-262">[itemActivity][] collection</span></span> | <span data-ttu-id="dcb37-263">最近发生在此项上的活动的列表。</span><span class="sxs-lookup"><span data-stu-id="dcb37-263">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="dcb37-264">分析</span><span class="sxs-lookup"><span data-stu-id="dcb37-264">analytics</span></span>          | <span data-ttu-id="dcb37-265">[itemAnalytics][] 资源</span><span class="sxs-lookup"><span data-stu-id="dcb37-265">[itemAnalytics][] resource</span></span>  | <span data-ttu-id="dcb37-266">此项目上发生的查看活动的相关分析。</span><span class="sxs-lookup"><span data-stu-id="dcb37-266">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="dcb37-267">children</span><span class="sxs-lookup"><span data-stu-id="dcb37-267">children</span></span>           | <span data-ttu-id="dcb37-268">driveItem 集合</span><span class="sxs-lookup"><span data-stu-id="dcb37-268">driveItem collection</span></span>        | <span data-ttu-id="dcb37-p134">包含项目直接子项的 Item 对象的集合。仅表示文件夹的项目包含子项。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="dcb37-p134">Collection containing Item objects for the immediate children of Item. Only items representing folders have children. Read-only. Nullable.</span></span>
| <span data-ttu-id="dcb37-273">createdByUser</span><span class="sxs-lookup"><span data-stu-id="dcb37-273">createdByUser</span></span>      | <span data-ttu-id="dcb37-274">[user][]</span><span class="sxs-lookup"><span data-stu-id="dcb37-274">[user][]</span></span>                    | <span data-ttu-id="dcb37-275">创建了项的用户的身份。</span><span class="sxs-lookup"><span data-stu-id="dcb37-275">Identity of the user who created the item.</span></span> <span data-ttu-id="dcb37-276">只读。</span><span class="sxs-lookup"><span data-stu-id="dcb37-276">Read-only.</span></span>
| <span data-ttu-id="dcb37-277">lastModifiedByUser</span><span class="sxs-lookup"><span data-stu-id="dcb37-277">lastModifiedByUser</span></span> | <span data-ttu-id="dcb37-278">[user][]</span><span class="sxs-lookup"><span data-stu-id="dcb37-278">[user][]</span></span>                    | <span data-ttu-id="dcb37-279">上次修改项的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="dcb37-279">Identity of the user who last modified the item.</span></span> <span data-ttu-id="dcb37-280">只读。</span><span class="sxs-lookup"><span data-stu-id="dcb37-280">Read-only.</span></span>
| <span data-ttu-id="dcb37-281">listItem</span><span class="sxs-lookup"><span data-stu-id="dcb37-281">listItem</span></span>           | <span data-ttu-id="dcb37-282">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="dcb37-282">[listItem][]</span></span>                | <span data-ttu-id="dcb37-283">对于 SharePoint 中的驱动器，关联的文档库列表项。</span><span class="sxs-lookup"><span data-stu-id="dcb37-283">For drives in SharePoint, the associated document library list item.</span></span> <span data-ttu-id="dcb37-284">只读。</span><span class="sxs-lookup"><span data-stu-id="dcb37-284">Read-only.</span></span> <span data-ttu-id="dcb37-285">可为 null。</span><span class="sxs-lookup"><span data-stu-id="dcb37-285">Nullable.</span></span>
| <span data-ttu-id="dcb37-286">permissions</span><span class="sxs-lookup"><span data-stu-id="dcb37-286">permissions</span></span>        | <span data-ttu-id="dcb37-287">[permission][] 集合</span><span class="sxs-lookup"><span data-stu-id="dcb37-287">[permission][] collection</span></span>   | <span data-ttu-id="dcb37-p138">项目的权限集。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="dcb37-p138">The set of permissions for the item. Read-only. Nullable.</span></span>
| <span data-ttu-id="dcb37-291">订阅</span><span class="sxs-lookup"><span data-stu-id="dcb37-291">subscriptions</span></span>      | <span data-ttu-id="dcb37-292">[订阅][]集合</span><span class="sxs-lookup"><span data-stu-id="dcb37-292">[subscription][] collection</span></span> | <span data-ttu-id="dcb37-293">项目上的订阅集。</span><span class="sxs-lookup"><span data-stu-id="dcb37-293">The set of subscriptions on the item.</span></span> <span data-ttu-id="dcb37-294">仅在驱动器根目录上支持。</span><span class="sxs-lookup"><span data-stu-id="dcb37-294">Only supported on the root of a drive.</span></span>
| <span data-ttu-id="dcb37-295">缩略图</span><span class="sxs-lookup"><span data-stu-id="dcb37-295">thumbnails</span></span>         | <span data-ttu-id="dcb37-296">[thumbnailSet][] 集合</span><span class="sxs-lookup"><span data-stu-id="dcb37-296">[thumbnailSet][] collection</span></span> | <span data-ttu-id="dcb37-p140">包含与项目关联的 [ThumbnailSet][] 对象的集合。有关详细信息，请参阅 [获取缩略图][]只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="dcb37-p140">Collection containing [ThumbnailSet][] objects associated with the item. For more info, see [getting thumbnails][]. Read-only. Nullable.</span></span>
| <span data-ttu-id="dcb37-301">版本</span><span class="sxs-lookup"><span data-stu-id="dcb37-301">versions</span></span>           | <span data-ttu-id="dcb37-302">[driveItemVersion][] 集合</span><span class="sxs-lookup"><span data-stu-id="dcb37-302">[driveItemVersion][] collection</span></span> | <span data-ttu-id="dcb37-303">旧版本项的列表。</span><span class="sxs-lookup"><span data-stu-id="dcb37-303">The list of previous versions of the item.</span></span> <span data-ttu-id="dcb37-304">有关详细信息，请参阅[获取旧版本][]。</span><span class="sxs-lookup"><span data-stu-id="dcb37-304">For more info, see [getting previous versions][].</span></span> <span data-ttu-id="dcb37-305">只读。</span><span class="sxs-lookup"><span data-stu-id="dcb37-305">Read-only.</span></span> <span data-ttu-id="dcb37-306">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="dcb37-306">Nullable.</span></span>
| <span data-ttu-id="dcb37-307">工作簿</span><span class="sxs-lookup"><span data-stu-id="dcb37-307">workbook</span></span>           | <span data-ttu-id="dcb37-308">[workbook][]</span><span class="sxs-lookup"><span data-stu-id="dcb37-308">[workbook][]</span></span>                | <span data-ttu-id="dcb37-309">如果是 Excel 工作表文件，访问工作簿 API 以使用工作表的内容。</span><span class="sxs-lookup"><span data-stu-id="dcb37-309">For files that are Excel spreadsheets, accesses the workbook API to work with the spreadsheet's contents.</span></span> <span data-ttu-id="dcb37-310">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="dcb37-310">Nullable.</span></span>

## <a name="instance-attributes"></a><span data-ttu-id="dcb37-311">实例属性</span><span class="sxs-lookup"><span data-stu-id="dcb37-311">Instance Attributes</span></span>

<span data-ttu-id="dcb37-p143">实例属性是具有特殊行为的属性。这些属性是临时的，并且 a) 定义服务应执行的行为或 b) 提供短期的属性值，例如过期项目的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="dcb37-p143">Instance attributes are properties with special behaviors. These properties are temporary and either a) define behavior the service should perform or b) provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="dcb37-314">属性名称</span><span class="sxs-lookup"><span data-stu-id="dcb37-314">Property name</span></span>                     | <span data-ttu-id="dcb37-315">类型</span><span class="sxs-lookup"><span data-stu-id="dcb37-315">Type</span></span>   | <span data-ttu-id="dcb37-316">说明</span><span class="sxs-lookup"><span data-stu-id="dcb37-316">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="dcb37-317">@microsoft.graph.conflictBehavior</span><span class="sxs-lookup"><span data-stu-id="dcb37-317">@microsoft.graph.conflictBehavior</span></span> | <span data-ttu-id="dcb37-318">string</span><span class="sxs-lookup"><span data-stu-id="dcb37-318">string</span></span> | <span data-ttu-id="dcb37-p144">为创建新项目的操作解决冲突的行为。你可以使用值 *fail*、*replace* 或 *rename*。PUT 的默认值是 *replace*。绝不会返回包含该批注的项目。只写。</span><span class="sxs-lookup"><span data-stu-id="dcb37-p144">The conflict resolution behavior for actions that create a new item. You can use the values *fail*, *replace*, or *rename*. The default for PUT is *replace*. An item will never be returned with this annotation. Write-only.</span></span>
| <span data-ttu-id="dcb37-324">@microsoft.graph.downloadUrl</span><span class="sxs-lookup"><span data-stu-id="dcb37-324">@microsoft.graph.downloadUrl</span></span>      | <span data-ttu-id="dcb37-325">string</span><span class="sxs-lookup"><span data-stu-id="dcb37-325">string</span></span> | <span data-ttu-id="dcb37-p145">一个可用于下载此文件的内容的 URL。不需要使用此 URL 进行身份验证。只读。</span><span class="sxs-lookup"><span data-stu-id="dcb37-p145">A URL that can be used to download this file's content. Authentication is not required with this URL. Read-only.</span></span>
| <span data-ttu-id="dcb37-329">@microsoft.graph.sourceUrl</span><span class="sxs-lookup"><span data-stu-id="dcb37-329">@microsoft.graph.sourceUrl</span></span>        | <span data-ttu-id="dcb37-330">string</span><span class="sxs-lookup"><span data-stu-id="dcb37-330">string</span></span> | <span data-ttu-id="dcb37-p146">发出 PUT 请求时，此实例批注可用于指示服务下载 URL 内容并将其存储为文件。只写。</span><span class="sxs-lookup"><span data-stu-id="dcb37-p146">When issuing a PUT request, this instance annotation can be used to instruct the service to download the contents of the URL, and store it as the file. Write-only.</span></span>

><span data-ttu-id="dcb37-333">**注意：** 参数 `@microsoft.graph.conflictBehavior` 应包含在 URL 中，而不是请求正文中。</span><span class="sxs-lookup"><span data-stu-id="dcb37-333">**Notes:** The parameter `@microsoft.graph.conflictBehavior` should be included in the URL instead of the body of the request.</span></span>
>
><span data-ttu-id="dcb37-334">`@microsoft.graph.downloadUrl` 值是一个短期 URL，不能缓存。</span><span class="sxs-lookup"><span data-stu-id="dcb37-334">The `@microsoft.graph.downloadUrl` value is a short-lived URL and can't be cached.</span></span> <span data-ttu-id="dcb37-335">此 URL 在失效前只能使用很短的时间（1 小时）。</span><span class="sxs-lookup"><span data-stu-id="dcb37-335">The URL will only be available for a short period of time (1 hour) before it is invalidated.</span></span>
<span data-ttu-id="dcb37-336">删除用户的文件权限可能不会立即使 URL 无效。</span><span class="sxs-lookup"><span data-stu-id="dcb37-336">Removing file permissions for a user might not immediately invalidate the URL.</span></span>
>
><span data-ttu-id="dcb37-337">OneDrive for Business、SharePoint Online 和 SharePoint Server 2016 [不支持](/onedrive/developer/rest-api/api/driveitem_upload_url?view=odsp-graph-online#remarks&preserve-view=true)使用 `@microsoft.graph.sourceUrl` 属性进行文件上载。</span><span class="sxs-lookup"><span data-stu-id="dcb37-337">Using the `@microsoft.graph.sourceUrl` property for file uploading is [not supported](/onedrive/developer/rest-api/api/driveitem_upload_url?view=odsp-graph-online#remarks&preserve-view=true) in OneDrive for Business, SharePoint Online, and SharePoint Server 2016.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dcb37-338">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dcb37-338">JSON representation</span></span>

<span data-ttu-id="dcb37-339">下面是 **driveItem** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dcb37-339">Here is a JSON representation of a **driveItem** resource.</span></span>

<span data-ttu-id="dcb37-340">
            \*\*driveItem\*\* 资源由 [\*\*baseItem\*\*][baseItem] 派生并继承该资源的属性。</span><span class="sxs-lookup"><span data-stu-id="dcb37-340">The **driveItem** resource is derived from [**baseItem**][baseItem] and inherits properties from that resource.</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.driveItem", "@type.aka": "oneDrive.item",
       "baseType": "microsoft.graph.baseItem",
       "optionalProperties": ["cTag", "children", "folder", "file", "image", "audio", "video",
       "location", "deleted", "specialFolder", "photo", "thumbnails", "searchResult", "remoteItem",
       "shared", "content", "@microsoft.graph.conflictBehavior", "@microsoft.graph.downloadUrl", "@content.sourceUrl",
       "sharepointIds"],
       "keyProperty": "id", "openType": true } -->

```json
{
  "audio": { "@odata.type": "microsoft.graph.audio" },
  "content": { "@odata.type": "Edm.Stream" },
  "cTag": "string (etag)",
  "deleted": { "@odata.type": "microsoft.graph.deleted"},
  "description": "string",
  "file": { "@odata.type": "microsoft.graph.file" },
  "fileSystemInfo": { "@odata.type": "microsoft.graph.fileSystemInfo" },
  "folder": { "@odata.type": "microsoft.graph.folder" },
  "image": { "@odata.type": "microsoft.graph.image" },
  "location": { "@odata.type": "microsoft.graph.geoCoordinates" },
  "package": { "@odata.type": "microsoft.graph.package" },
  "pendingOperations": { "@odata.type": "microsoft.graph.pendingOperations" },
  "photo": { "@odata.type": "microsoft.graph.photo" },
  "publication": {"@odata.type": "microsoft.graph.publicationFacet"},
  "remoteItem": { "@odata.type": "microsoft.graph.remoteItem" },
  "root": { "@odata.type": "microsoft.graph.root" },
  "searchResult": { "@odata.type": "microsoft.graph.searchResult" },
  "shared": { "@odata.type": "microsoft.graph.shared" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "size": 1024,
  "specialFolder": { "@odata.type": "microsoft.graph.specialFolder" },
  "video": { "@odata.type": "microsoft.graph.video" },
  "webDavUrl": "string",

  /* relationships */
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "analytics": {"@odata.type": "microsoft.graph.itemAnalytics"},
  "children": [{ "@odata.type": "microsoft.graph.driveItem" }],
  "createdByUser": { "@odata.type": "microsoft.graph.user" },
  "lastModifiedByUser": { "@odata.type": "microsoft.graph.user" },
  "permissions": [ {"@odata.type": "microsoft.graph.permission"} ],
  "subscriptions": [ {"@odata.type": "microsoft.graph.subscription"} ],
  "thumbnails": [ {"@odata.type": "microsoft.graph.thumbnailSet"}],
  "versions": [ {"@odata.type": "microsoft.graph.driveItemVersion"}],

  /* inherited from baseItem */
  "id": "string (identifier)",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "eTag": "string",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "parentReference": {"@odata.type": "microsoft.graph.itemReference"},
  "webUrl": "string",

  /* instance annotations */
  "@microsoft.graph.conflictBehavior": "string",
  "@microsoft.graph.downloadUrl": "url",
  "@microsoft.graph.sourceUrl": "url"
}
```

## <a name="methods"></a><span data-ttu-id="dcb37-341">方法</span><span class="sxs-lookup"><span data-stu-id="dcb37-341">Methods</span></span>

| <span data-ttu-id="dcb37-342">方法</span><span class="sxs-lookup"><span data-stu-id="dcb37-342">Method</span></span>                                                   | <span data-ttu-id="dcb37-343">返回类型</span><span class="sxs-lookup"><span data-stu-id="dcb37-343">Return Type</span></span> | <span data-ttu-id="dcb37-344">说明</span><span class="sxs-lookup"><span data-stu-id="dcb37-344">Description</span></span>
|:---------------------------------------------------------|:------------|:------------
| [<span data-ttu-id="dcb37-345">获取项目</span><span class="sxs-lookup"><span data-stu-id="dcb37-345">Get item</span></span>](../api/driveitem-get.md)                      | <span data-ttu-id="dcb37-346">driveItem</span><span class="sxs-lookup"><span data-stu-id="dcb37-346">driveItem</span></span> |<span data-ttu-id="dcb37-347">在驱动器中检索 DriveItem 的元数据。</span><span class="sxs-lookup"><span data-stu-id="dcb37-347">Retrieve the metadata for a DriveItem in a Drive.</span></span>
| <span data-ttu-id="dcb37-348">[获取分析结果][]</span><span class="sxs-lookup"><span data-stu-id="dcb37-348">[Get analytics][]</span></span>                                        | <span data-ttu-id="dcb37-349">[itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="dcb37-349">[itemAnalytics][]</span></span> | <span data-ttu-id="dcb37-350">对此资源可获取分析。</span><span class="sxs-lookup"><span data-stu-id="dcb37-350">Get analytics for this resource.</span></span> 
| <span data-ttu-id="dcb37-351">[按间隔获取活动][]</span><span class="sxs-lookup"><span data-stu-id="dcb37-351">[Get activities by interval][]</span></span>                           | <span data-ttu-id="dcb37-352">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="dcb37-352">[itemActivityStat][]</span></span> | <span data-ttu-id="dcb37-353">在指定的时间间隔内获取 itemActivityStats 的集合。</span><span class="sxs-lookup"><span data-stu-id="dcb37-353">Get a collection of itemActivityStats within the specified time interval.</span></span>
| [<span data-ttu-id="dcb37-354">列出子项</span><span class="sxs-lookup"><span data-stu-id="dcb37-354">List children</span></span>](../api/driveitem-list-children.md)       | <span data-ttu-id="dcb37-355">driveItem 集合</span><span class="sxs-lookup"><span data-stu-id="dcb37-355">collection of driveItem</span></span> | <span data-ttu-id="dcb37-356">在 DriveItem 的子项关系中返回 DriveItems 集合。</span><span class="sxs-lookup"><span data-stu-id="dcb37-356">Return a collection of DriveItems in the children relationship of a DriveItem.</span></span>
| [<span data-ttu-id="dcb37-357">列出版本</span><span class="sxs-lookup"><span data-stu-id="dcb37-357">List versions</span></span>](../api/driveitem-list-versions.md)       | <span data-ttu-id="dcb37-358">[DriveItemVersion][] 集合</span><span class="sxs-lookup"><span data-stu-id="dcb37-358">collection of [DriveItemVersion][]</span></span> | <span data-ttu-id="dcb37-359">检索当前用户驱动器中的文件的版本。</span><span class="sxs-lookup"><span data-stu-id="dcb37-359">Retrieves the versions of a file in the current user's drive.</span></span>
| [<span data-ttu-id="dcb37-360">创建项目</span><span class="sxs-lookup"><span data-stu-id="dcb37-360">Create item</span></span>](../api/driveitem-post-children.md)         | <span data-ttu-id="dcb37-361">driveItem</span><span class="sxs-lookup"><span data-stu-id="dcb37-361">driveItem</span></span> | <span data-ttu-id="dcb37-362">在指定的驱动器中创建一个 driveItem。</span><span class="sxs-lookup"><span data-stu-id="dcb37-362">Creates a driveItem in the specified drive.</span></span>
| [<span data-ttu-id="dcb37-363">更新项目</span><span class="sxs-lookup"><span data-stu-id="dcb37-363">Update item</span></span>](../api/driveitem-update.md)                | <span data-ttu-id="dcb37-364">driveItem</span><span class="sxs-lookup"><span data-stu-id="dcb37-364">driveItem</span></span> | <span data-ttu-id="dcb37-365">更新驱动器中的 driveItem。</span><span class="sxs-lookup"><span data-stu-id="dcb37-365">Updates a driveItem in the drive.</span></span>
| [<span data-ttu-id="dcb37-366">上传内容</span><span class="sxs-lookup"><span data-stu-id="dcb37-366">Upload content</span></span>](../api/driveitem-put-content.md)        | <span data-ttu-id="dcb37-367">driveItem</span><span class="sxs-lookup"><span data-stu-id="dcb37-367">driveItem</span></span> | <span data-ttu-id="dcb37-368">将内容上传到 driveItem。</span><span class="sxs-lookup"><span data-stu-id="dcb37-368">Uploads content to the driveItem.</span></span>
| [<span data-ttu-id="dcb37-369">下载内容</span><span class="sxs-lookup"><span data-stu-id="dcb37-369">Download content</span></span>](../api/driveitem-get-content.md)      | <span data-ttu-id="dcb37-370">下载 Url</span><span class="sxs-lookup"><span data-stu-id="dcb37-370">download Url</span></span> | <span data-ttu-id="dcb37-371">下载 driveItem 的内容。</span><span class="sxs-lookup"><span data-stu-id="dcb37-371">Downloads content of a driveItem.</span></span>
| <span data-ttu-id="dcb37-372">[下载特定文件格式][download-format]</span><span class="sxs-lookup"><span data-stu-id="dcb37-372">[Download specific file format][download-format]</span></span>         | <span data-ttu-id="dcb37-373">下载 Url</span><span class="sxs-lookup"><span data-stu-id="dcb37-373">download Url</span></span> | <span data-ttu-id="dcb37-374">下载具有特定格式的 driveItem 的内容。</span><span class="sxs-lookup"><span data-stu-id="dcb37-374">Downloads content of a driveItem with a specific format.</span></span>
| [<span data-ttu-id="dcb37-375">删除项</span><span class="sxs-lookup"><span data-stu-id="dcb37-375">Delete item</span></span>](../api/driveitem-delete.md)                | <span data-ttu-id="dcb37-376">无内容</span><span class="sxs-lookup"><span data-stu-id="dcb37-376">No Content</span></span> | <span data-ttu-id="dcb37-377">删除 DriveItem。</span><span class="sxs-lookup"><span data-stu-id="dcb37-377">Deletes a driveItem.</span></span>
| [<span data-ttu-id="dcb37-378">移动项目</span><span class="sxs-lookup"><span data-stu-id="dcb37-378">Move item</span></span>](../api/driveitem-move.md)                    | <span data-ttu-id="dcb37-379">driveItem</span><span class="sxs-lookup"><span data-stu-id="dcb37-379">driveItem</span></span> | <span data-ttu-id="dcb37-380">将 DriveItem 移动到父项。</span><span class="sxs-lookup"><span data-stu-id="dcb37-380">Move a DriveItem to a new parent item.</span></span>
| [<span data-ttu-id="dcb37-381">复制项目</span><span class="sxs-lookup"><span data-stu-id="dcb37-381">Copy item</span></span>](../api/driveitem-copy.md)                    | <span data-ttu-id="dcb37-382">有关如何[监视复制操作进度](/graph/long-running-actions-overview)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="dcb37-382">details about how to [monitor the progress](/graph/long-running-actions-overview) of the copy</span></span> | <span data-ttu-id="dcb37-383">创建 driveItem（包括任何子项）的副本。</span><span class="sxs-lookup"><span data-stu-id="dcb37-383">Creates a copy of an driveItem (including any children).</span></span>
| [<span data-ttu-id="dcb37-384">搜索项目</span><span class="sxs-lookup"><span data-stu-id="dcb37-384">Search items</span></span>](../api/driveitem-search.md)               | <span data-ttu-id="dcb37-385">driveItem 集合</span><span class="sxs-lookup"><span data-stu-id="dcb37-385">collection of driveItem</span></span> | <span data-ttu-id="dcb37-386">在项目层次结构中搜索与查询匹配的项目。</span><span class="sxs-lookup"><span data-stu-id="dcb37-386">Search the hierarchy of items for items matching a query.</span></span>
| [<span data-ttu-id="dcb37-387">列出驱动器中的更改</span><span class="sxs-lookup"><span data-stu-id="dcb37-387">List changes in a drive</span></span>](../api/driveitem-delta.md)     | <span data-ttu-id="dcb37-388">三角链接</span><span class="sxs-lookup"><span data-stu-id="dcb37-388">delta link</span></span> | <span data-ttu-id="dcb37-389">列出驱动器中的任何更改。</span><span class="sxs-lookup"><span data-stu-id="dcb37-389">List any changes in the drive.</span></span>
| [<span data-ttu-id="dcb37-390">关注项目</span><span class="sxs-lookup"><span data-stu-id="dcb37-390">Follow Item</span></span>](../api/driveitem-follow.md)                | <span data-ttu-id="dcb37-391">driveItem</span><span class="sxs-lookup"><span data-stu-id="dcb37-391">driveItem</span></span>  | <span data-ttu-id="dcb37-392">关注 driveItem。</span><span class="sxs-lookup"><span data-stu-id="dcb37-392">Follow a driveItem.</span></span>
| [<span data-ttu-id="dcb37-393">取消关注项目</span><span class="sxs-lookup"><span data-stu-id="dcb37-393">Unfollow Item</span></span>](../api/driveitem-unfollow.md)            | <span data-ttu-id="dcb37-394">无内容</span><span class="sxs-lookup"><span data-stu-id="dcb37-394">No content</span></span> | <span data-ttu-id="dcb37-395">取消关注 driveItem。</span><span class="sxs-lookup"><span data-stu-id="dcb37-395">Unfollow a driveItem.</span></span>
| [<span data-ttu-id="dcb37-396">列出缩略图</span><span class="sxs-lookup"><span data-stu-id="dcb37-396">List thumbnails</span></span>](../api/driveitem-list-thumbnails.md)   | <span data-ttu-id="dcb37-397">driveItem 集合</span><span class="sxs-lookup"><span data-stu-id="dcb37-397">collection of driveItem</span></span> | <span data-ttu-id="dcb37-398">使用缩略图列出 driveItems。</span><span class="sxs-lookup"><span data-stu-id="dcb37-398">List driveItems with their thumbnails.</span></span> 
| [<span data-ttu-id="dcb37-399">创建共享链接</span><span class="sxs-lookup"><span data-stu-id="dcb37-399">Create sharing link</span></span>](../api/driveitem-createlink.md)    | <span data-ttu-id="dcb37-400">共享链接</span><span class="sxs-lookup"><span data-stu-id="dcb37-400">sharing link</span></span> | <span data-ttu-id="dcb37-401">创建共享 driveItem 的链接。</span><span class="sxs-lookup"><span data-stu-id="dcb37-401">Create a link to share the driveItem.</span></span>
| [<span data-ttu-id="dcb37-402">添加权限</span><span class="sxs-lookup"><span data-stu-id="dcb37-402">Add permissions</span></span>](../api/driveitem-invite.md)            | <span data-ttu-id="dcb37-403">[权限][]集合</span><span class="sxs-lookup"><span data-stu-id="dcb37-403">collection of [permission][]</span></span> | <span data-ttu-id="dcb37-404">向用户发送共享邀请。</span><span class="sxs-lookup"><span data-stu-id="dcb37-404">Sends a sharing ivite to a user.</span></span>
| [<span data-ttu-id="dcb37-405">列出权限</span><span class="sxs-lookup"><span data-stu-id="dcb37-405">List permissions</span></span>](../api/driveitem-list-permissions.md) | <span data-ttu-id="dcb37-406">[权限][]集合</span><span class="sxs-lookup"><span data-stu-id="dcb37-406">collection of [permission][]</span></span> | <span data-ttu-id="dcb37-407">检索 driveItem 上的权限集合。</span><span class="sxs-lookup"><span data-stu-id="dcb37-407">Retrieves the collection of permissions on an driveItem.</span></span>
| [<span data-ttu-id="dcb37-408">删除权限</span><span class="sxs-lookup"><span data-stu-id="dcb37-408">Delete permission</span></span>](../api/permission-delete.md)         | <span data-ttu-id="dcb37-409">无内容</span><span class="sxs-lookup"><span data-stu-id="dcb37-409">No Content</span></span> | <span data-ttu-id="dcb37-410">从 driveItem 中删除权限。</span><span class="sxs-lookup"><span data-stu-id="dcb37-410">Removes the permission from the driveItem.</span></span>
| <span data-ttu-id="dcb37-411">[获取 WebSocket 频道][getWebSocket]</span><span class="sxs-lookup"><span data-stu-id="dcb37-411">[Get WebSocket channel][getWebSocket]</span></span>                    | <span data-ttu-id="dcb37-412">[订阅][]</span><span class="sxs-lookup"><span data-stu-id="dcb37-412">[subscription][]</span></span> | <span data-ttu-id="dcb37-413">使用 socket.io 接收驱动器的近实时更改通知。</span><span class="sxs-lookup"><span data-stu-id="dcb37-413">Receives near-real-time change notifications for a drive using socket.io.</span></span>
| <span data-ttu-id="dcb37-414">[预览项目][item-preview]</span><span class="sxs-lookup"><span data-stu-id="dcb37-414">[Preview item][item-preview]</span></span>                             | <span data-ttu-id="dcb37-415">json object</span><span class="sxs-lookup"><span data-stu-id="dcb37-415">json object</span></span> | <span data-ttu-id="dcb37-416">获取项目的短期可嵌入URL以呈现临时预览。</span><span class="sxs-lookup"><span data-stu-id="dcb37-416">Obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>
| [<span data-ttu-id="dcb37-417">签入</span><span class="sxs-lookup"><span data-stu-id="dcb37-417">Check in</span></span>](../api/driveitem-checkin.md)                  | `POST /drives/{driveId}/items/{itemId}/checkin`
| [<span data-ttu-id="dcb37-418">签出</span><span class="sxs-lookup"><span data-stu-id="dcb37-418">Check out</span></span>](../api/driveitem-checkout.md)                | `POST /drives/{driveId}/items/{itemId}/checkout`

[item-preview]: ../api/driveitem-preview.md
[获取分析结果]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[按间隔获取活动]: ../api/itemactivitystat-getactivitybyinterval.md
[Get activities by interval]: ../api/itemactivitystat-getactivitybyinterval.md

[audio]: audio.md
[baseItem]: baseitem.md
[Deleted]: deleted.md
[deleted]: deleted.md
[download-format]: ../api/driveitem-get-content-format.md
[driveItemVersion]: driveitemversion.md
[File]: file.md
[file]: file.md
[fileSystemInfo]: filesysteminfo.md
[folder]: folder.md
[获取旧版本]: ../api/driveitem-list-versions.md
[getting previous versions]: ../api/driveitem-list-versions.md
[获取缩略图]: ../api/driveitem-list-thumbnails.md
[getting thumbnails]: ../api/driveitem-list-thumbnails.md
[getWebSocket]: ../api/subscriptions-socketio.md
[identitySet]: identityset.md
[image]: image.md
[itemActivity]: itemactivity.md
[itemAnalytics]: itemanalytics.md
[itemReference]: itemreference.md
[geoCoordinates]: geocoordinates.md
[listItem]: listitem.md
[package]: package.md
[权限]: permission.md
[permission]: permission.md
[pendingOperations]: pendingoperations.md
[photo]: photo.md
[remoteItem]: remoteitem.md
[root]: root.md
[searchResult]: searchresult.md
[shared]: shared.md
[sharepointIds]: sharepointids.md
[specialFolder]: specialfolder.md
[订阅]: subscription.md
[subscription]: subscription.md
[thumbnailSet]: thumbnailset.md
[视频]: video.md
[video]: video.md
[工作簿]: workbook.md
[workbook]: workbook.md
[user]: /graph/api/resources/users
[publicationFacet]: publicationfacet.md

[DriveItemVersion]: driveitemversion.md
[权限]: permission.md
[permission]: permission.md
[订阅]: subscription.md
[subscription]: subscription.md
[itemActivityStat]: itemactivitystat.md

<!-- {
  "type": "#page.annotation",
  "description": "Item is the main data model in the OneDrive API. Everything is an item.",
  "keywords": "item,facet,resource",
  "section": "documentation",
  "tocPath": "Items",
  "tocBookmarks": { "Resources/Item": "#" }
} -->
