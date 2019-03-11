---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Drive
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: a6a406ef5cb011e82d14c54ea0a35cd93eaab837
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480605"
---
# <a name="drive-resource-type"></a><span data-ttu-id="7d0ed-102">Drive 资源类型</span><span class="sxs-lookup"><span data-stu-id="7d0ed-102">drive resource type</span></span>

<span data-ttu-id="7d0ed-103">驱动器资源是表示用户的 OneDrive 或 SharePoint 中文档库的顶级对象。</span><span class="sxs-lookup"><span data-stu-id="7d0ed-103">The drive resource is the top level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="7d0ed-p101">OneDrive 用户必须始终具有至少一个可用驱动器，即默认驱动器。没有 OneDrive 许可证的用户不能拥有可用的默认驱动器。</span><span class="sxs-lookup"><span data-stu-id="7d0ed-p101">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7d0ed-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7d0ed-106">JSON representation</span></span>

<span data-ttu-id="7d0ed-107">下面是 Drive 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7d0ed-107">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="7d0ed-108">**drive** 资源派生自 [**baseItem**](baseitem.md) 并继承该资源的属性。</span><span class="sxs-lookup"><span data-stu-id="7d0ed-108">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="7d0ed-109">属性</span><span class="sxs-lookup"><span data-stu-id="7d0ed-109">Properties</span></span>

| <span data-ttu-id="7d0ed-110">属性</span><span class="sxs-lookup"><span data-stu-id="7d0ed-110">Property</span></span>             | <span data-ttu-id="7d0ed-111">类型</span><span class="sxs-lookup"><span data-stu-id="7d0ed-111">Type</span></span>                          | <span data-ttu-id="7d0ed-112">说明</span><span class="sxs-lookup"><span data-stu-id="7d0ed-112">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="7d0ed-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="7d0ed-113">createdBy</span></span>            | <span data-ttu-id="7d0ed-114">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="7d0ed-114">[identitySet][]</span></span>               | <span data-ttu-id="7d0ed-p102">识别创建项目的用户、设备或应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="7d0ed-p102">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="7d0ed-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7d0ed-117">createdDateTime</span></span>      | <span data-ttu-id="7d0ed-118">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d0ed-118">dateTimeOffset</span></span>                | <span data-ttu-id="7d0ed-p103">创建项的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="7d0ed-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="7d0ed-121">description</span><span class="sxs-lookup"><span data-stu-id="7d0ed-121">description</span></span>          | <span data-ttu-id="7d0ed-122">String</span><span class="sxs-lookup"><span data-stu-id="7d0ed-122">String</span></span>                        | <span data-ttu-id="7d0ed-123">提供驱动器的用户可见说明。</span><span class="sxs-lookup"><span data-stu-id="7d0ed-123">Provide a user-visible description of the drive.</span></span> <span data-ttu-id="7d0ed-124">读写。</span><span class="sxs-lookup"><span data-stu-id="7d0ed-124">Read-write.</span></span>
| <span data-ttu-id="7d0ed-125">driveType</span><span class="sxs-lookup"><span data-stu-id="7d0ed-125">driveType</span></span>            | <span data-ttu-id="7d0ed-126">String</span><span class="sxs-lookup"><span data-stu-id="7d0ed-126">String</span></span>                        | <span data-ttu-id="7d0ed-p105">说明了由该资源表示的驱动器的类型。OneDrive 个人版驱动器将返回 `personal`。OneDrive for Business 将返回 `business`。SharePoint 文档库将返回 `documentLibrary`。只读。</span><span class="sxs-lookup"><span data-stu-id="7d0ed-p105">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="7d0ed-132">id</span><span class="sxs-lookup"><span data-stu-id="7d0ed-132">id</span></span>                   | <span data-ttu-id="7d0ed-133">String</span><span class="sxs-lookup"><span data-stu-id="7d0ed-133">String</span></span>                        | <span data-ttu-id="7d0ed-p106">驱动器唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="7d0ed-p106">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="7d0ed-136">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="7d0ed-136">lastModifiedBy</span></span>       | <span data-ttu-id="7d0ed-137">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="7d0ed-137">[identitySet][]</span></span>               | <span data-ttu-id="7d0ed-p107">上次修改项目的用户、设备和应用程序的标识。只读。</span><span class="sxs-lookup"><span data-stu-id="7d0ed-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="7d0ed-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7d0ed-140">lastModifiedDateTime</span></span> | <span data-ttu-id="7d0ed-141">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d0ed-141">dateTimeOffset</span></span>                | <span data-ttu-id="7d0ed-p108">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="7d0ed-p108">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="7d0ed-144">name</span><span class="sxs-lookup"><span data-stu-id="7d0ed-144">name</span></span>                 | <span data-ttu-id="7d0ed-145">string</span><span class="sxs-lookup"><span data-stu-id="7d0ed-145">string</span></span>                        | <span data-ttu-id="7d0ed-p109">项目名称。读写。</span><span class="sxs-lookup"><span data-stu-id="7d0ed-p109">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="7d0ed-148">所有者</span><span class="sxs-lookup"><span data-stu-id="7d0ed-148">owner</span></span>                | [<span data-ttu-id="7d0ed-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="7d0ed-149">identitySet</span></span>](identityset.md) | <span data-ttu-id="7d0ed-p110">可选。拥有此驱动器的用户帐户。只读。</span><span class="sxs-lookup"><span data-stu-id="7d0ed-p110">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="7d0ed-153">配额</span><span class="sxs-lookup"><span data-stu-id="7d0ed-153">quota</span></span>                | [<span data-ttu-id="7d0ed-154">配额</span><span class="sxs-lookup"><span data-stu-id="7d0ed-154">quota</span></span>](quota.md)             | <span data-ttu-id="7d0ed-p111">可选。有关驱动器的存储空间配额的信息。只读。</span><span class="sxs-lookup"><span data-stu-id="7d0ed-p111">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="7d0ed-158">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="7d0ed-158">sharepointIds</span></span>        | <span data-ttu-id="7d0ed-159">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="7d0ed-159">[sharepointIds][]</span></span>             | <span data-ttu-id="7d0ed-p112">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="7d0ed-p112">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="7d0ed-162">system</span><span class="sxs-lookup"><span data-stu-id="7d0ed-162">system</span></span>               | <span data-ttu-id="7d0ed-163">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="7d0ed-163">[systemFacet][]</span></span>               | <span data-ttu-id="7d0ed-164">如果存在，则表示这是系统管理的驱动器。</span><span class="sxs-lookup"><span data-stu-id="7d0ed-164">If present, indicates that this is a system-managed drive.</span></span> <span data-ttu-id="7d0ed-165">只读。</span><span class="sxs-lookup"><span data-stu-id="7d0ed-165">Read-only.</span></span>
| <span data-ttu-id="7d0ed-166">WebUrl</span><span class="sxs-lookup"><span data-stu-id="7d0ed-166">webUrl</span></span>               | <span data-ttu-id="7d0ed-167">string (url)</span><span class="sxs-lookup"><span data-stu-id="7d0ed-167">string (url)</span></span>                  | <span data-ttu-id="7d0ed-p114">在浏览器中显示此资源的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="7d0ed-p114">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a><span data-ttu-id="7d0ed-173">关系</span><span class="sxs-lookup"><span data-stu-id="7d0ed-173">Relationships</span></span>

| <span data-ttu-id="7d0ed-174">关系</span><span class="sxs-lookup"><span data-stu-id="7d0ed-174">Relationship</span></span> | <span data-ttu-id="7d0ed-175">类型</span><span class="sxs-lookup"><span data-stu-id="7d0ed-175">Type</span></span>                                 | <span data-ttu-id="7d0ed-176">说明</span><span class="sxs-lookup"><span data-stu-id="7d0ed-176">Description</span></span>
|:-------------|:-------------------------------------|:-----------------------
| <span data-ttu-id="7d0ed-177">items</span><span class="sxs-lookup"><span data-stu-id="7d0ed-177">items</span></span>        | <span data-ttu-id="7d0ed-178">[DriveItem](driveitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7d0ed-178">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="7d0ed-p115">驱动器中包含的所有项。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="7d0ed-p115">All items contained in the drive. Read-only. Nullable.</span></span>
| <span data-ttu-id="7d0ed-182">root</span><span class="sxs-lookup"><span data-stu-id="7d0ed-182">root</span></span>         | [<span data-ttu-id="7d0ed-183">DriveItem</span><span class="sxs-lookup"><span data-stu-id="7d0ed-183">DriveItem</span></span>](driveitem.md)            | <span data-ttu-id="7d0ed-p116">驱动器的根文件夹。只读。</span><span class="sxs-lookup"><span data-stu-id="7d0ed-p116">The root folder of the drive. Read-only.</span></span>
| <span data-ttu-id="7d0ed-186">special</span><span class="sxs-lookup"><span data-stu-id="7d0ed-186">special</span></span>      | <span data-ttu-id="7d0ed-187">[DriveItem](driveitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7d0ed-187">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="7d0ed-188">OneDrive 中可用的公用文件夹的集合。</span><span class="sxs-lookup"><span data-stu-id="7d0ed-188">Collection of common folders available in OneDrive.</span></span> <span data-ttu-id="7d0ed-189">只读。</span><span class="sxs-lookup"><span data-stu-id="7d0ed-189">Read-only.</span></span> <span data-ttu-id="7d0ed-190">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="7d0ed-190">Nullable.</span></span>
| <span data-ttu-id="7d0ed-191">list</span><span class="sxs-lookup"><span data-stu-id="7d0ed-191">list</span></span>         | [<span data-ttu-id="7d0ed-192">List</span><span class="sxs-lookup"><span data-stu-id="7d0ed-192">List</span></span>](list.md)                      | <span data-ttu-id="7d0ed-193">适合于 SharePoint 中的驱动器，基本文档库列表。</span><span class="sxs-lookup"><span data-stu-id="7d0ed-193">For drives in SharePoint, the underlying document library list.</span></span> <span data-ttu-id="7d0ed-194">只读。</span><span class="sxs-lookup"><span data-stu-id="7d0ed-194">Read-only.</span></span> <span data-ttu-id="7d0ed-195">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="7d0ed-195">Nullable.</span></span>

## <a name="methods"></a><span data-ttu-id="7d0ed-196">方法</span><span class="sxs-lookup"><span data-stu-id="7d0ed-196">Methods</span></span>

|                        <span data-ttu-id="7d0ed-197">常见任务</span><span class="sxs-lookup"><span data-stu-id="7d0ed-197">Common task</span></span>                         |         <span data-ttu-id="7d0ed-198">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="7d0ed-198">HTTP method</span></span>         |
| :--------------------------------------------------------- | :-------------------------- |
| <span data-ttu-id="7d0ed-199">[获取其他驱动器的驱动器元数据][drive-get]</span><span class="sxs-lookup"><span data-stu-id="7d0ed-199">[Get Drive metadata of another Drive][drive-get]</span></span>           | `GET /drives/{drive-id}`    |
| <span data-ttu-id="7d0ed-200">[获取用户默认驱动器的根文件夹][item-get]</span><span class="sxs-lookup"><span data-stu-id="7d0ed-200">[Get root folder for user's default Drive][item-get]</span></span>       | `GET /drive/root`           |
| <span data-ttu-id="7d0ed-201">[列出驱动器下的子项][item-children]</span><span class="sxs-lookup"><span data-stu-id="7d0ed-201">[List children under the Drive][item-children]</span></span>             | `GET /drive/root/children`  |
| <span data-ttu-id="7d0ed-202">[列出驱动器中所有项的变更][item-changes]</span><span class="sxs-lookup"><span data-stu-id="7d0ed-202">[List changes for all Items in the Drive][item-changes]</span></span>    | `GET /drive/root/delta`     |
| <span data-ttu-id="7d0ed-203">[搜索驱动器中的项][item-search]</span><span class="sxs-lookup"><span data-stu-id="7d0ed-203">[Search for Items in the Drive][item-search]</span></span>               | `GET /drive/root/search`    |
| [<span data-ttu-id="7d0ed-204">访问特殊文件夹</span><span class="sxs-lookup"><span data-stu-id="7d0ed-204">Access special folder</span></span>](../api/drive-get-specialfolder.md) | `GET /drive/special/{name}` |

<span data-ttu-id="7d0ed-205">在上表中，各示例使用的是 `/drive`，但其他路径也同样有效。</span><span class="sxs-lookup"><span data-stu-id="7d0ed-205">In the previous table, the examples use `/drive`, but other paths are valid too.</span></span>

[item-resource]: driveitem.md
[identity-set]: identityset.md
[quota-facet]: quota.md
[drive-resource]: drive.md
[drive-get]: ../api/drive-get.md
[item-get]: ../api/driveitem-get.md
[item-changes]: ../api/driveitem-delta.md
[item-search]: ../api/driveitem-search.md
[item-children]: ../api/driveitem-list-children.md


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
