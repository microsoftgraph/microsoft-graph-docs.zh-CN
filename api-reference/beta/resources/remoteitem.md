---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: RemoteItem
localization_priority: Normal
ms.openlocfilehash: 13eb7ff286467a7acfef85f58ea59763a13d9801
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514332"
---
# <a name="remoteitem-resource-type"></a><span data-ttu-id="aabfd-102">RemoteItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="aabfd-102">RemoteItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aabfd-p101">remoteItem 资源指示 driveItem 引用存在于其他驱动器中的项。该资源提供源驱动器和目标项的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="aabfd-p101">The **remoteItem** resource indicates that a [**driveItem**](driveitem.md) references an item that exists in another drive. This resource provides the unique IDs of the source drive and target item.</span></span>

<span data-ttu-id="aabfd-105">具有非 NULL **remoteItem** facet 的 [**DriveItems**](driveitem.md) 是共享、添加到用户的 OneDrive 的资源，或从项（例如搜索结果）的 hetrogenous 集合返回的项中的资源。</span><span class="sxs-lookup"><span data-stu-id="aabfd-105">[**DriveItems**](driveitem.md) with a non-null **remoteItem** facet are resources that are shared, added to the user's OneDrive, or on items returned from hetrogenous collections of items (like search results).</span></span>

<span data-ttu-id="aabfd-106">**注意：** 与同一驱动器中的文件夹不同，移动到远程项的 **driveItem** 可更改其 `id` 值。</span><span class="sxs-lookup"><span data-stu-id="aabfd-106">**Note:** Unlike with folders in the same drive, a **driveItem** moved into a remote item may have its `id` value changed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="aabfd-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aabfd-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="aabfd-108">属性</span><span class="sxs-lookup"><span data-stu-id="aabfd-108">Properties</span></span>

| <span data-ttu-id="aabfd-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="aabfd-109">Property name</span></span>        | <span data-ttu-id="aabfd-110">类型</span><span class="sxs-lookup"><span data-stu-id="aabfd-110">Type</span></span>                                | <span data-ttu-id="aabfd-111">说明</span><span class="sxs-lookup"><span data-stu-id="aabfd-111">Description</span></span>                                                                                                                                                       |
| :------------------- | :---------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="aabfd-112">createdBy</span><span class="sxs-lookup"><span data-stu-id="aabfd-112">createdBy</span></span>            | [<span data-ttu-id="aabfd-113">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="aabfd-113">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="aabfd-p102">创建项的用户、设备和应用程序标识。只读。</span><span class="sxs-lookup"><span data-stu-id="aabfd-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>                                                                                  |
| <span data-ttu-id="aabfd-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aabfd-116">createdDateTime</span></span>      | <span data-ttu-id="aabfd-117">Timestamp</span><span class="sxs-lookup"><span data-stu-id="aabfd-117">Timestamp</span></span>                           | <span data-ttu-id="aabfd-p103">创建项的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="aabfd-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                        |
| <span data-ttu-id="aabfd-120">文件</span><span class="sxs-lookup"><span data-stu-id="aabfd-120">file</span></span>                 | [<span data-ttu-id="aabfd-121">文件</span><span class="sxs-lookup"><span data-stu-id="aabfd-121">File</span></span>](file.md)                     | <span data-ttu-id="aabfd-p104">指示远程项是文件。只读。</span><span class="sxs-lookup"><span data-stu-id="aabfd-p104">Indicates that the remote item is a file. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="aabfd-124">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="aabfd-124">fileSystemInfo</span></span>       | [<span data-ttu-id="aabfd-125">FileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="aabfd-125">FileSystemInfo</span></span>](filesysteminfo.md) | <span data-ttu-id="aabfd-p105">本地文件系统中的远程项的有关信息。只读。</span><span class="sxs-lookup"><span data-stu-id="aabfd-p105">Information about the remote item from the local file system. Read-only.</span></span>                                                                                          |
| <span data-ttu-id="aabfd-128">文件夹</span><span class="sxs-lookup"><span data-stu-id="aabfd-128">folder</span></span>               | [<span data-ttu-id="aabfd-129">文件夹</span><span class="sxs-lookup"><span data-stu-id="aabfd-129">Folder</span></span>](folder.md)                 | <span data-ttu-id="aabfd-p106">指示远程项是文件夹。只读。</span><span class="sxs-lookup"><span data-stu-id="aabfd-p106">Indicates that the remote item is a folder. Read-only.</span></span>                                                                                                            |
| <span data-ttu-id="aabfd-132">id</span><span class="sxs-lookup"><span data-stu-id="aabfd-132">id</span></span>                   | <span data-ttu-id="aabfd-133">String</span><span class="sxs-lookup"><span data-stu-id="aabfd-133">String</span></span>                              | <span data-ttu-id="aabfd-p107">驱动器内远程项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="aabfd-p107">Unique identifier for the remote item in its drive. Read-only.</span></span>                                                                                                    |
| <span data-ttu-id="aabfd-136">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="aabfd-136">lastModifiedBy</span></span>       | [<span data-ttu-id="aabfd-137">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="aabfd-137">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="aabfd-p108">上次修改项的用户、设备和应用程序标识。只读。</span><span class="sxs-lookup"><span data-stu-id="aabfd-p108">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                            |
| <span data-ttu-id="aabfd-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aabfd-140">lastModifiedDateTime</span></span> | <span data-ttu-id="aabfd-141">Timestamp</span><span class="sxs-lookup"><span data-stu-id="aabfd-141">Timestamp</span></span>                           | <span data-ttu-id="aabfd-p109">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="aabfd-p109">Date and time the item was last modified. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="aabfd-144">名称</span><span class="sxs-lookup"><span data-stu-id="aabfd-144">name</span></span>                 | <span data-ttu-id="aabfd-145">String</span><span class="sxs-lookup"><span data-stu-id="aabfd-145">String</span></span>                              | <span data-ttu-id="aabfd-p110">可选。远程项的 Filename。只读。</span><span class="sxs-lookup"><span data-stu-id="aabfd-p110">Optional. Filename of the remote item. Read-only.</span></span>                                                                                                                 |
| <span data-ttu-id="aabfd-149">包</span><span class="sxs-lookup"><span data-stu-id="aabfd-149">package</span></span>              | [<span data-ttu-id="aabfd-150">包</span><span class="sxs-lookup"><span data-stu-id="aabfd-150">Package</span></span>](package.md)               | <span data-ttu-id="aabfd-p111">如果存在，则表示此项是包而不是文件夹或文件。在某些上下文中将包视为文件，在其他上下文中视为文件夹。只读。</span><span class="sxs-lookup"><span data-stu-id="aabfd-p111">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span> |
| <span data-ttu-id="aabfd-154">parentReference</span><span class="sxs-lookup"><span data-stu-id="aabfd-154">parentReference</span></span>      | [<span data-ttu-id="aabfd-155">ItemReference</span><span class="sxs-lookup"><span data-stu-id="aabfd-155">ItemReference</span></span>](itemreference.md)   | <span data-ttu-id="aabfd-p112">远程项的父级的属性。只读。</span><span class="sxs-lookup"><span data-stu-id="aabfd-p112">Properties of the parent of the remote item. Read-only.</span></span>                                                                                                           |
| <span data-ttu-id="aabfd-158">shared</span><span class="sxs-lookup"><span data-stu-id="aabfd-158">shared</span></span>               | [<span data-ttu-id="aabfd-159">共享</span><span class="sxs-lookup"><span data-stu-id="aabfd-159">shared</span></span>](shared.md)                 | <span data-ttu-id="aabfd-p113">表示此项已与他人共享，并提供有关项目共享状态的信息。只读。</span><span class="sxs-lookup"><span data-stu-id="aabfd-p113">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>                                       |
| <span data-ttu-id="aabfd-162">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="aabfd-162">sharepointIds</span></span>        | [<span data-ttu-id="aabfd-163">SharepointIds</span><span class="sxs-lookup"><span data-stu-id="aabfd-163">SharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="aabfd-p114">为 OneDrive for Business 和 SharePoint 中的项之间的互操作性提供了完整的项标识符集。只读。</span><span class="sxs-lookup"><span data-stu-id="aabfd-p114">Provides interop between items in OneDrive for Business and SharePoint with the full set of item identifiers. Read-only.</span></span>                                          |
| <span data-ttu-id="aabfd-166">size</span><span class="sxs-lookup"><span data-stu-id="aabfd-166">size</span></span>                 | <span data-ttu-id="aabfd-167">Int64</span><span class="sxs-lookup"><span data-stu-id="aabfd-167">Int64</span></span>                               | <span data-ttu-id="aabfd-p115">远程项的大小。只读。</span><span class="sxs-lookup"><span data-stu-id="aabfd-p115">Size of the remote item. Read-only.</span></span>                                                                                                                               |
| <span data-ttu-id="aabfd-170">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="aabfd-170">webDavUrl</span></span>            | <span data-ttu-id="aabfd-171">Url</span><span class="sxs-lookup"><span data-stu-id="aabfd-171">Url</span></span>                                 | <span data-ttu-id="aabfd-172">项的可兼容 DAV 的 URL。</span><span class="sxs-lookup"><span data-stu-id="aabfd-172">DAV compatible URL for the item.</span></span>                                                                                                                                  |
| <span data-ttu-id="aabfd-173">webUrl</span><span class="sxs-lookup"><span data-stu-id="aabfd-173">webUrl</span></span>               | <span data-ttu-id="aabfd-174">URL</span><span class="sxs-lookup"><span data-stu-id="aabfd-174">Url</span></span>                                 | <span data-ttu-id="aabfd-p116">在浏览器中显示此资源的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="aabfd-p116">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                         |

## <a name="remarks"></a><span data-ttu-id="aabfd-177">注解</span><span class="sxs-lookup"><span data-stu-id="aabfd-177">Remarks</span></span>

<span data-ttu-id="aabfd-178">有关 **driveItem** 上 facet 的详细信息，请参阅 [driveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="aabfd-178">For more information about the facets on a **driveItem**, see [driveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/RemoteItem",
  "suppressions": [
    "Error: /api-reference/beta/resources/remoteitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
