---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: DriveItem
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 8dbbf3b673fe7f436b9600366765425011ab129f
ms.sourcegitcommit: 3615f9475d57bfbb3a8c4402af863897f592dfbd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2019
ms.locfileid: "30789625"
---
# <a name="driveitem-resource-type"></a><span data-ttu-id="72bf3-102">DriveItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="72bf3-102">DriveItem resource type</span></span>

<span data-ttu-id="72bf3-p101">**driveItem** 资源代表文件、文件夹或存储在驱动器中的 其他项。OneDrive 和 SharePoint 中的所有文件系统对象将作为 **driveItem** 资源返回。</span><span class="sxs-lookup"><span data-stu-id="72bf3-p101">The **driveItem** resource represents a file, folder, or other item stored in a drive. All file system objects in OneDrive and SharePoint are returned as **driveItem** resources.</span></span>

<span data-ttu-id="72bf3-105">**driveItem** 资源的寻址方式主要有两种：</span><span class="sxs-lookup"><span data-stu-id="72bf3-105">There are two primary ways of addressing a **driveItem** resource:</span></span>

* <span data-ttu-id="72bf3-106">通过 **driveItem** 唯一标识符使用 `drive/items/{item-id}` 的方式</span><span class="sxs-lookup"><span data-stu-id="72bf3-106">By the **driveItem** unique identifier using `drive/items/{item-id}`</span></span>
* <span data-ttu-id="72bf3-107">通过使用文件系统路径 `/drive/root:/path/to/file` 的方式</span><span class="sxs-lookup"><span data-stu-id="72bf3-107">By file system path using `/drive/root:/path/to/file`</span></span>

<span data-ttu-id="72bf3-p102">**DriveItem** 资源拥有作为属性进行模块化的多个 Facet，用于提供 driveItem 的标识和功能相关数据。例如：</span><span class="sxs-lookup"><span data-stu-id="72bf3-p102">**DriveItem** resources have facets modeled as properties that provide data about the driveItem's identities and capabilities. For example:</span></span>

* <span data-ttu-id="72bf3-110">文件夹具有 [**folder facet**][folder]</span><span class="sxs-lookup"><span data-stu-id="72bf3-110">Folders have a [**folder facet**][folder]</span></span>
* <span data-ttu-id="72bf3-111">文件具有 [**file facet**][file]。</span><span class="sxs-lookup"><span data-stu-id="72bf3-111">Files have a [**file facet**][file].</span></span>
* <span data-ttu-id="72bf3-112">除了 file facet 之外，图像还具有 [**image facet**][image]。</span><span class="sxs-lookup"><span data-stu-id="72bf3-112">Images have an [**image facet**][image] in addition to their file facet.</span></span>
* <span data-ttu-id="72bf3-113">使用照相机拍摄的图像（照片）具有 [**photo facet**][photo]，用于将项标识为照片，并提供照片的拍摄时间和拍摄所用设备等属性。</span><span class="sxs-lookup"><span data-stu-id="72bf3-113">Images taken with a camera (photos) have a [**photo facet**][photo] that identifies the item as a photo and provides the properties of when the photo was taken and with what device.</span></span>

<span data-ttu-id="72bf3-114">具有**文件夹** Facet 的项目充当项目的容器，因此具有指向文件夹下的 **driveItems** 集合的 `children` 引用。</span><span class="sxs-lookup"><span data-stu-id="72bf3-114">Items with the **folder** facet act as containers of items and therefore have a `children` reference pointing to a collection of **driveItems** under the folder.</span></span>

## <a name="json-representation"></a><span data-ttu-id="72bf3-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="72bf3-115">JSON representation</span></span>

<span data-ttu-id="72bf3-116">下面是 **driveItem** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="72bf3-116">Here is a JSON representation of a **driveItem** resource.</span></span>

<span data-ttu-id="72bf3-117">**driveItem** 资源由 [**baseItem**][baseItem] 派生并继承该资源的属性。</span><span class="sxs-lookup"><span data-stu-id="72bf3-117">The **driveItem** resource is derived from [**baseItem**][baseItem] and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="72bf3-118">属性</span><span class="sxs-lookup"><span data-stu-id="72bf3-118">Properties</span></span>

| <span data-ttu-id="72bf3-119">属性</span><span class="sxs-lookup"><span data-stu-id="72bf3-119">Property</span></span>             | <span data-ttu-id="72bf3-120">类型</span><span class="sxs-lookup"><span data-stu-id="72bf3-120">Type</span></span>               | <span data-ttu-id="72bf3-121">说明</span><span class="sxs-lookup"><span data-stu-id="72bf3-121">Description</span></span>
|:---------------------|:-------------------|:---------------------------------
| <span data-ttu-id="72bf3-122">audio</span><span class="sxs-lookup"><span data-stu-id="72bf3-122">audio</span></span>                | <span data-ttu-id="72bf3-123">[audio][]</span><span class="sxs-lookup"><span data-stu-id="72bf3-123">[audio][]</span></span>          | <span data-ttu-id="72bf3-p103">音频元数据（如果此项是一个音频文件）。只读。</span><span class="sxs-lookup"><span data-stu-id="72bf3-p103">Audio metadata, if the item is an audio file. Read-only.</span></span>
| <span data-ttu-id="72bf3-126">content</span><span class="sxs-lookup"><span data-stu-id="72bf3-126">content</span></span>              | <span data-ttu-id="72bf3-127">流</span><span class="sxs-lookup"><span data-stu-id="72bf3-127">Stream</span></span>             | <span data-ttu-id="72bf3-128">内容流（如果此项表示一个文件）。</span><span class="sxs-lookup"><span data-stu-id="72bf3-128">The content stream, if the item represents a file.</span></span>
| <span data-ttu-id="72bf3-129">createdBy</span><span class="sxs-lookup"><span data-stu-id="72bf3-129">createdBy</span></span>            | <span data-ttu-id="72bf3-130">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="72bf3-130">[identitySet][]</span></span>    | <span data-ttu-id="72bf3-p104">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="72bf3-p104">Identity of the user, device, and application which created the item. Read-only.</span></span>
| <span data-ttu-id="72bf3-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="72bf3-133">createdDateTime</span></span>      | <span data-ttu-id="72bf3-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72bf3-134">DateTimeOffset</span></span>     | <span data-ttu-id="72bf3-p105">创建项的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="72bf3-p105">Date and time of item creation. Read-only.</span></span>
| <span data-ttu-id="72bf3-137">cTag</span><span class="sxs-lookup"><span data-stu-id="72bf3-137">cTag</span></span>                 | <span data-ttu-id="72bf3-138">String</span><span class="sxs-lookup"><span data-stu-id="72bf3-138">String</span></span>             | <span data-ttu-id="72bf3-p106">项目内容的 eTag。如果只有元数据更改，此 eTag 不会更改。**注意** 如果项目是文件夹，则不返回此属性。只读。</span><span class="sxs-lookup"><span data-stu-id="72bf3-p106">An eTag for the content of the item. This eTag is not changed if only the metadata is changed. **Note** This property is not returned if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="72bf3-143">deleted</span><span class="sxs-lookup"><span data-stu-id="72bf3-143">deleted</span></span>              | <span data-ttu-id="72bf3-144">[deleted][]</span><span class="sxs-lookup"><span data-stu-id="72bf3-144">[deleted][]</span></span>        | <span data-ttu-id="72bf3-p107">有关项目删除状态的信息。只读。</span><span class="sxs-lookup"><span data-stu-id="72bf3-p107">Information about the deleted state of the item. Read-only.</span></span>
| <span data-ttu-id="72bf3-147">description</span><span class="sxs-lookup"><span data-stu-id="72bf3-147">description</span></span>          | <span data-ttu-id="72bf3-148">字符串</span><span class="sxs-lookup"><span data-stu-id="72bf3-148">String</span></span>             | <span data-ttu-id="72bf3-p108">提供项的用户可见的说明。读写。仅在 OneDrive 个人版上</span><span class="sxs-lookup"><span data-stu-id="72bf3-p108">Provides a user-visible description of the item. Read-write. Only on OneDrive Personal</span></span>
| <span data-ttu-id="72bf3-152">eTag</span><span class="sxs-lookup"><span data-stu-id="72bf3-152">eTag</span></span>                 | <span data-ttu-id="72bf3-153">String</span><span class="sxs-lookup"><span data-stu-id="72bf3-153">String</span></span>             | <span data-ttu-id="72bf3-p109">整个项目（元数据和内容）的 eTag。只读。</span><span class="sxs-lookup"><span data-stu-id="72bf3-p109">eTag for the entire item (metadata + content). Read-only.</span></span>
| <span data-ttu-id="72bf3-156">file</span><span class="sxs-lookup"><span data-stu-id="72bf3-156">file</span></span>                 | <span data-ttu-id="72bf3-157">[file][]</span><span class="sxs-lookup"><span data-stu-id="72bf3-157">[file][]</span></span>           | <span data-ttu-id="72bf3-p110">文件元数据（如果此项是一个文件）。只读。</span><span class="sxs-lookup"><span data-stu-id="72bf3-p110">File metadata, if the item is a file. Read-only.</span></span>
| <span data-ttu-id="72bf3-160">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="72bf3-160">fileSystemInfo</span></span>       | <span data-ttu-id="72bf3-161">[fileSystemInfo][]</span><span class="sxs-lookup"><span data-stu-id="72bf3-161">[fileSystemInfo][]</span></span> | <span data-ttu-id="72bf3-p111">客户端上的文件系统信息。读写。</span><span class="sxs-lookup"><span data-stu-id="72bf3-p111">File system information on client. Read-write.</span></span>
| <span data-ttu-id="72bf3-164">folder</span><span class="sxs-lookup"><span data-stu-id="72bf3-164">folder</span></span>               | <span data-ttu-id="72bf3-165">[folder][]</span><span class="sxs-lookup"><span data-stu-id="72bf3-165">[folder][]</span></span>         | <span data-ttu-id="72bf3-p112">文件夹元数据（如果此项是一个文件夹）。只读。</span><span class="sxs-lookup"><span data-stu-id="72bf3-p112">Folder metadata, if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="72bf3-168">id</span><span class="sxs-lookup"><span data-stu-id="72bf3-168">id</span></span>                   | <span data-ttu-id="72bf3-169">String</span><span class="sxs-lookup"><span data-stu-id="72bf3-169">String</span></span>             | <span data-ttu-id="72bf3-p113">项在驱动器中的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="72bf3-p113">The unique identifier of the item within the Drive. Read-only.</span></span>
| <span data-ttu-id="72bf3-172">image</span><span class="sxs-lookup"><span data-stu-id="72bf3-172">image</span></span>                | <span data-ttu-id="72bf3-173">[image][]</span><span class="sxs-lookup"><span data-stu-id="72bf3-173">[image][]</span></span>          | <span data-ttu-id="72bf3-p114">图像元数据（如果此项是一个图像）。只读。</span><span class="sxs-lookup"><span data-stu-id="72bf3-p114">Image metadata, if the item is an image. Read-only.</span></span>
| <span data-ttu-id="72bf3-176">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="72bf3-176">lastModifiedBy</span></span>       | <span data-ttu-id="72bf3-177">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="72bf3-177">[identitySet][]</span></span>    | <span data-ttu-id="72bf3-p115">上次修改项目的用户、设备和应用程序的标识。只读。</span><span class="sxs-lookup"><span data-stu-id="72bf3-p115">Identity of the user, device, and application which last modified the item. Read-only.</span></span>
| <span data-ttu-id="72bf3-180">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="72bf3-180">lastModifiedDateTime</span></span> | <span data-ttu-id="72bf3-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72bf3-181">DateTimeOffset</span></span>     | <span data-ttu-id="72bf3-p116">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="72bf3-p116">Date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="72bf3-184">location</span><span class="sxs-lookup"><span data-stu-id="72bf3-184">location</span></span>             | <span data-ttu-id="72bf3-185">[geoCoordinates][]</span><span class="sxs-lookup"><span data-stu-id="72bf3-185">[geoCoordinates][]</span></span> | <span data-ttu-id="72bf3-p117">位置元数据（如果此项包含位置数据）。只读。</span><span class="sxs-lookup"><span data-stu-id="72bf3-p117">Location metadata, if the item has location data. Read-only.</span></span>
| <span data-ttu-id="72bf3-188">name</span><span class="sxs-lookup"><span data-stu-id="72bf3-188">name</span></span>                 | <span data-ttu-id="72bf3-189">String</span><span class="sxs-lookup"><span data-stu-id="72bf3-189">String</span></span>             | <span data-ttu-id="72bf3-p118">项目名称（文件名和扩展名）。读写。</span><span class="sxs-lookup"><span data-stu-id="72bf3-p118">The name of the item (filename and extension). Read-write.</span></span>
| <span data-ttu-id="72bf3-192">package</span><span class="sxs-lookup"><span data-stu-id="72bf3-192">package</span></span>              | <span data-ttu-id="72bf3-193">[package][]</span><span class="sxs-lookup"><span data-stu-id="72bf3-193">[package][]</span></span>        | <span data-ttu-id="72bf3-p119">如果存在，则表示此项是一个包，而不是文件夹或文件。包被视为某些上下文中的文件和其他上下文中的文件夹。只读。</span><span class="sxs-lookup"><span data-stu-id="72bf3-p119">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span>
| <span data-ttu-id="72bf3-197">parentReference</span><span class="sxs-lookup"><span data-stu-id="72bf3-197">parentReference</span></span>      | <span data-ttu-id="72bf3-198">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="72bf3-198">[itemReference][]</span></span>  | <span data-ttu-id="72bf3-p120">父信息（如果此项具有父级）。读写。</span><span class="sxs-lookup"><span data-stu-id="72bf3-p120">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="72bf3-201">photo</span><span class="sxs-lookup"><span data-stu-id="72bf3-201">photo</span></span>                | <span data-ttu-id="72bf3-202">[照片][]</span><span class="sxs-lookup"><span data-stu-id="72bf3-202">[photo][]</span></span>          | <span data-ttu-id="72bf3-p121">照片元数据（如果此项包含照片）。只读。</span><span class="sxs-lookup"><span data-stu-id="72bf3-p121">Photo metadata, if the item is a photo. Read-only.</span></span>
| <span data-ttu-id="72bf3-205">publication</span><span class="sxs-lookup"><span data-stu-id="72bf3-205">publication</span></span>          | <span data-ttu-id="72bf3-206">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="72bf3-206">[publicationFacet][]</span></span> | <span data-ttu-id="72bf3-207">在支持此类操作的位置提供有关某个项目的已发布或签出状态信息。</span><span class="sxs-lookup"><span data-stu-id="72bf3-207">Provides information about the published or checked-out state of an item, in locations that support such actions.</span></span> <span data-ttu-id="72bf3-208">默认情况下，不会返回此属性。</span><span class="sxs-lookup"><span data-stu-id="72bf3-208">This property is not returned by default.</span></span> <span data-ttu-id="72bf3-209">只读。</span><span class="sxs-lookup"><span data-stu-id="72bf3-209">Read-only.</span></span> |
| <span data-ttu-id="72bf3-210">remoteItem</span><span class="sxs-lookup"><span data-stu-id="72bf3-210">remoteItem</span></span>           | <span data-ttu-id="72bf3-211">[remoteItem][]</span><span class="sxs-lookup"><span data-stu-id="72bf3-211">[remoteItem][]</span></span>     | <span data-ttu-id="72bf3-p123">远程项目数据（如果此项是从驱动器共享的项目，而不是被访问的项目）。只读。</span><span class="sxs-lookup"><span data-stu-id="72bf3-p123">Remote item data, if the item is shared from a drive other than the one being accessed. Read-only.</span></span>
| <span data-ttu-id="72bf3-214">root</span><span class="sxs-lookup"><span data-stu-id="72bf3-214">root</span></span>                 | <span data-ttu-id="72bf3-215">[root][]</span><span class="sxs-lookup"><span data-stu-id="72bf3-215">[root][]</span></span>           | <span data-ttu-id="72bf3-216">如果此属性为非 NULL，则表明 driveItem 是驱动器中最上面的 driveItem。</span><span class="sxs-lookup"><span data-stu-id="72bf3-216">If this property is non-null, it indicates that the driveItem is the top-most driveItem in the drive.</span></span>
| <span data-ttu-id="72bf3-217">searchResult</span><span class="sxs-lookup"><span data-stu-id="72bf3-217">searchResult</span></span>         | <span data-ttu-id="72bf3-218">[searchResult][]</span><span class="sxs-lookup"><span data-stu-id="72bf3-218">[searchResult][]</span></span>   | <span data-ttu-id="72bf3-p124">搜索元数据（如果此项目来自搜索结果）。只读。</span><span class="sxs-lookup"><span data-stu-id="72bf3-p124">Search metadata, if the item is from a search result. Read-only.</span></span>
| <span data-ttu-id="72bf3-221">shared</span><span class="sxs-lookup"><span data-stu-id="72bf3-221">shared</span></span>               | <span data-ttu-id="72bf3-222">[shared][]</span><span class="sxs-lookup"><span data-stu-id="72bf3-222">[shared][]</span></span>         | <span data-ttu-id="72bf3-p125">表示此项已与他人共享，并提供有关项目共享状态的信息。只读。</span><span class="sxs-lookup"><span data-stu-id="72bf3-p125">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>
| <span data-ttu-id="72bf3-225">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="72bf3-225">sharepointIds</span></span>        | <span data-ttu-id="72bf3-226">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="72bf3-226">[sharepointIds][]</span></span>  | <span data-ttu-id="72bf3-p126">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="72bf3-p126">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="72bf3-229">size</span><span class="sxs-lookup"><span data-stu-id="72bf3-229">size</span></span>                 | <span data-ttu-id="72bf3-230">Int64</span><span class="sxs-lookup"><span data-stu-id="72bf3-230">Int64</span></span>              | <span data-ttu-id="72bf3-p127">项目大小，以字节为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="72bf3-p127">Size of the item in bytes. Read-only.</span></span>
| <span data-ttu-id="72bf3-233">specialFolder</span><span class="sxs-lookup"><span data-stu-id="72bf3-233">specialFolder</span></span>        | <span data-ttu-id="72bf3-234">[specialFolder][]</span><span class="sxs-lookup"><span data-stu-id="72bf3-234">[specialFolder][]</span></span>  | <span data-ttu-id="72bf3-p128">如果当前项同时也是一个特殊的文件夹，则返回此 facet。只读。</span><span class="sxs-lookup"><span data-stu-id="72bf3-p128">If the current item is also available as a special folder, this facet is returned. Read-only.</span></span>
| <span data-ttu-id="72bf3-237">video</span><span class="sxs-lookup"><span data-stu-id="72bf3-237">video</span></span>                | <span data-ttu-id="72bf3-238">[video][]</span><span class="sxs-lookup"><span data-stu-id="72bf3-238">[video][]</span></span>          | <span data-ttu-id="72bf3-p129">视频元数据（如果此项是一个视频）。只读。</span><span class="sxs-lookup"><span data-stu-id="72bf3-p129">Video metadata, if the item is a video. Read-only.</span></span>
| <span data-ttu-id="72bf3-241">WebDavUrl</span><span class="sxs-lookup"><span data-stu-id="72bf3-241">webDavUrl</span></span>            | <span data-ttu-id="72bf3-242">String</span><span class="sxs-lookup"><span data-stu-id="72bf3-242">String</span></span>             | <span data-ttu-id="72bf3-243">项的可兼容 WebDAV 的 URL。</span><span class="sxs-lookup"><span data-stu-id="72bf3-243">WebDAV compatible URL for the item.</span></span>
| <span data-ttu-id="72bf3-244">WebUrl</span><span class="sxs-lookup"><span data-stu-id="72bf3-244">webUrl</span></span>               | <span data-ttu-id="72bf3-245">String</span><span class="sxs-lookup"><span data-stu-id="72bf3-245">String</span></span>             | <span data-ttu-id="72bf3-p130">在浏览器中显示此资源的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="72bf3-p130">URL that displays the resource in the browser. Read-only.</span></span>

<span data-ttu-id="72bf3-p131">**注意：** ETag 和 cTag 属性在容器（文件夹）中以不同的方式工作。更改任意文件夹后代的内容或元数据时，也会修改 CTag 值。除了从后代派生的属性（例如 **childCount** 或 **lastModifiedDateTime**），仅在更改文件夹的属性时修改 eTag 值。</span><span class="sxs-lookup"><span data-stu-id="72bf3-p131">**Note:** The eTag and cTag properties work differently on containers (folders). The cTag value is modified when content or metadata of any descendant of the folder is changed. The eTag value is only modified when the folder's properties are changed, except for properties that are derived from descendants (like **childCount** or **lastModifiedDateTime**).</span></span>

## <a name="relationships"></a><span data-ttu-id="72bf3-251">关系</span><span class="sxs-lookup"><span data-stu-id="72bf3-251">Relationships</span></span>

| <span data-ttu-id="72bf3-252">关系</span><span class="sxs-lookup"><span data-stu-id="72bf3-252">Relationship</span></span>       | <span data-ttu-id="72bf3-253">类型</span><span class="sxs-lookup"><span data-stu-id="72bf3-253">Type</span></span>                        | <span data-ttu-id="72bf3-254">说明</span><span class="sxs-lookup"><span data-stu-id="72bf3-254">Description</span></span>
|:-------------------|:----------------------------|:--------------------------
| <span data-ttu-id="72bf3-255">children</span><span class="sxs-lookup"><span data-stu-id="72bf3-255">children</span></span>           | <span data-ttu-id="72bf3-256">driveItem 集合</span><span class="sxs-lookup"><span data-stu-id="72bf3-256">driveItem collection</span></span>        | <span data-ttu-id="72bf3-p132">包含项目直接子项的 Item 对象的集合。仅表示文件夹的项目包含子项。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="72bf3-p132">Collection containing Item objects for the immediate children of Item. Only items representing folders have children. Read-only. Nullable.</span></span>
| <span data-ttu-id="72bf3-261">createdByUser</span><span class="sxs-lookup"><span data-stu-id="72bf3-261">createdByUser</span></span>      | <span data-ttu-id="72bf3-262">[user][]</span><span class="sxs-lookup"><span data-stu-id="72bf3-262">[user][]</span></span>                    | <span data-ttu-id="72bf3-263">创建了项的用户的身份。</span><span class="sxs-lookup"><span data-stu-id="72bf3-263">Identity of the user who created the item.</span></span> <span data-ttu-id="72bf3-264">只读。</span><span class="sxs-lookup"><span data-stu-id="72bf3-264">Read-only.</span></span>
| <span data-ttu-id="72bf3-265">lastModifiedByUser</span><span class="sxs-lookup"><span data-stu-id="72bf3-265">lastModifiedByUser</span></span> | <span data-ttu-id="72bf3-266">[user][]</span><span class="sxs-lookup"><span data-stu-id="72bf3-266">[user][]</span></span>                    | <span data-ttu-id="72bf3-267">上次修改项的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="72bf3-267">Identity of the user who last modified the item.</span></span> <span data-ttu-id="72bf3-268">只读。</span><span class="sxs-lookup"><span data-stu-id="72bf3-268">Read-only.</span></span>
| <span data-ttu-id="72bf3-269">listItem</span><span class="sxs-lookup"><span data-stu-id="72bf3-269">listItem</span></span>           | <span data-ttu-id="72bf3-270">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="72bf3-270">[listItem][]</span></span>                | <span data-ttu-id="72bf3-271">对于 SharePoint 中的驱动器，关联的文档库列表项。</span><span class="sxs-lookup"><span data-stu-id="72bf3-271">For drives in SharePoint, the associated document library list item.</span></span> <span data-ttu-id="72bf3-272">只读。</span><span class="sxs-lookup"><span data-stu-id="72bf3-272">Read-only.</span></span> <span data-ttu-id="72bf3-273">可为 null。</span><span class="sxs-lookup"><span data-stu-id="72bf3-273">Nullable.</span></span>
| <span data-ttu-id="72bf3-274">permissions</span><span class="sxs-lookup"><span data-stu-id="72bf3-274">permissions</span></span>        | <span data-ttu-id="72bf3-275">[permission][] 集合</span><span class="sxs-lookup"><span data-stu-id="72bf3-275">[permission][] collection</span></span>   | <span data-ttu-id="72bf3-p136">项目的权限集。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="72bf3-p136">The set of permissions for the item. Read-only. Nullable.</span></span>
| <span data-ttu-id="72bf3-279">订阅</span><span class="sxs-lookup"><span data-stu-id="72bf3-279">Subscriptions</span></span>      | <span data-ttu-id="72bf3-280">[订阅][]集合</span><span class="sxs-lookup"><span data-stu-id="72bf3-280">[subscription][] collection</span></span> | <span data-ttu-id="72bf3-281">项目上的订阅集。</span><span class="sxs-lookup"><span data-stu-id="72bf3-281">The set of subscriptions on the item.</span></span> <span data-ttu-id="72bf3-282">仅在驱动器根目录上支持。</span><span class="sxs-lookup"><span data-stu-id="72bf3-282">Only supported on the root of a drive.</span></span>
| <span data-ttu-id="72bf3-283">缩略图</span><span class="sxs-lookup"><span data-stu-id="72bf3-283">thumbnails</span></span>         | <span data-ttu-id="72bf3-284">[thumbnailSet][] 集合</span><span class="sxs-lookup"><span data-stu-id="72bf3-284">[thumbnailSet][] collection</span></span> | <span data-ttu-id="72bf3-p138">包含与项目关联的 [ThumbnailSet][] 对象的集合。有关详细信息，请参阅 [获取缩略图][]只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="72bf3-p138">Collection containing [ThumbnailSet][] objects associated with the item. For more info, see [getting thumbnails][]. Read-only. Nullable.</span></span>
| <span data-ttu-id="72bf3-289">版本</span><span class="sxs-lookup"><span data-stu-id="72bf3-289">versions</span></span>           | <span data-ttu-id="72bf3-290">[driveItemVersion][] 集合</span><span class="sxs-lookup"><span data-stu-id="72bf3-290">[driveItemVersion][] collection</span></span> | <span data-ttu-id="72bf3-291">旧版本项的列表。</span><span class="sxs-lookup"><span data-stu-id="72bf3-291">The list of previous versions of the item.</span></span> <span data-ttu-id="72bf3-292">有关详细信息，请参阅[获取旧版本][]。</span><span class="sxs-lookup"><span data-stu-id="72bf3-292">For more info, see [getting previous versions][].</span></span> <span data-ttu-id="72bf3-293">只读。</span><span class="sxs-lookup"><span data-stu-id="72bf3-293">Read-only.</span></span> <span data-ttu-id="72bf3-294">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="72bf3-294">Nullable.</span></span>
| <span data-ttu-id="72bf3-295">工作簿</span><span class="sxs-lookup"><span data-stu-id="72bf3-295">workbook</span></span>           | <span data-ttu-id="72bf3-296">[workbook][]</span><span class="sxs-lookup"><span data-stu-id="72bf3-296">[workbook][]</span></span>                | <span data-ttu-id="72bf3-297">如果是 Excel 工作表文件，访问工作簿 API 以使用工作表的内容。</span><span class="sxs-lookup"><span data-stu-id="72bf3-297">For files that are Excel spreadsheets, accesses the workbook API to work with the spreadsheet's contents.</span></span> <span data-ttu-id="72bf3-298">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="72bf3-298">Nullable.</span></span>

## <a name="instance-attributes"></a><span data-ttu-id="72bf3-299">实例属性</span><span class="sxs-lookup"><span data-stu-id="72bf3-299">Instance Attributes</span></span>

<span data-ttu-id="72bf3-p141">实例属性是具有特殊行为的属性。这些属性是临时的，并且 a) 定义服务应执行的行为或 b) 提供短期的属性值，例如过期项目的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="72bf3-p141">Instance attributes are properties with special behaviors. These properties are temporary and either a) define behavior the service should perform or b) provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="72bf3-302">属性名称</span><span class="sxs-lookup"><span data-stu-id="72bf3-302">Property name</span></span>                     | <span data-ttu-id="72bf3-303">类型</span><span class="sxs-lookup"><span data-stu-id="72bf3-303">Type</span></span>   | <span data-ttu-id="72bf3-304">说明</span><span class="sxs-lookup"><span data-stu-id="72bf3-304">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="72bf3-305">@microsoft.graph.conflictBehavior</span><span class="sxs-lookup"><span data-stu-id="72bf3-305">@microsoft.graph.conflictBehavior</span></span> | <span data-ttu-id="72bf3-306">string</span><span class="sxs-lookup"><span data-stu-id="72bf3-306">string</span></span> | <span data-ttu-id="72bf3-p142">为创建新项目的操作解决冲突的行为。你可以使用值 *fail*、*replace* 或 *rename*。PUT 的默认值是*replace*。绝不会返回包含该批注的项目。只写。</span><span class="sxs-lookup"><span data-stu-id="72bf3-p142">The conflict resolution behavior for actions that create a new item. You can use the values *fail*, *replace*, or *rename*. The default for PUT is *replace*. An item will never be returned with this annotation. Write-only.</span></span>
| <span data-ttu-id="72bf3-312">@microsoft.graph.downloadUrl</span><span class="sxs-lookup"><span data-stu-id="72bf3-312">@microsoft.graph.downloadUrl</span></span>      | <span data-ttu-id="72bf3-313">string</span><span class="sxs-lookup"><span data-stu-id="72bf3-313">string</span></span> | <span data-ttu-id="72bf3-p143">一个可用于下载此文件的内容的 URL。不需要使用此 URL 进行身份验证。只读。</span><span class="sxs-lookup"><span data-stu-id="72bf3-p143">A URL that can be used to download this file's content. Authentication is not required with this URL. Read-only.</span></span>
| <span data-ttu-id="72bf3-317">@microsoft.graph.sourceUrl</span><span class="sxs-lookup"><span data-stu-id="72bf3-317">@microsoft.graph.sourceUrl</span></span>        | <span data-ttu-id="72bf3-318">string</span><span class="sxs-lookup"><span data-stu-id="72bf3-318">string</span></span> | <span data-ttu-id="72bf3-p144">发出 PUT 请求时，此实例批注可用于指示服务下载 URL 内容并将其存储为文件。只写。</span><span class="sxs-lookup"><span data-stu-id="72bf3-p144">When issuing a PUT request, this instance annotation can be used to instruct the service to download the contents of the URL, and store it as the file. Write-only.</span></span>

<span data-ttu-id="72bf3-321">**注意：**@microsoft.graph.downloadUrl 值是一个短期 URL，不能缓存。</span><span class="sxs-lookup"><span data-stu-id="72bf3-321">**Note:** The @microsoft.graph.downloadUrl value is a short-lived URL and can't be cached.</span></span>
<span data-ttu-id="72bf3-322">此 URL 在失效前只能使用很短的时间（1 小时）。</span><span class="sxs-lookup"><span data-stu-id="72bf3-322">The URL will only be available for a short period of time (1 hour) before it is invalidated.</span></span>
<span data-ttu-id="72bf3-323">删除用户的文件权限可能不会立即使 URL 无效。</span><span class="sxs-lookup"><span data-stu-id="72bf3-323">Removing file permissions for a user may not immediately invalidate the URL.</span></span>

## <a name="methods"></a><span data-ttu-id="72bf3-324">方法</span><span class="sxs-lookup"><span data-stu-id="72bf3-324">Methods</span></span>

| <span data-ttu-id="72bf3-325">方法</span><span class="sxs-lookup"><span data-stu-id="72bf3-325">Method</span></span>                                                   | <span data-ttu-id="72bf3-326">REST 路径</span><span class="sxs-lookup"><span data-stu-id="72bf3-326">REST Path</span></span>
|:---------------------------------------------------------|:------------------
| [<span data-ttu-id="72bf3-327">获取项目</span><span class="sxs-lookup"><span data-stu-id="72bf3-327">Get item</span></span>](../api/driveitem-get.md)                      | `GET /drive/items/{item-id}`
| [<span data-ttu-id="72bf3-328">列出子项</span><span class="sxs-lookup"><span data-stu-id="72bf3-328">List children</span></span>](../api/driveitem-list-children.md)       | `GET /drive/items/{item-id}/children`
| [<span data-ttu-id="72bf3-329">列出版本</span><span class="sxs-lookup"><span data-stu-id="72bf3-329">List versions</span></span>](../api/driveitem-list-versions.md)       | `GET /drive/items/{item-id}/versions`
| [<span data-ttu-id="72bf3-330">创建项目</span><span class="sxs-lookup"><span data-stu-id="72bf3-330">Create item</span></span>](../api/driveitem-post-children.md)         | `POST /drive/items/{item-id}/children`
| [<span data-ttu-id="72bf3-331">更新项目</span><span class="sxs-lookup"><span data-stu-id="72bf3-331">Update item</span></span>](../api/driveitem-update.md)                | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="72bf3-332">上载内容</span><span class="sxs-lookup"><span data-stu-id="72bf3-332">Upload content</span></span>](../api/driveitem-put-content.md)        | `PUT /drive/items/{item-id}/content`
| [<span data-ttu-id="72bf3-333">下载内容</span><span class="sxs-lookup"><span data-stu-id="72bf3-333">Download content</span></span>](../api/driveitem-get-content.md)      | `GET /drive/items/{item-id}/content`
| <span data-ttu-id="72bf3-334">[下载特定格式文件][download-format]</span><span class="sxs-lookup"><span data-stu-id="72bf3-334">[Download specific file format][download-format]</span></span>         | `GET /drive/items/{item-id}/content?format={format}`
| [<span data-ttu-id="72bf3-335">删除项</span><span class="sxs-lookup"><span data-stu-id="72bf3-335">Delete item</span></span>](../api/driveitem-delete.md)                | `DELETE /drive/items/{item-id}`
| [<span data-ttu-id="72bf3-336">移动项目</span><span class="sxs-lookup"><span data-stu-id="72bf3-336">Move item</span></span>](../api/driveitem-move.md)                    | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="72bf3-337">复制项目</span><span class="sxs-lookup"><span data-stu-id="72bf3-337">Copy item</span></span>](../api/driveitem-copy.md)                    | `POST /drive/items/{item-id}/copy`
| [<span data-ttu-id="72bf3-338">搜索项目</span><span class="sxs-lookup"><span data-stu-id="72bf3-338">Search items</span></span>](../api/driveitem-search.md)               | `GET /drive/items/{item-id}/search(q='text')`
| [<span data-ttu-id="72bf3-339">列出驱动器中的更改</span><span class="sxs-lookup"><span data-stu-id="72bf3-339">List changes in a drive</span></span>](../api/driveitem-delta.md)     | `GET /drive/root/delta`
| [<span data-ttu-id="72bf3-340">列出缩略图</span><span class="sxs-lookup"><span data-stu-id="72bf3-340">List thumbnails</span></span>](../api/driveitem-list-thumbnails.md)   | `GET /drive/items/{item-id}/thumbnails`
| [<span data-ttu-id="72bf3-341">创建共享链接</span><span class="sxs-lookup"><span data-stu-id="72bf3-341">Create sharing link</span></span>](../api/driveitem-createlink.md)    | `POST /drive/items/{item-id}/createLink`
| [<span data-ttu-id="72bf3-342">添加权限</span><span class="sxs-lookup"><span data-stu-id="72bf3-342">Add permissions</span></span>](../api/driveitem-invite.md)            | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="72bf3-343">列出权限</span><span class="sxs-lookup"><span data-stu-id="72bf3-343">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="72bf3-344">删除权限</span><span class="sxs-lookup"><span data-stu-id="72bf3-344">Delete permission</span></span>](../api/permission-delete.md)         | `DELETE /drive/items/{item-id}/permissions/{perm-id}`
| <span data-ttu-id="72bf3-345">[获取 WebSocket 频道][getWebSocket]</span><span class="sxs-lookup"><span data-stu-id="72bf3-345">[Get WebSocket channel][getWebSocket]</span></span>                    | `GET /drive/root/subscriptions/socketIo`
| <span data-ttu-id="72bf3-346">[预览项][item-preview]</span><span class="sxs-lookup"><span data-stu-id="72bf3-346">[Preview item][item-preview]</span></span>                             | `POST /drive/items/{item-id}/preview`

[item-preview]: ../api/driveitem-preview.md

## <a name="remarks"></a><span data-ttu-id="72bf3-347">说明</span><span class="sxs-lookup"><span data-stu-id="72bf3-347">Remarks</span></span>

<span data-ttu-id="72bf3-348">在 OneDrive for Business 或 SharePoint 文档库中，如果 **driveItem** 具有[folder][] Facet，则不返回 **cTag** 属性。</span><span class="sxs-lookup"><span data-stu-id="72bf3-348">In OneDrive for Business or SharePoint document libraries, the **cTag** property is not returned, if the **driveItem** has a [folder][] facet.</span></span>

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
[getWebSocket]: ../api/driveitem-subscriptions-socketio.md
[identitySet]: identityset.md
[image]: image.md
[itemReference]: itemreference.md
[geoCoordinates]: geocoordinates.md
[listItem]: listitem.md
[package]: package.md
[permission]: permission.md
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
[user]: https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/users
[publicationFacet]: publicationfacet.md

<!-- {
  "type": "#page.annotation",
  "description": "Item is the main data model in the OneDrive API. Everything is an item.",
  "keywords": "item,facet,resource",
  "section": "documentation",
  "tocPath": "Items",
  "tocBookmarks": { "Resources/Item": "#" }
} -->
