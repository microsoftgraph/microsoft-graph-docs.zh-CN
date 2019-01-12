---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Drive
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 581a611fa077eab6d44db01d998d5ea42886f052
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938186"
---
# <a name="drive-resource-type"></a><span data-ttu-id="348e5-102">驱动器资源类型</span><span class="sxs-lookup"><span data-stu-id="348e5-102">drive resource type</span></span>

> <span data-ttu-id="348e5-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="348e5-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="348e5-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="348e5-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="348e5-105">驱动器资源是表示用户的 OneDrive 或 SharePoint 中文档库的顶级对象。</span><span class="sxs-lookup"><span data-stu-id="348e5-105">The drive resource is the top level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="348e5-p102">OneDrive 用户必须始终具有至少一个可用驱动器，即默认驱动器。没有 OneDrive 许可证的用户不能拥有可用的默认驱动器。</span><span class="sxs-lookup"><span data-stu-id="348e5-p102">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="json-representation"></a><span data-ttu-id="348e5-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="348e5-108">JSON representation</span></span>

<span data-ttu-id="348e5-109">下面是 Drive 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="348e5-109">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="348e5-110">**drive** 资源由 [**baseItem**](baseitem.md) 派生并继承该资源的属性。</span><span class="sxs-lookup"><span data-stu-id="348e5-110">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
    "special",
    "system"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.drive"
}-->

```json
{
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "id": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "string (timestamp)",
  "description": "string",
  "driveType": "personal | business | documentLibrary",
  "following": [ { "@odata.type": "microsoft.graph.driveItem" } ],
  "items": [ { "@odata.type": "microsoft.graph.driveItem" } ],
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "string (timestamp)",
  "name": "string",
  "owner": { "@odata.type": "microsoft.graph.identitySet" },
  "quota": { "@odata.type": "microsoft.graph.quota" },
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "special": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "system": { "@odata.type": "microsoft.graph.systemFacet" },
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="348e5-111">属性</span><span class="sxs-lookup"><span data-stu-id="348e5-111">Properties</span></span>

| <span data-ttu-id="348e5-112">属性</span><span class="sxs-lookup"><span data-stu-id="348e5-112">Property</span></span>             | <span data-ttu-id="348e5-113">类型</span><span class="sxs-lookup"><span data-stu-id="348e5-113">Type</span></span>                          | <span data-ttu-id="348e5-114">说明</span><span class="sxs-lookup"><span data-stu-id="348e5-114">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="348e5-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="348e5-115">createdBy</span></span>            | <span data-ttu-id="348e5-116">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="348e5-116">[identitySet][]</span></span>               | <span data-ttu-id="348e5-p103">识别创建项目的用户、设备或应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="348e5-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="348e5-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="348e5-119">createdDateTime</span></span>      | <span data-ttu-id="348e5-120">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="348e5-120">dateTimeOffset</span></span>                | <span data-ttu-id="348e5-p104">创建项的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="348e5-p104">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="348e5-123">说明</span><span class="sxs-lookup"><span data-stu-id="348e5-123">description</span></span>          | <span data-ttu-id="348e5-124">字符串</span><span class="sxs-lookup"><span data-stu-id="348e5-124">String</span></span>                        | <span data-ttu-id="348e5-125">提供驱动器的用户可见说明。</span><span class="sxs-lookup"><span data-stu-id="348e5-125">Provide a user-visible description of the drive.</span></span> <span data-ttu-id="348e5-126">读写。</span><span class="sxs-lookup"><span data-stu-id="348e5-126">Read-write.</span></span>
| <span data-ttu-id="348e5-127">driveType</span><span class="sxs-lookup"><span data-stu-id="348e5-127">driveType</span></span>            | <span data-ttu-id="348e5-128">String</span><span class="sxs-lookup"><span data-stu-id="348e5-128">String</span></span>                        | <span data-ttu-id="348e5-p106">说明了由该资源表示的驱动器的类型。OneDrive 个人版驱动器将返回 `personal`。OneDrive for Business 将返回 `business`。SharePoint 文档库将返回 `documentLibrary`。只读。</span><span class="sxs-lookup"><span data-stu-id="348e5-p106">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="348e5-134">id</span><span class="sxs-lookup"><span data-stu-id="348e5-134">id</span></span>                   | <span data-ttu-id="348e5-135">String</span><span class="sxs-lookup"><span data-stu-id="348e5-135">String</span></span>                        | <span data-ttu-id="348e5-p107">驱动器唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="348e5-p107">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="348e5-138">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="348e5-138">lastModifiedBy</span></span>       | <span data-ttu-id="348e5-139">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="348e5-139">[identitySet][]</span></span>               | <span data-ttu-id="348e5-p108">上次修改项目的用户、设备和应用程序的标识。只读。</span><span class="sxs-lookup"><span data-stu-id="348e5-p108">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="348e5-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="348e5-142">lastModifiedDateTime</span></span> | <span data-ttu-id="348e5-143">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="348e5-143">dateTimeOffset</span></span>                | <span data-ttu-id="348e5-p109">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="348e5-p109">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="348e5-146">name</span><span class="sxs-lookup"><span data-stu-id="348e5-146">name</span></span>                 | <span data-ttu-id="348e5-147">string</span><span class="sxs-lookup"><span data-stu-id="348e5-147">string</span></span>                        | <span data-ttu-id="348e5-p110">项目名称。读写。</span><span class="sxs-lookup"><span data-stu-id="348e5-p110">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="348e5-150">所有者</span><span class="sxs-lookup"><span data-stu-id="348e5-150">owner</span></span>                | [<span data-ttu-id="348e5-151">identitySet</span><span class="sxs-lookup"><span data-stu-id="348e5-151">identitySet</span></span>](identityset.md) | <span data-ttu-id="348e5-p111">可选。拥有此驱动器的用户帐户。只读。</span><span class="sxs-lookup"><span data-stu-id="348e5-p111">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="348e5-155">配额</span><span class="sxs-lookup"><span data-stu-id="348e5-155">quota</span></span>                | [<span data-ttu-id="348e5-156">配额</span><span class="sxs-lookup"><span data-stu-id="348e5-156">quota</span></span>](quota.md)             | <span data-ttu-id="348e5-p112">可选。有关驱动器的存储空间配额的信息。只读。</span><span class="sxs-lookup"><span data-stu-id="348e5-p112">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="348e5-160">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="348e5-160">sharepointIds</span></span>        | <span data-ttu-id="348e5-161">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="348e5-161">[sharepointIds][]</span></span>             | <span data-ttu-id="348e5-p113">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="348e5-p113">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="348e5-164">system</span><span class="sxs-lookup"><span data-stu-id="348e5-164">system</span></span>               | <span data-ttu-id="348e5-165">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="348e5-165">[systemFacet][]</span></span>               | <span data-ttu-id="348e5-166">如果存在，则表示这是系统管理的驱动器。</span><span class="sxs-lookup"><span data-stu-id="348e5-166">If present, indicates that this is a system-managed drive.</span></span> <span data-ttu-id="348e5-167">只读。</span><span class="sxs-lookup"><span data-stu-id="348e5-167">Read-only.</span></span>
| <span data-ttu-id="348e5-168">WebUrl</span><span class="sxs-lookup"><span data-stu-id="348e5-168">webUrl</span></span>               | <span data-ttu-id="348e5-169">string (url)</span><span class="sxs-lookup"><span data-stu-id="348e5-169">string (url)</span></span>                  | <span data-ttu-id="348e5-p115">在浏览器中显示此资源的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="348e5-p115">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a><span data-ttu-id="348e5-175">关系</span><span class="sxs-lookup"><span data-stu-id="348e5-175">Relationships</span></span>

| <span data-ttu-id="348e5-176">关系</span><span class="sxs-lookup"><span data-stu-id="348e5-176">Relationship</span></span> | <span data-ttu-id="348e5-177">类型</span><span class="sxs-lookup"><span data-stu-id="348e5-177">Type</span></span>                                 | <span data-ttu-id="348e5-178">说明</span><span class="sxs-lookup"><span data-stu-id="348e5-178">Description</span></span>
|:-------------|:-------------------------------------|:-----------------------
| <span data-ttu-id="348e5-179">activities</span><span class="sxs-lookup"><span data-stu-id="348e5-179">activities</span></span>   | <span data-ttu-id="348e5-180">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="348e5-180">[itemActivity][] collection</span></span>          | <span data-ttu-id="348e5-181">最近发生在此驱动器下的活动的列表。</span><span class="sxs-lookup"><span data-stu-id="348e5-181">The list of recent activities that took place under this drive.</span></span>
| <span data-ttu-id="348e5-182">项目</span><span class="sxs-lookup"><span data-stu-id="348e5-182">items</span></span>        | <span data-ttu-id="348e5-183">[driveitem](driveitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="348e5-183">[driveitem](driveitem.md) collection</span></span> | <span data-ttu-id="348e5-p116">驱动器中包含的所有项。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="348e5-p116">All items contained in the drive. Read-only. Nullable.</span></span>
| <span data-ttu-id="348e5-187">root</span><span class="sxs-lookup"><span data-stu-id="348e5-187">root</span></span>         | [<span data-ttu-id="348e5-188">driveitem</span><span class="sxs-lookup"><span data-stu-id="348e5-188">driveitem</span></span>](driveitem.md)            | <span data-ttu-id="348e5-p117">驱动器的根文件夹。只读。</span><span class="sxs-lookup"><span data-stu-id="348e5-p117">The root folder of the drive. Read-only.</span></span>
| <span data-ttu-id="348e5-191">special</span><span class="sxs-lookup"><span data-stu-id="348e5-191">special</span></span>      | <span data-ttu-id="348e5-192">[driveitem](driveitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="348e5-192">[driveitem](driveitem.md) collection</span></span> | <span data-ttu-id="348e5-p118">OneDrive 中可用的公用文件夹的集合。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="348e5-p118">Collection of common folders available in OneDrive. Read-only. Nullable.</span></span>
| <span data-ttu-id="348e5-196">以下</span><span class="sxs-lookup"><span data-stu-id="348e5-196">following</span></span>    | <span data-ttu-id="348e5-197">[DriveItem](driveitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="348e5-197">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="348e5-198">用户正在关注的项的列表。</span><span class="sxs-lookup"><span data-stu-id="348e5-198">The list of items the user is following.</span></span> <span data-ttu-id="348e5-199">仅在 OneDrive for Business。</span><span class="sxs-lookup"><span data-stu-id="348e5-199">Only in OneDrive for Business.</span></span>

## <a name="methods"></a><span data-ttu-id="348e5-200">方法</span><span class="sxs-lookup"><span data-stu-id="348e5-200">Methods</span></span>

|                        <span data-ttu-id="348e5-201">常见任务</span><span class="sxs-lookup"><span data-stu-id="348e5-201">Common task</span></span>                         |         <span data-ttu-id="348e5-202">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="348e5-202">HTTP method</span></span>         |
| :--------------------------------------------------------- | :-------------------------- |
| <span data-ttu-id="348e5-203">[获取其他驱动器的驱动器元数据][drive-get]</span><span class="sxs-lookup"><span data-stu-id="348e5-203">[Get Drive metadata of another Drive][drive-get]</span></span>           | `GET /drives/{drive-id}`    |
| <span data-ttu-id="348e5-204">[获取用户默认驱动器的根文件夹][item-get]</span><span class="sxs-lookup"><span data-stu-id="348e5-204">[Get root folder for user's default Drive][item-get]</span></span>       | `GET /drive/root`           |
| <span data-ttu-id="348e5-205">[列出驱动器下的活动][drive-activities]</span><span class="sxs-lookup"><span data-stu-id="348e5-205">[List activities under the Drive][drive-activities]</span></span>        | `GET /drive/activities`     |
| <span data-ttu-id="348e5-206">[列表后面的项目][drive-following]</span><span class="sxs-lookup"><span data-stu-id="348e5-206">[List followed Items][drive-following]</span></span>                     | `GET /drive/following`      |
| <span data-ttu-id="348e5-207">[列出驱动器下的子项][item-children]</span><span class="sxs-lookup"><span data-stu-id="348e5-207">[List children under the Drive][item-children]</span></span>             | `GET /drive/root/children`  |
| <span data-ttu-id="348e5-208">[列出驱动器中所有项的变更][item-changes]</span><span class="sxs-lookup"><span data-stu-id="348e5-208">[List changes for all Items in the Drive][item-changes]</span></span>    | `GET /drive/root/delta`     |
| <span data-ttu-id="348e5-209">[搜索驱动器中的项][item-search]</span><span class="sxs-lookup"><span data-stu-id="348e5-209">[Search for Items in the Drive][item-search]</span></span>               | `GET /drive/root/search`    |
| [<span data-ttu-id="348e5-210">访问特殊文件夹</span><span class="sxs-lookup"><span data-stu-id="348e5-210">Access special folder</span></span>](../api/drive-get-specialfolder.md) | `GET /drive/special/{name}` |

<span data-ttu-id="348e5-211">上表中，在此示例使用`/drive`，但其他路径太是否有效。</span><span class="sxs-lookup"><span data-stu-id="348e5-211">In the previous table, the examples use `/drive`, but other paths are valid too.</span></span>

[itemActivity]: itemactivity.md
[item-resource]: driveitem.md
[identity-set]: identityset.md
[quota-facet]: quota.md
[drive-resource]: drive.md
[drive-activities]: ../api/activities-list.md
[drive-following]: ../api/drive-list-following.md
[drive-get]: ../api/drive-get.md
[item-get]: ../api/driveitem-get.md
[item-changes]: ../api/driveitem-delta.md
[item-search]: ../api/driveitem-search.md
[item-children]: ../api/driveitem-list-children.md


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Drive is a top level object for OneDrive API that provides access to the contents of a drive. ",
  "keywords": "drive,objects,resources",
  "section": "documentation",
  "tocPath": "Drives",
  "tocBookmarks": { "Resources/Drive": "#" }
} -->
