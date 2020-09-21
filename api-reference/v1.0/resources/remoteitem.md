---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: RemoteItem
localization_priority: Normal
description: remoteItem 资源指示 driveItem 引用存在于其他驱动器中的项。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3688711b588ee40b8ec0aac0dc04f543cf2e2294
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47967329"
---
# <a name="remoteitem-resource-type"></a><span data-ttu-id="1394e-103">RemoteItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="1394e-103">RemoteItem resource type</span></span>

<span data-ttu-id="1394e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1394e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1394e-105">**remoteItem** 资源指示 [**driveItem**](driveitem.md) 引用存在于其他驱动器中的项。</span><span class="sxs-lookup"><span data-stu-id="1394e-105">The **remoteItem** resource indicates that a [**driveItem**](driveitem.md) references an item that exists in another drive.</span></span>
<span data-ttu-id="1394e-106">该资源提供源驱动器和目标项的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="1394e-106">This resource provides the unique IDs of the source drive and target item.</span></span>

<span data-ttu-id="1394e-107">具有非 NULL **remoteItem** facet 的 [**DriveItems**](driveitem.md) 是共享、添加到用户的 OneDrive 的资源，或从项（例如搜索结果）的 hetrogenous 集合返回的项中的资源。</span><span class="sxs-lookup"><span data-stu-id="1394e-107">[**DriveItems**](driveitem.md) with a non-null **remoteItem** facet are resources that are shared, added to the user's OneDrive, or on items returned from hetrogenous collections of items (like search results).</span></span>

<span data-ttu-id="1394e-108">**注意：** 与同一驱动器中的文件夹不同，移动到远程项的 **driveItem** 可更改其 `id` 值。</span><span class="sxs-lookup"><span data-stu-id="1394e-108">**Note:** Unlike with folders in the same drive, a **driveItem** moved into a remote item may have its `id` value changed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1394e-109">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1394e-109">JSON representation</span></span>

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.remoteItem", 
       "optionalProperties": ["name", "fileSystemInfo", "file", "folder"] } -->

```json
{
  "id": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "file": { "@odata.type": "microsoft.graph.file" },
  "fileSystemInfo": { "@odata.type": "microsoft.graph.fileSystemInfo" },
  "folder": { "@odata.type": "microsoft.graph.folder" },
  "image" : { "@odata.type": "microsoft.graph.image" },
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "name": "string",
  "package": { "@odata.type": "microsoft.graph.package" },
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "shared": { "@odata.type": "microsoft.graph.shared" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "specialFolder": { "@odata.type": "microsoft.graph.specialFolder" },
  "size": 1024,
  "video": { "@odata.type": "microsoft.graph.video" },
  "webDavUrl": "url",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="1394e-110">属性</span><span class="sxs-lookup"><span data-stu-id="1394e-110">Properties</span></span>

| <span data-ttu-id="1394e-111">属性名称</span><span class="sxs-lookup"><span data-stu-id="1394e-111">Property name</span></span>        | <span data-ttu-id="1394e-112">类型</span><span class="sxs-lookup"><span data-stu-id="1394e-112">Type</span></span>                                | <span data-ttu-id="1394e-113">说明</span><span class="sxs-lookup"><span data-stu-id="1394e-113">Description</span></span>                                                                                                                                                       |
| :------------------- | :---------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="1394e-114">createdBy</span><span class="sxs-lookup"><span data-stu-id="1394e-114">createdBy</span></span>            | [<span data-ttu-id="1394e-115">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="1394e-115">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="1394e-p102">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="1394e-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>                                                                                  |
| <span data-ttu-id="1394e-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1394e-118">createdDateTime</span></span>      | <span data-ttu-id="1394e-119">Timestamp</span><span class="sxs-lookup"><span data-stu-id="1394e-119">Timestamp</span></span>                           | <span data-ttu-id="1394e-p103">创建项的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="1394e-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                        |
| <span data-ttu-id="1394e-122">文件</span><span class="sxs-lookup"><span data-stu-id="1394e-122">file</span></span>                 | [<span data-ttu-id="1394e-123">文件</span><span class="sxs-lookup"><span data-stu-id="1394e-123">File</span></span>](file.md)                     | <span data-ttu-id="1394e-p104">指示远程项是文件。只读。</span><span class="sxs-lookup"><span data-stu-id="1394e-p104">Indicates that the remote item is a file. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="1394e-126">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="1394e-126">fileSystemInfo</span></span>       | [<span data-ttu-id="1394e-127">FileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="1394e-127">FileSystemInfo</span></span>](filesysteminfo.md) | <span data-ttu-id="1394e-p105">本地文件系统中的远程项的有关信息。只读。</span><span class="sxs-lookup"><span data-stu-id="1394e-p105">Information about the remote item from the local file system. Read-only.</span></span>                                                                                          |
| <span data-ttu-id="1394e-130">文件夹</span><span class="sxs-lookup"><span data-stu-id="1394e-130">folder</span></span>               | [<span data-ttu-id="1394e-131">文件夹</span><span class="sxs-lookup"><span data-stu-id="1394e-131">Folder</span></span>](folder.md)                 | <span data-ttu-id="1394e-p106">指示远程项是文件夹。只读。</span><span class="sxs-lookup"><span data-stu-id="1394e-p106">Indicates that the remote item is a folder. Read-only.</span></span>                                                                                                            |
| <span data-ttu-id="1394e-134">id</span><span class="sxs-lookup"><span data-stu-id="1394e-134">id</span></span>                   | <span data-ttu-id="1394e-135">String</span><span class="sxs-lookup"><span data-stu-id="1394e-135">String</span></span>                              | <span data-ttu-id="1394e-p107">驱动器内远程项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="1394e-p107">Unique identifier for the remote item in its drive. Read-only.</span></span>                                                                                                    |
| <span data-ttu-id="1394e-138">image</span><span class="sxs-lookup"><span data-stu-id="1394e-138">image</span></span>                | [<span data-ttu-id="1394e-139">Image</span><span class="sxs-lookup"><span data-stu-id="1394e-139">Image</span></span>](image.md)                   | <span data-ttu-id="1394e-p108">图像元数据（如果此项是一个图像）。只读。</span><span class="sxs-lookup"><span data-stu-id="1394e-p108">Image metadata, if the item is an image. Read-only.</span></span>                                                                                               |
| <span data-ttu-id="1394e-142">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="1394e-142">lastModifiedBy</span></span>       | [<span data-ttu-id="1394e-143">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="1394e-143">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="1394e-p109">上次修改项目的用户、设备和应用程序的标识。只读。</span><span class="sxs-lookup"><span data-stu-id="1394e-p109">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                            |
| <span data-ttu-id="1394e-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1394e-146">lastModifiedDateTime</span></span> | <span data-ttu-id="1394e-147">Timestamp</span><span class="sxs-lookup"><span data-stu-id="1394e-147">Timestamp</span></span>                           | <span data-ttu-id="1394e-p110">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="1394e-p110">Date and time the item was last modified. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="1394e-150">name</span><span class="sxs-lookup"><span data-stu-id="1394e-150">name</span></span>                 | <span data-ttu-id="1394e-151">String</span><span class="sxs-lookup"><span data-stu-id="1394e-151">String</span></span>                              | <span data-ttu-id="1394e-p111">可选。远程项的 Filename。只读。</span><span class="sxs-lookup"><span data-stu-id="1394e-p111">Optional. Filename of the remote item. Read-only.</span></span>                                                                                                                 |
| <span data-ttu-id="1394e-155">包</span><span class="sxs-lookup"><span data-stu-id="1394e-155">package</span></span>              | [<span data-ttu-id="1394e-156">包</span><span class="sxs-lookup"><span data-stu-id="1394e-156">Package</span></span>](package.md)               | <span data-ttu-id="1394e-p112">如果存在，则表示此项是一个包，而不是文件夹或文件。包被视为某些上下文中的文件和其他上下文中的文件夹。只读。</span><span class="sxs-lookup"><span data-stu-id="1394e-p112">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span> |
| <span data-ttu-id="1394e-160">parentReference</span><span class="sxs-lookup"><span data-stu-id="1394e-160">parentReference</span></span>      | [<span data-ttu-id="1394e-161">ItemReference</span><span class="sxs-lookup"><span data-stu-id="1394e-161">ItemReference</span></span>](itemreference.md)   | <span data-ttu-id="1394e-p113">远程项的父级的属性。只读。</span><span class="sxs-lookup"><span data-stu-id="1394e-p113">Properties of the parent of the remote item. Read-only.</span></span>                                                                                                           |
| <span data-ttu-id="1394e-164">shared</span><span class="sxs-lookup"><span data-stu-id="1394e-164">shared</span></span>               | [<span data-ttu-id="1394e-165">shared</span><span class="sxs-lookup"><span data-stu-id="1394e-165">shared</span></span>](shared.md)                 | <span data-ttu-id="1394e-p114">表示此项已与他人共享，并提供有关项目共享状态的信息。只读。</span><span class="sxs-lookup"><span data-stu-id="1394e-p114">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>                                       |
| <span data-ttu-id="1394e-168">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="1394e-168">sharepointIds</span></span>        | [<span data-ttu-id="1394e-169">SharepointIds</span><span class="sxs-lookup"><span data-stu-id="1394e-169">SharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="1394e-p115">为 OneDrive for Business 和 SharePoint 中的项之间的互操作性提供了完整的项标识符集。只读。</span><span class="sxs-lookup"><span data-stu-id="1394e-p115">Provides interop between items in OneDrive for Business and SharePoint with the full set of item identifiers. Read-only.</span></span>                                          |
| <span data-ttu-id="1394e-172">size</span><span class="sxs-lookup"><span data-stu-id="1394e-172">size</span></span>                 | <span data-ttu-id="1394e-173">Int64</span><span class="sxs-lookup"><span data-stu-id="1394e-173">Int64</span></span>                               | <span data-ttu-id="1394e-p116">远程项的大小。只读。</span><span class="sxs-lookup"><span data-stu-id="1394e-p116">Size of the remote item. Read-only.</span></span>                                                                                                                               |
| <span data-ttu-id="1394e-176">specialFolder</span><span class="sxs-lookup"><span data-stu-id="1394e-176">specialFolder</span></span>        | <span data-ttu-id="1394e-177">[specialFolder][]</span><span class="sxs-lookup"><span data-stu-id="1394e-177">[specialFolder][]</span></span>                   | <span data-ttu-id="1394e-p117">如果当前项同时也是一个特殊的文件夹，则返回此 facet。只读。</span><span class="sxs-lookup"><span data-stu-id="1394e-p117">If the current item is also available as a special folder, this facet is returned. Read-only.</span></span>                                                                     |
| <span data-ttu-id="1394e-180">video</span><span class="sxs-lookup"><span data-stu-id="1394e-180">video</span></span>                | [<span data-ttu-id="1394e-181">Video</span><span class="sxs-lookup"><span data-stu-id="1394e-181">Video</span></span>](video.md)                   | <span data-ttu-id="1394e-p118">视频元数据（如果此项是一个视频）。只读。</span><span class="sxs-lookup"><span data-stu-id="1394e-p118">Video metadata, if the item is a video. Read-only.</span></span>                                                                                                    |
| <span data-ttu-id="1394e-184">WebDavUrl</span><span class="sxs-lookup"><span data-stu-id="1394e-184">webDavUrl</span></span>            | <span data-ttu-id="1394e-185">Url</span><span class="sxs-lookup"><span data-stu-id="1394e-185">Url</span></span>                                 | <span data-ttu-id="1394e-186">项的可兼容 DAV 的 URL。</span><span class="sxs-lookup"><span data-stu-id="1394e-186">DAV compatible URL for the item.</span></span>                                                                                                                                  |
| <span data-ttu-id="1394e-187">WebUrl</span><span class="sxs-lookup"><span data-stu-id="1394e-187">webUrl</span></span>               | <span data-ttu-id="1394e-188">Url</span><span class="sxs-lookup"><span data-stu-id="1394e-188">Url</span></span>                                 | <span data-ttu-id="1394e-p119">在浏览器中显示此资源的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="1394e-p119">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                         |

[specialFolder]: specialfolder.md

## <a name="remarks"></a><span data-ttu-id="1394e-192">注解</span><span class="sxs-lookup"><span data-stu-id="1394e-192">Remarks</span></span>

<span data-ttu-id="1394e-193">有关 **driveItem** 上 facet 的详细信息，请参阅 [driveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="1394e-193">For more information about the facets on a **driveItem**, see [driveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/RemoteItem"
} -->

