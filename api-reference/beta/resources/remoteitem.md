---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: RemoteItem
localization_priority: Normal
ms.openlocfilehash: 122e13513db1a59e23a41cadd16e61996e6a6c04
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843188"
---
# <a name="remoteitem-resource-type"></a><span data-ttu-id="fad30-102">RemoteItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="fad30-102">RemoteItem resource type</span></span>

> <span data-ttu-id="fad30-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fad30-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fad30-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fad30-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fad30-p102">**remoteItem** 资源指示 [**driveItem**](driveitem.md) 引用存在于其他驱动器中的项。该资源提供源驱动器和目标项的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="fad30-p102">The **remoteItem** resource indicates that a [**driveItem**](driveitem.md) references an item that exists in another drive. This resource provides the unique IDs of the source drive and target item.</span></span>

<span data-ttu-id="fad30-107">具有非 NULL **remoteItem** facet 的 [**DriveItems**](driveitem.md) 是共享、添加到用户的 OneDrive 的资源，或从项（例如搜索结果）的 hetrogenous 集合返回的项中的资源。</span><span class="sxs-lookup"><span data-stu-id="fad30-107">[**DriveItems**](driveitem.md) with a non-null **remoteItem** facet are resources that are shared, added to the user's OneDrive, or on items returned from hetrogenous collections of items (like search results).</span></span>

<span data-ttu-id="fad30-108">**注意：** 与同一驱动器中的文件夹不同，移动到远程项的 **driveItem** 可更改其 `id` 值。</span><span class="sxs-lookup"><span data-stu-id="fad30-108">**Note:** Unlike with folders in the same drive, a **driveItem** moved into a remote item may have its `id` value changed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fad30-109">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fad30-109">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="fad30-110">属性</span><span class="sxs-lookup"><span data-stu-id="fad30-110">Properties</span></span>

| <span data-ttu-id="fad30-111">属性名称</span><span class="sxs-lookup"><span data-stu-id="fad30-111">Property name</span></span>        | <span data-ttu-id="fad30-112">类型</span><span class="sxs-lookup"><span data-stu-id="fad30-112">Type</span></span>                                | <span data-ttu-id="fad30-113">说明</span><span class="sxs-lookup"><span data-stu-id="fad30-113">Description</span></span>                                                                                                                                                       |
| :------------------- | :---------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="fad30-114">createdBy</span><span class="sxs-lookup"><span data-stu-id="fad30-114">createdBy</span></span>            | [<span data-ttu-id="fad30-115">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="fad30-115">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="fad30-p103">创建项的用户、设备和应用程序标识。只读。</span><span class="sxs-lookup"><span data-stu-id="fad30-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>                                                                                  |
| <span data-ttu-id="fad30-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fad30-118">createdDateTime</span></span>      | <span data-ttu-id="fad30-119">Timestamp</span><span class="sxs-lookup"><span data-stu-id="fad30-119">Timestamp</span></span>                           | <span data-ttu-id="fad30-p104">创建项的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="fad30-p104">Date and time of item creation. Read-only.</span></span>                                                                                                                        |
| <span data-ttu-id="fad30-122">文件</span><span class="sxs-lookup"><span data-stu-id="fad30-122">file</span></span>                 | [<span data-ttu-id="fad30-123">文件</span><span class="sxs-lookup"><span data-stu-id="fad30-123">File</span></span>](file.md)                     | <span data-ttu-id="fad30-p105">指示远程项是文件。只读。</span><span class="sxs-lookup"><span data-stu-id="fad30-p105">Indicates that the remote item is a file. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="fad30-126">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="fad30-126">fileSystemInfo</span></span>       | [<span data-ttu-id="fad30-127">FileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="fad30-127">FileSystemInfo</span></span>](filesysteminfo.md) | <span data-ttu-id="fad30-p106">本地文件系统中的远程项的有关信息。只读。</span><span class="sxs-lookup"><span data-stu-id="fad30-p106">Information about the remote item from the local file system. Read-only.</span></span>                                                                                          |
| <span data-ttu-id="fad30-130">文件夹</span><span class="sxs-lookup"><span data-stu-id="fad30-130">folder</span></span>               | [<span data-ttu-id="fad30-131">文件夹</span><span class="sxs-lookup"><span data-stu-id="fad30-131">Folder</span></span>](folder.md)                 | <span data-ttu-id="fad30-p107">指示远程项是文件夹。只读。</span><span class="sxs-lookup"><span data-stu-id="fad30-p107">Indicates that the remote item is a folder. Read-only.</span></span>                                                                                                            |
| <span data-ttu-id="fad30-134">id</span><span class="sxs-lookup"><span data-stu-id="fad30-134">id</span></span>                   | <span data-ttu-id="fad30-135">String</span><span class="sxs-lookup"><span data-stu-id="fad30-135">String</span></span>                              | <span data-ttu-id="fad30-p108">驱动器内远程项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="fad30-p108">Unique identifier for the remote item in its drive. Read-only.</span></span>                                                                                                    |
| <span data-ttu-id="fad30-138">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="fad30-138">lastModifiedBy</span></span>       | [<span data-ttu-id="fad30-139">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="fad30-139">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="fad30-p109">上次修改项的用户、设备和应用程序标识。只读。</span><span class="sxs-lookup"><span data-stu-id="fad30-p109">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                            |
| <span data-ttu-id="fad30-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fad30-142">lastModifiedDateTime</span></span> | <span data-ttu-id="fad30-143">Timestamp</span><span class="sxs-lookup"><span data-stu-id="fad30-143">Timestamp</span></span>                           | <span data-ttu-id="fad30-p110">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="fad30-p110">Date and time the item was last modified. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="fad30-146">name</span><span class="sxs-lookup"><span data-stu-id="fad30-146">name</span></span>                 | <span data-ttu-id="fad30-147">String</span><span class="sxs-lookup"><span data-stu-id="fad30-147">String</span></span>                              | <span data-ttu-id="fad30-p111">可选。远程项的 Filename。只读。</span><span class="sxs-lookup"><span data-stu-id="fad30-p111">Optional. Filename of the remote item. Read-only.</span></span>                                                                                                                 |
| <span data-ttu-id="fad30-151">包</span><span class="sxs-lookup"><span data-stu-id="fad30-151">package</span></span>              | [<span data-ttu-id="fad30-152">包</span><span class="sxs-lookup"><span data-stu-id="fad30-152">Package</span></span>](package.md)               | <span data-ttu-id="fad30-p112">如果存在，则表示此项是包而不是文件夹或文件。在某些上下文中将包视为文件，在其他上下文中视为文件夹。只读。</span><span class="sxs-lookup"><span data-stu-id="fad30-p112">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span> |
| <span data-ttu-id="fad30-156">parentReference</span><span class="sxs-lookup"><span data-stu-id="fad30-156">parentReference</span></span>      | [<span data-ttu-id="fad30-157">ItemReference</span><span class="sxs-lookup"><span data-stu-id="fad30-157">ItemReference</span></span>](itemreference.md)   | <span data-ttu-id="fad30-p113">远程项的父级的属性。只读。</span><span class="sxs-lookup"><span data-stu-id="fad30-p113">Properties of the parent of the remote item. Read-only.</span></span>                                                                                                           |
| <span data-ttu-id="fad30-160">shared</span><span class="sxs-lookup"><span data-stu-id="fad30-160">shared</span></span>               | [<span data-ttu-id="fad30-161">共享</span><span class="sxs-lookup"><span data-stu-id="fad30-161">shared</span></span>](shared.md)                 | <span data-ttu-id="fad30-p114">表示此项已与他人共享，并提供有关项目共享状态的信息。只读。</span><span class="sxs-lookup"><span data-stu-id="fad30-p114">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>                                       |
| <span data-ttu-id="fad30-164">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="fad30-164">sharepointIds</span></span>        | [<span data-ttu-id="fad30-165">SharepointIds</span><span class="sxs-lookup"><span data-stu-id="fad30-165">SharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="fad30-p115">为 OneDrive for Business 和 SharePoint 中的项之间的互操作性提供了完整的项标识符集。只读。</span><span class="sxs-lookup"><span data-stu-id="fad30-p115">Provides interop between items in OneDrive for Business and SharePoint with the full set of item identifiers. Read-only.</span></span>                                          |
| <span data-ttu-id="fad30-168">size</span><span class="sxs-lookup"><span data-stu-id="fad30-168">size</span></span>                 | <span data-ttu-id="fad30-169">Int64</span><span class="sxs-lookup"><span data-stu-id="fad30-169">Int64</span></span>                               | <span data-ttu-id="fad30-p116">远程项的大小。只读。</span><span class="sxs-lookup"><span data-stu-id="fad30-p116">Size of the remote item. Read-only.</span></span>                                                                                                                               |
| <span data-ttu-id="fad30-172">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="fad30-172">webDavUrl</span></span>            | <span data-ttu-id="fad30-173">Url</span><span class="sxs-lookup"><span data-stu-id="fad30-173">Url</span></span>                                 | <span data-ttu-id="fad30-174">项的可兼容 DAV 的 URL。</span><span class="sxs-lookup"><span data-stu-id="fad30-174">DAV compatible URL for the item.</span></span>                                                                                                                                  |
| <span data-ttu-id="fad30-175">webUrl</span><span class="sxs-lookup"><span data-stu-id="fad30-175">webUrl</span></span>               | <span data-ttu-id="fad30-176">Url</span><span class="sxs-lookup"><span data-stu-id="fad30-176">Url</span></span>                                 | <span data-ttu-id="fad30-p117">在浏览器中显示此资源的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="fad30-p117">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                         |

## <a name="remarks"></a><span data-ttu-id="fad30-179">注解</span><span class="sxs-lookup"><span data-stu-id="fad30-179">Remarks</span></span>

<span data-ttu-id="fad30-180">有关 **driveItem** 上 facet 的详细信息，请参阅 [driveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="fad30-180">For more information about the facets on a **driveItem**, see [driveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/RemoteItem"
} -->
