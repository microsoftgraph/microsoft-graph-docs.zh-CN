---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: RemoteItem
localization_priority: Normal
ms.openlocfilehash: 0b29ba14273bad7306518c290029a9ebc444f07d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888086"
---
# <a name="remoteitem-resource-type"></a><span data-ttu-id="b7ad0-102">RemoteItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="b7ad0-102">RemoteItem resource type</span></span>

<span data-ttu-id="b7ad0-p101">**remoteItem** 资源指示 [**driveItem**](driveitem.md) 引用存在于其他驱动器中的项。该资源提供源驱动器和目标项的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="b7ad0-p101">The **remoteItem** resource indicates that a [**driveItem**](driveitem.md) references an item that exists in another drive. This resource provides the unique IDs of the source drive and target item.</span></span>

<span data-ttu-id="b7ad0-105">具有非 NULL **remoteItem** facet 的 [**DriveItems**](driveitem.md) 是共享、添加到用户的 OneDrive 的资源，或从项（例如搜索结果）的 hetrogenous 集合返回的项中的资源。</span><span class="sxs-lookup"><span data-stu-id="b7ad0-105">[**DriveItems**](driveitem.md) with a non-null **remoteItem** facet are resources that are shared, added to the user's OneDrive, or on items returned from hetrogenous collections of items (like search results).</span></span>

<span data-ttu-id="b7ad0-106">**注意：** 与同一驱动器中的文件夹不同，移动到远程项的 **driveItem** 可更改其 `id` 值。</span><span class="sxs-lookup"><span data-stu-id="b7ad0-106">**Note:** Unlike with folders in the same drive, a **driveItem** moved into a remote item may have its `id` value changed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b7ad0-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b7ad0-107">JSON representation</span></span>

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
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "name": "string",
  "package": { "@odata.type": "microsoft.graph.package" },
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "shared": { "@odata.type": "microsoft.graph.shared" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "specialFolder": { "@odata.type": "microsoft.graph.specialFolder" },
  "size": 1024,
  "webDavUrl": "url",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="b7ad0-108">属性</span><span class="sxs-lookup"><span data-stu-id="b7ad0-108">Properties</span></span>

| <span data-ttu-id="b7ad0-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="b7ad0-109">Property name</span></span>        | <span data-ttu-id="b7ad0-110">类型</span><span class="sxs-lookup"><span data-stu-id="b7ad0-110">Type</span></span>                                | <span data-ttu-id="b7ad0-111">说明</span><span class="sxs-lookup"><span data-stu-id="b7ad0-111">Description</span></span>                                                                                                                                                       |
| :------------------- | :---------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="b7ad0-112">createdBy</span><span class="sxs-lookup"><span data-stu-id="b7ad0-112">createdBy</span></span>            | [<span data-ttu-id="b7ad0-113">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="b7ad0-113">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="b7ad0-p102">创建项的用户、设备和应用程序标识。只读。</span><span class="sxs-lookup"><span data-stu-id="b7ad0-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>                                                                                  |
| <span data-ttu-id="b7ad0-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b7ad0-116">createdDateTime</span></span>      | <span data-ttu-id="b7ad0-117">Timestamp</span><span class="sxs-lookup"><span data-stu-id="b7ad0-117">Timestamp</span></span>                           | <span data-ttu-id="b7ad0-p103">创建项的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="b7ad0-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                        |
| <span data-ttu-id="b7ad0-120">文件</span><span class="sxs-lookup"><span data-stu-id="b7ad0-120">file</span></span>                 | [<span data-ttu-id="b7ad0-121">文件</span><span class="sxs-lookup"><span data-stu-id="b7ad0-121">File</span></span>](file.md)                     | <span data-ttu-id="b7ad0-p104">指示远程项是文件。只读。</span><span class="sxs-lookup"><span data-stu-id="b7ad0-p104">Indicates that the remote item is a file. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="b7ad0-124">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="b7ad0-124">fileSystemInfo</span></span>       | [<span data-ttu-id="b7ad0-125">FileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="b7ad0-125">FileSystemInfo</span></span>](filesysteminfo.md) | <span data-ttu-id="b7ad0-p105">本地文件系统中的远程项的有关信息。只读。</span><span class="sxs-lookup"><span data-stu-id="b7ad0-p105">Information about the remote item from the local file system. Read-only.</span></span>                                                                                          |
| <span data-ttu-id="b7ad0-128">文件夹</span><span class="sxs-lookup"><span data-stu-id="b7ad0-128">folder</span></span>               | [<span data-ttu-id="b7ad0-129">文件夹</span><span class="sxs-lookup"><span data-stu-id="b7ad0-129">Folder</span></span>](folder.md)                 | <span data-ttu-id="b7ad0-p106">指示远程项是文件夹。只读。</span><span class="sxs-lookup"><span data-stu-id="b7ad0-p106">Indicates that the remote item is a folder. Read-only.</span></span>                                                                                                            |
| <span data-ttu-id="b7ad0-132">id</span><span class="sxs-lookup"><span data-stu-id="b7ad0-132">id</span></span>                   | <span data-ttu-id="b7ad0-133">String</span><span class="sxs-lookup"><span data-stu-id="b7ad0-133">String</span></span>                              | <span data-ttu-id="b7ad0-p107">驱动器内远程项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="b7ad0-p107">Unique identifier for the remote item in its drive. Read-only.</span></span>                                                                                                    |
| <span data-ttu-id="b7ad0-136">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="b7ad0-136">lastModifiedBy</span></span>       | [<span data-ttu-id="b7ad0-137">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="b7ad0-137">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="b7ad0-p108">上次修改项的用户、设备和应用程序标识。只读。</span><span class="sxs-lookup"><span data-stu-id="b7ad0-p108">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                            |
| <span data-ttu-id="b7ad0-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b7ad0-140">lastModifiedDateTime</span></span> | <span data-ttu-id="b7ad0-141">Timestamp</span><span class="sxs-lookup"><span data-stu-id="b7ad0-141">Timestamp</span></span>                           | <span data-ttu-id="b7ad0-p109">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="b7ad0-p109">Date and time the item was last modified. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="b7ad0-144">名称</span><span class="sxs-lookup"><span data-stu-id="b7ad0-144">name</span></span>                 | <span data-ttu-id="b7ad0-145">String</span><span class="sxs-lookup"><span data-stu-id="b7ad0-145">String</span></span>                              | <span data-ttu-id="b7ad0-p110">可选。远程项的 Filename。只读。</span><span class="sxs-lookup"><span data-stu-id="b7ad0-p110">Optional. Filename of the remote item. Read-only.</span></span>                                                                                                                 |
| <span data-ttu-id="b7ad0-149">包</span><span class="sxs-lookup"><span data-stu-id="b7ad0-149">package</span></span>              | [<span data-ttu-id="b7ad0-150">包</span><span class="sxs-lookup"><span data-stu-id="b7ad0-150">Package</span></span>](package.md)               | <span data-ttu-id="b7ad0-p111">如果存在，则表示此项是包而不是文件夹或文件。在某些上下文中将包视为文件，在其他上下文中视为文件夹。只读。</span><span class="sxs-lookup"><span data-stu-id="b7ad0-p111">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span> |
| <span data-ttu-id="b7ad0-154">parentReference</span><span class="sxs-lookup"><span data-stu-id="b7ad0-154">parentReference</span></span>      | [<span data-ttu-id="b7ad0-155">ItemReference</span><span class="sxs-lookup"><span data-stu-id="b7ad0-155">ItemReference</span></span>](itemreference.md)   | <span data-ttu-id="b7ad0-p112">远程项的父级的属性。只读。</span><span class="sxs-lookup"><span data-stu-id="b7ad0-p112">Properties of the parent of the remote item. Read-only.</span></span>                                                                                                           |
| <span data-ttu-id="b7ad0-158">shared</span><span class="sxs-lookup"><span data-stu-id="b7ad0-158">shared</span></span>               | [<span data-ttu-id="b7ad0-159">共享</span><span class="sxs-lookup"><span data-stu-id="b7ad0-159">shared</span></span>](shared.md)                 | <span data-ttu-id="b7ad0-p113">表示此项已与他人共享，并提供有关项目共享状态的信息。只读。</span><span class="sxs-lookup"><span data-stu-id="b7ad0-p113">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>                                       |
| <span data-ttu-id="b7ad0-162">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="b7ad0-162">sharepointIds</span></span>        | [<span data-ttu-id="b7ad0-163">SharepointIds</span><span class="sxs-lookup"><span data-stu-id="b7ad0-163">SharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="b7ad0-p114">为 OneDrive for Business 和 SharePoint 中的项之间的互操作性提供了完整的项标识符集。只读。</span><span class="sxs-lookup"><span data-stu-id="b7ad0-p114">Provides interop between items in OneDrive for Business and SharePoint with the full set of item identifiers. Read-only.</span></span>                                          |
| <span data-ttu-id="b7ad0-166">size</span><span class="sxs-lookup"><span data-stu-id="b7ad0-166">size</span></span>                 | <span data-ttu-id="b7ad0-167">Int64</span><span class="sxs-lookup"><span data-stu-id="b7ad0-167">Int64</span></span>                               | <span data-ttu-id="b7ad0-p115">远程项的大小。只读。</span><span class="sxs-lookup"><span data-stu-id="b7ad0-p115">Size of the remote item. Read-only.</span></span>                                                                                                                               |
| <span data-ttu-id="b7ad0-170">specialFolder</span><span class="sxs-lookup"><span data-stu-id="b7ad0-170">specialFolder</span></span>        | <span data-ttu-id="b7ad0-171">[specialFolder][]</span><span class="sxs-lookup"><span data-stu-id="b7ad0-171">[specialFolder][]</span></span>                   | <span data-ttu-id="b7ad0-p116">如果当前项同时也是一个特殊的文件夹，则返回此 facet。只读。</span><span class="sxs-lookup"><span data-stu-id="b7ad0-p116">If the current item is also available as a special folder, this facet is returned. Read-only.</span></span>                                                                     |
| <span data-ttu-id="b7ad0-174">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="b7ad0-174">webDavUrl</span></span>            | <span data-ttu-id="b7ad0-175">Url</span><span class="sxs-lookup"><span data-stu-id="b7ad0-175">Url</span></span>                                 | <span data-ttu-id="b7ad0-176">项的可兼容 DAV 的 URL。</span><span class="sxs-lookup"><span data-stu-id="b7ad0-176">DAV compatible URL for the item.</span></span>                                                                                                                                  |
| <span data-ttu-id="b7ad0-177">webUrl</span><span class="sxs-lookup"><span data-stu-id="b7ad0-177">webUrl</span></span>               | <span data-ttu-id="b7ad0-178">Url</span><span class="sxs-lookup"><span data-stu-id="b7ad0-178">Url</span></span>                                 | <span data-ttu-id="b7ad0-p117">在浏览器中显示此资源的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="b7ad0-p117">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                         |

[specialFolder]: specialfolder.md

## <a name="remarks"></a><span data-ttu-id="b7ad0-182">注解</span><span class="sxs-lookup"><span data-stu-id="b7ad0-182">Remarks</span></span>

<span data-ttu-id="b7ad0-183">有关 **driveItem** 上 facet 的详细信息，请参阅 [driveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="b7ad0-183">For more information about the facets on a **driveItem**, see [driveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/RemoteItem"
} -->
