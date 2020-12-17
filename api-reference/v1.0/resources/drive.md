---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 驱动器
localization_priority: Priority
ms.prod: sharepoint
description: 驱动器资源是表示用户的 OneDrive 或 SharePoint 中文档库的顶级对象。
doc_type: resourcePageType
ms.openlocfilehash: c389d801f8aea070dd310e1d826c9139298578cd
ms.sourcegitcommit: eafb1629e52450dab0da6a1fb6d1ddfa878777c6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2020
ms.locfileid: "49082284"
---
# <a name="drive-resource-type"></a><span data-ttu-id="6c9af-103">Drive 资源类型</span><span class="sxs-lookup"><span data-stu-id="6c9af-103">Drive resource type</span></span>

<span data-ttu-id="6c9af-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c9af-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6c9af-105">驱动器资源是代表用户的 OneDrive 或在 SharePoint 中文档库的顶级对象。</span><span class="sxs-lookup"><span data-stu-id="6c9af-105">The drive resource is the top-level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="6c9af-p101">OneDrive 用户必须始终具有至少一个可用驱动器，即默认驱动器。没有 OneDrive 许可证的用户不能拥有可用的默认驱动器。</span><span class="sxs-lookup"><span data-stu-id="6c9af-p101">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c9af-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6c9af-108">JSON representation</span></span>

<span data-ttu-id="6c9af-109">下面是 Drive 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c9af-109">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="6c9af-110">**drive** 资源派生自 [**baseItem**](baseitem.md) 并继承该资源的属性。</span><span class="sxs-lookup"><span data-stu-id="6c9af-110">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "activities",
    "createdBy",
    "createdDateTime",
    "description",
    "lastModifiedBy",
    "lastModifiedDateTime",
    "name",
    "webUrl",
    "items",
    "root",
    "sharepointIds",
    "special",
    "system"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.drive"
}-->

```json
{
  "id": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "string (timestamp)",
  "description": "string",
  "driveType": "personal | business | documentLibrary",
  "following": [{"@odata.type": "microsoft.graph.driveItem"}],
  "items": [ { "@odata.type": "microsoft.graph.driveItem" } ],
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "string (timestamp)",
  "name": "string",
  "owner": { "@odata.type": "microsoft.graph.identitySet" },
  "quota": { "@odata.type": "microsoft.graph.quota" },
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "special": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "system": { "@odata.type": "microsoft.graph.systemFacet" },
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="6c9af-111">属性</span><span class="sxs-lookup"><span data-stu-id="6c9af-111">Properties</span></span>

| <span data-ttu-id="6c9af-112">属性</span><span class="sxs-lookup"><span data-stu-id="6c9af-112">Property</span></span>             | <span data-ttu-id="6c9af-113">类型</span><span class="sxs-lookup"><span data-stu-id="6c9af-113">Type</span></span>                          | <span data-ttu-id="6c9af-114">说明</span><span class="sxs-lookup"><span data-stu-id="6c9af-114">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="6c9af-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="6c9af-115">createdBy</span></span>            | <span data-ttu-id="6c9af-116">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="6c9af-116">[identitySet][]</span></span>               | <span data-ttu-id="6c9af-p102">识别创建项目的用户、设备或应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="6c9af-p102">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="6c9af-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c9af-119">createdDateTime</span></span>      | <span data-ttu-id="6c9af-120">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c9af-120">dateTimeOffset</span></span>                | <span data-ttu-id="6c9af-p103">创建项的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="6c9af-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="6c9af-123">description</span><span class="sxs-lookup"><span data-stu-id="6c9af-123">description</span></span>          | <span data-ttu-id="6c9af-124">String</span><span class="sxs-lookup"><span data-stu-id="6c9af-124">String</span></span>                        | <span data-ttu-id="6c9af-125">提供驱动器的用户可见说明。</span><span class="sxs-lookup"><span data-stu-id="6c9af-125">Provide a user-visible description of the drive.</span></span> <span data-ttu-id="6c9af-126">读写。</span><span class="sxs-lookup"><span data-stu-id="6c9af-126">Read-write.</span></span>
| <span data-ttu-id="6c9af-127">driveType</span><span class="sxs-lookup"><span data-stu-id="6c9af-127">driveType</span></span>            | <span data-ttu-id="6c9af-128">String</span><span class="sxs-lookup"><span data-stu-id="6c9af-128">String</span></span>                        | <span data-ttu-id="6c9af-p105">说明了由该资源表示的驱动器的类型。OneDrive 个人版驱动器将返回 `personal`。OneDrive for Business 将返回 `business`。SharePoint 文档库将返回 `documentLibrary`。只读。</span><span class="sxs-lookup"><span data-stu-id="6c9af-p105">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="6c9af-134">id</span><span class="sxs-lookup"><span data-stu-id="6c9af-134">id</span></span>                   | <span data-ttu-id="6c9af-135">String</span><span class="sxs-lookup"><span data-stu-id="6c9af-135">String</span></span>                        | <span data-ttu-id="6c9af-p106">驱动器唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="6c9af-p106">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="6c9af-138">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="6c9af-138">lastModifiedBy</span></span>       | <span data-ttu-id="6c9af-139">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="6c9af-139">[identitySet][]</span></span>               | <span data-ttu-id="6c9af-p107">上次修改项目的用户、设备和应用程序的标识。只读。</span><span class="sxs-lookup"><span data-stu-id="6c9af-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="6c9af-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c9af-142">lastModifiedDateTime</span></span> | <span data-ttu-id="6c9af-143">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c9af-143">dateTimeOffset</span></span>                | <span data-ttu-id="6c9af-p108">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="6c9af-p108">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="6c9af-146">name</span><span class="sxs-lookup"><span data-stu-id="6c9af-146">name</span></span>                 | <span data-ttu-id="6c9af-147">string</span><span class="sxs-lookup"><span data-stu-id="6c9af-147">string</span></span>                        | <span data-ttu-id="6c9af-p109">项目名称。读写。</span><span class="sxs-lookup"><span data-stu-id="6c9af-p109">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="6c9af-150">所有者</span><span class="sxs-lookup"><span data-stu-id="6c9af-150">owner</span></span>                | [<span data-ttu-id="6c9af-151">identitySet</span><span class="sxs-lookup"><span data-stu-id="6c9af-151">identitySet</span></span>](identityset.md) | <span data-ttu-id="6c9af-p110">可选。拥有此驱动器的用户帐户。只读。</span><span class="sxs-lookup"><span data-stu-id="6c9af-p110">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="6c9af-155">配额</span><span class="sxs-lookup"><span data-stu-id="6c9af-155">quota</span></span>                | [<span data-ttu-id="6c9af-156">配额</span><span class="sxs-lookup"><span data-stu-id="6c9af-156">quota</span></span>](quota.md)             | <span data-ttu-id="6c9af-p111">可选。有关驱动器的存储空间配额的信息。只读。</span><span class="sxs-lookup"><span data-stu-id="6c9af-p111">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="6c9af-160">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="6c9af-160">sharepointIds</span></span>        | <span data-ttu-id="6c9af-161">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="6c9af-161">[sharepointIds][]</span></span>             | <span data-ttu-id="6c9af-p112">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="6c9af-p112">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="6c9af-164">system</span><span class="sxs-lookup"><span data-stu-id="6c9af-164">system</span></span>               | <span data-ttu-id="6c9af-165">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="6c9af-165">[systemFacet][]</span></span>               | <span data-ttu-id="6c9af-166">如果存在，则表示这是系统管理的驱动器。</span><span class="sxs-lookup"><span data-stu-id="6c9af-166">If present, indicates that this is a system-managed drive.</span></span> <span data-ttu-id="6c9af-167">只读。</span><span class="sxs-lookup"><span data-stu-id="6c9af-167">Read-only.</span></span>
| <span data-ttu-id="6c9af-168">WebUrl</span><span class="sxs-lookup"><span data-stu-id="6c9af-168">webUrl</span></span>               | <span data-ttu-id="6c9af-169">string (url)</span><span class="sxs-lookup"><span data-stu-id="6c9af-169">string (url)</span></span>                  | <span data-ttu-id="6c9af-p114">在浏览器中显示此资源的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="6c9af-p114">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a><span data-ttu-id="6c9af-175">关系</span><span class="sxs-lookup"><span data-stu-id="6c9af-175">Relationships</span></span>

| <span data-ttu-id="6c9af-176">关系</span><span class="sxs-lookup"><span data-stu-id="6c9af-176">Relationship</span></span> | <span data-ttu-id="6c9af-177">类型</span><span class="sxs-lookup"><span data-stu-id="6c9af-177">Type</span></span>                                 | <span data-ttu-id="6c9af-178">说明</span><span class="sxs-lookup"><span data-stu-id="6c9af-178">Description</span></span>
|:-------------|:-------------------------------------|:-----------------------
| <span data-ttu-id="6c9af-179">following</span><span class="sxs-lookup"><span data-stu-id="6c9af-179">following</span></span>    | <span data-ttu-id="6c9af-180">[DriveItem](driveitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6c9af-180">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="6c9af-181">用户关注的项列表。</span><span class="sxs-lookup"><span data-stu-id="6c9af-181">The list of items the user is following.</span></span> <span data-ttu-id="6c9af-182">仅适用于 OneDrive for Business 中。</span><span class="sxs-lookup"><span data-stu-id="6c9af-182">Only in OneDrive for Business.</span></span>
| <span data-ttu-id="6c9af-183">items</span><span class="sxs-lookup"><span data-stu-id="6c9af-183">items</span></span>        | <span data-ttu-id="6c9af-184">[DriveItem](driveitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6c9af-184">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="6c9af-p116">驱动器中包含的所有项。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="6c9af-p116">All items contained in the drive. Read-only. Nullable.</span></span>
| <span data-ttu-id="6c9af-188">root</span><span class="sxs-lookup"><span data-stu-id="6c9af-188">root</span></span>         | [<span data-ttu-id="6c9af-189">DriveItem</span><span class="sxs-lookup"><span data-stu-id="6c9af-189">DriveItem</span></span>](driveitem.md)            | <span data-ttu-id="6c9af-p117">驱动器的根文件夹。只读。</span><span class="sxs-lookup"><span data-stu-id="6c9af-p117">The root folder of the drive. Read-only.</span></span>
| <span data-ttu-id="6c9af-192">special</span><span class="sxs-lookup"><span data-stu-id="6c9af-192">special</span></span>      | <span data-ttu-id="6c9af-193">[DriveItem](driveitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6c9af-193">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="6c9af-194">OneDrive 中可用的公用文件夹的集合。</span><span class="sxs-lookup"><span data-stu-id="6c9af-194">Collection of common folders available in OneDrive.</span></span> <span data-ttu-id="6c9af-195">只读。</span><span class="sxs-lookup"><span data-stu-id="6c9af-195">Read-only.</span></span> <span data-ttu-id="6c9af-196">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="6c9af-196">Nullable.</span></span>
| <span data-ttu-id="6c9af-197">list</span><span class="sxs-lookup"><span data-stu-id="6c9af-197">list</span></span>         | [<span data-ttu-id="6c9af-198">List</span><span class="sxs-lookup"><span data-stu-id="6c9af-198">List</span></span>](list.md)                      | <span data-ttu-id="6c9af-199">适合于 SharePoint 中的驱动器，基本文档库列表。</span><span class="sxs-lookup"><span data-stu-id="6c9af-199">For drives in SharePoint, the underlying document library list.</span></span> <span data-ttu-id="6c9af-200">只读。</span><span class="sxs-lookup"><span data-stu-id="6c9af-200">Read-only.</span></span> <span data-ttu-id="6c9af-201">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="6c9af-201">Nullable.</span></span>

## <a name="methods"></a><span data-ttu-id="6c9af-202">方法</span><span class="sxs-lookup"><span data-stu-id="6c9af-202">Methods</span></span>

|                        <span data-ttu-id="6c9af-203">常见任务</span><span class="sxs-lookup"><span data-stu-id="6c9af-203">Common task</span></span>                         |         <span data-ttu-id="6c9af-204">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="6c9af-204">HTTP method</span></span>         |
| :--------------------------------------------------------- | :-------------------------- |
| <span data-ttu-id="6c9af-205">[获取其他驱动器的驱动器元数据][drive-get]</span><span class="sxs-lookup"><span data-stu-id="6c9af-205">[Get Drive metadata of another Drive][drive-get]</span></span>           | `GET /drives/{drive-id}`    |
| <span data-ttu-id="6c9af-206">[获取用户默认驱动器的根文件夹][item-get]</span><span class="sxs-lookup"><span data-stu-id="6c9af-206">[Get root folder for user's default Drive][item-get]</span></span>       | `GET /drive/root`           |
| <span data-ttu-id="6c9af-207">[列出驱动器下的子项][item-children]</span><span class="sxs-lookup"><span data-stu-id="6c9af-207">[List children under the Drive][item-children]</span></span>             | `GET /drive/root/children`  |
| <span data-ttu-id="6c9af-208">[列出驱动器中所有项的变更][item-changes]</span><span class="sxs-lookup"><span data-stu-id="6c9af-208">[List changes for all Items in the Drive][item-changes]</span></span>    | `GET /drive/root/delta`     |
| <span data-ttu-id="6c9af-209">[列出用户的关注 driveItems][drive-following]</span><span class="sxs-lookup"><span data-stu-id="6c9af-209">[List user's followed driveItems][drive-following]</span></span>         | `Get /drive/following`       |
| <span data-ttu-id="6c9af-210">[搜索驱动器中的项][item-search]</span><span class="sxs-lookup"><span data-stu-id="6c9af-210">[Search for Items in the Drive][item-search]</span></span>               | `GET /drive/root/search`    |
| [<span data-ttu-id="6c9af-211">访问特殊文件夹</span><span class="sxs-lookup"><span data-stu-id="6c9af-211">Access special folder</span></span>](../api/drive-get-specialfolder.md) | `GET /drive/special/{name}` |

<span data-ttu-id="6c9af-212">在上表中，各示例使用的是 `/drive`，但其他路径也同样有效。</span><span class="sxs-lookup"><span data-stu-id="6c9af-212">In the previous table, the examples use `/drive`, but other paths are valid too.</span></span>

[item-resource]: driveitem.md
[identity-set]: identityset.md
[quota-facet]: quota.md
[drive-resource]: drive.md
[drive-get]: ../api/drive-get.md
[item-get]: ../api/driveitem-get.md
[item-changes]: ../api/driveitem-delta.md
[item-search]: ../api/driveitem-search.md
[item-children]: ../api/driveitem-list-children.md
[drive-following]: ../api/drive-list-following.md


<!-- {
  "type": "#page.annotation",
  "description": "Drive is a top level object for OneDrive API that provides access to the contents of a drive. ",
  "keywords": "drive,objects,resources",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/drive.md:
      Found potential enums in resource example that weren't defined in a table:(personal,business,documentLibrary) are in resource, but () are in table"
  ],
  "tocPath": "Drives",
  "tocBookmarks": { "Resources/Drive": "#" }
} -->

