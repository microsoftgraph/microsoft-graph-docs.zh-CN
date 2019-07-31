---
author: JeremyKelley
description: remoteItem 资源指示 driveItem 引用存在于其他驱动器中的项。
ms.date: 09/10/2017
title: RemoteItem
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 05da43fb3d7b1e2adec01f707eeed61df4623f04
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008703"
---
# <a name="remoteitem-resource-type"></a><span data-ttu-id="9fdc9-103">RemoteItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="9fdc9-103">RemoteItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fdc9-104">**remoteItem** 资源指示 [**driveItem**](driveitem.md) 引用存在于其他驱动器中的项。</span><span class="sxs-lookup"><span data-stu-id="9fdc9-104">The **remoteItem** resource indicates that a [**driveItem**](driveitem.md) references an item that exists in another drive.</span></span>
<span data-ttu-id="9fdc9-105">该资源提供源驱动器和目标项的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="9fdc9-105">This resource provides the unique IDs of the source drive and target item.</span></span>

<span data-ttu-id="9fdc9-106">具有非 NULL **remoteItem** facet 的 [**DriveItems**](driveitem.md) 是共享、添加到用户的 OneDrive 的资源，或从项（例如搜索结果）的 hetrogenous 集合返回的项中的资源。</span><span class="sxs-lookup"><span data-stu-id="9fdc9-106">[**DriveItems**](driveitem.md) with a non-null **remoteItem** facet are resources that are shared, added to the user's OneDrive, or on items returned from hetrogenous collections of items (like search results).</span></span>

<span data-ttu-id="9fdc9-107">**注意：** 与同一驱动器中的文件夹不同，移动到远程项的 **driveItem** 可更改其 `id` 值。</span><span class="sxs-lookup"><span data-stu-id="9fdc9-107">**Note:** Unlike with folders in the same drive, a **driveItem** moved into a remote item may have its `id` value changed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9fdc9-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9fdc9-108">JSON representation</span></span>

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
  "size": 1024,
  "webDavUrl": "url",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="9fdc9-109">属性</span><span class="sxs-lookup"><span data-stu-id="9fdc9-109">Properties</span></span>

| <span data-ttu-id="9fdc9-110">属性名称</span><span class="sxs-lookup"><span data-stu-id="9fdc9-110">Property name</span></span>        | <span data-ttu-id="9fdc9-111">类型</span><span class="sxs-lookup"><span data-stu-id="9fdc9-111">Type</span></span>                                | <span data-ttu-id="9fdc9-112">说明</span><span class="sxs-lookup"><span data-stu-id="9fdc9-112">Description</span></span>                                                                                                                                                       |
| :------------------- | :---------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="9fdc9-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="9fdc9-113">createdBy</span></span>            | [<span data-ttu-id="9fdc9-114">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="9fdc9-114">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="9fdc9-p102">识别创建项目的用户、设备和应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="9fdc9-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>                                                                                  |
| <span data-ttu-id="9fdc9-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9fdc9-117">createdDateTime</span></span>      | <span data-ttu-id="9fdc9-118">Timestamp</span><span class="sxs-lookup"><span data-stu-id="9fdc9-118">Timestamp</span></span>                           | <span data-ttu-id="9fdc9-p103">创建项的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="9fdc9-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                        |
| <span data-ttu-id="9fdc9-121">文件</span><span class="sxs-lookup"><span data-stu-id="9fdc9-121">file</span></span>                 | [<span data-ttu-id="9fdc9-122">文件</span><span class="sxs-lookup"><span data-stu-id="9fdc9-122">File</span></span>](file.md)                     | <span data-ttu-id="9fdc9-p104">指示远程项是文件。只读。</span><span class="sxs-lookup"><span data-stu-id="9fdc9-p104">Indicates that the remote item is a file. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="9fdc9-125">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="9fdc9-125">fileSystemInfo</span></span>       | [<span data-ttu-id="9fdc9-126">FileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="9fdc9-126">FileSystemInfo</span></span>](filesysteminfo.md) | <span data-ttu-id="9fdc9-p105">本地文件系统中的远程项的有关信息。只读。</span><span class="sxs-lookup"><span data-stu-id="9fdc9-p105">Information about the remote item from the local file system. Read-only.</span></span>                                                                                          |
| <span data-ttu-id="9fdc9-129">文件夹</span><span class="sxs-lookup"><span data-stu-id="9fdc9-129">folder</span></span>               | [<span data-ttu-id="9fdc9-130">文件夹</span><span class="sxs-lookup"><span data-stu-id="9fdc9-130">Folder</span></span>](folder.md)                 | <span data-ttu-id="9fdc9-p106">指示远程项是文件夹。只读。</span><span class="sxs-lookup"><span data-stu-id="9fdc9-p106">Indicates that the remote item is a folder. Read-only.</span></span>                                                                                                            |
| <span data-ttu-id="9fdc9-133">id</span><span class="sxs-lookup"><span data-stu-id="9fdc9-133">id</span></span>                   | <span data-ttu-id="9fdc9-134">String</span><span class="sxs-lookup"><span data-stu-id="9fdc9-134">String</span></span>                              | <span data-ttu-id="9fdc9-p107">驱动器内远程项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="9fdc9-p107">Unique identifier for the remote item in its drive. Read-only.</span></span>                                                                                                    |
| <span data-ttu-id="9fdc9-137">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="9fdc9-137">lastModifiedBy</span></span>       | [<span data-ttu-id="9fdc9-138">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="9fdc9-138">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="9fdc9-p108">上次修改项目的用户、设备和应用程序的标识。只读。</span><span class="sxs-lookup"><span data-stu-id="9fdc9-p108">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                            |
| <span data-ttu-id="9fdc9-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9fdc9-141">lastModifiedDateTime</span></span> | <span data-ttu-id="9fdc9-142">Timestamp</span><span class="sxs-lookup"><span data-stu-id="9fdc9-142">Timestamp</span></span>                           | <span data-ttu-id="9fdc9-p109">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="9fdc9-p109">Date and time the item was last modified. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="9fdc9-145">name</span><span class="sxs-lookup"><span data-stu-id="9fdc9-145">name</span></span>                 | <span data-ttu-id="9fdc9-146">String</span><span class="sxs-lookup"><span data-stu-id="9fdc9-146">String</span></span>                              | <span data-ttu-id="9fdc9-p110">可选。远程项的 Filename。只读。</span><span class="sxs-lookup"><span data-stu-id="9fdc9-p110">Optional. Filename of the remote item. Read-only.</span></span>                                                                                                                 |
| <span data-ttu-id="9fdc9-150">包</span><span class="sxs-lookup"><span data-stu-id="9fdc9-150">package</span></span>              | [<span data-ttu-id="9fdc9-151">包</span><span class="sxs-lookup"><span data-stu-id="9fdc9-151">Package</span></span>](package.md)               | <span data-ttu-id="9fdc9-p111">如果存在，则表示此项是一个包，而不是文件夹或文件。包被视为某些上下文中的文件和其他上下文中的文件夹。只读。</span><span class="sxs-lookup"><span data-stu-id="9fdc9-p111">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span> |
| <span data-ttu-id="9fdc9-155">parentReference</span><span class="sxs-lookup"><span data-stu-id="9fdc9-155">parentReference</span></span>      | [<span data-ttu-id="9fdc9-156">ItemReference</span><span class="sxs-lookup"><span data-stu-id="9fdc9-156">ItemReference</span></span>](itemreference.md)   | <span data-ttu-id="9fdc9-p112">远程项的父级的属性。只读。</span><span class="sxs-lookup"><span data-stu-id="9fdc9-p112">Properties of the parent of the remote item. Read-only.</span></span>                                                                                                           |
| <span data-ttu-id="9fdc9-159">shared</span><span class="sxs-lookup"><span data-stu-id="9fdc9-159">shared</span></span>               | [<span data-ttu-id="9fdc9-160">shared</span><span class="sxs-lookup"><span data-stu-id="9fdc9-160">shared</span></span>](shared.md)                 | <span data-ttu-id="9fdc9-p113">表示此项已与他人共享，并提供有关项目共享状态的信息。只读。</span><span class="sxs-lookup"><span data-stu-id="9fdc9-p113">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>                                       |
| <span data-ttu-id="9fdc9-163">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="9fdc9-163">sharepointIds</span></span>        | [<span data-ttu-id="9fdc9-164">SharepointIds</span><span class="sxs-lookup"><span data-stu-id="9fdc9-164">SharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="9fdc9-p114">为 OneDrive for Business 和 SharePoint 中的项之间的互操作性提供了完整的项标识符集。只读。</span><span class="sxs-lookup"><span data-stu-id="9fdc9-p114">Provides interop between items in OneDrive for Business and SharePoint with the full set of item identifiers. Read-only.</span></span>                                          |
| <span data-ttu-id="9fdc9-167">size</span><span class="sxs-lookup"><span data-stu-id="9fdc9-167">size</span></span>                 | <span data-ttu-id="9fdc9-168">Int64</span><span class="sxs-lookup"><span data-stu-id="9fdc9-168">Int64</span></span>                               | <span data-ttu-id="9fdc9-p115">远程项的大小。只读。</span><span class="sxs-lookup"><span data-stu-id="9fdc9-p115">Size of the remote item. Read-only.</span></span>                                                                                                                               |
| <span data-ttu-id="9fdc9-171">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="9fdc9-171">webDavUrl</span></span>            | <span data-ttu-id="9fdc9-172">Url</span><span class="sxs-lookup"><span data-stu-id="9fdc9-172">Url</span></span>                                 | <span data-ttu-id="9fdc9-173">项的可兼容 DAV 的 URL。</span><span class="sxs-lookup"><span data-stu-id="9fdc9-173">DAV compatible URL for the item.</span></span>                                                                                                                                  |
| <span data-ttu-id="9fdc9-174">WebUrl</span><span class="sxs-lookup"><span data-stu-id="9fdc9-174">webUrl</span></span>               | <span data-ttu-id="9fdc9-175">Url</span><span class="sxs-lookup"><span data-stu-id="9fdc9-175">Url</span></span>                                 | <span data-ttu-id="9fdc9-p116">在浏览器中显示此资源的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="9fdc9-p116">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                         |

## <a name="remarks"></a><span data-ttu-id="9fdc9-178">注解</span><span class="sxs-lookup"><span data-stu-id="9fdc9-178">Remarks</span></span>

<span data-ttu-id="9fdc9-179">有关 **driveItem** 上 facet 的详细信息，请参阅 [driveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="9fdc9-179">For more information about the facets on a **driveItem**, see [driveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/RemoteItem",
  "suppressions": []
}
-->
