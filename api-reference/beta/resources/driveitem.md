---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveItem
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 98930017f9ca3f70501cd10e4a3029f7a240ce41
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977772"
---
# <a name="driveitem-resource-type"></a><span data-ttu-id="cc4e8-102">driveItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="cc4e8-102">driveItem resource type</span></span>

> <span data-ttu-id="cc4e8-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cc4e8-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cc4e8-p102">**driveItem** 资源代表文件、文件夹或存储在驱动器中的 其他项。OneDrive 和 SharePoint 中的所有文件系统对象将作为 **driveItem** 资源返回。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p102">The **driveItem** resource represents a file, folder, or other item stored in a drive. All file system objects in OneDrive and SharePoint are returned as **driveItem** resources.</span></span>

<span data-ttu-id="cc4e8-107">**driveItem** 资源的寻址方式主要有两种：</span><span class="sxs-lookup"><span data-stu-id="cc4e8-107">There are two primary ways of addressing a **driveItem** resource:</span></span>

* <span data-ttu-id="cc4e8-108">通过 **driveItem** 唯一标识符使用 `drive/items/{item-id}` 的方式</span><span class="sxs-lookup"><span data-stu-id="cc4e8-108">By the **driveItem** unique identifier using `drive/items/{item-id}`</span></span>
* <span data-ttu-id="cc4e8-109">通过使用文件系统路径 `/drive/root:/path/to/file` 的方式</span><span class="sxs-lookup"><span data-stu-id="cc4e8-109">By file system path using `/drive/root:/path/to/file`</span></span>

<span data-ttu-id="cc4e8-p103">**DriveItem** 资源拥有作为属性进行模块化的多个 Facet，用于提供 driveItem 的标识和功能相关数据。例如：</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p103">**DriveItem** resources have facets modeled as properties that provide data about the driveItem's identities and capabilities. For example:</span></span>

* <span data-ttu-id="cc4e8-112">文件夹具有[**文件夹 facet**][folder]</span><span class="sxs-lookup"><span data-stu-id="cc4e8-112">Folders have a [**folder facet**][folder]</span></span>
* <span data-ttu-id="cc4e8-113">文件具有[**文件 facet**][file]。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-113">Files have a [**file facet**][file].</span></span>
* <span data-ttu-id="cc4e8-114">除了文件 facet，图像还具有[**图像 facet**][image]。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-114">Images have an [**image facet**][image] in addition to their file facet.</span></span>
* <span data-ttu-id="cc4e8-115">使用照相机拍摄的图像（照片）具有[**照片 facet**][photo]，用于将项标识为照片，并提供照片的拍摄时间和拍摄所用设备等属性。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-115">Images taken with a camera (photos) have a [**photo facet**][photo] that identifies the item as a photo and provides the properties of when the photo was taken and with what device.</span></span>

<span data-ttu-id="cc4e8-116">具有**文件夹** Facet 的项目充当项目的容器，因此具有指向文件夹下的 **driveItems** 集合的 `children` 引用。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-116">Items with the **folder** facet act as containers of items and therefore have a `children` reference pointing to a collection of **driveItems** under the folder.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc4e8-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cc4e8-117">JSON representation</span></span>

<span data-ttu-id="cc4e8-118">下面是 **driveItem** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-118">Here is a JSON representation of a **driveItem** resource.</span></span>

<span data-ttu-id="cc4e8-119">**driveItem** 资源由 [**baseItem**][baseItem] 派生并继承该资源的属性。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-119">The **driveItem** resource is derived from [**baseItem**][baseItem] and inherits properties from that resource.</span></span>

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
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "content": { "@odata.type": "Edm.Stream" },
  "children": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "permissions": [ {"@odata.type": "microsoft.graph.permission"} ],
  "thumbnails": [ {"@odata.type": "microsoft.graph.thumbnailSet"}],
  "versions": [ {"@odata.type": "Collection(microsoft.graph.driveItemVersion)"}],

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

## <a name="properties"></a><span data-ttu-id="cc4e8-120">属性</span><span class="sxs-lookup"><span data-stu-id="cc4e8-120">Properties</span></span>

| <span data-ttu-id="cc4e8-121">属性</span><span class="sxs-lookup"><span data-stu-id="cc4e8-121">Property</span></span>             | <span data-ttu-id="cc4e8-122">类型</span><span class="sxs-lookup"><span data-stu-id="cc4e8-122">Type</span></span>               | <span data-ttu-id="cc4e8-123">说明</span><span class="sxs-lookup"><span data-stu-id="cc4e8-123">Description</span></span>
|:---------------------|:-------------------|:---------------------------------
| <span data-ttu-id="cc4e8-124">audio</span><span class="sxs-lookup"><span data-stu-id="cc4e8-124">audio</span></span>                | <span data-ttu-id="cc4e8-125">[音频][]</span><span class="sxs-lookup"><span data-stu-id="cc4e8-125">[audio][]</span></span>          | <span data-ttu-id="cc4e8-p104">音频元数据（如果此项是一个音频文件）。只读。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p104">Audio metadata, if the item is an audio file. Read-only.</span></span>
| <span data-ttu-id="cc4e8-128">createdBy</span><span class="sxs-lookup"><span data-stu-id="cc4e8-128">createdBy</span></span>            | <span data-ttu-id="cc4e8-129">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="cc4e8-129">[identitySet][]</span></span>    | <span data-ttu-id="cc4e8-p105">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p105">Identity of the user, device, and application which created the item. Read-only.</span></span>
| <span data-ttu-id="cc4e8-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cc4e8-132">createdDateTime</span></span>      | <span data-ttu-id="cc4e8-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc4e8-133">DateTimeOffset</span></span>     | <span data-ttu-id="cc4e8-p106">创建项的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p106">Date and time of item creation. Read-only.</span></span>
| <span data-ttu-id="cc4e8-136">cTag</span><span class="sxs-lookup"><span data-stu-id="cc4e8-136">cTag</span></span>                 | <span data-ttu-id="cc4e8-137">String</span><span class="sxs-lookup"><span data-stu-id="cc4e8-137">String</span></span>             | <span data-ttu-id="cc4e8-p107">项目内容的 eTag。如果只有元数据更改，此 eTag 不会更改。**注意** 如果项目是文件夹，则不返回此属性。只读。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p107">An eTag for the content of the item. This eTag is not changed if only the metadata is changed. **Note** This property is not returned if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="cc4e8-142">deleted</span><span class="sxs-lookup"><span data-stu-id="cc4e8-142">deleted</span></span>              | <span data-ttu-id="cc4e8-143">[deleted][]</span><span class="sxs-lookup"><span data-stu-id="cc4e8-143">[deleted][]</span></span>        | <span data-ttu-id="cc4e8-p108">有关项目删除状态的信息。只读。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p108">Information about the deleted state of the item. Read-only.</span></span>
| <span data-ttu-id="cc4e8-146">说明</span><span class="sxs-lookup"><span data-stu-id="cc4e8-146">description</span></span>          | <span data-ttu-id="cc4e8-147">字符串</span><span class="sxs-lookup"><span data-stu-id="cc4e8-147">String</span></span>             | <span data-ttu-id="cc4e8-p109">提供项的用户可见的说明。读写。仅在 OneDrive 个人版上</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p109">Provides a user-visible description of the item. Read-write. Only on OneDrive Personal</span></span>
| <span data-ttu-id="cc4e8-151">eTag</span><span class="sxs-lookup"><span data-stu-id="cc4e8-151">eTag</span></span>                 | <span data-ttu-id="cc4e8-152">String</span><span class="sxs-lookup"><span data-stu-id="cc4e8-152">String</span></span>             | <span data-ttu-id="cc4e8-p110">整个项目（元数据和内容）的 eTag。只读。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p110">eTag for the entire item (metadata + content). Read-only.</span></span>
| <span data-ttu-id="cc4e8-155">file</span><span class="sxs-lookup"><span data-stu-id="cc4e8-155">file</span></span>                 | <span data-ttu-id="cc4e8-156">[file][]</span><span class="sxs-lookup"><span data-stu-id="cc4e8-156">[file][]</span></span>           | <span data-ttu-id="cc4e8-p111">文件元数据（如果此项是一个文件）。只读。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p111">File metadata, if the item is a file. Read-only.</span></span>
| <span data-ttu-id="cc4e8-159">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="cc4e8-159">fileSystemInfo</span></span>       | <span data-ttu-id="cc4e8-160">[fileSystemInfo][]</span><span class="sxs-lookup"><span data-stu-id="cc4e8-160">[fileSystemInfo][]</span></span> | <span data-ttu-id="cc4e8-p112">客户端上的文件系统信息。读写。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p112">File system information on client. Read-write.</span></span>
| <span data-ttu-id="cc4e8-163">folder</span><span class="sxs-lookup"><span data-stu-id="cc4e8-163">folder</span></span>               | <span data-ttu-id="cc4e8-164">[folder][]</span><span class="sxs-lookup"><span data-stu-id="cc4e8-164">[folder][]</span></span>         | <span data-ttu-id="cc4e8-p113">文件夹元数据（如果此项是一个文件夹）。只读。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p113">Folder metadata, if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="cc4e8-167">id</span><span class="sxs-lookup"><span data-stu-id="cc4e8-167">id</span></span>                   | <span data-ttu-id="cc4e8-168">字符串</span><span class="sxs-lookup"><span data-stu-id="cc4e8-168">String</span></span>             | <span data-ttu-id="cc4e8-p114">项在驱动器中的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p114">The unique identifier of the item within the Drive. Read-only.</span></span>
| <span data-ttu-id="cc4e8-171">image</span><span class="sxs-lookup"><span data-stu-id="cc4e8-171">image</span></span>                | <span data-ttu-id="cc4e8-172">[image][]</span><span class="sxs-lookup"><span data-stu-id="cc4e8-172">[image][]</span></span>          | <span data-ttu-id="cc4e8-p115">图像元数据（如果此项是一个图像）。只读。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p115">Image metadata, if the item is an image. Read-only.</span></span>
| <span data-ttu-id="cc4e8-175">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="cc4e8-175">lastModifiedBy</span></span>       | <span data-ttu-id="cc4e8-176">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="cc4e8-176">[identitySet][]</span></span>    | <span data-ttu-id="cc4e8-p116">上次修改项目的用户、设备和应用程序的标识。只读。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p116">Identity of the user, device, and application which last modified the item. Read-only.</span></span>
| <span data-ttu-id="cc4e8-179">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc4e8-179">lastModifiedDateTime</span></span> | <span data-ttu-id="cc4e8-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc4e8-180">DateTimeOffset</span></span>     | <span data-ttu-id="cc4e8-p117">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p117">Date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="cc4e8-183">location</span><span class="sxs-lookup"><span data-stu-id="cc4e8-183">location</span></span>             | <span data-ttu-id="cc4e8-184">[geoCoordinates][]</span><span class="sxs-lookup"><span data-stu-id="cc4e8-184">[geoCoordinates][]</span></span> | <span data-ttu-id="cc4e8-p118">位置元数据（如果此项包含位置数据）。只读。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p118">Location metadata, if the item has location data. Read-only.</span></span>
| <span data-ttu-id="cc4e8-187">name</span><span class="sxs-lookup"><span data-stu-id="cc4e8-187">name</span></span>                 | <span data-ttu-id="cc4e8-188">字符串</span><span class="sxs-lookup"><span data-stu-id="cc4e8-188">String</span></span>             | <span data-ttu-id="cc4e8-p119">项目名称（文件名和扩展名）。读写。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p119">The name of the item (filename and extension). Read-write.</span></span>
| <span data-ttu-id="cc4e8-191">包</span><span class="sxs-lookup"><span data-stu-id="cc4e8-191">package</span></span>              | <span data-ttu-id="cc4e8-192">[package][]</span><span class="sxs-lookup"><span data-stu-id="cc4e8-192">[package][]</span></span>        | <span data-ttu-id="cc4e8-p120">如果存在，则表示此项是一个包，而不是文件夹或文件。包被视为某些上下文中的文件和其他上下文中的文件夹。只读。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p120">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span>
| <span data-ttu-id="cc4e8-196">parentReference</span><span class="sxs-lookup"><span data-stu-id="cc4e8-196">parentReference</span></span>      | <span data-ttu-id="cc4e8-197">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="cc4e8-197">[itemReference][]</span></span>  | <span data-ttu-id="cc4e8-p121">父信息（如果此项具有父级）。读写。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p121">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="cc4e8-200">photo</span><span class="sxs-lookup"><span data-stu-id="cc4e8-200">photo</span></span>                | <span data-ttu-id="cc4e8-201">[照片][]</span><span class="sxs-lookup"><span data-stu-id="cc4e8-201">[photo][]</span></span>          | <span data-ttu-id="cc4e8-p122">照片元数据（如果此项包含照片）。只读。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p122">Photo metadata, if the item is a photo. Read-only.</span></span>
| <span data-ttu-id="cc4e8-204">publication</span><span class="sxs-lookup"><span data-stu-id="cc4e8-204">publication</span></span>          | <span data-ttu-id="cc4e8-205">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="cc4e8-205">[publicationFacet][]</span></span> | <span data-ttu-id="cc4e8-206">在支持此类操作的位置提供有关某个项目的已发布或签出状态信息。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-206">Provides information about the published or checked-out state of an item, in locations that support such actions.</span></span> <span data-ttu-id="cc4e8-207">默认情况下，不会返回此属性。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-207">This property is not returned by default.</span></span> <span data-ttu-id="cc4e8-208">只读。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-208">Read-only.</span></span> |
| <span data-ttu-id="cc4e8-209">remoteItem</span><span class="sxs-lookup"><span data-stu-id="cc4e8-209">remoteItem</span></span>           | <span data-ttu-id="cc4e8-210">[remoteItem][]</span><span class="sxs-lookup"><span data-stu-id="cc4e8-210">[remoteItem][]</span></span>     | <span data-ttu-id="cc4e8-p124">远程项目数据（如果此项是从驱动器共享的项目，而不是被访问的项目）。只读。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p124">Remote item data, if the item is shared from a drive other than the one being accessed. Read-only.</span></span>
| <span data-ttu-id="cc4e8-213">root</span><span class="sxs-lookup"><span data-stu-id="cc4e8-213">root</span></span>                 | <span data-ttu-id="cc4e8-214">[根][]</span><span class="sxs-lookup"><span data-stu-id="cc4e8-214">[root][]</span></span>           | <span data-ttu-id="cc4e8-215">如果此属性为非 NULL，则表明 driveItem 是驱动器中最上面的 driveItem。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-215">If this property is non-null, it indicates that the driveItem is the top-most driveItem in the drive.</span></span>
| <span data-ttu-id="cc4e8-216">searchResult</span><span class="sxs-lookup"><span data-stu-id="cc4e8-216">searchResult</span></span>         | <span data-ttu-id="cc4e8-217">[searchResult][]</span><span class="sxs-lookup"><span data-stu-id="cc4e8-217">[searchResult][]</span></span>   | <span data-ttu-id="cc4e8-p125">搜索元数据（如果此项目来自搜索结果）。只读。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p125">Search metadata, if the item is from a search result. Read-only.</span></span>
| <span data-ttu-id="cc4e8-220">shared</span><span class="sxs-lookup"><span data-stu-id="cc4e8-220">shared</span></span>               | <span data-ttu-id="cc4e8-221">[共享][]</span><span class="sxs-lookup"><span data-stu-id="cc4e8-221">[shared][]</span></span>         | <span data-ttu-id="cc4e8-p126">表示此项已与他人共享，并提供有关项目共享状态的信息。只读。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p126">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>
| <span data-ttu-id="cc4e8-224">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="cc4e8-224">sharepointIds</span></span>        | <span data-ttu-id="cc4e8-225">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="cc4e8-225">[sharepointIds][]</span></span>  | <span data-ttu-id="cc4e8-p127">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p127">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="cc4e8-228">size</span><span class="sxs-lookup"><span data-stu-id="cc4e8-228">size</span></span>                 | <span data-ttu-id="cc4e8-229">Int64</span><span class="sxs-lookup"><span data-stu-id="cc4e8-229">Int64</span></span>              | <span data-ttu-id="cc4e8-p128">项目大小，以字节为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p128">Size of the item in bytes. Read-only.</span></span>
| <span data-ttu-id="cc4e8-232">specialFolder</span><span class="sxs-lookup"><span data-stu-id="cc4e8-232">specialFolder</span></span>        | <span data-ttu-id="cc4e8-233">[specialFolder][]</span><span class="sxs-lookup"><span data-stu-id="cc4e8-233">[specialFolder][]</span></span>  | <span data-ttu-id="cc4e8-p129">如果当前项同时也是一个特殊的文件夹，则返回此 facet。只读。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p129">If the current item is also available as a special folder, this facet is returned. Read-only.</span></span>
| <span data-ttu-id="cc4e8-236">video</span><span class="sxs-lookup"><span data-stu-id="cc4e8-236">video</span></span>                | <span data-ttu-id="cc4e8-237">[视频][]</span><span class="sxs-lookup"><span data-stu-id="cc4e8-237">[video][]</span></span>          | <span data-ttu-id="cc4e8-p130">视频元数据（如果此项是一个视频）。只读。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p130">Video metadata, if the item is a video. Read-only.</span></span>
| <span data-ttu-id="cc4e8-240">WebDavUrl</span><span class="sxs-lookup"><span data-stu-id="cc4e8-240">webDavUrl</span></span>            | <span data-ttu-id="cc4e8-241">String</span><span class="sxs-lookup"><span data-stu-id="cc4e8-241">String</span></span>             | <span data-ttu-id="cc4e8-242">项的可兼容 WebDAV 的 URL。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-242">WebDAV compatible URL for the item.</span></span>
| <span data-ttu-id="cc4e8-243">WebUrl</span><span class="sxs-lookup"><span data-stu-id="cc4e8-243">webUrl</span></span>               | <span data-ttu-id="cc4e8-244">String</span><span class="sxs-lookup"><span data-stu-id="cc4e8-244">String</span></span>             | <span data-ttu-id="cc4e8-p131">在浏览器中显示此资源的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p131">URL that displays the resource in the browser. Read-only.</span></span>

<span data-ttu-id="cc4e8-p132">**注意：** ETag 和 cTag 属性在容器（文件夹）中以不同的方式工作。更改任意文件夹后代的内容或元数据时，也会修改 CTag 值。除了从后代派生的属性（例如 **childCount** 或 **lastModifiedDateTime**），仅在更改文件夹的属性时修改 eTag 值。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p132">**Note:** The eTag and cTag properties work differently on containers (folders). The cTag value is modified when content or metadata of any descendant of the folder is changed. The eTag value is only modified when the folder's properties are changed, except for properties that are derived from descendants (like **childCount** or **lastModifiedDateTime**).</span></span>

## <a name="relationships"></a><span data-ttu-id="cc4e8-250">关系</span><span class="sxs-lookup"><span data-stu-id="cc4e8-250">Relationships</span></span>

| <span data-ttu-id="cc4e8-251">关系</span><span class="sxs-lookup"><span data-stu-id="cc4e8-251">Relationship</span></span>       | <span data-ttu-id="cc4e8-252">类型</span><span class="sxs-lookup"><span data-stu-id="cc4e8-252">Type</span></span>                            | <span data-ttu-id="cc4e8-253">说明</span><span class="sxs-lookup"><span data-stu-id="cc4e8-253">Description</span></span>
|:-------------------|:--------------------------------|:--------------------------
| <span data-ttu-id="cc4e8-254">activities</span><span class="sxs-lookup"><span data-stu-id="cc4e8-254">activities</span></span>         | <span data-ttu-id="cc4e8-255">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="cc4e8-255">[itemActivity][] collection</span></span>     | <span data-ttu-id="cc4e8-256">最近发生在此项上的活动的列表。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-256">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="cc4e8-257">分析</span><span class="sxs-lookup"><span data-stu-id="cc4e8-257">analytics</span></span>          | <span data-ttu-id="cc4e8-258">[itemAnalytics][]资源</span><span class="sxs-lookup"><span data-stu-id="cc4e8-258">[itemAnalytics][] resource</span></span>      | <span data-ttu-id="cc4e8-259">有关此项发生查看活动的分析。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-259">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="cc4e8-260">content</span><span class="sxs-lookup"><span data-stu-id="cc4e8-260">content</span></span>            | <span data-ttu-id="cc4e8-261">流</span><span class="sxs-lookup"><span data-stu-id="cc4e8-261">Stream</span></span>                          | <span data-ttu-id="cc4e8-262">内容流（如果此项表示一个文件）。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-262">The content stream, if the item represents a file.</span></span>
| <span data-ttu-id="cc4e8-263">children</span><span class="sxs-lookup"><span data-stu-id="cc4e8-263">children</span></span>           | <span data-ttu-id="cc4e8-264">driveItem 集合</span><span class="sxs-lookup"><span data-stu-id="cc4e8-264">driveitem collection</span></span>            | <span data-ttu-id="cc4e8-p133">包含项目直接子项的 Item 对象的集合。仅表示文件夹的项目包含子项。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p133">Collection containing Item objects for the immediate children of Item. Only items representing folders have children. Read-only. Nullable.</span></span>
| <span data-ttu-id="cc4e8-269">listItem</span><span class="sxs-lookup"><span data-stu-id="cc4e8-269">listItem</span></span>           | <span data-ttu-id="cc4e8-270">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="cc4e8-270">[listItem][]</span></span>                    | <span data-ttu-id="cc4e8-271">在 SharePoint 中，关联的文档库列表项的驱动器。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-271">For drives in SharePoint, the associated document library list item.</span></span> <span data-ttu-id="cc4e8-272">只读。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-272">Read-only.</span></span> <span data-ttu-id="cc4e8-273">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-273">Nullable.</span></span>
| <span data-ttu-id="cc4e8-274">permissions</span><span class="sxs-lookup"><span data-stu-id="cc4e8-274">permissions</span></span>        | <span data-ttu-id="cc4e8-275">[permission][] 集合</span><span class="sxs-lookup"><span data-stu-id="cc4e8-275">[permission][] collection</span></span>       | <span data-ttu-id="cc4e8-p135">项目的权限集。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p135">The set of permissions for the item. Read-only. Nullable.</span></span>
| <span data-ttu-id="cc4e8-279">缩略图</span><span class="sxs-lookup"><span data-stu-id="cc4e8-279">thumbnails</span></span>         | <span data-ttu-id="cc4e8-280">[thumbnailSet][] 集合</span><span class="sxs-lookup"><span data-stu-id="cc4e8-280">[thumbnailSet][] collection</span></span>     | <span data-ttu-id="cc4e8-p136">包含与项目关联的 [ThumbnailSet][] 对象的集合。有关详细信息，请参阅 [获取缩略图][]只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p136">Collection containing [ThumbnailSet][] objects associated with the item. For more info, see [getting thumbnails][]. Read-only. Nullable.</span></span>
| <span data-ttu-id="cc4e8-285">版本</span><span class="sxs-lookup"><span data-stu-id="cc4e8-285">versions</span></span>           | <span data-ttu-id="cc4e8-286">[driveItemVersion][]集合</span><span class="sxs-lookup"><span data-stu-id="cc4e8-286">[driveItemVersion][] collection</span></span> | <span data-ttu-id="cc4e8-287">早期版本的项目列表。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-287">The list of previous versions of the item.</span></span> <span data-ttu-id="cc4e8-288">有关详细信息，请参阅[获取早期版本][]。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-288">For more info, see [getting previous versions][].</span></span> <span data-ttu-id="cc4e8-289">只读。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-289">Read-only.</span></span> <span data-ttu-id="cc4e8-290">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-290">Nullable.</span></span>

## <a name="instance-attributes"></a><span data-ttu-id="cc4e8-291">实例属性</span><span class="sxs-lookup"><span data-stu-id="cc4e8-291">Instance Attributes</span></span>

<span data-ttu-id="cc4e8-p138">实例属性是具有特殊行为的属性。这些属性是临时的，并且 a) 定义服务应执行的行为或 b) 提供短期的属性值，例如过期项目的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p138">Instance attributes are properties with special behaviors. These properties are temporary and either a) define behavior the service should perform or b) provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="cc4e8-294">属性名称</span><span class="sxs-lookup"><span data-stu-id="cc4e8-294">Property name</span></span>                     | <span data-ttu-id="cc4e8-295">类型</span><span class="sxs-lookup"><span data-stu-id="cc4e8-295">Type</span></span>   | <span data-ttu-id="cc4e8-296">说明</span><span class="sxs-lookup"><span data-stu-id="cc4e8-296">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="cc4e8-297">@microsoft.graph.conflictBehavior</span><span class="sxs-lookup"><span data-stu-id="cc4e8-297">@microsoft.graph.conflictBehavior</span></span> | <span data-ttu-id="cc4e8-298">string</span><span class="sxs-lookup"><span data-stu-id="cc4e8-298">string</span></span> | <span data-ttu-id="cc4e8-p139">为创建新项目的操作解决冲突的行为。你可以使用值 *fail*、*replace* 或 *rename*。PUT 的默认值是*replace*。绝不会返回包含该批注的项目。只写。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p139">The conflict resolution behavior for actions that create a new item. You can use the values *fail*, *replace*, or *rename*. The default for PUT is *replace*. An item will never be returned with this annotation. Write-only.</span></span>
| <span data-ttu-id="cc4e8-304">@microsoft.graph.downloadUrl</span><span class="sxs-lookup"><span data-stu-id="cc4e8-304">@microsoft.graph.downloadUrl</span></span>      | <span data-ttu-id="cc4e8-305">string</span><span class="sxs-lookup"><span data-stu-id="cc4e8-305">string</span></span> | <span data-ttu-id="cc4e8-p140">一个可用于下载此文件的内容的 URL。不需要使用此 URL 进行身份验证。只读。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p140">A URL that can be used to download this file's content. Authentication is not required with this URL. Read-only.</span></span>
| <span data-ttu-id="cc4e8-309">@microsoft.graph.sourceUrl</span><span class="sxs-lookup"><span data-stu-id="cc4e8-309">@microsoft.graph.sourceUrl</span></span>        | <span data-ttu-id="cc4e8-310">string</span><span class="sxs-lookup"><span data-stu-id="cc4e8-310">string</span></span> | <span data-ttu-id="cc4e8-p141">发出 PUT 请求时，此实例批注可用于指示服务下载 URL 内容并将其存储为文件。只写。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-p141">When issuing a PUT request, this instance annotation can be used to instruct the service to download the contents of the URL, and store it as the file. Write-only.</span></span>

<span data-ttu-id="cc4e8-313">**注意：**@Microsoft.graph.downloadUrl 值是短期 URL，并且不能缓存。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-313">**Note:** The @microsoft.graph.downloadUrl value is a short-lived URL and can't be cached.</span></span>
<span data-ttu-id="cc4e8-314">URL 期间较短的时间 （1 小时） 之前失效将只能可用。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-314">The URL will only be available for a short period of time (1 hour) before it is invalidated.</span></span> <span data-ttu-id="cc4e8-315">删除文件的用户权限可能不立即使无效 URL。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-315">Removing file permissions for a user may not immediately invalidate the URL.</span></span>

## <a name="methods"></a><span data-ttu-id="cc4e8-316">方法</span><span class="sxs-lookup"><span data-stu-id="cc4e8-316">Methods</span></span>

| <span data-ttu-id="cc4e8-317">方法</span><span class="sxs-lookup"><span data-stu-id="cc4e8-317">Method</span></span>                                                   | <span data-ttu-id="cc4e8-318">REST 路径</span><span class="sxs-lookup"><span data-stu-id="cc4e8-318">REST Path</span></span>
|:---------------------------------------------------------|:------------------
| [<span data-ttu-id="cc4e8-319">获取项目</span><span class="sxs-lookup"><span data-stu-id="cc4e8-319">Get item</span></span>](../api/driveitem-get.md)                      | `GET /drive/items/{item-id}`
| [<span data-ttu-id="cc4e8-320">列出活动</span><span class="sxs-lookup"><span data-stu-id="cc4e8-320">List activities</span></span>](../api/activities-list.md)             | `GET /drive/items/{item-id}/activities`
| <span data-ttu-id="cc4e8-321">[获取分析][]</span><span class="sxs-lookup"><span data-stu-id="cc4e8-321">[Get analytics][]</span></span>                                        | `GET /drive/items/{item-id}/analytics`
| <span data-ttu-id="cc4e8-322">[按间隔获取活动][]</span><span class="sxs-lookup"><span data-stu-id="cc4e8-322">[Get activities by interval][]</span></span>                           | `GET /drive/items/{item-id}/getActivitiesByInterval`
| [<span data-ttu-id="cc4e8-323">列出子项</span><span class="sxs-lookup"><span data-stu-id="cc4e8-323">List children</span></span>](../api/driveitem-list-children.md)       | `GET /drive/items/{item-id}/children`
| [<span data-ttu-id="cc4e8-324">列出版本</span><span class="sxs-lookup"><span data-stu-id="cc4e8-324">List versions</span></span>](../api/driveitem-list-versions.md)       | `GET /drive/items/{item-id}/versions`
| [<span data-ttu-id="cc4e8-325">创建项目</span><span class="sxs-lookup"><span data-stu-id="cc4e8-325">Create item</span></span>](../api/driveitem-post-children.md)         | `POST /drive/items/{item-id}/children`
| [<span data-ttu-id="cc4e8-326">更新项目</span><span class="sxs-lookup"><span data-stu-id="cc4e8-326">Update item</span></span>](../api/driveitem-update.md)                | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="cc4e8-327">上载内容</span><span class="sxs-lookup"><span data-stu-id="cc4e8-327">Upload content</span></span>](../api/driveitem-put-content.md)        | `PUT /drive/items/{item-id}/content`
| [<span data-ttu-id="cc4e8-328">下载内容</span><span class="sxs-lookup"><span data-stu-id="cc4e8-328">Download content</span></span>](../api/driveitem-get-content.md)      | `GET /drive/items/{item-id}/content`
| <span data-ttu-id="cc4e8-329">[下载特定格式文件][download-format]</span><span class="sxs-lookup"><span data-stu-id="cc4e8-329">[Download specific file format][download-format]</span></span>         | `GET /drive/items/{item-id}/content?format={format}`
| [<span data-ttu-id="cc4e8-330">删除项</span><span class="sxs-lookup"><span data-stu-id="cc4e8-330">Delete item</span></span>](../api/driveitem-delete.md)                | `DELETE /drive/items/{item-id}`
| [<span data-ttu-id="cc4e8-331">移动项目</span><span class="sxs-lookup"><span data-stu-id="cc4e8-331">Move item</span></span>](../api/driveitem-move.md)                    | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="cc4e8-332">复制项目</span><span class="sxs-lookup"><span data-stu-id="cc4e8-332">Copy item</span></span>](../api/driveitem-copy.md)                    | `POST /drive/items/{item-id}/copy`
| [<span data-ttu-id="cc4e8-333">搜索项目</span><span class="sxs-lookup"><span data-stu-id="cc4e8-333">Search items</span></span>](../api/driveitem-search.md)               | `GET /drive/items/{item-id}/search(q='text')`
| [<span data-ttu-id="cc4e8-334">列出驱动器中的更改</span><span class="sxs-lookup"><span data-stu-id="cc4e8-334">List changes in a drive</span></span>](../api/driveitem-delta.md)     | `GET /drive/root/delta`
| [<span data-ttu-id="cc4e8-335">列出缩略图</span><span class="sxs-lookup"><span data-stu-id="cc4e8-335">List thumbnails</span></span>](../api/driveitem-list-thumbnails.md)   | `GET /drive/items/{item-id}/thumbnails`
| [<span data-ttu-id="cc4e8-336">创建共享链接</span><span class="sxs-lookup"><span data-stu-id="cc4e8-336">Create sharing link</span></span>](../api/driveitem-createlink.md)    | `POST /drive/items/{item-id}/createLink`
| [<span data-ttu-id="cc4e8-337">添加权限</span><span class="sxs-lookup"><span data-stu-id="cc4e8-337">Add permissions</span></span>](../api/driveitem-invite.md)            | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="cc4e8-338">列出权限</span><span class="sxs-lookup"><span data-stu-id="cc4e8-338">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="cc4e8-339">删除权限</span><span class="sxs-lookup"><span data-stu-id="cc4e8-339">Delete permission</span></span>](../api/permission-delete.md)         | `DELETE /drive/items/{item-id}/permissions/{perm-id}`
| <span data-ttu-id="cc4e8-340">[获取 WebSocket 通道][getWebSocket]</span><span class="sxs-lookup"><span data-stu-id="cc4e8-340">[Get WebSocket channel][getWebSocket]</span></span>                    | `GET /drive/root/subscriptions/socketIo`
| <span data-ttu-id="cc4e8-341">[预览项][item-preview]</span><span class="sxs-lookup"><span data-stu-id="cc4e8-341">[Preview item][item-preview]</span></span>                             | `POST /drive/items/{item-id}/preview`

[item-preview]: ../api/driveitem-preview.md
[获取分析]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[按间隔获取活动]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md

## <a name="remarks"></a><span data-ttu-id="cc4e8-344">注解</span><span class="sxs-lookup"><span data-stu-id="cc4e8-344">Remarks</span></span>

<span data-ttu-id="cc4e8-345">在 OneDrive for Business 或 SharePoint 文档库中，如果 **driveItem** 具有[folder][] Facet，则不返回 **cTag** 属性。</span><span class="sxs-lookup"><span data-stu-id="cc4e8-345">In OneDrive for Business or SharePoint document libraries, the **cTag** property is not returned, if the **driveItem** has a [folder][] facet.</span></span>

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
[获取早期版本]: ../api/driveitem-list-versions.md
[getting previous versions]: ../api/driveitem-list-versions.md
[获取缩略图]: ../api/driveitem-list-thumbnails.md
[getting thumbnails]: ../api/driveitem-list-thumbnails.md
[getWebSocket]: ../api/driveitem-subscriptions-socketio.md
[identitySet]: identityset.md
[image]: image.md
[itemActivity]: itemactivity.md
[itemAnalytics]: itemanalytics.md
[itemReference]: itemreference.md
[geoCoordinates]: geocoordinates.md
[List activities]: ../api/activities-list.md
[listItem]: listitem.md
[package]: package.md
[permission]: permission.md
[photo]: photo.md
[remoteItem]: remoteitem.md
[Root]: root.md
[root]: root.md
[searchResult]: searchresult.md
[Shared]: shared.md
[shared]: shared.md
[sharepointIds]: sharepointids.md
[specialFolder]: specialfolder.md
[thumbnailSet]: thumbnailset.md
[video]: video.md
[user]: https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/users
[publicationFacet]: publicationfacet.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Item is the main data model in the OneDrive API. Everything is an item.",
  "keywords": "item,facet,resource",
  "section": "documentation",
  "tocPath": "Items",
  "tocBookmarks": { "Resources/Item": "#" }
} -->
