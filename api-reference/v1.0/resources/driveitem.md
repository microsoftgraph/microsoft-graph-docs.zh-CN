---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveItem
ms.openlocfilehash: 526001ad9a6c52c5b031c1734466772861f1c67e
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="driveitem-resource-type"></a><span data-ttu-id="f9ae5-102">DriveItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="f9ae5-102">DriveItem resource type</span></span>

<span data-ttu-id="f9ae5-p101">**driveItem** 资源代表文件、文件夹或存储在驱动器中的 其他项。OneDrive 和 SharePoint 中的所有文件系统对象将作为 **driveItem** 资源返回。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p101">The **driveItem** resource represents a file, folder, or other item stored in a drive. All file system objects in OneDrive and SharePoint are returned as **driveItem** resources.</span></span>

<span data-ttu-id="f9ae5-105">**driveItem** 资源的寻址方式主要有两种：</span><span class="sxs-lookup"><span data-stu-id="f9ae5-105">There are two primary ways of addressing a **driveItem** resource:</span></span>

* <span data-ttu-id="f9ae5-106">通过 **driveItem** 唯一标识符使用 `drive/items/{item-id}` 的方式</span><span class="sxs-lookup"><span data-stu-id="f9ae5-106">By the **driveItem** unique identifier using `drive/items/{item-id}`</span></span>
* <span data-ttu-id="f9ae5-107">通过使用文件系统路径 `/drive/root:/path/to/file` 的方式</span><span class="sxs-lookup"><span data-stu-id="f9ae5-107">By file system path using `/drive/root:/path/to/file`</span></span>

<span data-ttu-id="f9ae5-p102">**DriveItem** 资源拥有作为属性进行模块化的多个 Facet，用于提供 driveItem 的标识和功能相关数据。例如：</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p102">**DriveItem** resources have facets modeled as properties that provide data about the driveItem's identities and capabilities. For example:</span></span>

* <span data-ttu-id="f9ae5-110">文件夹具有 [**folder facet**][folder]</span><span class="sxs-lookup"><span data-stu-id="f9ae5-110">Folders have a [**folder facet**]</span></span>
* <span data-ttu-id="f9ae5-111">文件具有 [**file facet**][file]。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-111">Files have a [**file facet**].</span></span>
* <span data-ttu-id="f9ae5-112">除了 file facet 之外，图像还具有 [**image facet**][image]。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-112">Images have an [**image facet**] in addition to their file facet.</span></span>
* <span data-ttu-id="f9ae5-113">使用照相机拍摄的图像（照片）具有 [**photo facet**][photo]，用于将项标识为照片，并提供照片的拍摄时间和拍摄所用设备等属性。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-113">Images taken with a camera (photos) have a [**photo facet**] that identifies the item as a photo and provides the properties of when the photo was taken and with what device.</span></span>

<span data-ttu-id="f9ae5-114">具有**文件夹** Facet 的项目充当项目的容器，因此具有指向文件夹下的 **driveItems** 集合的 `children` 引用。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-114">Items with the **folder** facet act as containers of items and therefore have a `children` reference pointing to a collection of **driveItems** under the folder.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f9ae5-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f9ae5-115">JSON representation</span></span>

<span data-ttu-id="f9ae5-116">下面是 **driveItem** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-116">Here is a JSON representation of a **driveItem** resource.</span></span>

<span data-ttu-id="f9ae5-117">**driveItem** 资源由 [**baseItem**][baseItem] 派生并继承该资源的属性。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-117">The **driveItem** resource is derived from [**baseItem**] and inherits properties from that resource.</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.driveItem", "@type.aka": "oneDrive.item",
       "optionalProperties": ["cTag", "children", "folder", "file", "image", "audio", "video",
       "location", "deleted", "specialFolder", "photo", "thumbnails", "searchResult", "remoteItem",
       "shared", "content", "@microsoft.graph.conflictBehavior", "@microsoft.graph.downloadUrl", "@content.sourceUrl",
       "sharepointIds"],
       "keyProperty": "id", "openType": true } -->

```json
{
  "audio": { "@odata.type": "microsoft.graph.audio" },
  "cTag": "string (etag)",
  "deleted": { "@odata.type": "microsoft.graph.deleted"},
  "description": "string",
  "file": { "@odata.type": "microsoft.graph.file" },
  "fileSystemInfo": { "@odata.type": "microsoft.graph.fileSystemInfo" },
  "folder": { "@odata.type": "microsoft.graph.folder" },
  "image": { "@odata.type": "microsoft.graph.image" },
  "location": { "@odata.type": "microsoft.graph.geoCoordinates" },
  "package": { "@odata.type": "microsoft.graph.package" },
  "photo": { "@odata.type": "microsoft.graph.photo" },
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
  "content": { "@odata.type": "Edm.Stream" },
  "createdByUser": { "@odata.type": "microsoft.graph.user" },
  "lastModifiedByUser": { "@odata.type": "microsoft.graph.user" },
  "children": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "thumbnails": [ {"@odata.type": "microsoft.graph.thumbnailSet"}],
  "permissions": [ {"@odata.type": "microsoft.graph.permission"} ],

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

## <a name="properties"></a><span data-ttu-id="f9ae5-118">属性</span><span class="sxs-lookup"><span data-stu-id="f9ae5-118">Properties</span></span>

| <span data-ttu-id="f9ae5-119">属性</span><span class="sxs-lookup"><span data-stu-id="f9ae5-119">Property</span></span>             | <span data-ttu-id="f9ae5-120">类型</span><span class="sxs-lookup"><span data-stu-id="f9ae5-120">Type</span></span>               | <span data-ttu-id="f9ae5-121">说明</span><span class="sxs-lookup"><span data-stu-id="f9ae5-121">Description</span></span>
|:---------------------|:-------------------|:---------------------------------
| <span data-ttu-id="f9ae5-122">audio</span><span class="sxs-lookup"><span data-stu-id="f9ae5-122">audio</span></span>                | <span data-ttu-id="f9ae5-123">[音频][]</span><span class="sxs-lookup"><span data-stu-id="f9ae5-123">[audio][]</span></span>          | <span data-ttu-id="f9ae5-p103">音频元数据（如果此项是一个音频文件）。只读。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p103">Audio metadata, if the item is an audio file. Read-only.</span></span>
| <span data-ttu-id="f9ae5-126">createdBy</span><span class="sxs-lookup"><span data-stu-id="f9ae5-126">createdBy</span></span>            | <span data-ttu-id="f9ae5-127">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="f9ae5-127">[identitySet][]</span></span>    | <span data-ttu-id="f9ae5-p104">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p104">Identity of the user, device, and application which created the item. Read-only.</span></span>
| <span data-ttu-id="f9ae5-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f9ae5-130">createdDateTime</span></span>      | <span data-ttu-id="f9ae5-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9ae5-131">DateTimeOffset</span></span>     | <span data-ttu-id="f9ae5-p105">创建项的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p105">Date and time of item creation. Read-only.</span></span>
| <span data-ttu-id="f9ae5-134">cTag</span><span class="sxs-lookup"><span data-stu-id="f9ae5-134">cTag</span></span>                 | <span data-ttu-id="f9ae5-135">String</span><span class="sxs-lookup"><span data-stu-id="f9ae5-135">String</span></span>             | <span data-ttu-id="f9ae5-p106">项目内容的 eTag。如果只有元数据更改，此 eTag 不会更改。**注意** 如果项目是文件夹，则不返回此属性。只读。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p106">An eTag for the content of the item. This eTag is not changed if only the metadata is changed. **Note** This property is not returned if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="f9ae5-140">deleted</span><span class="sxs-lookup"><span data-stu-id="f9ae5-140">deleted</span></span>              | <span data-ttu-id="f9ae5-141">[删除][]</span><span class="sxs-lookup"><span data-stu-id="f9ae5-141">[deleted][]</span></span>        | <span data-ttu-id="f9ae5-p107">有关项目删除状态的信息。只读。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p107">Information about the deleted state of the item. Read-only.</span></span>
| <span data-ttu-id="f9ae5-144">description</span><span class="sxs-lookup"><span data-stu-id="f9ae5-144">description</span></span>          | <span data-ttu-id="f9ae5-145">字符串</span><span class="sxs-lookup"><span data-stu-id="f9ae5-145">String</span></span>             | <span data-ttu-id="f9ae5-p108">提供项的用户可见的说明。读写。仅在 OneDrive 个人版上</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p108">Provides a user-visible description of the item. Read-write. Only on OneDrive Personal</span></span>
| <span data-ttu-id="f9ae5-149">eTag</span><span class="sxs-lookup"><span data-stu-id="f9ae5-149">eTag</span></span>                 | <span data-ttu-id="f9ae5-150">String</span><span class="sxs-lookup"><span data-stu-id="f9ae5-150">String</span></span>             | <span data-ttu-id="f9ae5-p109">整个项目（元数据和内容）的 eTag。只读。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p109">eTag for the entire item (metadata + content). Read-only.</span></span>
| <span data-ttu-id="f9ae5-153">文件</span><span class="sxs-lookup"><span data-stu-id="f9ae5-153">file</span></span>                 | <span data-ttu-id="f9ae5-154">[文件][]</span><span class="sxs-lookup"><span data-stu-id="f9ae5-154">[file][]</span></span>           | <span data-ttu-id="f9ae5-p110">文件元数据（如果此项是一个文件）。只读。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p110">File metadata, if the item is a file. Read-only.</span></span>
| <span data-ttu-id="f9ae5-157">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="f9ae5-157">fileSystemInfo</span></span>       | <span data-ttu-id="f9ae5-158">[fileSystemInfo][]</span><span class="sxs-lookup"><span data-stu-id="f9ae5-158">[fileSystemInfo][]</span></span> | <span data-ttu-id="f9ae5-p111">客户端上的文件系统信息。读写。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p111">File system information on client. Read-write.</span></span>
| <span data-ttu-id="f9ae5-161">文件夹</span><span class="sxs-lookup"><span data-stu-id="f9ae5-161">folder</span></span>               | <span data-ttu-id="f9ae5-162">[文件夹][]</span><span class="sxs-lookup"><span data-stu-id="f9ae5-162">[folder][]</span></span>         | <span data-ttu-id="f9ae5-p112">文件夹元数据（如果此项是一个文件夹）。只读。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p112">Folder metadata, if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="f9ae5-165">id</span><span class="sxs-lookup"><span data-stu-id="f9ae5-165">id</span></span>                   | <span data-ttu-id="f9ae5-166">String</span><span class="sxs-lookup"><span data-stu-id="f9ae5-166">String</span></span>             | <span data-ttu-id="f9ae5-p113">项在驱动器中的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p113">The unique identifier of the item within the Drive. Read-only.</span></span>
| <span data-ttu-id="f9ae5-169">image</span><span class="sxs-lookup"><span data-stu-id="f9ae5-169">image</span></span>                | <span data-ttu-id="f9ae5-170">[图像][]</span><span class="sxs-lookup"><span data-stu-id="f9ae5-170">[image][]</span></span>          | <span data-ttu-id="f9ae5-p114">图像元数据（如果此项是一个图像）。只读。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p114">Image metadata, if the item is an image. Read-only.</span></span>
| <span data-ttu-id="f9ae5-173">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="f9ae5-173">lastModifiedBy</span></span>       | <span data-ttu-id="f9ae5-174">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="f9ae5-174">[identitySet][]</span></span>    | <span data-ttu-id="f9ae5-p115">上次修改项目的用户、设备和应用程序的标识。只读。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p115">Identity of the user, device, and application which last modified the item. Read-only.</span></span>
| <span data-ttu-id="f9ae5-177">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f9ae5-177">lastModifiedDateTime</span></span> | <span data-ttu-id="f9ae5-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9ae5-178">DateTimeOffset</span></span>     | <span data-ttu-id="f9ae5-p116">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p116">Date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="f9ae5-181">location</span><span class="sxs-lookup"><span data-stu-id="f9ae5-181">location</span></span>             | <span data-ttu-id="f9ae5-182">[geoCoordinates][]</span><span class="sxs-lookup"><span data-stu-id="f9ae5-182">[geoCoordinates][]</span></span> | <span data-ttu-id="f9ae5-p117">位置元数据（如果此项包含位置数据）。只读。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p117">Location metadata, if the item has location data. Read-only.</span></span>
| <span data-ttu-id="f9ae5-185">name</span><span class="sxs-lookup"><span data-stu-id="f9ae5-185">name</span></span>                 | <span data-ttu-id="f9ae5-186">String</span><span class="sxs-lookup"><span data-stu-id="f9ae5-186">String</span></span>             | <span data-ttu-id="f9ae5-p118">项目名称（文件名和扩展名）。读写。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p118">The name of the item (filename and extension). Read-write.</span></span>
| <span data-ttu-id="f9ae5-189">包</span><span class="sxs-lookup"><span data-stu-id="f9ae5-189">package</span></span>              | <span data-ttu-id="f9ae5-190">[包][]</span><span class="sxs-lookup"><span data-stu-id="f9ae5-190">[package][]</span></span>        | <span data-ttu-id="f9ae5-p119">如果存在，则表示此项是一个包，而不是文件夹或文件。包被视为某些上下文中的文件和其他上下文中的文件夹。只读。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p119">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span>
| <span data-ttu-id="f9ae5-194">parentReference</span><span class="sxs-lookup"><span data-stu-id="f9ae5-194">parentReference</span></span>      | <span data-ttu-id="f9ae5-195">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="f9ae5-195">[itemReference][]</span></span>  | <span data-ttu-id="f9ae5-p120">父信息（如果此项具有父级）。读写。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p120">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="f9ae5-198">照片</span><span class="sxs-lookup"><span data-stu-id="f9ae5-198">photo</span></span>                | <span data-ttu-id="f9ae5-199">[照片][]</span><span class="sxs-lookup"><span data-stu-id="f9ae5-199">[photo][]</span></span>          | <span data-ttu-id="f9ae5-p121">照片元数据（如果此项包含照片）。只读。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p121">Photo metadata, if the item is a photo. Read-only.</span></span>
| <span data-ttu-id="f9ae5-202">remoteItem</span><span class="sxs-lookup"><span data-stu-id="f9ae5-202">remoteItem</span></span>           | <span data-ttu-id="f9ae5-203">[remoteItem][]</span><span class="sxs-lookup"><span data-stu-id="f9ae5-203">[remoteItem][]</span></span>     | <span data-ttu-id="f9ae5-p122">远程项目数据（如果此项是从驱动器共享的项目，而不是被访问的项目）。只读。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p122">Remote item data, if the item is shared from a drive other than the one being accessed. Read-only.</span></span>
| <span data-ttu-id="f9ae5-206">根</span><span class="sxs-lookup"><span data-stu-id="f9ae5-206">root</span></span>                 | <span data-ttu-id="f9ae5-207">[根][]</span><span class="sxs-lookup"><span data-stu-id="f9ae5-207">[root][]</span></span>           | <span data-ttu-id="f9ae5-208">如果此属性为非 NULL，则表明 driveItem 是驱动器中最上面的 driveItem。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-208">If this property is non-null, it indicates that the driveItem is the top-most driveItem in the drive.</span></span>
| <span data-ttu-id="f9ae5-209">searchResult</span><span class="sxs-lookup"><span data-stu-id="f9ae5-209">searchResult</span></span>         | <span data-ttu-id="f9ae5-210">[searchResult][]</span><span class="sxs-lookup"><span data-stu-id="f9ae5-210">[searchResult][]</span></span>   | <span data-ttu-id="f9ae5-p123">搜索元数据（如果此项目来自搜索结果）。只读。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p123">Search metadata, if the item is from a search result. Read-only.</span></span>
| <span data-ttu-id="f9ae5-213">共享</span><span class="sxs-lookup"><span data-stu-id="f9ae5-213">shared</span></span>               | <span data-ttu-id="f9ae5-214">[共享][]</span><span class="sxs-lookup"><span data-stu-id="f9ae5-214">[shared][]</span></span>         | <span data-ttu-id="f9ae5-p124">表示此项已与他人共享，并提供有关项目共享状态的信息。只读。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p124">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>
| <span data-ttu-id="f9ae5-217">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="f9ae5-217">sharepointIds</span></span>        | <span data-ttu-id="f9ae5-218">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="f9ae5-218">[sharepointIds][]</span></span>  | <span data-ttu-id="f9ae5-p125">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p125">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="f9ae5-221">size</span><span class="sxs-lookup"><span data-stu-id="f9ae5-221">size</span></span>                 | <span data-ttu-id="f9ae5-222">Int64</span><span class="sxs-lookup"><span data-stu-id="f9ae5-222">Int64</span></span>              | <span data-ttu-id="f9ae5-p126">项目大小，以字节为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p126">Size of the item in bytes. Read-only.</span></span>
| <span data-ttu-id="f9ae5-225">specialFolder</span><span class="sxs-lookup"><span data-stu-id="f9ae5-225">specialFolder</span></span>        | <span data-ttu-id="f9ae5-226">[specialFolder][]</span><span class="sxs-lookup"><span data-stu-id="f9ae5-226">[specialFolder][]</span></span>  | <span data-ttu-id="f9ae5-p127">如果当前项同时也是一个特殊的文件夹，则返回此 facet。只读。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p127">If the current item is also available as a special folder, this facet is returned. Read-only.</span></span>
| <span data-ttu-id="f9ae5-229">video</span><span class="sxs-lookup"><span data-stu-id="f9ae5-229">video</span></span>                | <span data-ttu-id="f9ae5-230">[视频][]</span><span class="sxs-lookup"><span data-stu-id="f9ae5-230">[video][]</span></span>          | <span data-ttu-id="f9ae5-p128">视频元数据（如果此项是一个视频）。只读。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p128">Video metadata, if the item is a video. Read-only.</span></span>
| <span data-ttu-id="f9ae5-233">WebDavUrl</span><span class="sxs-lookup"><span data-stu-id="f9ae5-233">webDavUrl</span></span>            | <span data-ttu-id="f9ae5-234">String</span><span class="sxs-lookup"><span data-stu-id="f9ae5-234">String</span></span>             | <span data-ttu-id="f9ae5-235">项的可兼容 WebDAV 的 URL。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-235">WebDAV compatible URL for the item.</span></span>
| <span data-ttu-id="f9ae5-236">WebUrl</span><span class="sxs-lookup"><span data-stu-id="f9ae5-236">webUrl</span></span>               | <span data-ttu-id="f9ae5-237">String</span><span class="sxs-lookup"><span data-stu-id="f9ae5-237">String</span></span>             | <span data-ttu-id="f9ae5-p129">在浏览器中显示此资源的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p129">URL that displays the resource in the browser. Read-only.</span></span>

<span data-ttu-id="f9ae5-p130">**注意：**ETag 和 cTag 属性在容器（文件夹）中以不同的方式工作。更改任意文件夹后代的内容或元数据时，也会修改 CTag 值。除了从后代派生的属性（例如 **childCount** 或 **lastModifiedDateTime**），仅在更改文件夹的属性时修改 eTag 值。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p130">**Note:** The eTag and cTag properties work differently on containers (folders). The cTag value is modified when content or metadata of any descendant of the folder is changed. The eTag value is only modified when the folder's properties are changed, except for properties that are derived from descendants (like **childCount** or **lastModifiedDateTime**).</span></span>

## <a name="relationships"></a><span data-ttu-id="f9ae5-243">关系</span><span class="sxs-lookup"><span data-stu-id="f9ae5-243">Relationships</span></span>

| <span data-ttu-id="f9ae5-244">关系</span><span class="sxs-lookup"><span data-stu-id="f9ae5-244">Relationship</span></span>       | <span data-ttu-id="f9ae5-245">类型</span><span class="sxs-lookup"><span data-stu-id="f9ae5-245">Type</span></span>                        | <span data-ttu-id="f9ae5-246">说明</span><span class="sxs-lookup"><span data-stu-id="f9ae5-246">Description</span></span>
|:-------------------|:----------------------------|:--------------------------
| <span data-ttu-id="f9ae5-247">内容</span><span class="sxs-lookup"><span data-stu-id="f9ae5-247">content</span></span>            | <span data-ttu-id="f9ae5-248">流</span><span class="sxs-lookup"><span data-stu-id="f9ae5-248">Stream</span></span>                      | <span data-ttu-id="f9ae5-249">内容流（如果此项表示一个文件）。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-249">The content stream, if the item represents a file.</span></span>
| <span data-ttu-id="f9ae5-250">children</span><span class="sxs-lookup"><span data-stu-id="f9ae5-250">children</span></span>           | <span data-ttu-id="f9ae5-251">driveitem collection</span><span class="sxs-lookup"><span data-stu-id="f9ae5-251">driveitem collection</span></span>        | <span data-ttu-id="f9ae5-p131">包含项目直接子项的 Item 对象的集合。仅表示文件夹的项目包含子项。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p131">Collection containing Item objects for the immediate children of Item. Only items representing folders have children. Read-only. Nullable.</span></span>
| <span data-ttu-id="f9ae5-256">createdByUser</span><span class="sxs-lookup"><span data-stu-id="f9ae5-256">createdByUser</span></span>      | <span data-ttu-id="f9ae5-257">[user][]</span><span class="sxs-lookup"><span data-stu-id="f9ae5-257">[user][]</span></span>                    | <span data-ttu-id="f9ae5-258">创建了项的用户的身份。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-258">Identity of the user who created the item.</span></span> <span data-ttu-id="f9ae5-259">只读。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-259">Read-only.</span></span>
| <span data-ttu-id="f9ae5-260">lastModifiedByUser</span><span class="sxs-lookup"><span data-stu-id="f9ae5-260">lastModifiedByUser</span></span> | <span data-ttu-id="f9ae5-261">[user][]</span><span class="sxs-lookup"><span data-stu-id="f9ae5-261">[user][]</span></span>                    | <span data-ttu-id="f9ae5-262">上次修改项的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-262">Identity of the user, device, and application which last modified the item. Read-only.</span></span> <span data-ttu-id="f9ae5-263">只读。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-263">Read-only.</span></span>
| <span data-ttu-id="f9ae5-264">permissions</span><span class="sxs-lookup"><span data-stu-id="f9ae5-264">permissions</span></span>        | <span data-ttu-id="f9ae5-265">[权限][] 集合</span><span class="sxs-lookup"><span data-stu-id="f9ae5-265">[permission][] collection</span></span>   | <span data-ttu-id="f9ae5-p134">项目的权限集。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p134">The set of permissions for the item. Read-only. Nullable.</span></span>
| <span data-ttu-id="f9ae5-269">缩略图</span><span class="sxs-lookup"><span data-stu-id="f9ae5-269">thumbnails</span></span>         | <span data-ttu-id="f9ae5-270">[thumbnailSet][] 集合</span><span class="sxs-lookup"><span data-stu-id="f9ae5-270">[thumbnailSet][] collection</span></span> | <span data-ttu-id="f9ae5-p135">包含与项目关联的 [ThumbnailSet][] 对象的集合。有关详细信息，请参阅 [获取缩略图][]只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p135">Collection containing [ThumbnailSet][] objects associated with the item. For more info, see [getting thumbnails][]. Read-only. Nullable.</span></span>

## <a name="instance-attributes"></a><span data-ttu-id="f9ae5-275">实例属性</span><span class="sxs-lookup"><span data-stu-id="f9ae5-275">Instance Attributes</span></span>

<span data-ttu-id="f9ae5-p136">实例属性是具有特殊行为的属性。这些属性是临时的，并且 a) 定义服务应执行的行为或 b) 提供短期的属性值，例如过期项目的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p136">Instance attributes are properties with special behaviors. These properties are temporary and either a) define behavior the service should perform or b) provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="f9ae5-278">属性名称</span><span class="sxs-lookup"><span data-stu-id="f9ae5-278">Property name</span></span>                     | <span data-ttu-id="f9ae5-279">类型</span><span class="sxs-lookup"><span data-stu-id="f9ae5-279">Type</span></span>   | <span data-ttu-id="f9ae5-280">说明</span><span class="sxs-lookup"><span data-stu-id="f9ae5-280">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="f9ae5-281">@microsoft.graph.conflictBehavior</span><span class="sxs-lookup"><span data-stu-id="f9ae5-281">@microsoft.graph.conflictBehavior</span></span> | <span data-ttu-id="f9ae5-282">string</span><span class="sxs-lookup"><span data-stu-id="f9ae5-282">string</span></span> | <span data-ttu-id="f9ae5-p137">为创建新项目的操作解决冲突的行为。你可以使用值 *fail*、*replace* 或 *rename*。PUT 的默认值是*replace*。绝不会返回包含该批注的项目。只写。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p137">The conflict resolution behavior for actions that create a new item. You can use the values *fail*, *replace*, or *rename*. The default for PUT is *replace*. An item will never be returned with this annotation. Write-only.</span></span>
| <span data-ttu-id="f9ae5-288">@microsoft.graph.downloadUrl</span><span class="sxs-lookup"><span data-stu-id="f9ae5-288">@microsoft.graph.downloadUrl</span></span>      | <span data-ttu-id="f9ae5-289">string</span><span class="sxs-lookup"><span data-stu-id="f9ae5-289">string</span></span> | <span data-ttu-id="f9ae5-p138">一个可用于下载此文件的内容的 URL。不需要使用此 URL 进行身份验证。只读。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p138">A URL that can be used to download this file's content. Authentication is not required with this URL. Read-only.</span></span>
| <span data-ttu-id="f9ae5-293">@microsoft.graph.sourceUrl</span><span class="sxs-lookup"><span data-stu-id="f9ae5-293">@microsoft.graph.sourceUrl</span></span>        | <span data-ttu-id="f9ae5-294">string</span><span class="sxs-lookup"><span data-stu-id="f9ae5-294">string</span></span> | <span data-ttu-id="f9ae5-p139">发出 PUT 请求时，此实例批注可用于指示服务下载 URL 内容并将其存储为文件。只写。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p139">When issuing a PUT request, this instance annotation can be used to instruct the service to download the contents of the URL, and store it as the file. Write-only.</span></span>

<span data-ttu-id="f9ae5-p140">**注意：**@microsoft.graph.downloadUrl 值是一个短期 URL，不能缓存。此 URL 在失效前只能使用很短的时间（1 小时）。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-p140">**Note:** The @microsoft.graph.downloadUrl value is a short-lived URL and can't be cached. The URL will only be available for a short period of time (1 hour) before it is invalidated.</span></span>

## <a name="methods"></a><span data-ttu-id="f9ae5-299">方法</span><span class="sxs-lookup"><span data-stu-id="f9ae5-299">Methods</span></span>

| <span data-ttu-id="f9ae5-300">方法</span><span class="sxs-lookup"><span data-stu-id="f9ae5-300">Method</span></span>                                                   | <span data-ttu-id="f9ae5-301">REST 路径</span><span class="sxs-lookup"><span data-stu-id="f9ae5-301">REST Path</span></span>
|:---------------------------------------------------------|:------------------
| [<span data-ttu-id="f9ae5-302">获取项目</span><span class="sxs-lookup"><span data-stu-id="f9ae5-302">Get item</span></span>](../api/driveitem_get.md)                      | `GET /drive/items/{item-id}`
| [<span data-ttu-id="f9ae5-303">列出子项</span><span class="sxs-lookup"><span data-stu-id="f9ae5-303">List children</span></span>](../api/driveitem_list_children.md)       | `GET /drive/items/{item-id}/children`
| [<span data-ttu-id="f9ae5-304">创建项目</span><span class="sxs-lookup"><span data-stu-id="f9ae5-304">Create item</span></span>](../api/driveitem_post_children.md)         | `POST /drive/items/{item-id}/children`
| [<span data-ttu-id="f9ae5-305">更新项目</span><span class="sxs-lookup"><span data-stu-id="f9ae5-305">Update item</span></span>](../api/driveitem_update.md)                | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="f9ae5-306">上载内容</span><span class="sxs-lookup"><span data-stu-id="f9ae5-306">Upload content</span></span>](../api/driveitem_put_content.md)        | `PUT /drive/items/{item-id}/content`
| [<span data-ttu-id="f9ae5-307">下载内容</span><span class="sxs-lookup"><span data-stu-id="f9ae5-307">Download content</span></span>](../api/driveitem_get_content.md)      | `GET /drive/items/{item-id}/content`
| <span data-ttu-id="f9ae5-308">[下载特定格式文件][download-format]</span><span class="sxs-lookup"><span data-stu-id="f9ae5-308">[Download specific file format][download-format]</span></span>         | `GET /drive/items/{item-id}/content?format={format}`
| [<span data-ttu-id="f9ae5-309">删除项</span><span class="sxs-lookup"><span data-stu-id="f9ae5-309">Delete item</span></span>](../api/driveitem_delete.md)                | `DELETE /drive/items/{item-id}`
| [<span data-ttu-id="f9ae5-310">移动项目</span><span class="sxs-lookup"><span data-stu-id="f9ae5-310">Move item</span></span>](../api/driveitem_move.md)                    | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="f9ae5-311">复制项目</span><span class="sxs-lookup"><span data-stu-id="f9ae5-311">Copy item</span></span>](../api/driveitem_copy.md)                    | `POST /drive/items/{item-id}/copy`
| [<span data-ttu-id="f9ae5-312">搜索项目</span><span class="sxs-lookup"><span data-stu-id="f9ae5-312">Search items</span></span>](../api/driveitem_search.md)               | `GET /drive/items/{item-id}/search(q='text')`
| [<span data-ttu-id="f9ae5-313">列出驱动器中的更改</span><span class="sxs-lookup"><span data-stu-id="f9ae5-313">List changes in a drive</span></span>](../api/driveitem_delta.md)     | `GET /drive/root/delta`
| [<span data-ttu-id="f9ae5-314">列出缩略图</span><span class="sxs-lookup"><span data-stu-id="f9ae5-314">List thumbnails</span></span>](../api/driveitem_list_thumbnails.md)   | `GET /drive/items/{item-id}/thumbnails`
| [<span data-ttu-id="f9ae5-315">创建共享链接</span><span class="sxs-lookup"><span data-stu-id="f9ae5-315">Create sharing link</span></span>](../api/driveitem_createlink.md)    | `POST /drive/items/{item-id}/createLink`
| [<span data-ttu-id="f9ae5-316">添加权限</span><span class="sxs-lookup"><span data-stu-id="f9ae5-316">Add permissions</span></span>](../api/driveitem_invite.md)            | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="f9ae5-317">列出权限</span><span class="sxs-lookup"><span data-stu-id="f9ae5-317">List permissions</span></span>](../api/driveitem_list_permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="f9ae5-318">删除权限</span><span class="sxs-lookup"><span data-stu-id="f9ae5-318">Delete permission</span></span>](../api/permission_delete.md)         | `DELETE /drive/items/{item-id}/permissions/{perm-id}`


## <a name="remarks"></a><span data-ttu-id="f9ae5-319">注解</span><span class="sxs-lookup"><span data-stu-id="f9ae5-319">Remarks</span></span>

<span data-ttu-id="f9ae5-320">在 OneDrive for Business 或 SharePoint 文档库中，如果 **driveItem** 具有 [folder][] Facet，则不返回 **cTag** 属性。</span><span class="sxs-lookup"><span data-stu-id="f9ae5-320">In OneDrive for Business or SharePoint document libraries, the **cTag** property is not returned, if the **driveItem** has a [folder][] facet.</span></span>

[audio]: audio.md
[baseItem]: baseItem.md
[Deleted]: deleted.md
[download-format]: ../api/driveitem_get_content_format.md
[File]: file.md
[fileSystemInfo]: fileSystemInfo.md
[folder]: folder.md
[getting thumbnails]: ../api/driveitem_list_thumbnails.md
[identitySet]: identitySet.md
[image]: image.md
[itemReference]: itemReference.md
[geoCoordinates]: geoCoordinates.md
[package]: package.md
[permission]: permission.md
[photo]: photo.md
[remoteItem]: remoteItem.md
[Root]: root.md
[searchResult]: searchResult.md
[Shared]: shared.md
[sharepointIds]: sharepointIds.md
[specialFolder]: specialFolder.md
[thumbnailSet]: thumbnailSet.md
[video]: video.md
[user]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/users

<!-- {
  "type": "#page.annotation",
  "description": "Item is the main data model in the OneDrive API. Everything is an item.",
  "keywords": "item,facet,resource",
  "section": "documentation",
  "tocPath": "Items",
  "tocBookmarks": { "Resources/Item": "#" }
} -->
