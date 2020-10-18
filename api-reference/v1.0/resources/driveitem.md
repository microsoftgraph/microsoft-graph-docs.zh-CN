---
author: JeremyKelley
ms.author: JeremyKelley
title: DriveItem 资源类型
description: 项目是 OneDrive API 中的主数据模型。 每项都是一个项目。
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 22b3d62ea83aa9e1b91f6be1f181bbe575341138
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/17/2020
ms.locfileid: "48581986"
---
# <a name="driveitem-resource-type"></a><span data-ttu-id="e8f95-104">DriveItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="e8f95-104">driveItem resource type</span></span>

<span data-ttu-id="e8f95-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8f95-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e8f95-p102">**driveItem** 资源代表文件、文件夹或存储在驱动器中的 其他项。OneDrive 和 SharePoint 中的所有文件系统对象将作为 **driveItem** 资源返回。</span><span class="sxs-lookup"><span data-stu-id="e8f95-p102">The **driveItem** resource represents a file, folder, or other item stored in a drive. All file system objects in OneDrive and SharePoint are returned as **driveItem** resources.</span></span>

<span data-ttu-id="e8f95-108">**driveItem** 资源的寻址方式主要有两种：</span><span class="sxs-lookup"><span data-stu-id="e8f95-108">There are two primary ways of addressing a **driveItem** resource:</span></span>

* <span data-ttu-id="e8f95-109">通过 **driveItem** 唯一标识符使用 `drive/items/{item-id}` 的方式</span><span class="sxs-lookup"><span data-stu-id="e8f95-109">By the **driveItem** unique identifier using `drive/items/{item-id}`</span></span>
* <span data-ttu-id="e8f95-110">通过使用文件系统路径 `/drive/root:/path/to/file` 的方式</span><span class="sxs-lookup"><span data-stu-id="e8f95-110">By file system path using `/drive/root:/path/to/file`</span></span>

<span data-ttu-id="e8f95-111">**DriveItem** 资源具有多个建模为属性的 Facet，用于提供 driveItem 的标识和功能相关数据。</span><span class="sxs-lookup"><span data-stu-id="e8f95-111">**driveItem** resources have facets modeled as properties that provide data about the driveItem's identities and capabilities.</span></span>
<span data-ttu-id="e8f95-112">例如：</span><span class="sxs-lookup"><span data-stu-id="e8f95-112">For example:</span></span>

* <span data-ttu-id="e8f95-113">文件夹具有 [**folder facet**][folder]</span><span class="sxs-lookup"><span data-stu-id="e8f95-113">Folders have a [**folder facet**][folder]</span></span>
* <span data-ttu-id="e8f95-114">文件具有 [**file facet**][file]。</span><span class="sxs-lookup"><span data-stu-id="e8f95-114">Files have a [**file facet**][file].</span></span>
* <span data-ttu-id="e8f95-115">除了 file facet 之外，图像还具有 [**image facet**][image]。</span><span class="sxs-lookup"><span data-stu-id="e8f95-115">Images have an [**image facet**][image] in addition to their file facet.</span></span>
* <span data-ttu-id="e8f95-116">使用照相机拍摄的图像（照片）具有 [**photo facet**][photo]，用于将项标识为照片，并提供照片的拍摄时间和拍摄所用设备等属性。</span><span class="sxs-lookup"><span data-stu-id="e8f95-116">Images taken with a camera (photos) have a [**photo facet**][photo] that identifies the item as a photo and provides the properties of when the photo was taken and with what device.</span></span>

<span data-ttu-id="e8f95-117">具有**文件夹** Facet 的项目充当项目的容器，因此具有指向文件夹下的 **driveItems** 集合的 `children` 引用。</span><span class="sxs-lookup"><span data-stu-id="e8f95-117">Items with the **folder** facet act as containers of items and therefore have a `children` reference pointing to a collection of **driveItems** under the folder.</span></span>

><span data-ttu-id="e8f95-118">**注意：** 在 OneDrive for Business 或 SharePoint 文档库中，如果 **driveItem** 具有 [folder][] Facet，则不返回 **cTag** 属性。</span><span class="sxs-lookup"><span data-stu-id="e8f95-118">**Note:** In OneDrive for Business or SharePoint document libraries, the **cTag** property is not returned, if the **driveItem** has a [folder][] facet.</span></span>

## <a name="properties"></a><span data-ttu-id="e8f95-119">属性</span><span class="sxs-lookup"><span data-stu-id="e8f95-119">Properties</span></span>

| <span data-ttu-id="e8f95-120">属性</span><span class="sxs-lookup"><span data-stu-id="e8f95-120">Property</span></span>             | <span data-ttu-id="e8f95-121">类型</span><span class="sxs-lookup"><span data-stu-id="e8f95-121">Type</span></span>               | <span data-ttu-id="e8f95-122">说明</span><span class="sxs-lookup"><span data-stu-id="e8f95-122">Description</span></span>
|:---------------------|:-------------------|:---------------------------------
| <span data-ttu-id="e8f95-123">audio</span><span class="sxs-lookup"><span data-stu-id="e8f95-123">audio</span></span>                | <span data-ttu-id="e8f95-124">[audio][]</span><span class="sxs-lookup"><span data-stu-id="e8f95-124">[audio][]</span></span>          | <span data-ttu-id="e8f95-p104">音频元数据（如果此项是一个音频文件）。只读。</span><span class="sxs-lookup"><span data-stu-id="e8f95-p104">Audio metadata, if the item is an audio file. Read-only.</span></span>
| <span data-ttu-id="e8f95-127">content</span><span class="sxs-lookup"><span data-stu-id="e8f95-127">content</span></span>              | <span data-ttu-id="e8f95-128">流</span><span class="sxs-lookup"><span data-stu-id="e8f95-128">Stream</span></span>             | <span data-ttu-id="e8f95-129">内容流（如果此项表示一个文件）。</span><span class="sxs-lookup"><span data-stu-id="e8f95-129">The content stream, if the item represents a file.</span></span>
| <span data-ttu-id="e8f95-130">createdBy</span><span class="sxs-lookup"><span data-stu-id="e8f95-130">createdBy</span></span>            | <span data-ttu-id="e8f95-131">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="e8f95-131">[identitySet][]</span></span>    | <span data-ttu-id="e8f95-p105">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="e8f95-p105">Identity of the user, device, and application which created the item. Read-only.</span></span>
| <span data-ttu-id="e8f95-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e8f95-134">createdDateTime</span></span>      | <span data-ttu-id="e8f95-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8f95-135">DateTimeOffset</span></span>     | <span data-ttu-id="e8f95-p106">创建项的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="e8f95-p106">Date and time of item creation. Read-only.</span></span>
| <span data-ttu-id="e8f95-138">cTag</span><span class="sxs-lookup"><span data-stu-id="e8f95-138">cTag</span></span>                 | <span data-ttu-id="e8f95-139">String</span><span class="sxs-lookup"><span data-stu-id="e8f95-139">String</span></span>             | <span data-ttu-id="e8f95-p107">项目内容的 eTag。如果只有元数据更改，此 eTag 不会更改。**注意** 如果项目是文件夹，则不返回此属性。只读。</span><span class="sxs-lookup"><span data-stu-id="e8f95-p107">An eTag for the content of the item. This eTag is not changed if only the metadata is changed. **Note** This property is not returned if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="e8f95-144">deleted</span><span class="sxs-lookup"><span data-stu-id="e8f95-144">deleted</span></span>              | <span data-ttu-id="e8f95-145">[deleted][]</span><span class="sxs-lookup"><span data-stu-id="e8f95-145">[deleted][]</span></span>        | <span data-ttu-id="e8f95-p108">有关项目删除状态的信息。只读。</span><span class="sxs-lookup"><span data-stu-id="e8f95-p108">Information about the deleted state of the item. Read-only.</span></span>
| <span data-ttu-id="e8f95-148">description</span><span class="sxs-lookup"><span data-stu-id="e8f95-148">description</span></span>          | <span data-ttu-id="e8f95-149">字符串</span><span class="sxs-lookup"><span data-stu-id="e8f95-149">String</span></span>             | <span data-ttu-id="e8f95-p109">提供项的用户可见的说明。读写。仅在 OneDrive 个人版上</span><span class="sxs-lookup"><span data-stu-id="e8f95-p109">Provides a user-visible description of the item. Read-write. Only on OneDrive Personal</span></span>
| <span data-ttu-id="e8f95-153">eTag</span><span class="sxs-lookup"><span data-stu-id="e8f95-153">eTag</span></span>                 | <span data-ttu-id="e8f95-154">String</span><span class="sxs-lookup"><span data-stu-id="e8f95-154">String</span></span>             | <span data-ttu-id="e8f95-p110">整个项目（元数据和内容）的 eTag。只读。</span><span class="sxs-lookup"><span data-stu-id="e8f95-p110">eTag for the entire item (metadata + content). Read-only.</span></span>
| <span data-ttu-id="e8f95-157">file</span><span class="sxs-lookup"><span data-stu-id="e8f95-157">file</span></span>                 | <span data-ttu-id="e8f95-158">[file][]</span><span class="sxs-lookup"><span data-stu-id="e8f95-158">[file][]</span></span>           | <span data-ttu-id="e8f95-p111">文件元数据（如果此项是一个文件）。只读。</span><span class="sxs-lookup"><span data-stu-id="e8f95-p111">File metadata, if the item is a file. Read-only.</span></span>
| <span data-ttu-id="e8f95-161">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="e8f95-161">fileSystemInfo</span></span>       | <span data-ttu-id="e8f95-162">[fileSystemInfo][]</span><span class="sxs-lookup"><span data-stu-id="e8f95-162">[fileSystemInfo][]</span></span> | <span data-ttu-id="e8f95-p112">客户端上的文件系统信息。读写。</span><span class="sxs-lookup"><span data-stu-id="e8f95-p112">File system information on client. Read-write.</span></span>
| <span data-ttu-id="e8f95-165">folder</span><span class="sxs-lookup"><span data-stu-id="e8f95-165">folder</span></span>               | <span data-ttu-id="e8f95-166">[folder][]</span><span class="sxs-lookup"><span data-stu-id="e8f95-166">[folder][]</span></span>         | <span data-ttu-id="e8f95-p113">文件夹元数据（如果此项是一个文件夹）。只读。</span><span class="sxs-lookup"><span data-stu-id="e8f95-p113">Folder metadata, if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="e8f95-169">id</span><span class="sxs-lookup"><span data-stu-id="e8f95-169">id</span></span>                   | <span data-ttu-id="e8f95-170">String</span><span class="sxs-lookup"><span data-stu-id="e8f95-170">String</span></span>             | <span data-ttu-id="e8f95-p114">项在驱动器中的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="e8f95-p114">The unique identifier of the item within the Drive. Read-only.</span></span>
| <span data-ttu-id="e8f95-173">image</span><span class="sxs-lookup"><span data-stu-id="e8f95-173">image</span></span>                | <span data-ttu-id="e8f95-174">[image][]</span><span class="sxs-lookup"><span data-stu-id="e8f95-174">[image][]</span></span>          | <span data-ttu-id="e8f95-p115">图像元数据（如果此项是一个图像）。只读。</span><span class="sxs-lookup"><span data-stu-id="e8f95-p115">Image metadata, if the item is an image. Read-only.</span></span>
| <span data-ttu-id="e8f95-177">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="e8f95-177">lastModifiedBy</span></span>       | <span data-ttu-id="e8f95-178">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="e8f95-178">[identitySet][]</span></span>    | <span data-ttu-id="e8f95-p116">上次修改项目的用户、设备和应用程序的标识。只读。</span><span class="sxs-lookup"><span data-stu-id="e8f95-p116">Identity of the user, device, and application which last modified the item. Read-only.</span></span>
| <span data-ttu-id="e8f95-181">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e8f95-181">lastModifiedDateTime</span></span> | <span data-ttu-id="e8f95-182">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8f95-182">DateTimeOffset</span></span>     | <span data-ttu-id="e8f95-p117">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="e8f95-p117">Date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="e8f95-185">location</span><span class="sxs-lookup"><span data-stu-id="e8f95-185">location</span></span>             | <span data-ttu-id="e8f95-186">[geoCoordinates][]</span><span class="sxs-lookup"><span data-stu-id="e8f95-186">[geoCoordinates][]</span></span> | <span data-ttu-id="e8f95-p118">位置元数据（如果此项包含位置数据）。只读。</span><span class="sxs-lookup"><span data-stu-id="e8f95-p118">Location metadata, if the item has location data. Read-only.</span></span>
| <span data-ttu-id="e8f95-189">name</span><span class="sxs-lookup"><span data-stu-id="e8f95-189">name</span></span>                 | <span data-ttu-id="e8f95-190">String</span><span class="sxs-lookup"><span data-stu-id="e8f95-190">String</span></span>             | <span data-ttu-id="e8f95-p119">项目名称（文件名和扩展名）。读写。</span><span class="sxs-lookup"><span data-stu-id="e8f95-p119">The name of the item (filename and extension). Read-write.</span></span>
| <span data-ttu-id="e8f95-193">package</span><span class="sxs-lookup"><span data-stu-id="e8f95-193">package</span></span>              | <span data-ttu-id="e8f95-194">[package][]</span><span class="sxs-lookup"><span data-stu-id="e8f95-194">[package][]</span></span>        | <span data-ttu-id="e8f95-p120">如果存在，则表示此项是一个包，而不是文件夹或文件。包被视为某些上下文中的文件和其他上下文中的文件夹。只读。</span><span class="sxs-lookup"><span data-stu-id="e8f95-p120">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span>
| <span data-ttu-id="e8f95-198">parentReference</span><span class="sxs-lookup"><span data-stu-id="e8f95-198">parentReference</span></span>      | <span data-ttu-id="e8f95-199">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="e8f95-199">[itemReference][]</span></span>  | <span data-ttu-id="e8f95-p121">父信息（如果此项具有父级）。读写。</span><span class="sxs-lookup"><span data-stu-id="e8f95-p121">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="e8f95-202">pendingOperations</span><span class="sxs-lookup"><span data-stu-id="e8f95-202">pendingOperations</span></span>    | <span data-ttu-id="e8f95-203">[pendingOperations][]</span><span class="sxs-lookup"><span data-stu-id="e8f95-203">[pendingOperations][]</span></span> | <span data-ttu-id="e8f95-204">如果存在，则表示可能影响 driveItem 状态的一个或多个操作正在等待完成。</span><span class="sxs-lookup"><span data-stu-id="e8f95-204">If present, indicates that one or more operations that might affect the state of the driveItem are pending completion.</span></span> <span data-ttu-id="e8f95-205">只读。</span><span class="sxs-lookup"><span data-stu-id="e8f95-205">Read-only.</span></span>
| <span data-ttu-id="e8f95-206">photo</span><span class="sxs-lookup"><span data-stu-id="e8f95-206">photo</span></span>                | <span data-ttu-id="e8f95-207">[照片][]</span><span class="sxs-lookup"><span data-stu-id="e8f95-207">[photo][]</span></span>          | <span data-ttu-id="e8f95-p123">照片元数据（如果此项包含照片）。只读。</span><span class="sxs-lookup"><span data-stu-id="e8f95-p123">Photo metadata, if the item is a photo. Read-only.</span></span>
| <span data-ttu-id="e8f95-210">publication</span><span class="sxs-lookup"><span data-stu-id="e8f95-210">publication</span></span>          | <span data-ttu-id="e8f95-211">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="e8f95-211">[publicationFacet][]</span></span> | <span data-ttu-id="e8f95-212">在支持此类操作的位置提供有关某个项目的已发布或签出状态信息。</span><span class="sxs-lookup"><span data-stu-id="e8f95-212">Provides information about the published or checked-out state of an item, in locations that support such actions.</span></span> <span data-ttu-id="e8f95-213">默认情况下，不会返回此属性。</span><span class="sxs-lookup"><span data-stu-id="e8f95-213">This property is not returned by default.</span></span> <span data-ttu-id="e8f95-214">只读。</span><span class="sxs-lookup"><span data-stu-id="e8f95-214">Read-only.</span></span> |
| <span data-ttu-id="e8f95-215">remoteItem</span><span class="sxs-lookup"><span data-stu-id="e8f95-215">remoteItem</span></span>           | <span data-ttu-id="e8f95-216">[remoteItem][]</span><span class="sxs-lookup"><span data-stu-id="e8f95-216">[remoteItem][]</span></span>     | <span data-ttu-id="e8f95-p125">远程项目数据（如果此项是从驱动器共享的项目，而不是被访问的项目）。只读。</span><span class="sxs-lookup"><span data-stu-id="e8f95-p125">Remote item data, if the item is shared from a drive other than the one being accessed. Read-only.</span></span>
| <span data-ttu-id="e8f95-219">root</span><span class="sxs-lookup"><span data-stu-id="e8f95-219">root</span></span>                 | <span data-ttu-id="e8f95-220">[root][]</span><span class="sxs-lookup"><span data-stu-id="e8f95-220">[root][]</span></span>           | <span data-ttu-id="e8f95-221">如果此属性为非 NULL，则表明 driveItem 是驱动器中最上面的 driveItem。</span><span class="sxs-lookup"><span data-stu-id="e8f95-221">If this property is non-null, it indicates that the driveItem is the top-most driveItem in the drive.</span></span>
| <span data-ttu-id="e8f95-222">searchResult</span><span class="sxs-lookup"><span data-stu-id="e8f95-222">searchResult</span></span>         | <span data-ttu-id="e8f95-223">[searchResult][]</span><span class="sxs-lookup"><span data-stu-id="e8f95-223">[searchResult][]</span></span>   | <span data-ttu-id="e8f95-p126">搜索元数据（如果此项目来自搜索结果）。只读。</span><span class="sxs-lookup"><span data-stu-id="e8f95-p126">Search metadata, if the item is from a search result. Read-only.</span></span>
| <span data-ttu-id="e8f95-226">shared</span><span class="sxs-lookup"><span data-stu-id="e8f95-226">shared</span></span>               | <span data-ttu-id="e8f95-227">[shared][]</span><span class="sxs-lookup"><span data-stu-id="e8f95-227">[shared][]</span></span>         | <span data-ttu-id="e8f95-p127">表示此项已与他人共享，并提供有关项目共享状态的信息。只读。</span><span class="sxs-lookup"><span data-stu-id="e8f95-p127">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>
| <span data-ttu-id="e8f95-230">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="e8f95-230">sharepointIds</span></span>        | <span data-ttu-id="e8f95-231">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="e8f95-231">[sharepointIds][]</span></span>  | <span data-ttu-id="e8f95-p128">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="e8f95-p128">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="e8f95-234">size</span><span class="sxs-lookup"><span data-stu-id="e8f95-234">size</span></span>                 | <span data-ttu-id="e8f95-235">Int64</span><span class="sxs-lookup"><span data-stu-id="e8f95-235">Int64</span></span>              | <span data-ttu-id="e8f95-p129">项目大小，以字节为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="e8f95-p129">Size of the item in bytes. Read-only.</span></span>
| <span data-ttu-id="e8f95-238">specialFolder</span><span class="sxs-lookup"><span data-stu-id="e8f95-238">specialFolder</span></span>        | <span data-ttu-id="e8f95-239">[specialFolder][]</span><span class="sxs-lookup"><span data-stu-id="e8f95-239">[specialFolder][]</span></span>  | <span data-ttu-id="e8f95-p130">如果当前项同时也是一个特殊的文件夹，则返回此 facet。只读。</span><span class="sxs-lookup"><span data-stu-id="e8f95-p130">If the current item is also available as a special folder, this facet is returned. Read-only.</span></span>
| <span data-ttu-id="e8f95-242">video</span><span class="sxs-lookup"><span data-stu-id="e8f95-242">video</span></span>                | <span data-ttu-id="e8f95-243">[video][]</span><span class="sxs-lookup"><span data-stu-id="e8f95-243">[video][]</span></span>          | <span data-ttu-id="e8f95-p131">视频元数据（如果此项是一个视频）。只读。</span><span class="sxs-lookup"><span data-stu-id="e8f95-p131">Video metadata, if the item is a video. Read-only.</span></span>
| <span data-ttu-id="e8f95-246">WebDavUrl</span><span class="sxs-lookup"><span data-stu-id="e8f95-246">webDavUrl</span></span>            | <span data-ttu-id="e8f95-247">String</span><span class="sxs-lookup"><span data-stu-id="e8f95-247">String</span></span>             | <span data-ttu-id="e8f95-248">项的可兼容 WebDAV 的 URL。</span><span class="sxs-lookup"><span data-stu-id="e8f95-248">WebDAV compatible URL for the item.</span></span>
| <span data-ttu-id="e8f95-249">WebUrl</span><span class="sxs-lookup"><span data-stu-id="e8f95-249">webUrl</span></span>               | <span data-ttu-id="e8f95-250">String</span><span class="sxs-lookup"><span data-stu-id="e8f95-250">String</span></span>             | <span data-ttu-id="e8f95-p132">在浏览器中显示此资源的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="e8f95-p132">URL that displays the resource in the browser. Read-only.</span></span>

<span data-ttu-id="e8f95-p133">**注意：** ETag 和 cTag 属性在容器（文件夹）中以不同的方式工作。更改任意文件夹后代的内容或元数据时，也会修改 CTag 值。除了从后代派生的属性（例如 **childCount** 或 **lastModifiedDateTime**），仅在更改文件夹的属性时修改 eTag 值。</span><span class="sxs-lookup"><span data-stu-id="e8f95-p133">**Note:** The eTag and cTag properties work differently on containers (folders). The cTag value is modified when content or metadata of any descendant of the folder is changed. The eTag value is only modified when the folder's properties are changed, except for properties that are derived from descendants (like **childCount** or **lastModifiedDateTime**).</span></span>

## <a name="relationships"></a><span data-ttu-id="e8f95-256">关系</span><span class="sxs-lookup"><span data-stu-id="e8f95-256">Relationships</span></span>

| <span data-ttu-id="e8f95-257">关系</span><span class="sxs-lookup"><span data-stu-id="e8f95-257">Relationship</span></span>       | <span data-ttu-id="e8f95-258">类型</span><span class="sxs-lookup"><span data-stu-id="e8f95-258">Type</span></span>                        | <span data-ttu-id="e8f95-259">说明</span><span class="sxs-lookup"><span data-stu-id="e8f95-259">Description</span></span>
|:-------------------|:----------------------------|:--------------------------
| <span data-ttu-id="e8f95-260">activities</span><span class="sxs-lookup"><span data-stu-id="e8f95-260">activities</span></span>         | <span data-ttu-id="e8f95-261">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="e8f95-261">[itemActivity][] collection</span></span> | <span data-ttu-id="e8f95-262">最近发生在此项上的活动的列表。</span><span class="sxs-lookup"><span data-stu-id="e8f95-262">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="e8f95-263">分析</span><span class="sxs-lookup"><span data-stu-id="e8f95-263">analytics</span></span>          | <span data-ttu-id="e8f95-264">[itemAnalytics][] 资源</span><span class="sxs-lookup"><span data-stu-id="e8f95-264">[itemAnalytics][] resource</span></span>  | <span data-ttu-id="e8f95-265">此项目上发生的查看活动的相关分析。</span><span class="sxs-lookup"><span data-stu-id="e8f95-265">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="e8f95-266">children</span><span class="sxs-lookup"><span data-stu-id="e8f95-266">children</span></span>           | <span data-ttu-id="e8f95-267">driveItem 集合</span><span class="sxs-lookup"><span data-stu-id="e8f95-267">driveItem collection</span></span>        | <span data-ttu-id="e8f95-p134">包含项目直接子项的 Item 对象的集合。仅表示文件夹的项目包含子项。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="e8f95-p134">Collection containing Item objects for the immediate children of Item. Only items representing folders have children. Read-only. Nullable.</span></span>
| <span data-ttu-id="e8f95-272">createdByUser</span><span class="sxs-lookup"><span data-stu-id="e8f95-272">createdByUser</span></span>      | <span data-ttu-id="e8f95-273">[user][]</span><span class="sxs-lookup"><span data-stu-id="e8f95-273">[user][]</span></span>                    | <span data-ttu-id="e8f95-274">创建了项的用户的身份。</span><span class="sxs-lookup"><span data-stu-id="e8f95-274">Identity of the user who created the item.</span></span> <span data-ttu-id="e8f95-275">只读。</span><span class="sxs-lookup"><span data-stu-id="e8f95-275">Read-only.</span></span>
| <span data-ttu-id="e8f95-276">lastModifiedByUser</span><span class="sxs-lookup"><span data-stu-id="e8f95-276">lastModifiedByUser</span></span> | <span data-ttu-id="e8f95-277">[user][]</span><span class="sxs-lookup"><span data-stu-id="e8f95-277">[user][]</span></span>                    | <span data-ttu-id="e8f95-278">上次修改项的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="e8f95-278">Identity of the user who last modified the item.</span></span> <span data-ttu-id="e8f95-279">只读。</span><span class="sxs-lookup"><span data-stu-id="e8f95-279">Read-only.</span></span>
| <span data-ttu-id="e8f95-280">listItem</span><span class="sxs-lookup"><span data-stu-id="e8f95-280">listItem</span></span>           | <span data-ttu-id="e8f95-281">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="e8f95-281">[listItem][]</span></span>                | <span data-ttu-id="e8f95-282">对于 SharePoint 中的驱动器，关联的文档库列表项。</span><span class="sxs-lookup"><span data-stu-id="e8f95-282">For drives in SharePoint, the associated document library list item.</span></span> <span data-ttu-id="e8f95-283">只读。</span><span class="sxs-lookup"><span data-stu-id="e8f95-283">Read-only.</span></span> <span data-ttu-id="e8f95-284">可为 null。</span><span class="sxs-lookup"><span data-stu-id="e8f95-284">Nullable.</span></span>
| <span data-ttu-id="e8f95-285">permissions</span><span class="sxs-lookup"><span data-stu-id="e8f95-285">permissions</span></span>        | <span data-ttu-id="e8f95-286">[permission][] 集合</span><span class="sxs-lookup"><span data-stu-id="e8f95-286">[permission][] collection</span></span>   | <span data-ttu-id="e8f95-p138">项目的权限集。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="e8f95-p138">The set of permissions for the item. Read-only. Nullable.</span></span>
| <span data-ttu-id="e8f95-290">订阅</span><span class="sxs-lookup"><span data-stu-id="e8f95-290">subscriptions</span></span>      | <span data-ttu-id="e8f95-291">[订阅][]集合</span><span class="sxs-lookup"><span data-stu-id="e8f95-291">[subscription][] collection</span></span> | <span data-ttu-id="e8f95-292">项目上的订阅集。</span><span class="sxs-lookup"><span data-stu-id="e8f95-292">The set of subscriptions on the item.</span></span> <span data-ttu-id="e8f95-293">仅在驱动器根目录上支持。</span><span class="sxs-lookup"><span data-stu-id="e8f95-293">Only supported on the root of a drive.</span></span>
| <span data-ttu-id="e8f95-294">缩略图</span><span class="sxs-lookup"><span data-stu-id="e8f95-294">thumbnails</span></span>         | <span data-ttu-id="e8f95-295">[thumbnailSet][] 集合</span><span class="sxs-lookup"><span data-stu-id="e8f95-295">[thumbnailSet][] collection</span></span> | <span data-ttu-id="e8f95-p140">包含与项目关联的 [ThumbnailSet][] 对象的集合。有关详细信息，请参阅 [获取缩略图][]只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="e8f95-p140">Collection containing [ThumbnailSet][] objects associated with the item. For more info, see [getting thumbnails][]. Read-only. Nullable.</span></span>
| <span data-ttu-id="e8f95-300">版本</span><span class="sxs-lookup"><span data-stu-id="e8f95-300">versions</span></span>           | <span data-ttu-id="e8f95-301">[driveItemVersion][] 集合</span><span class="sxs-lookup"><span data-stu-id="e8f95-301">[driveItemVersion][] collection</span></span> | <span data-ttu-id="e8f95-302">旧版本项的列表。</span><span class="sxs-lookup"><span data-stu-id="e8f95-302">The list of previous versions of the item.</span></span> <span data-ttu-id="e8f95-303">有关详细信息，请参阅[获取旧版本][]。</span><span class="sxs-lookup"><span data-stu-id="e8f95-303">For more info, see [getting previous versions][].</span></span> <span data-ttu-id="e8f95-304">只读。</span><span class="sxs-lookup"><span data-stu-id="e8f95-304">Read-only.</span></span> <span data-ttu-id="e8f95-305">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="e8f95-305">Nullable.</span></span>
| <span data-ttu-id="e8f95-306">工作簿</span><span class="sxs-lookup"><span data-stu-id="e8f95-306">workbook</span></span>           | <span data-ttu-id="e8f95-307">[workbook][]</span><span class="sxs-lookup"><span data-stu-id="e8f95-307">[workbook][]</span></span>                | <span data-ttu-id="e8f95-308">如果是 Excel 工作表文件，访问工作簿 API 以使用工作表的内容。</span><span class="sxs-lookup"><span data-stu-id="e8f95-308">For files that are Excel spreadsheets, accesses the workbook API to work with the spreadsheet's contents.</span></span> <span data-ttu-id="e8f95-309">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="e8f95-309">Nullable.</span></span>

## <a name="instance-attributes"></a><span data-ttu-id="e8f95-310">实例属性</span><span class="sxs-lookup"><span data-stu-id="e8f95-310">Instance Attributes</span></span>

<span data-ttu-id="e8f95-p143">实例属性是具有特殊行为的属性。这些属性是临时的，并且 a) 定义服务应执行的行为或 b) 提供短期的属性值，例如过期项目的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="e8f95-p143">Instance attributes are properties with special behaviors. These properties are temporary and either a) define behavior the service should perform or b) provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="e8f95-313">属性名称</span><span class="sxs-lookup"><span data-stu-id="e8f95-313">Property name</span></span>                     | <span data-ttu-id="e8f95-314">类型</span><span class="sxs-lookup"><span data-stu-id="e8f95-314">Type</span></span>   | <span data-ttu-id="e8f95-315">说明</span><span class="sxs-lookup"><span data-stu-id="e8f95-315">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="e8f95-316">@microsoft.graph.conflictBehavior</span><span class="sxs-lookup"><span data-stu-id="e8f95-316">@microsoft.graph.conflictBehavior</span></span> | <span data-ttu-id="e8f95-317">string</span><span class="sxs-lookup"><span data-stu-id="e8f95-317">string</span></span> | <span data-ttu-id="e8f95-p144">为创建新项目的操作解决冲突的行为。你可以使用值 *fail*、*replace* 或 *rename*。PUT 的默认值是*replace*。绝不会返回包含该批注的项目。只写。</span><span class="sxs-lookup"><span data-stu-id="e8f95-p144">The conflict resolution behavior for actions that create a new item. You can use the values *fail*, *replace*, or *rename*. The default for PUT is *replace*. An item will never be returned with this annotation. Write-only.</span></span>
| <span data-ttu-id="e8f95-323">@microsoft.graph.downloadUrl</span><span class="sxs-lookup"><span data-stu-id="e8f95-323">@microsoft.graph.downloadUrl</span></span>      | <span data-ttu-id="e8f95-324">string</span><span class="sxs-lookup"><span data-stu-id="e8f95-324">string</span></span> | <span data-ttu-id="e8f95-p145">一个可用于下载此文件的内容的 URL。不需要使用此 URL 进行身份验证。只读。</span><span class="sxs-lookup"><span data-stu-id="e8f95-p145">A URL that can be used to download this file's content. Authentication is not required with this URL. Read-only.</span></span>
| <span data-ttu-id="e8f95-328">@microsoft.graph.sourceUrl</span><span class="sxs-lookup"><span data-stu-id="e8f95-328">@microsoft.graph.sourceUrl</span></span>        | <span data-ttu-id="e8f95-329">string</span><span class="sxs-lookup"><span data-stu-id="e8f95-329">string</span></span> | <span data-ttu-id="e8f95-p146">发出 PUT 请求时，此实例批注可用于指示服务下载 URL 内容并将其存储为文件。只写。</span><span class="sxs-lookup"><span data-stu-id="e8f95-p146">When issuing a PUT request, this instance annotation can be used to instruct the service to download the contents of the URL, and store it as the file. Write-only.</span></span>

<span data-ttu-id="e8f95-332">**注意：**@microsoft.graph.downloadUrl 值是一个短期 URL，不能缓存。</span><span class="sxs-lookup"><span data-stu-id="e8f95-332">**Note:** The @microsoft.graph.downloadUrl value is a short-lived URL and can't be cached.</span></span>
<span data-ttu-id="e8f95-333">此 URL 在失效前只能使用很短的时间（1 小时）。</span><span class="sxs-lookup"><span data-stu-id="e8f95-333">The URL will only be available for a short period of time (1 hour) before it is invalidated.</span></span>
<span data-ttu-id="e8f95-334">删除用户的文件权限可能不会立即使 URL 无效。</span><span class="sxs-lookup"><span data-stu-id="e8f95-334">Removing file permissions for a user may not immediately invalidate the URL.</span></span>

><span data-ttu-id="e8f95-335">**注意：** 参数 @microsoft.graph.conflictBehavior 应包含在 URL 中，而不是请求正文中。</span><span class="sxs-lookup"><span data-stu-id="e8f95-335">**Note:** The parameter @microsoft.graph.conflictBehavior should be included in the URL instead of the body of the request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8f95-336">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e8f95-336">JSON representation</span></span>

<span data-ttu-id="e8f95-337">下面是 **driveItem** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e8f95-337">Here is a JSON representation of a **driveItem** resource.</span></span>

<span data-ttu-id="e8f95-338">
            \*\*driveItem\*\* 资源由 [\*\*baseItem\*\*][baseItem] 派生并继承该资源的属性。</span><span class="sxs-lookup"><span data-stu-id="e8f95-338">The **driveItem** resource is derived from [**baseItem**][baseItem] and inherits properties from that resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="e8f95-339">方法</span><span class="sxs-lookup"><span data-stu-id="e8f95-339">Methods</span></span>

| <span data-ttu-id="e8f95-340">方法</span><span class="sxs-lookup"><span data-stu-id="e8f95-340">Method</span></span>                                                   | <span data-ttu-id="e8f95-341">返回类型</span><span class="sxs-lookup"><span data-stu-id="e8f95-341">Return Type</span></span> | <span data-ttu-id="e8f95-342">说明</span><span class="sxs-lookup"><span data-stu-id="e8f95-342">Description</span></span>
|:---------------------------------------------------------|:------------|:------------
| [<span data-ttu-id="e8f95-343">获取项目</span><span class="sxs-lookup"><span data-stu-id="e8f95-343">Get item</span></span>](../api/driveitem-get.md)                      | <span data-ttu-id="e8f95-344">driveItem</span><span class="sxs-lookup"><span data-stu-id="e8f95-344">driveItem</span></span> |<span data-ttu-id="e8f95-345">在驱动器中检索 DriveItem 的元数据。</span><span class="sxs-lookup"><span data-stu-id="e8f95-345">Retrieve the metadata for a DriveItem in a Drive.</span></span>
| <span data-ttu-id="e8f95-346">[获取分析结果][]</span><span class="sxs-lookup"><span data-stu-id="e8f95-346">[Get analytics][]</span></span>                                        | <span data-ttu-id="e8f95-347">[itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="e8f95-347">[itemAnalytics][]</span></span> | <span data-ttu-id="e8f95-348">对此资源可获取分析。</span><span class="sxs-lookup"><span data-stu-id="e8f95-348">Get analytics for this resource.</span></span> 
| <span data-ttu-id="e8f95-349">[按间隔获取活动][]</span><span class="sxs-lookup"><span data-stu-id="e8f95-349">[Get activities by interval][]</span></span>                           | <span data-ttu-id="e8f95-350">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="e8f95-350">[itemActivityStat][]</span></span> | <span data-ttu-id="e8f95-351">在指定的时间间隔内获取 itemActivityStats 的集合。</span><span class="sxs-lookup"><span data-stu-id="e8f95-351">Get a collection of itemActivityStats within the specified time interval.</span></span>
| [<span data-ttu-id="e8f95-352">列出子项</span><span class="sxs-lookup"><span data-stu-id="e8f95-352">List children</span></span>](../api/driveitem-list-children.md)       | <span data-ttu-id="e8f95-353">driveItem 集合</span><span class="sxs-lookup"><span data-stu-id="e8f95-353">collection of driveItem</span></span> | <span data-ttu-id="e8f95-354">在 DriveItem 的子项关系中返回 DriveItems 集合。</span><span class="sxs-lookup"><span data-stu-id="e8f95-354">Return a collection of DriveItems in the children relationship of a DriveItem.</span></span>
| [<span data-ttu-id="e8f95-355">列出版本</span><span class="sxs-lookup"><span data-stu-id="e8f95-355">List versions</span></span>](../api/driveitem-list-versions.md)       | <span data-ttu-id="e8f95-356">[DriveItemVersion][] 集合</span><span class="sxs-lookup"><span data-stu-id="e8f95-356">collection of [DriveItemVersion][]</span></span> | <span data-ttu-id="e8f95-357">检索当前用户驱动器中的文件的版本。</span><span class="sxs-lookup"><span data-stu-id="e8f95-357">Retrieves the versions of a file in the current user's drive.</span></span>
| [<span data-ttu-id="e8f95-358">创建项目</span><span class="sxs-lookup"><span data-stu-id="e8f95-358">Create item</span></span>](../api/driveitem-post-children.md)         | <span data-ttu-id="e8f95-359">driveItem</span><span class="sxs-lookup"><span data-stu-id="e8f95-359">driveItem</span></span> | <span data-ttu-id="e8f95-360">在指定的驱动器中创建一个 driveItem。</span><span class="sxs-lookup"><span data-stu-id="e8f95-360">Creates a driveItem in the specified drive.</span></span>
| [<span data-ttu-id="e8f95-361">更新项目</span><span class="sxs-lookup"><span data-stu-id="e8f95-361">Update item</span></span>](../api/driveitem-update.md)                | <span data-ttu-id="e8f95-362">driveItem</span><span class="sxs-lookup"><span data-stu-id="e8f95-362">driveItem</span></span> | <span data-ttu-id="e8f95-363">更新驱动器中的 driveItem。</span><span class="sxs-lookup"><span data-stu-id="e8f95-363">Updates a driveItem in the drive.</span></span>
| [<span data-ttu-id="e8f95-364">上传内容</span><span class="sxs-lookup"><span data-stu-id="e8f95-364">Upload content</span></span>](../api/driveitem-put-content.md)        | <span data-ttu-id="e8f95-365">driveItem</span><span class="sxs-lookup"><span data-stu-id="e8f95-365">driveItem</span></span> | <span data-ttu-id="e8f95-366">将内容上传到 driveItem。</span><span class="sxs-lookup"><span data-stu-id="e8f95-366">Uploads content to the driveItem.</span></span>
| [<span data-ttu-id="e8f95-367">下载内容</span><span class="sxs-lookup"><span data-stu-id="e8f95-367">Download content</span></span>](../api/driveitem-get-content.md)      | <span data-ttu-id="e8f95-368">下载 Url</span><span class="sxs-lookup"><span data-stu-id="e8f95-368">download Url</span></span> | <span data-ttu-id="e8f95-369">下载 driveItem 的内容。</span><span class="sxs-lookup"><span data-stu-id="e8f95-369">Downloads content of a driveItem.</span></span>
| <span data-ttu-id="e8f95-370">[下载特定文件格式][download-format]</span><span class="sxs-lookup"><span data-stu-id="e8f95-370">[Download specific file format][download-format]</span></span>         | <span data-ttu-id="e8f95-371">下载 Url</span><span class="sxs-lookup"><span data-stu-id="e8f95-371">download Url</span></span> | <span data-ttu-id="e8f95-372">下载具有特定格式的 driveItem 的内容。</span><span class="sxs-lookup"><span data-stu-id="e8f95-372">Downloads content of a driveItem with a specific format.</span></span>
| [<span data-ttu-id="e8f95-373">删除项</span><span class="sxs-lookup"><span data-stu-id="e8f95-373">Delete item</span></span>](../api/driveitem-delete.md)                | <span data-ttu-id="e8f95-374">无内容</span><span class="sxs-lookup"><span data-stu-id="e8f95-374">No Content</span></span> | <span data-ttu-id="e8f95-375">删除 DriveItem。</span><span class="sxs-lookup"><span data-stu-id="e8f95-375">Deletes a driveItem.</span></span>
| [<span data-ttu-id="e8f95-376">移动项目</span><span class="sxs-lookup"><span data-stu-id="e8f95-376">Move item</span></span>](../api/driveitem-move.md)                    | <span data-ttu-id="e8f95-377">driveItem</span><span class="sxs-lookup"><span data-stu-id="e8f95-377">driveItem</span></span> | <span data-ttu-id="e8f95-378">将 DriveItem 移动到父项。</span><span class="sxs-lookup"><span data-stu-id="e8f95-378">Move a DriveItem to a new parent item.</span></span>
| [<span data-ttu-id="e8f95-379">复制项目</span><span class="sxs-lookup"><span data-stu-id="e8f95-379">Copy item</span></span>](../api/driveitem-copy.md)                    | <span data-ttu-id="e8f95-380">有关如何[监视复制操作进度](/graph/long-running-actions-overview)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="e8f95-380">details about how to [monitor the progress](/graph/long-running-actions-overview) of the copy</span></span> | <span data-ttu-id="e8f95-381">创建 driveItem（包括任何子项）的副本。</span><span class="sxs-lookup"><span data-stu-id="e8f95-381">Creates a copy of an driveItem (including any children).</span></span>
| [<span data-ttu-id="e8f95-382">搜索项目</span><span class="sxs-lookup"><span data-stu-id="e8f95-382">Search items</span></span>](../api/driveitem-search.md)               | <span data-ttu-id="e8f95-383">driveItem 集合</span><span class="sxs-lookup"><span data-stu-id="e8f95-383">collection of driveItem</span></span> | <span data-ttu-id="e8f95-384">在项目层次结构中搜索与查询匹配的项目。</span><span class="sxs-lookup"><span data-stu-id="e8f95-384">Search the hierarchy of items for items matching a query.</span></span>
| [<span data-ttu-id="e8f95-385">列出驱动器中的更改</span><span class="sxs-lookup"><span data-stu-id="e8f95-385">List changes in a drive</span></span>](../api/driveitem-delta.md)     | <span data-ttu-id="e8f95-386">三角链接</span><span class="sxs-lookup"><span data-stu-id="e8f95-386">delta link</span></span> | <span data-ttu-id="e8f95-387">列出驱动器中的任何更改。</span><span class="sxs-lookup"><span data-stu-id="e8f95-387">List any changes in the drive.</span></span>
| [<span data-ttu-id="e8f95-388">关注项目</span><span class="sxs-lookup"><span data-stu-id="e8f95-388">Follow Item</span></span>](../api/driveitem-follow.md)                | <span data-ttu-id="e8f95-389">driveItem</span><span class="sxs-lookup"><span data-stu-id="e8f95-389">driveItem</span></span>  | <span data-ttu-id="e8f95-390">关注 driveItem。</span><span class="sxs-lookup"><span data-stu-id="e8f95-390">Follow a driveItem.</span></span>
| [<span data-ttu-id="e8f95-391">取消关注项目</span><span class="sxs-lookup"><span data-stu-id="e8f95-391">Unfollow Item</span></span>](../api/driveitem-unfollow.md)            | <span data-ttu-id="e8f95-392">无内容</span><span class="sxs-lookup"><span data-stu-id="e8f95-392">No content</span></span> | <span data-ttu-id="e8f95-393">取消关注 driveItem。</span><span class="sxs-lookup"><span data-stu-id="e8f95-393">Unfollow a driveItem.</span></span>
| [<span data-ttu-id="e8f95-394">列出缩略图</span><span class="sxs-lookup"><span data-stu-id="e8f95-394">List thumbnails</span></span>](../api/driveitem-list-thumbnails.md)   | <span data-ttu-id="e8f95-395">driveItem 集合</span><span class="sxs-lookup"><span data-stu-id="e8f95-395">collection of driveItem</span></span> | <span data-ttu-id="e8f95-396">使用缩略图列出 driveItems。</span><span class="sxs-lookup"><span data-stu-id="e8f95-396">List driveItems with their thumbnails.</span></span> 
| [<span data-ttu-id="e8f95-397">创建共享链接</span><span class="sxs-lookup"><span data-stu-id="e8f95-397">Create sharing link</span></span>](../api/driveitem-createlink.md)    | <span data-ttu-id="e8f95-398">共享链接</span><span class="sxs-lookup"><span data-stu-id="e8f95-398">sharing link</span></span> | <span data-ttu-id="e8f95-399">创建共享 driveItem 的链接。</span><span class="sxs-lookup"><span data-stu-id="e8f95-399">Create a link to share the driveItem.</span></span>
| [<span data-ttu-id="e8f95-400">添加权限</span><span class="sxs-lookup"><span data-stu-id="e8f95-400">Add permissions</span></span>](../api/driveitem-invite.md)            | <span data-ttu-id="e8f95-401">[权限][]集合</span><span class="sxs-lookup"><span data-stu-id="e8f95-401">collection of [permission][]</span></span> | <span data-ttu-id="e8f95-402">向用户发送共享邀请。</span><span class="sxs-lookup"><span data-stu-id="e8f95-402">Sends a sharing ivite to a user.</span></span>
| [<span data-ttu-id="e8f95-403">列出权限</span><span class="sxs-lookup"><span data-stu-id="e8f95-403">List permissions</span></span>](../api/driveitem-list-permissions.md) | <span data-ttu-id="e8f95-404">[权限][]集合</span><span class="sxs-lookup"><span data-stu-id="e8f95-404">collection of [permission][]</span></span> | <span data-ttu-id="e8f95-405">检索 driveItem 上的权限集合。</span><span class="sxs-lookup"><span data-stu-id="e8f95-405">Retrieves the collection of permissions on an driveItem.</span></span>
| [<span data-ttu-id="e8f95-406">删除权限</span><span class="sxs-lookup"><span data-stu-id="e8f95-406">Delete permission</span></span>](../api/permission-delete.md)         | <span data-ttu-id="e8f95-407">无内容</span><span class="sxs-lookup"><span data-stu-id="e8f95-407">No Content</span></span> | <span data-ttu-id="e8f95-408">从 driveItem 中删除权限。</span><span class="sxs-lookup"><span data-stu-id="e8f95-408">Removes the permission from the driveItem.</span></span>
| <span data-ttu-id="e8f95-409">[获取 WebSocket 频道][getWebSocket]</span><span class="sxs-lookup"><span data-stu-id="e8f95-409">[Get WebSocket channel][getWebSocket]</span></span>                    | <span data-ttu-id="e8f95-410">[订阅][]</span><span class="sxs-lookup"><span data-stu-id="e8f95-410">[subscription][]</span></span> | <span data-ttu-id="e8f95-411">使用 socket.io 接收驱动器的近实时更改通知。</span><span class="sxs-lookup"><span data-stu-id="e8f95-411">Receives near-real-time change notifications for a drive using socket.io.</span></span>
| <span data-ttu-id="e8f95-412">[预览项目][item-preview]</span><span class="sxs-lookup"><span data-stu-id="e8f95-412">[Preview item][item-preview]</span></span>                             | <span data-ttu-id="e8f95-413">json object</span><span class="sxs-lookup"><span data-stu-id="e8f95-413">json object</span></span> | <span data-ttu-id="e8f95-414">获取项目的短期可嵌入URL以呈现临时预览。</span><span class="sxs-lookup"><span data-stu-id="e8f95-414">Obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>
| [<span data-ttu-id="e8f95-415">签入</span><span class="sxs-lookup"><span data-stu-id="e8f95-415">Check in</span></span>](../api/driveitem-checkin.md)                  | `POST /drives/{driveId}/items/{itemId}/checkin`
| [<span data-ttu-id="e8f95-416">签出</span><span class="sxs-lookup"><span data-stu-id="e8f95-416">Check out</span></span>](../api/driveitem-checkout.md)                | `POST /drives/{driveId}/items/{itemId}/checkout`

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