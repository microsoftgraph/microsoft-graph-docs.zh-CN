---
author: JeremyKelley
title: DriveItem 资源类型
description: 项目是 OneDrive API 中的主数据模型。 每项都是一个项目。
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: a4c05dece6a73977137240d63368d30fe94712d9
ms.sourcegitcommit: 0d4377b0153bc339ab7b3b1a6ee4d52848b622d4
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2020
ms.locfileid: "49714324"
---
# <a name="driveitem-resource-type"></a><span data-ttu-id="6c9bb-104">DriveItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="6c9bb-104">driveItem resource type</span></span>

<span data-ttu-id="6c9bb-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c9bb-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6c9bb-106">**driveItem** 资源代表文件、文件夹或存储在驱动器中的 其他项。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-106">The **driveItem** resource represents a file, folder, or other item stored in a drive.</span></span>

<span data-ttu-id="6c9bb-107">OneDrive 和 SharePoint 中的所有文件系统对象将作为 **driveItem** 资源返回。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-107">All file system objects in OneDrive and SharePoint are returned as **driveItem** resources.</span></span> <span data-ttu-id="6c9bb-108">SharePoint 文档库中的项目可以表示为 [listItem][] 或 **driveItem** 资源。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-108">Items in SharePoint document libraries can be represented as [listItem][] or **driveItem** resources.</span></span>

<span data-ttu-id="6c9bb-109">**driveItem** 资源的寻址方式主要有两种：</span><span class="sxs-lookup"><span data-stu-id="6c9bb-109">There are two primary ways of addressing a **driveItem** resource:</span></span>

* <span data-ttu-id="6c9bb-110">通过 **driveItem** 唯一标识符使用 `drive/items/{item-id}` 的方式</span><span class="sxs-lookup"><span data-stu-id="6c9bb-110">By the **driveItem** unique identifier using `drive/items/{item-id}`</span></span>
* <span data-ttu-id="6c9bb-111">通过使用文件系统路径 `/drive/root:/path/to/file` 的方式</span><span class="sxs-lookup"><span data-stu-id="6c9bb-111">By file system path using `/drive/root:/path/to/file`</span></span>

<span data-ttu-id="6c9bb-112">**DriveItem** 资源具有多个建模为属性的 Facet，用于提供 driveItem 的标识和功能相关数据。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-112">**driveItem** resources have facets modeled as properties that provide data about the driveItem's identities and capabilities.</span></span>
<span data-ttu-id="6c9bb-113">例如：</span><span class="sxs-lookup"><span data-stu-id="6c9bb-113">For example:</span></span>

* <span data-ttu-id="6c9bb-114">文件夹具有 [**folder facet**][folder]</span><span class="sxs-lookup"><span data-stu-id="6c9bb-114">Folders have a [**folder facet**][folder]</span></span>
* <span data-ttu-id="6c9bb-115">文件具有 [**file facet**][file]。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-115">Files have a [**file facet**][file].</span></span>
* <span data-ttu-id="6c9bb-116">除了 file facet 之外，图像还具有 [**image facet**][image]。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-116">Images have an [**image facet**][image] in addition to their file facet.</span></span>
* <span data-ttu-id="6c9bb-117">使用照相机拍摄的图像（照片）具有 [**photo facet**][photo]，用于将项标识为照片，并提供照片的拍摄时间和拍摄所用设备等属性。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-117">Images taken with a camera (photos) have a [**photo facet**][photo] that identifies the item as a photo and provides the properties of when the photo was taken and with what device.</span></span>

<span data-ttu-id="6c9bb-118">具有 **文件夹** Facet 的项目充当项目的容器，因此具有指向文件夹下的 **driveItems** 集合的 `children` 引用。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-118">Items with the **folder** facet act as containers of items and therefore have a `children` reference pointing to a collection of **driveItems** under the folder.</span></span>

><span data-ttu-id="6c9bb-119">**注意：** 在 OneDrive for Business 或 SharePoint 文档库中，如果 **driveItem** 具有 [folder][] Facet，则不返回 **cTag** 属性。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-119">**Note:** In OneDrive for Business or SharePoint document libraries, the **cTag** property is not returned, if the **driveItem** has a [folder][] facet.</span></span>

## <a name="properties"></a><span data-ttu-id="6c9bb-120">属性</span><span class="sxs-lookup"><span data-stu-id="6c9bb-120">Properties</span></span>

| <span data-ttu-id="6c9bb-121">属性</span><span class="sxs-lookup"><span data-stu-id="6c9bb-121">Property</span></span>             | <span data-ttu-id="6c9bb-122">类型</span><span class="sxs-lookup"><span data-stu-id="6c9bb-122">Type</span></span>               | <span data-ttu-id="6c9bb-123">说明</span><span class="sxs-lookup"><span data-stu-id="6c9bb-123">Description</span></span>
|:---------------------|:-------------------|:---------------------------------
| <span data-ttu-id="6c9bb-124">audio</span><span class="sxs-lookup"><span data-stu-id="6c9bb-124">audio</span></span>                | <span data-ttu-id="6c9bb-125">[audio][]</span><span class="sxs-lookup"><span data-stu-id="6c9bb-125">[audio][]</span></span>          | <span data-ttu-id="6c9bb-p104">音频元数据（如果此项是一个音频文件）。只读。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-p104">Audio metadata, if the item is an audio file. Read-only.</span></span>
| <span data-ttu-id="6c9bb-128">content</span><span class="sxs-lookup"><span data-stu-id="6c9bb-128">content</span></span>              | <span data-ttu-id="6c9bb-129">流</span><span class="sxs-lookup"><span data-stu-id="6c9bb-129">Stream</span></span>             | <span data-ttu-id="6c9bb-130">内容流（如果此项表示一个文件）。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-130">The content stream, if the item represents a file.</span></span>
| <span data-ttu-id="6c9bb-131">createdBy</span><span class="sxs-lookup"><span data-stu-id="6c9bb-131">createdBy</span></span>            | <span data-ttu-id="6c9bb-132">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="6c9bb-132">[identitySet][]</span></span>    | <span data-ttu-id="6c9bb-p105">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-p105">Identity of the user, device, and application which created the item. Read-only.</span></span>
| <span data-ttu-id="6c9bb-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c9bb-135">createdDateTime</span></span>      | <span data-ttu-id="6c9bb-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c9bb-136">DateTimeOffset</span></span>     | <span data-ttu-id="6c9bb-p106">创建项的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-p106">Date and time of item creation. Read-only.</span></span>
| <span data-ttu-id="6c9bb-139">cTag</span><span class="sxs-lookup"><span data-stu-id="6c9bb-139">cTag</span></span>                 | <span data-ttu-id="6c9bb-140">String</span><span class="sxs-lookup"><span data-stu-id="6c9bb-140">String</span></span>             | <span data-ttu-id="6c9bb-p107">项目内容的 eTag。如果只有元数据更改，此 eTag 不会更改。**注意** 如果项目是文件夹，则不返回此属性。只读。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-p107">An eTag for the content of the item. This eTag is not changed if only the metadata is changed. **Note** This property is not returned if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="6c9bb-145">deleted</span><span class="sxs-lookup"><span data-stu-id="6c9bb-145">deleted</span></span>              | <span data-ttu-id="6c9bb-146">[deleted][]</span><span class="sxs-lookup"><span data-stu-id="6c9bb-146">[deleted][]</span></span>        | <span data-ttu-id="6c9bb-p108">有关项目删除状态的信息。只读。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-p108">Information about the deleted state of the item. Read-only.</span></span>
| <span data-ttu-id="6c9bb-149">description</span><span class="sxs-lookup"><span data-stu-id="6c9bb-149">description</span></span>          | <span data-ttu-id="6c9bb-150">字符串</span><span class="sxs-lookup"><span data-stu-id="6c9bb-150">String</span></span>             | <span data-ttu-id="6c9bb-p109">提供项的用户可见的说明。读写。仅在 OneDrive 个人版上</span><span class="sxs-lookup"><span data-stu-id="6c9bb-p109">Provides a user-visible description of the item. Read-write. Only on OneDrive Personal</span></span>
| <span data-ttu-id="6c9bb-154">eTag</span><span class="sxs-lookup"><span data-stu-id="6c9bb-154">eTag</span></span>                 | <span data-ttu-id="6c9bb-155">String</span><span class="sxs-lookup"><span data-stu-id="6c9bb-155">String</span></span>             | <span data-ttu-id="6c9bb-p110">整个项目（元数据和内容）的 eTag。只读。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-p110">eTag for the entire item (metadata + content). Read-only.</span></span>
| <span data-ttu-id="6c9bb-158">file</span><span class="sxs-lookup"><span data-stu-id="6c9bb-158">file</span></span>                 | <span data-ttu-id="6c9bb-159">[file][]</span><span class="sxs-lookup"><span data-stu-id="6c9bb-159">[file][]</span></span>           | <span data-ttu-id="6c9bb-p111">文件元数据（如果此项是一个文件）。只读。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-p111">File metadata, if the item is a file. Read-only.</span></span>
| <span data-ttu-id="6c9bb-162">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="6c9bb-162">fileSystemInfo</span></span>       | <span data-ttu-id="6c9bb-163">[fileSystemInfo][]</span><span class="sxs-lookup"><span data-stu-id="6c9bb-163">[fileSystemInfo][]</span></span> | <span data-ttu-id="6c9bb-p112">客户端上的文件系统信息。读写。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-p112">File system information on client. Read-write.</span></span>
| <span data-ttu-id="6c9bb-166">folder</span><span class="sxs-lookup"><span data-stu-id="6c9bb-166">folder</span></span>               | <span data-ttu-id="6c9bb-167">[folder][]</span><span class="sxs-lookup"><span data-stu-id="6c9bb-167">[folder][]</span></span>         | <span data-ttu-id="6c9bb-p113">文件夹元数据（如果此项是一个文件夹）。只读。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-p113">Folder metadata, if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="6c9bb-170">id</span><span class="sxs-lookup"><span data-stu-id="6c9bb-170">id</span></span>                   | <span data-ttu-id="6c9bb-171">String</span><span class="sxs-lookup"><span data-stu-id="6c9bb-171">String</span></span>             | <span data-ttu-id="6c9bb-p114">项在驱动器中的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-p114">The unique identifier of the item within the Drive. Read-only.</span></span>
| <span data-ttu-id="6c9bb-174">image</span><span class="sxs-lookup"><span data-stu-id="6c9bb-174">image</span></span>                | <span data-ttu-id="6c9bb-175">[image][]</span><span class="sxs-lookup"><span data-stu-id="6c9bb-175">[image][]</span></span>          | <span data-ttu-id="6c9bb-p115">图像元数据（如果此项是一个图像）。只读。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-p115">Image metadata, if the item is an image. Read-only.</span></span>
| <span data-ttu-id="6c9bb-178">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="6c9bb-178">lastModifiedBy</span></span>       | <span data-ttu-id="6c9bb-179">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="6c9bb-179">[identitySet][]</span></span>    | <span data-ttu-id="6c9bb-p116">上次修改项目的用户、设备和应用程序的标识。只读。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-p116">Identity of the user, device, and application which last modified the item. Read-only.</span></span>
| <span data-ttu-id="6c9bb-182">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c9bb-182">lastModifiedDateTime</span></span> | <span data-ttu-id="6c9bb-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c9bb-183">DateTimeOffset</span></span>     | <span data-ttu-id="6c9bb-p117">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-p117">Date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="6c9bb-186">location</span><span class="sxs-lookup"><span data-stu-id="6c9bb-186">location</span></span>             | <span data-ttu-id="6c9bb-187">[geoCoordinates][]</span><span class="sxs-lookup"><span data-stu-id="6c9bb-187">[geoCoordinates][]</span></span> | <span data-ttu-id="6c9bb-p118">位置元数据（如果此项包含位置数据）。只读。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-p118">Location metadata, if the item has location data. Read-only.</span></span>
| <span data-ttu-id="6c9bb-190">name</span><span class="sxs-lookup"><span data-stu-id="6c9bb-190">name</span></span>                 | <span data-ttu-id="6c9bb-191">String</span><span class="sxs-lookup"><span data-stu-id="6c9bb-191">String</span></span>             | <span data-ttu-id="6c9bb-p119">项目名称（文件名和扩展名）。读写。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-p119">The name of the item (filename and extension). Read-write.</span></span>
| <span data-ttu-id="6c9bb-194">package</span><span class="sxs-lookup"><span data-stu-id="6c9bb-194">package</span></span>              | <span data-ttu-id="6c9bb-195">[package][]</span><span class="sxs-lookup"><span data-stu-id="6c9bb-195">[package][]</span></span>        | <span data-ttu-id="6c9bb-p120">如果存在，则表示此项是一个包，而不是文件夹或文件。包被视为某些上下文中的文件和其他上下文中的文件夹。只读。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-p120">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span>
| <span data-ttu-id="6c9bb-199">parentReference</span><span class="sxs-lookup"><span data-stu-id="6c9bb-199">parentReference</span></span>      | <span data-ttu-id="6c9bb-200">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="6c9bb-200">[itemReference][]</span></span>  | <span data-ttu-id="6c9bb-p121">父信息（如果此项具有父级）。读写。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-p121">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="6c9bb-203">pendingOperations</span><span class="sxs-lookup"><span data-stu-id="6c9bb-203">pendingOperations</span></span>    | <span data-ttu-id="6c9bb-204">[pendingOperations][]</span><span class="sxs-lookup"><span data-stu-id="6c9bb-204">[pendingOperations][]</span></span> | <span data-ttu-id="6c9bb-205">如果存在，则表示可能影响 driveItem 状态的一个或多个操作正在等待完成。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-205">If present, indicates that one or more operations that might affect the state of the driveItem are pending completion.</span></span> <span data-ttu-id="6c9bb-206">只读。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-206">Read-only.</span></span>
| <span data-ttu-id="6c9bb-207">photo</span><span class="sxs-lookup"><span data-stu-id="6c9bb-207">photo</span></span>                | <span data-ttu-id="6c9bb-208">[照片][]</span><span class="sxs-lookup"><span data-stu-id="6c9bb-208">[photo][]</span></span>          | <span data-ttu-id="6c9bb-p123">照片元数据（如果此项包含照片）。只读。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-p123">Photo metadata, if the item is a photo. Read-only.</span></span>
| <span data-ttu-id="6c9bb-211">publication</span><span class="sxs-lookup"><span data-stu-id="6c9bb-211">publication</span></span>          | <span data-ttu-id="6c9bb-212">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="6c9bb-212">[publicationFacet][]</span></span> | <span data-ttu-id="6c9bb-213">在支持此类操作的位置提供有关某个项目的已发布或签出状态信息。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-213">Provides information about the published or checked-out state of an item, in locations that support such actions.</span></span> <span data-ttu-id="6c9bb-214">默认情况下，不会返回此属性。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-214">This property is not returned by default.</span></span> <span data-ttu-id="6c9bb-215">只读。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-215">Read-only.</span></span> |
| <span data-ttu-id="6c9bb-216">remoteItem</span><span class="sxs-lookup"><span data-stu-id="6c9bb-216">remoteItem</span></span>           | <span data-ttu-id="6c9bb-217">[remoteItem][]</span><span class="sxs-lookup"><span data-stu-id="6c9bb-217">[remoteItem][]</span></span>     | <span data-ttu-id="6c9bb-p125">远程项目数据（如果此项是从驱动器共享的项目，而不是被访问的项目）。只读。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-p125">Remote item data, if the item is shared from a drive other than the one being accessed. Read-only.</span></span>
| <span data-ttu-id="6c9bb-220">root</span><span class="sxs-lookup"><span data-stu-id="6c9bb-220">root</span></span>                 | <span data-ttu-id="6c9bb-221">[root][]</span><span class="sxs-lookup"><span data-stu-id="6c9bb-221">[root][]</span></span>           | <span data-ttu-id="6c9bb-222">如果此属性为非 NULL，则表明 driveItem 是驱动器中最上面的 driveItem。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-222">If this property is non-null, it indicates that the driveItem is the top-most driveItem in the drive.</span></span>
| <span data-ttu-id="6c9bb-223">searchResult</span><span class="sxs-lookup"><span data-stu-id="6c9bb-223">searchResult</span></span>         | <span data-ttu-id="6c9bb-224">[searchResult][]</span><span class="sxs-lookup"><span data-stu-id="6c9bb-224">[searchResult][]</span></span>   | <span data-ttu-id="6c9bb-p126">搜索元数据（如果此项目来自搜索结果）。只读。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-p126">Search metadata, if the item is from a search result. Read-only.</span></span>
| <span data-ttu-id="6c9bb-227">shared</span><span class="sxs-lookup"><span data-stu-id="6c9bb-227">shared</span></span>               | <span data-ttu-id="6c9bb-228">[shared][]</span><span class="sxs-lookup"><span data-stu-id="6c9bb-228">[shared][]</span></span>         | <span data-ttu-id="6c9bb-p127">表示此项已与他人共享，并提供有关项目共享状态的信息。只读。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-p127">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>
| <span data-ttu-id="6c9bb-231">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="6c9bb-231">sharepointIds</span></span>        | <span data-ttu-id="6c9bb-232">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="6c9bb-232">[sharepointIds][]</span></span>  | <span data-ttu-id="6c9bb-p128">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-p128">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="6c9bb-235">size</span><span class="sxs-lookup"><span data-stu-id="6c9bb-235">size</span></span>                 | <span data-ttu-id="6c9bb-236">Int64</span><span class="sxs-lookup"><span data-stu-id="6c9bb-236">Int64</span></span>              | <span data-ttu-id="6c9bb-p129">项目大小，以字节为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-p129">Size of the item in bytes. Read-only.</span></span>
| <span data-ttu-id="6c9bb-239">specialFolder</span><span class="sxs-lookup"><span data-stu-id="6c9bb-239">specialFolder</span></span>        | <span data-ttu-id="6c9bb-240">[specialFolder][]</span><span class="sxs-lookup"><span data-stu-id="6c9bb-240">[specialFolder][]</span></span>  | <span data-ttu-id="6c9bb-p130">如果当前项同时也是一个特殊的文件夹，则返回此 facet。只读。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-p130">If the current item is also available as a special folder, this facet is returned. Read-only.</span></span>
| <span data-ttu-id="6c9bb-243">video</span><span class="sxs-lookup"><span data-stu-id="6c9bb-243">video</span></span>                | <span data-ttu-id="6c9bb-244">[video][]</span><span class="sxs-lookup"><span data-stu-id="6c9bb-244">[video][]</span></span>          | <span data-ttu-id="6c9bb-p131">视频元数据（如果此项是一个视频）。只读。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-p131">Video metadata, if the item is a video. Read-only.</span></span>
| <span data-ttu-id="6c9bb-247">WebDavUrl</span><span class="sxs-lookup"><span data-stu-id="6c9bb-247">webDavUrl</span></span>            | <span data-ttu-id="6c9bb-248">String</span><span class="sxs-lookup"><span data-stu-id="6c9bb-248">String</span></span>             | <span data-ttu-id="6c9bb-249">项的可兼容 WebDAV 的 URL。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-249">WebDAV compatible URL for the item.</span></span>
| <span data-ttu-id="6c9bb-250">WebUrl</span><span class="sxs-lookup"><span data-stu-id="6c9bb-250">webUrl</span></span>               | <span data-ttu-id="6c9bb-251">String</span><span class="sxs-lookup"><span data-stu-id="6c9bb-251">String</span></span>             | <span data-ttu-id="6c9bb-p132">在浏览器中显示此资源的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-p132">URL that displays the resource in the browser. Read-only.</span></span>

<span data-ttu-id="6c9bb-p133">**注意：** ETag 和 cTag 属性在容器（文件夹）中以不同的方式工作。更改任意文件夹后代的内容或元数据时，也会修改 CTag 值。除了从后代派生的属性（例如 **childCount** 或 **lastModifiedDateTime**），仅在更改文件夹的属性时修改 eTag 值。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-p133">**Note:** The eTag and cTag properties work differently on containers (folders). The cTag value is modified when content or metadata of any descendant of the folder is changed. The eTag value is only modified when the folder's properties are changed, except for properties that are derived from descendants (like **childCount** or **lastModifiedDateTime**).</span></span>

## <a name="relationships"></a><span data-ttu-id="6c9bb-257">关系</span><span class="sxs-lookup"><span data-stu-id="6c9bb-257">Relationships</span></span>

| <span data-ttu-id="6c9bb-258">关系</span><span class="sxs-lookup"><span data-stu-id="6c9bb-258">Relationship</span></span>       | <span data-ttu-id="6c9bb-259">类型</span><span class="sxs-lookup"><span data-stu-id="6c9bb-259">Type</span></span>                        | <span data-ttu-id="6c9bb-260">说明</span><span class="sxs-lookup"><span data-stu-id="6c9bb-260">Description</span></span>
|:-------------------|:----------------------------|:--------------------------
| <span data-ttu-id="6c9bb-261">activities</span><span class="sxs-lookup"><span data-stu-id="6c9bb-261">activities</span></span>         | <span data-ttu-id="6c9bb-262">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="6c9bb-262">[itemActivity][] collection</span></span> | <span data-ttu-id="6c9bb-263">最近发生在此项上的活动的列表。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-263">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="6c9bb-264">分析</span><span class="sxs-lookup"><span data-stu-id="6c9bb-264">analytics</span></span>          | <span data-ttu-id="6c9bb-265">[itemAnalytics][] 资源</span><span class="sxs-lookup"><span data-stu-id="6c9bb-265">[itemAnalytics][] resource</span></span>  | <span data-ttu-id="6c9bb-266">此项目上发生的查看活动的相关分析。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-266">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="6c9bb-267">children</span><span class="sxs-lookup"><span data-stu-id="6c9bb-267">children</span></span>           | <span data-ttu-id="6c9bb-268">driveItem 集合</span><span class="sxs-lookup"><span data-stu-id="6c9bb-268">driveItem collection</span></span>        | <span data-ttu-id="6c9bb-p134">包含项目直接子项的 Item 对象的集合。仅表示文件夹的项目包含子项。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-p134">Collection containing Item objects for the immediate children of Item. Only items representing folders have children. Read-only. Nullable.</span></span>
| <span data-ttu-id="6c9bb-273">createdByUser</span><span class="sxs-lookup"><span data-stu-id="6c9bb-273">createdByUser</span></span>      | <span data-ttu-id="6c9bb-274">[user][]</span><span class="sxs-lookup"><span data-stu-id="6c9bb-274">[user][]</span></span>                    | <span data-ttu-id="6c9bb-275">创建了项的用户的身份。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-275">Identity of the user who created the item.</span></span> <span data-ttu-id="6c9bb-276">只读。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-276">Read-only.</span></span>
| <span data-ttu-id="6c9bb-277">lastModifiedByUser</span><span class="sxs-lookup"><span data-stu-id="6c9bb-277">lastModifiedByUser</span></span> | <span data-ttu-id="6c9bb-278">[user][]</span><span class="sxs-lookup"><span data-stu-id="6c9bb-278">[user][]</span></span>                    | <span data-ttu-id="6c9bb-279">上次修改项的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-279">Identity of the user who last modified the item.</span></span> <span data-ttu-id="6c9bb-280">只读。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-280">Read-only.</span></span>
| <span data-ttu-id="6c9bb-281">listItem</span><span class="sxs-lookup"><span data-stu-id="6c9bb-281">listItem</span></span>           | <span data-ttu-id="6c9bb-282">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="6c9bb-282">[listItem][]</span></span>                | <span data-ttu-id="6c9bb-283">对于 SharePoint 中的驱动器，关联的文档库列表项。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-283">For drives in SharePoint, the associated document library list item.</span></span> <span data-ttu-id="6c9bb-284">只读。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-284">Read-only.</span></span> <span data-ttu-id="6c9bb-285">可为 null。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-285">Nullable.</span></span>
| <span data-ttu-id="6c9bb-286">permissions</span><span class="sxs-lookup"><span data-stu-id="6c9bb-286">permissions</span></span>        | <span data-ttu-id="6c9bb-287">[permission][] 集合</span><span class="sxs-lookup"><span data-stu-id="6c9bb-287">[permission][] collection</span></span>   | <span data-ttu-id="6c9bb-p138">项目的权限集。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-p138">The set of permissions for the item. Read-only. Nullable.</span></span>
| <span data-ttu-id="6c9bb-291">订阅</span><span class="sxs-lookup"><span data-stu-id="6c9bb-291">subscriptions</span></span>      | <span data-ttu-id="6c9bb-292">[订阅][]集合</span><span class="sxs-lookup"><span data-stu-id="6c9bb-292">[subscription][] collection</span></span> | <span data-ttu-id="6c9bb-293">项目上的订阅集。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-293">The set of subscriptions on the item.</span></span> <span data-ttu-id="6c9bb-294">仅在驱动器根目录上支持。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-294">Only supported on the root of a drive.</span></span>
| <span data-ttu-id="6c9bb-295">缩略图</span><span class="sxs-lookup"><span data-stu-id="6c9bb-295">thumbnails</span></span>         | <span data-ttu-id="6c9bb-296">[thumbnailSet][] 集合</span><span class="sxs-lookup"><span data-stu-id="6c9bb-296">[thumbnailSet][] collection</span></span> | <span data-ttu-id="6c9bb-p140">包含与项目关联的 [ThumbnailSet][] 对象的集合。有关详细信息，请参阅 [获取缩略图][]只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-p140">Collection containing [ThumbnailSet][] objects associated with the item. For more info, see [getting thumbnails][]. Read-only. Nullable.</span></span>
| <span data-ttu-id="6c9bb-301">版本</span><span class="sxs-lookup"><span data-stu-id="6c9bb-301">versions</span></span>           | <span data-ttu-id="6c9bb-302">[driveItemVersion][] 集合</span><span class="sxs-lookup"><span data-stu-id="6c9bb-302">[driveItemVersion][] collection</span></span> | <span data-ttu-id="6c9bb-303">旧版本项的列表。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-303">The list of previous versions of the item.</span></span> <span data-ttu-id="6c9bb-304">有关详细信息，请参阅[获取旧版本][]。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-304">For more info, see [getting previous versions][].</span></span> <span data-ttu-id="6c9bb-305">只读。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-305">Read-only.</span></span> <span data-ttu-id="6c9bb-306">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-306">Nullable.</span></span>
| <span data-ttu-id="6c9bb-307">工作簿</span><span class="sxs-lookup"><span data-stu-id="6c9bb-307">workbook</span></span>           | <span data-ttu-id="6c9bb-308">[workbook][]</span><span class="sxs-lookup"><span data-stu-id="6c9bb-308">[workbook][]</span></span>                | <span data-ttu-id="6c9bb-309">如果是 Excel 工作表文件，访问工作簿 API 以使用工作表的内容。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-309">For files that are Excel spreadsheets, accesses the workbook API to work with the spreadsheet's contents.</span></span> <span data-ttu-id="6c9bb-310">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-310">Nullable.</span></span>

## <a name="instance-attributes"></a><span data-ttu-id="6c9bb-311">实例属性</span><span class="sxs-lookup"><span data-stu-id="6c9bb-311">Instance Attributes</span></span>

<span data-ttu-id="6c9bb-p143">实例属性是具有特殊行为的属性。这些属性是临时的，并且 a) 定义服务应执行的行为或 b) 提供短期的属性值，例如过期项目的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-p143">Instance attributes are properties with special behaviors. These properties are temporary and either a) define behavior the service should perform or b) provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="6c9bb-314">属性名称</span><span class="sxs-lookup"><span data-stu-id="6c9bb-314">Property name</span></span>                     | <span data-ttu-id="6c9bb-315">类型</span><span class="sxs-lookup"><span data-stu-id="6c9bb-315">Type</span></span>   | <span data-ttu-id="6c9bb-316">说明</span><span class="sxs-lookup"><span data-stu-id="6c9bb-316">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="6c9bb-317">@microsoft.graph.conflictBehavior</span><span class="sxs-lookup"><span data-stu-id="6c9bb-317">@microsoft.graph.conflictBehavior</span></span> | <span data-ttu-id="6c9bb-318">string</span><span class="sxs-lookup"><span data-stu-id="6c9bb-318">string</span></span> | <span data-ttu-id="6c9bb-p144">为创建新项目的操作解决冲突的行为。你可以使用值 *fail*、*replace* 或 *rename*。PUT 的默认值是 *replace*。绝不会返回包含该批注的项目。只写。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-p144">The conflict resolution behavior for actions that create a new item. You can use the values *fail*, *replace*, or *rename*. The default for PUT is *replace*. An item will never be returned with this annotation. Write-only.</span></span>
| <span data-ttu-id="6c9bb-324">@microsoft.graph.downloadUrl</span><span class="sxs-lookup"><span data-stu-id="6c9bb-324">@microsoft.graph.downloadUrl</span></span>      | <span data-ttu-id="6c9bb-325">string</span><span class="sxs-lookup"><span data-stu-id="6c9bb-325">string</span></span> | <span data-ttu-id="6c9bb-p145">一个可用于下载此文件的内容的 URL。不需要使用此 URL 进行身份验证。只读。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-p145">A URL that can be used to download this file's content. Authentication is not required with this URL. Read-only.</span></span>
| <span data-ttu-id="6c9bb-329">@microsoft.graph.sourceUrl</span><span class="sxs-lookup"><span data-stu-id="6c9bb-329">@microsoft.graph.sourceUrl</span></span>        | <span data-ttu-id="6c9bb-330">string</span><span class="sxs-lookup"><span data-stu-id="6c9bb-330">string</span></span> | <span data-ttu-id="6c9bb-p146">发出 PUT 请求时，此实例批注可用于指示服务下载 URL 内容并将其存储为文件。只写。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-p146">When issuing a PUT request, this instance annotation can be used to instruct the service to download the contents of the URL, and store it as the file. Write-only.</span></span>

<span data-ttu-id="6c9bb-333">**注意：**@microsoft.graph.downloadUrl 值是一个短期 URL，不能缓存。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-333">**Note:** The @microsoft.graph.downloadUrl value is a short-lived URL and can't be cached.</span></span>
<span data-ttu-id="6c9bb-334">此 URL 在失效前只能使用很短的时间（1 小时）。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-334">The URL will only be available for a short period of time (1 hour) before it is invalidated.</span></span>
<span data-ttu-id="6c9bb-335">删除用户的文件权限可能不会立即使 URL 无效。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-335">Removing file permissions for a user may not immediately invalidate the URL.</span></span>

><span data-ttu-id="6c9bb-336">**注意：** 参数 @microsoft.graph.conflictBehavior 应包含在 URL 中，而不是请求正文中。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-336">**Note:** The parameter @microsoft.graph.conflictBehavior should be included in the URL instead of the body of the request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c9bb-337">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6c9bb-337">JSON representation</span></span>

<span data-ttu-id="6c9bb-338">下面是 **driveItem** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-338">Here is a JSON representation of a **driveItem** resource.</span></span>

<span data-ttu-id="6c9bb-339">
            \*\*driveItem\*\* 资源由 [\*\*baseItem\*\*][baseItem] 派生并继承该资源的属性。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-339">The **driveItem** resource is derived from [**baseItem**][baseItem] and inherits properties from that resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="6c9bb-340">方法</span><span class="sxs-lookup"><span data-stu-id="6c9bb-340">Methods</span></span>

| <span data-ttu-id="6c9bb-341">方法</span><span class="sxs-lookup"><span data-stu-id="6c9bb-341">Method</span></span>                                                   | <span data-ttu-id="6c9bb-342">返回类型</span><span class="sxs-lookup"><span data-stu-id="6c9bb-342">Return Type</span></span> | <span data-ttu-id="6c9bb-343">说明</span><span class="sxs-lookup"><span data-stu-id="6c9bb-343">Description</span></span>
|:---------------------------------------------------------|:------------|:------------
| [<span data-ttu-id="6c9bb-344">获取项目</span><span class="sxs-lookup"><span data-stu-id="6c9bb-344">Get item</span></span>](../api/driveitem-get.md)                      | <span data-ttu-id="6c9bb-345">driveItem</span><span class="sxs-lookup"><span data-stu-id="6c9bb-345">driveItem</span></span> |<span data-ttu-id="6c9bb-346">在驱动器中检索 DriveItem 的元数据。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-346">Retrieve the metadata for a DriveItem in a Drive.</span></span>
| <span data-ttu-id="6c9bb-347">[获取分析结果][]</span><span class="sxs-lookup"><span data-stu-id="6c9bb-347">[Get analytics][]</span></span>                                        | <span data-ttu-id="6c9bb-348">[itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="6c9bb-348">[itemAnalytics][]</span></span> | <span data-ttu-id="6c9bb-349">对此资源可获取分析。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-349">Get analytics for this resource.</span></span> 
| <span data-ttu-id="6c9bb-350">[按间隔获取活动][]</span><span class="sxs-lookup"><span data-stu-id="6c9bb-350">[Get activities by interval][]</span></span>                           | <span data-ttu-id="6c9bb-351">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="6c9bb-351">[itemActivityStat][]</span></span> | <span data-ttu-id="6c9bb-352">在指定的时间间隔内获取 itemActivityStats 的集合。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-352">Get a collection of itemActivityStats within the specified time interval.</span></span>
| [<span data-ttu-id="6c9bb-353">列出子项</span><span class="sxs-lookup"><span data-stu-id="6c9bb-353">List children</span></span>](../api/driveitem-list-children.md)       | <span data-ttu-id="6c9bb-354">driveItem 集合</span><span class="sxs-lookup"><span data-stu-id="6c9bb-354">collection of driveItem</span></span> | <span data-ttu-id="6c9bb-355">在 DriveItem 的子项关系中返回 DriveItems 集合。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-355">Return a collection of DriveItems in the children relationship of a DriveItem.</span></span>
| [<span data-ttu-id="6c9bb-356">列出版本</span><span class="sxs-lookup"><span data-stu-id="6c9bb-356">List versions</span></span>](../api/driveitem-list-versions.md)       | <span data-ttu-id="6c9bb-357">[DriveItemVersion][] 集合</span><span class="sxs-lookup"><span data-stu-id="6c9bb-357">collection of [DriveItemVersion][]</span></span> | <span data-ttu-id="6c9bb-358">检索当前用户驱动器中的文件的版本。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-358">Retrieves the versions of a file in the current user's drive.</span></span>
| [<span data-ttu-id="6c9bb-359">创建项目</span><span class="sxs-lookup"><span data-stu-id="6c9bb-359">Create item</span></span>](../api/driveitem-post-children.md)         | <span data-ttu-id="6c9bb-360">driveItem</span><span class="sxs-lookup"><span data-stu-id="6c9bb-360">driveItem</span></span> | <span data-ttu-id="6c9bb-361">在指定的驱动器中创建一个 driveItem。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-361">Creates a driveItem in the specified drive.</span></span>
| [<span data-ttu-id="6c9bb-362">更新项目</span><span class="sxs-lookup"><span data-stu-id="6c9bb-362">Update item</span></span>](../api/driveitem-update.md)                | <span data-ttu-id="6c9bb-363">driveItem</span><span class="sxs-lookup"><span data-stu-id="6c9bb-363">driveItem</span></span> | <span data-ttu-id="6c9bb-364">更新驱动器中的 driveItem。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-364">Updates a driveItem in the drive.</span></span>
| [<span data-ttu-id="6c9bb-365">上传内容</span><span class="sxs-lookup"><span data-stu-id="6c9bb-365">Upload content</span></span>](../api/driveitem-put-content.md)        | <span data-ttu-id="6c9bb-366">driveItem</span><span class="sxs-lookup"><span data-stu-id="6c9bb-366">driveItem</span></span> | <span data-ttu-id="6c9bb-367">将内容上传到 driveItem。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-367">Uploads content to the driveItem.</span></span>
| [<span data-ttu-id="6c9bb-368">下载内容</span><span class="sxs-lookup"><span data-stu-id="6c9bb-368">Download content</span></span>](../api/driveitem-get-content.md)      | <span data-ttu-id="6c9bb-369">下载 Url</span><span class="sxs-lookup"><span data-stu-id="6c9bb-369">download Url</span></span> | <span data-ttu-id="6c9bb-370">下载 driveItem 的内容。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-370">Downloads content of a driveItem.</span></span>
| <span data-ttu-id="6c9bb-371">[下载特定文件格式][download-format]</span><span class="sxs-lookup"><span data-stu-id="6c9bb-371">[Download specific file format][download-format]</span></span>         | <span data-ttu-id="6c9bb-372">下载 Url</span><span class="sxs-lookup"><span data-stu-id="6c9bb-372">download Url</span></span> | <span data-ttu-id="6c9bb-373">下载具有特定格式的 driveItem 的内容。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-373">Downloads content of a driveItem with a specific format.</span></span>
| [<span data-ttu-id="6c9bb-374">删除项</span><span class="sxs-lookup"><span data-stu-id="6c9bb-374">Delete item</span></span>](../api/driveitem-delete.md)                | <span data-ttu-id="6c9bb-375">无内容</span><span class="sxs-lookup"><span data-stu-id="6c9bb-375">No Content</span></span> | <span data-ttu-id="6c9bb-376">删除 DriveItem。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-376">Deletes a driveItem.</span></span>
| [<span data-ttu-id="6c9bb-377">移动项目</span><span class="sxs-lookup"><span data-stu-id="6c9bb-377">Move item</span></span>](../api/driveitem-move.md)                    | <span data-ttu-id="6c9bb-378">driveItem</span><span class="sxs-lookup"><span data-stu-id="6c9bb-378">driveItem</span></span> | <span data-ttu-id="6c9bb-379">将 DriveItem 移动到父项。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-379">Move a DriveItem to a new parent item.</span></span>
| [<span data-ttu-id="6c9bb-380">复制项目</span><span class="sxs-lookup"><span data-stu-id="6c9bb-380">Copy item</span></span>](../api/driveitem-copy.md)                    | <span data-ttu-id="6c9bb-381">有关如何[监视复制操作进度](/graph/long-running-actions-overview)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-381">details about how to [monitor the progress](/graph/long-running-actions-overview) of the copy</span></span> | <span data-ttu-id="6c9bb-382">创建 driveItem（包括任何子项）的副本。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-382">Creates a copy of an driveItem (including any children).</span></span>
| [<span data-ttu-id="6c9bb-383">搜索项目</span><span class="sxs-lookup"><span data-stu-id="6c9bb-383">Search items</span></span>](../api/driveitem-search.md)               | <span data-ttu-id="6c9bb-384">driveItem 集合</span><span class="sxs-lookup"><span data-stu-id="6c9bb-384">collection of driveItem</span></span> | <span data-ttu-id="6c9bb-385">在项目层次结构中搜索与查询匹配的项目。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-385">Search the hierarchy of items for items matching a query.</span></span>
| [<span data-ttu-id="6c9bb-386">列出驱动器中的更改</span><span class="sxs-lookup"><span data-stu-id="6c9bb-386">List changes in a drive</span></span>](../api/driveitem-delta.md)     | <span data-ttu-id="6c9bb-387">三角链接</span><span class="sxs-lookup"><span data-stu-id="6c9bb-387">delta link</span></span> | <span data-ttu-id="6c9bb-388">列出驱动器中的任何更改。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-388">List any changes in the drive.</span></span>
| [<span data-ttu-id="6c9bb-389">关注项目</span><span class="sxs-lookup"><span data-stu-id="6c9bb-389">Follow Item</span></span>](../api/driveitem-follow.md)                | <span data-ttu-id="6c9bb-390">driveItem</span><span class="sxs-lookup"><span data-stu-id="6c9bb-390">driveItem</span></span>  | <span data-ttu-id="6c9bb-391">关注 driveItem。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-391">Follow a driveItem.</span></span>
| [<span data-ttu-id="6c9bb-392">取消关注项目</span><span class="sxs-lookup"><span data-stu-id="6c9bb-392">Unfollow Item</span></span>](../api/driveitem-unfollow.md)            | <span data-ttu-id="6c9bb-393">无内容</span><span class="sxs-lookup"><span data-stu-id="6c9bb-393">No content</span></span> | <span data-ttu-id="6c9bb-394">取消关注 driveItem。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-394">Unfollow a driveItem.</span></span>
| [<span data-ttu-id="6c9bb-395">列出缩略图</span><span class="sxs-lookup"><span data-stu-id="6c9bb-395">List thumbnails</span></span>](../api/driveitem-list-thumbnails.md)   | <span data-ttu-id="6c9bb-396">driveItem 集合</span><span class="sxs-lookup"><span data-stu-id="6c9bb-396">collection of driveItem</span></span> | <span data-ttu-id="6c9bb-397">使用缩略图列出 driveItems。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-397">List driveItems with their thumbnails.</span></span> 
| [<span data-ttu-id="6c9bb-398">创建共享链接</span><span class="sxs-lookup"><span data-stu-id="6c9bb-398">Create sharing link</span></span>](../api/driveitem-createlink.md)    | <span data-ttu-id="6c9bb-399">共享链接</span><span class="sxs-lookup"><span data-stu-id="6c9bb-399">sharing link</span></span> | <span data-ttu-id="6c9bb-400">创建共享 driveItem 的链接。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-400">Create a link to share the driveItem.</span></span>
| [<span data-ttu-id="6c9bb-401">添加权限</span><span class="sxs-lookup"><span data-stu-id="6c9bb-401">Add permissions</span></span>](../api/driveitem-invite.md)            | <span data-ttu-id="6c9bb-402">[权限][]集合</span><span class="sxs-lookup"><span data-stu-id="6c9bb-402">collection of [permission][]</span></span> | <span data-ttu-id="6c9bb-403">向用户发送共享邀请。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-403">Sends a sharing ivite to a user.</span></span>
| [<span data-ttu-id="6c9bb-404">列出权限</span><span class="sxs-lookup"><span data-stu-id="6c9bb-404">List permissions</span></span>](../api/driveitem-list-permissions.md) | <span data-ttu-id="6c9bb-405">[权限][]集合</span><span class="sxs-lookup"><span data-stu-id="6c9bb-405">collection of [permission][]</span></span> | <span data-ttu-id="6c9bb-406">检索 driveItem 上的权限集合。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-406">Retrieves the collection of permissions on an driveItem.</span></span>
| [<span data-ttu-id="6c9bb-407">删除权限</span><span class="sxs-lookup"><span data-stu-id="6c9bb-407">Delete permission</span></span>](../api/permission-delete.md)         | <span data-ttu-id="6c9bb-408">无内容</span><span class="sxs-lookup"><span data-stu-id="6c9bb-408">No Content</span></span> | <span data-ttu-id="6c9bb-409">从 driveItem 中删除权限。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-409">Removes the permission from the driveItem.</span></span>
| <span data-ttu-id="6c9bb-410">[获取 WebSocket 频道][getWebSocket]</span><span class="sxs-lookup"><span data-stu-id="6c9bb-410">[Get WebSocket channel][getWebSocket]</span></span>                    | <span data-ttu-id="6c9bb-411">[订阅][]</span><span class="sxs-lookup"><span data-stu-id="6c9bb-411">[subscription][]</span></span> | <span data-ttu-id="6c9bb-412">使用 socket.io 接收驱动器的近实时更改通知。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-412">Receives near-real-time change notifications for a drive using socket.io.</span></span>
| <span data-ttu-id="6c9bb-413">[预览项目][item-preview]</span><span class="sxs-lookup"><span data-stu-id="6c9bb-413">[Preview item][item-preview]</span></span>                             | <span data-ttu-id="6c9bb-414">json object</span><span class="sxs-lookup"><span data-stu-id="6c9bb-414">json object</span></span> | <span data-ttu-id="6c9bb-415">获取项目的短期可嵌入URL以呈现临时预览。</span><span class="sxs-lookup"><span data-stu-id="6c9bb-415">Obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>
| [<span data-ttu-id="6c9bb-416">签入</span><span class="sxs-lookup"><span data-stu-id="6c9bb-416">Check in</span></span>](../api/driveitem-checkin.md)                  | `POST /drives/{driveId}/items/{itemId}/checkin`
| [<span data-ttu-id="6c9bb-417">签出</span><span class="sxs-lookup"><span data-stu-id="6c9bb-417">Check out</span></span>](../api/driveitem-checkout.md)                | `POST /drives/{driveId}/items/{itemId}/checkout`

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