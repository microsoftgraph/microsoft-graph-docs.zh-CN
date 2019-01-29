---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 驱动器
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: e788765c3405a1455eda55f6fefdc21ade3da8fd
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573926"
---
# <a name="drive-resource-type"></a><span data-ttu-id="c327a-102">驱动器资源类型</span><span class="sxs-lookup"><span data-stu-id="c327a-102">Drive resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c327a-103">驱动器资源是表示用户的 OneDrive 或 SharePoint 中文档库的顶级对象。</span><span class="sxs-lookup"><span data-stu-id="c327a-103">The drive resource is the top level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="c327a-p101">OneDrive 用户必须始终具有至少一个可用驱动器，即默认驱动器。没有 OneDrive 许可证的用户不能拥有可用的默认驱动器。</span><span class="sxs-lookup"><span data-stu-id="c327a-p101">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c327a-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c327a-106">JSON representation</span></span>

<span data-ttu-id="c327a-107">下面是 Drive 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c327a-107">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="c327a-108">**drive** 资源派生自 [**baseItem**](baseitem.md) 并继承该资源的属性。</span><span class="sxs-lookup"><span data-stu-id="c327a-108">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="c327a-109">属性</span><span class="sxs-lookup"><span data-stu-id="c327a-109">Properties</span></span>

| <span data-ttu-id="c327a-110">属性</span><span class="sxs-lookup"><span data-stu-id="c327a-110">Property</span></span>             | <span data-ttu-id="c327a-111">类型</span><span class="sxs-lookup"><span data-stu-id="c327a-111">Type</span></span>                          | <span data-ttu-id="c327a-112">说明</span><span class="sxs-lookup"><span data-stu-id="c327a-112">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="c327a-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="c327a-113">createdBy</span></span>            | <span data-ttu-id="c327a-114">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="c327a-114">[identitySet][]</span></span>               | <span data-ttu-id="c327a-p102">识别创建项目的用户、设备或应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="c327a-p102">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="c327a-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c327a-117">createdDateTime</span></span>      | <span data-ttu-id="c327a-118">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c327a-118">dateTimeOffset</span></span>                | <span data-ttu-id="c327a-p103">创建项的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="c327a-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="c327a-121">description</span><span class="sxs-lookup"><span data-stu-id="c327a-121">description</span></span>          | <span data-ttu-id="c327a-122">String</span><span class="sxs-lookup"><span data-stu-id="c327a-122">String</span></span>                        | <span data-ttu-id="c327a-123">提供驱动器的用户可见说明。</span><span class="sxs-lookup"><span data-stu-id="c327a-123">Provide a user-visible description of the drive.</span></span> <span data-ttu-id="c327a-124">读写。</span><span class="sxs-lookup"><span data-stu-id="c327a-124">Read-write.</span></span>
| <span data-ttu-id="c327a-125">driveType</span><span class="sxs-lookup"><span data-stu-id="c327a-125">driveType</span></span>            | <span data-ttu-id="c327a-126">String</span><span class="sxs-lookup"><span data-stu-id="c327a-126">String</span></span>                        | <span data-ttu-id="c327a-p105">说明了由该资源表示的驱动器的类型。OneDrive 个人版驱动器将返回 `personal`。OneDrive for Business 将返回 `business`。SharePoint 文档库将返回 `documentLibrary`。只读。</span><span class="sxs-lookup"><span data-stu-id="c327a-p105">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="c327a-132">id</span><span class="sxs-lookup"><span data-stu-id="c327a-132">id</span></span>                   | <span data-ttu-id="c327a-133">String</span><span class="sxs-lookup"><span data-stu-id="c327a-133">String</span></span>                        | <span data-ttu-id="c327a-p106">驱动器唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="c327a-p106">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="c327a-136">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="c327a-136">lastModifiedBy</span></span>       | <span data-ttu-id="c327a-137">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="c327a-137">[identitySet][]</span></span>               | <span data-ttu-id="c327a-p107">上次修改项目的用户、设备和应用程序的标识。只读。</span><span class="sxs-lookup"><span data-stu-id="c327a-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="c327a-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c327a-140">lastModifiedDateTime</span></span> | <span data-ttu-id="c327a-141">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c327a-141">dateTimeOffset</span></span>                | <span data-ttu-id="c327a-p108">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="c327a-p108">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="c327a-144">name</span><span class="sxs-lookup"><span data-stu-id="c327a-144">name</span></span>                 | <span data-ttu-id="c327a-145">string</span><span class="sxs-lookup"><span data-stu-id="c327a-145">string</span></span>                        | <span data-ttu-id="c327a-p109">项目名称。读写。</span><span class="sxs-lookup"><span data-stu-id="c327a-p109">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="c327a-148">所有者</span><span class="sxs-lookup"><span data-stu-id="c327a-148">owner</span></span>                | [<span data-ttu-id="c327a-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="c327a-149">identitySet</span></span>](identityset.md) | <span data-ttu-id="c327a-p110">可选。拥有此驱动器的用户帐户。只读。</span><span class="sxs-lookup"><span data-stu-id="c327a-p110">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="c327a-153">配额</span><span class="sxs-lookup"><span data-stu-id="c327a-153">quota</span></span>                | [<span data-ttu-id="c327a-154">配额</span><span class="sxs-lookup"><span data-stu-id="c327a-154">quota</span></span>](quota.md)             | <span data-ttu-id="c327a-p111">可选。有关驱动器的存储空间配额的信息。只读。</span><span class="sxs-lookup"><span data-stu-id="c327a-p111">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="c327a-158">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="c327a-158">sharepointIds</span></span>        | <span data-ttu-id="c327a-159">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="c327a-159">[sharepointIds][]</span></span>             | <span data-ttu-id="c327a-p112">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="c327a-p112">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="c327a-162">system</span><span class="sxs-lookup"><span data-stu-id="c327a-162">system</span></span>               | <span data-ttu-id="c327a-163">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="c327a-163">[systemFacet][]</span></span>               | <span data-ttu-id="c327a-164">如果存在，则表示这是系统管理的驱动器。</span><span class="sxs-lookup"><span data-stu-id="c327a-164">If present, indicates that this is a system-managed drive.</span></span> <span data-ttu-id="c327a-165">只读。</span><span class="sxs-lookup"><span data-stu-id="c327a-165">Read-only.</span></span>
| <span data-ttu-id="c327a-166">WebUrl</span><span class="sxs-lookup"><span data-stu-id="c327a-166">webUrl</span></span>               | <span data-ttu-id="c327a-167">string (url)</span><span class="sxs-lookup"><span data-stu-id="c327a-167">string (url)</span></span>                  | <span data-ttu-id="c327a-p114">在浏览器中显示此资源的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="c327a-p114">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a><span data-ttu-id="c327a-173">关系</span><span class="sxs-lookup"><span data-stu-id="c327a-173">Relationships</span></span>

| <span data-ttu-id="c327a-174">关系</span><span class="sxs-lookup"><span data-stu-id="c327a-174">Relationship</span></span> | <span data-ttu-id="c327a-175">类型</span><span class="sxs-lookup"><span data-stu-id="c327a-175">Type</span></span>                                 | <span data-ttu-id="c327a-176">说明</span><span class="sxs-lookup"><span data-stu-id="c327a-176">Description</span></span>
|:-------------|:-------------------------------------|:-----------------------
| <span data-ttu-id="c327a-177">activities</span><span class="sxs-lookup"><span data-stu-id="c327a-177">activities</span></span>   | <span data-ttu-id="c327a-178">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="c327a-178">[itemActivity][] collection</span></span>          | <span data-ttu-id="c327a-179">最近发生在此驱动器下的活动的列表。</span><span class="sxs-lookup"><span data-stu-id="c327a-179">The list of recent activities that took place under this drive.</span></span>
| <span data-ttu-id="c327a-180">items</span><span class="sxs-lookup"><span data-stu-id="c327a-180">items</span></span>        | <span data-ttu-id="c327a-181">[driveItem](driveitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c327a-181">[driveItem](driveitem.md) collection</span></span> | <span data-ttu-id="c327a-p115">驱动器中包含的所有项。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="c327a-p115">All items contained in the drive. Read-only. Nullable.</span></span>
| <span data-ttu-id="c327a-185">root</span><span class="sxs-lookup"><span data-stu-id="c327a-185">root</span></span>         | [<span data-ttu-id="c327a-186">driveItem</span><span class="sxs-lookup"><span data-stu-id="c327a-186">driveItem</span></span>](driveitem.md)            | <span data-ttu-id="c327a-p116">驱动器的根文件夹。只读。</span><span class="sxs-lookup"><span data-stu-id="c327a-p116">The root folder of the drive. Read-only.</span></span>
| <span data-ttu-id="c327a-189">special</span><span class="sxs-lookup"><span data-stu-id="c327a-189">special</span></span>      | <span data-ttu-id="c327a-190">[driveItem](driveitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c327a-190">[driveItem](driveitem.md) collection</span></span> | <span data-ttu-id="c327a-p117">OneDrive 中可用的公用文件夹的集合。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="c327a-p117">Collection of common folders available in OneDrive. Read-only. Nullable.</span></span>
| <span data-ttu-id="c327a-194">following</span><span class="sxs-lookup"><span data-stu-id="c327a-194">" following</span></span>    | <span data-ttu-id="c327a-195">[driveItem](driveitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c327a-195">[driveItem](driveitem.md) collection</span></span> | <span data-ttu-id="c327a-196">用户关注的项列表。</span><span class="sxs-lookup"><span data-stu-id="c327a-196">The list of items the user is following.</span></span> <span data-ttu-id="c327a-197">仅适用于 OneDrive for Business 中。</span><span class="sxs-lookup"><span data-stu-id="c327a-197">Only in OneDrive for Business.</span></span>

## <a name="methods"></a><span data-ttu-id="c327a-198">方法</span><span class="sxs-lookup"><span data-stu-id="c327a-198">Methods</span></span>

|                        <span data-ttu-id="c327a-199">常见任务</span><span class="sxs-lookup"><span data-stu-id="c327a-199">Common task</span></span>                         |         <span data-ttu-id="c327a-200">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="c327a-200">HTTP method</span></span>         |
| :--------------------------------------------------------- | :-------------------------- |
| <span data-ttu-id="c327a-201">[获取其他驱动器的驱动器元数据][drive-get]</span><span class="sxs-lookup"><span data-stu-id="c327a-201">[Get Drive metadata of another Drive][drive-get]</span></span>           | `GET /drives/{drive-id}`    |
| <span data-ttu-id="c327a-202">[获取用户默认驱动器的根文件夹][item-get]</span><span class="sxs-lookup"><span data-stu-id="c327a-202">[Get root folder for user's default Drive][item-get]</span></span>       | `GET /drive/root`           |
| <span data-ttu-id="c327a-203">[列出驱动器下的活动][drive-activities]</span><span class="sxs-lookup"><span data-stu-id="c327a-203">[List activities under the Drive][drive-activities]</span></span>        | `GET /drive/activities`     |
| <span data-ttu-id="c327a-204">[列出关注的项][drive-following]</span><span class="sxs-lookup"><span data-stu-id="c327a-204">[List followed Items][drive-following]</span></span>                     | `GET /drive/following`      |
| <span data-ttu-id="c327a-205">[列出驱动器下的子项][item-children]</span><span class="sxs-lookup"><span data-stu-id="c327a-205">[List children under the Drive][item-children]</span></span>             | `GET /drive/root/children`  |
| <span data-ttu-id="c327a-206">[列出驱动器中所有项的变更][item-changes]</span><span class="sxs-lookup"><span data-stu-id="c327a-206">[List changes for all Items in the Drive][item-changes]</span></span>    | `GET /drive/root/delta`     |
| <span data-ttu-id="c327a-207">[搜索驱动器中的项][item-search]</span><span class="sxs-lookup"><span data-stu-id="c327a-207">[Search for Items in the Drive][item-search]</span></span>               | `GET /drive/root/search`    |
| [<span data-ttu-id="c327a-208">访问特殊文件夹</span><span class="sxs-lookup"><span data-stu-id="c327a-208">Access special folder</span></span>](../api/drive-get-specialfolder.md) | `GET /drive/special/{name}` |

<span data-ttu-id="c327a-209">在上表中，各示例使用的是 `/drive`，但其他路径也同样有效。</span><span class="sxs-lookup"><span data-stu-id="c327a-209">In the previous table, the examples use `/drive`, but other pathes are valid too.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Drive is a top level object for OneDrive API that provides access to the contents of a drive. ",
  "keywords": "drive,objects,resources",
  "section": "documentation",
  "tocPath": "Drives",
  "tocBookmarks": {
    "Resources/Drive": "#"
  },
  "suppressions": [
    "Error: /api-reference/beta/resources/drive.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
