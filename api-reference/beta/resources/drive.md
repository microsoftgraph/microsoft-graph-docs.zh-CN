---
author: JeremyKelley
ms.author: JeremyKelley
title: 驱动器资源类型
description: 表示用户的 OneDrive 或 SharePoint 中文档库的驱动器资源。
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: f47bacdac64a535ba3d7ff695d1aa0c1c46b06b8
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932005"
---
# <a name="drive-resource-type"></a><span data-ttu-id="804ca-103">驱动器资源类型</span><span class="sxs-lookup"><span data-stu-id="804ca-103">drive resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="804ca-104">驱动器资源是表示用户的 OneDrive 或 SharePoint 中文档库的顶级对象。</span><span class="sxs-lookup"><span data-stu-id="804ca-104">The drive resource is the top level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="804ca-p101">OneDrive 用户必须始终具有至少一个可用驱动器，即默认驱动器。没有 OneDrive 许可证的用户不能拥有可用的默认驱动器。</span><span class="sxs-lookup"><span data-stu-id="804ca-p101">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="methods"></a><span data-ttu-id="804ca-107">方法</span><span class="sxs-lookup"><span data-stu-id="804ca-107">Methods</span></span>

|                        <span data-ttu-id="804ca-108">方法</span><span class="sxs-lookup"><span data-stu-id="804ca-108">Method</span></span>                              |         <span data-ttu-id="804ca-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="804ca-109">Return type</span></span>         | <span data-ttu-id="804ca-110">说明</span><span class="sxs-lookup"><span data-stu-id="804ca-110">Description</span></span> |
| :--------------------------------------------------------- | :-------------------------- |-------------|
| <span data-ttu-id="804ca-111">[获取驱动器][drive-get]</span><span class="sxs-lookup"><span data-stu-id="804ca-111">[Get drive][drive-get]</span></span>                                     | <span data-ttu-id="804ca-112">驱动器</span><span class="sxs-lookup"><span data-stu-id="804ca-112">drive</span></span>                       | <span data-ttu-id="804ca-113">获取有关驱动器的元数据</span><span class="sxs-lookup"><span data-stu-id="804ca-113">Get metadata about a user's default drive on OneDrive.</span></span> |
| <span data-ttu-id="804ca-114">[获取驱动器根][item-get]</span><span class="sxs-lookup"><span data-stu-id="804ca-114">[Get drive root][item-get]</span></span>                                 | <span data-ttu-id="804ca-115">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="804ca-115">[driveItem][]</span></span>               | <span data-ttu-id="804ca-116">获取驱动器的根文件夹</span><span class="sxs-lookup"><span data-stu-id="804ca-116">Get root folder for a drive</span></span> |
| <span data-ttu-id="804ca-117">[列出活动][drive-activities]</span><span class="sxs-lookup"><span data-stu-id="804ca-117">[List activities][drive-activities]</span></span>                        | <span data-ttu-id="804ca-118">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="804ca-118">[itemActivity][] collection</span></span> | <span data-ttu-id="804ca-119">列出在驱动器下发生的活动</span><span class="sxs-lookup"><span data-stu-id="804ca-119">List activities that occurred under the drive</span></span> |
| <span data-ttu-id="804ca-120">[列出关注的项][drive-following]</span><span class="sxs-lookup"><span data-stu-id="804ca-120">[List followed Items][drive-following]</span></span>                     | <span data-ttu-id="804ca-121">[driveItem][] 集合</span><span class="sxs-lookup"><span data-stu-id="804ca-121">[driveItem][] collection</span></span>    | <span data-ttu-id="804ca-122">列出用户的关注 driveItems</span><span class="sxs-lookup"><span data-stu-id="804ca-122">List the user's followed driveItems</span></span> |
| <span data-ttu-id="804ca-123">[列出子项][item-children]</span><span class="sxs-lookup"><span data-stu-id="804ca-123">[List children][item-children]</span></span>                             | <span data-ttu-id="804ca-124">[driveItem][] 集合</span><span class="sxs-lookup"><span data-stu-id="804ca-124">[driveItem][] collection</span></span>    | <span data-ttu-id="804ca-125">列出驱动器根文件夹的子项</span><span class="sxs-lookup"><span data-stu-id="804ca-125">List children of the root folder of a drive</span></span> |
| <span data-ttu-id="804ca-126">[列出变更][item-changes]</span><span class="sxs-lookup"><span data-stu-id="804ca-126">[List changes][item-changes]</span></span>                               | <span data-ttu-id="804ca-127">[driveItem][] 集合</span><span class="sxs-lookup"><span data-stu-id="804ca-127">[driveItem][] collection</span></span>    | <span data-ttu-id="804ca-128">列出驱动器中所有 DriveItem 的变更</span><span class="sxs-lookup"><span data-stu-id="804ca-128">List changes for all Items in the Drive</span></span> |
| <span data-ttu-id="804ca-129">[搜索][item-search]</span><span class="sxs-lookup"><span data-stu-id="804ca-129">[Search][item-search]</span></span>                                      | <span data-ttu-id="804ca-130">[driveItem][] 集合</span><span class="sxs-lookup"><span data-stu-id="804ca-130">[driveItem][] collection</span></span>    | <span data-ttu-id="804ca-131">搜索驱动器中的 DriveItem</span><span class="sxs-lookup"><span data-stu-id="804ca-131">Search for driveItems in a drive</span></span> |
| [<span data-ttu-id="804ca-132">获取特殊文件夹</span><span class="sxs-lookup"><span data-stu-id="804ca-132">Get special folder</span></span>](../api/drive-get-specialfolder.md)    | <span data-ttu-id="804ca-133">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="804ca-133">[driveItem][]</span></span>               | <span data-ttu-id="804ca-134">通过特殊文件夹的规范名称访问它</span><span class="sxs-lookup"><span data-stu-id="804ca-134">Access a special (named) folder in the user's OneDrive by its known name.</span></span> |


## <a name="properties"></a><span data-ttu-id="804ca-135">属性</span><span class="sxs-lookup"><span data-stu-id="804ca-135">Properties</span></span>

| <span data-ttu-id="804ca-136">属性</span><span class="sxs-lookup"><span data-stu-id="804ca-136">Property</span></span>             | <span data-ttu-id="804ca-137">类型</span><span class="sxs-lookup"><span data-stu-id="804ca-137">Type</span></span>                          | <span data-ttu-id="804ca-138">说明</span><span class="sxs-lookup"><span data-stu-id="804ca-138">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="804ca-139">createdBy</span><span class="sxs-lookup"><span data-stu-id="804ca-139">createdBy</span></span>            | <span data-ttu-id="804ca-140">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="804ca-140">[identitySet][]</span></span>               | <span data-ttu-id="804ca-p102">识别创建项目的用户、设备或应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="804ca-p102">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="804ca-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="804ca-143">createdDateTime</span></span>      | <span data-ttu-id="804ca-144">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="804ca-144">dateTimeOffset</span></span>                | <span data-ttu-id="804ca-p103">创建项的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="804ca-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="804ca-147">description</span><span class="sxs-lookup"><span data-stu-id="804ca-147">description</span></span>          | <span data-ttu-id="804ca-148">String</span><span class="sxs-lookup"><span data-stu-id="804ca-148">String</span></span>                        | <span data-ttu-id="804ca-149">提供驱动器的用户可见说明。</span><span class="sxs-lookup"><span data-stu-id="804ca-149">Provide a user-visible description of the drive.</span></span> <span data-ttu-id="804ca-150">读写。</span><span class="sxs-lookup"><span data-stu-id="804ca-150">Read-write.</span></span>
| <span data-ttu-id="804ca-151">driveType</span><span class="sxs-lookup"><span data-stu-id="804ca-151">driveType</span></span>            | <span data-ttu-id="804ca-152">String</span><span class="sxs-lookup"><span data-stu-id="804ca-152">String</span></span>                        | <span data-ttu-id="804ca-p105">说明了由该资源表示的驱动器的类型。OneDrive 个人版驱动器将返回 `personal`。OneDrive for Business 将返回 `business`。SharePoint 文档库将返回 `documentLibrary`。只读。</span><span class="sxs-lookup"><span data-stu-id="804ca-p105">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="804ca-158">id</span><span class="sxs-lookup"><span data-stu-id="804ca-158">id</span></span>                   | <span data-ttu-id="804ca-159">String</span><span class="sxs-lookup"><span data-stu-id="804ca-159">String</span></span>                        | <span data-ttu-id="804ca-p106">驱动器唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="804ca-p106">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="804ca-162">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="804ca-162">lastModifiedBy</span></span>       | <span data-ttu-id="804ca-163">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="804ca-163">[identitySet][]</span></span>               | <span data-ttu-id="804ca-p107">上次修改项目的用户、设备和应用程序的标识。只读。</span><span class="sxs-lookup"><span data-stu-id="804ca-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="804ca-166">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="804ca-166">lastModifiedDateTime</span></span> | <span data-ttu-id="804ca-167">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="804ca-167">dateTimeOffset</span></span>                | <span data-ttu-id="804ca-p108">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="804ca-p108">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="804ca-170">name</span><span class="sxs-lookup"><span data-stu-id="804ca-170">name</span></span>                 | <span data-ttu-id="804ca-171">string</span><span class="sxs-lookup"><span data-stu-id="804ca-171">string</span></span>                        | <span data-ttu-id="804ca-p109">项目名称。读写。</span><span class="sxs-lookup"><span data-stu-id="804ca-p109">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="804ca-174">所有者</span><span class="sxs-lookup"><span data-stu-id="804ca-174">owner</span></span>                | [<span data-ttu-id="804ca-175">identitySet</span><span class="sxs-lookup"><span data-stu-id="804ca-175">identitySet</span></span>](identityset.md) | <span data-ttu-id="804ca-p110">可选。拥有此驱动器的用户帐户。只读。</span><span class="sxs-lookup"><span data-stu-id="804ca-p110">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="804ca-179">配额</span><span class="sxs-lookup"><span data-stu-id="804ca-179">quota</span></span>                | [<span data-ttu-id="804ca-180">配额</span><span class="sxs-lookup"><span data-stu-id="804ca-180">quota</span></span>](quota.md)             | <span data-ttu-id="804ca-p111">可选。有关驱动器的存储空间配额的信息。只读。</span><span class="sxs-lookup"><span data-stu-id="804ca-p111">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="804ca-184">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="804ca-184">sharepointIds</span></span>        | <span data-ttu-id="804ca-185">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="804ca-185">[sharepointIds][]</span></span>             | <span data-ttu-id="804ca-p112">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="804ca-p112">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="804ca-188">system</span><span class="sxs-lookup"><span data-stu-id="804ca-188">system</span></span>               | <span data-ttu-id="804ca-189">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="804ca-189">[systemFacet][]</span></span>               | <span data-ttu-id="804ca-190">如果存在，则表示这是系统管理的驱动器。</span><span class="sxs-lookup"><span data-stu-id="804ca-190">If present, indicates that this is a system-managed drive.</span></span> <span data-ttu-id="804ca-191">只读。</span><span class="sxs-lookup"><span data-stu-id="804ca-191">Read-only.</span></span>
| <span data-ttu-id="804ca-192">WebUrl</span><span class="sxs-lookup"><span data-stu-id="804ca-192">webUrl</span></span>               | <span data-ttu-id="804ca-193">string (url)</span><span class="sxs-lookup"><span data-stu-id="804ca-193">string (url)</span></span>                  | <span data-ttu-id="804ca-p114">在浏览器中显示此资源的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="804ca-p114">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a><span data-ttu-id="804ca-199">关系</span><span class="sxs-lookup"><span data-stu-id="804ca-199">Relationships</span></span>

| <span data-ttu-id="804ca-200">关系</span><span class="sxs-lookup"><span data-stu-id="804ca-200">Relationship</span></span> | <span data-ttu-id="804ca-201">类型</span><span class="sxs-lookup"><span data-stu-id="804ca-201">Type</span></span>                                 | <span data-ttu-id="804ca-202">说明</span><span class="sxs-lookup"><span data-stu-id="804ca-202">Description</span></span>
|:-------------|:-------------------------------------|:-----------------------
| <span data-ttu-id="804ca-203">activities</span><span class="sxs-lookup"><span data-stu-id="804ca-203">activities</span></span>   | <span data-ttu-id="804ca-204">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="804ca-204">[itemActivity][] collection</span></span>          | <span data-ttu-id="804ca-205">最近发生在此驱动器下的活动的列表。</span><span class="sxs-lookup"><span data-stu-id="804ca-205">The list of recent activities that took place under this drive.</span></span>
| <span data-ttu-id="804ca-206">捆绑</span><span class="sxs-lookup"><span data-stu-id="804ca-206">Multiple bundles</span></span>      | <span data-ttu-id="804ca-207">[driveItem][] 集合</span><span class="sxs-lookup"><span data-stu-id="804ca-207">[driveItem][] collection</span></span>             | <span data-ttu-id="804ca-208">[捆绑][bundle] (相册和多选共享项目集) 的集合。</span><span class="sxs-lookup"><span data-stu-id="804ca-208">Collection of [bundles][bundle] (albums and multi-select-shared sets of items).</span></span> <span data-ttu-id="804ca-209">只在个人的 OneDrive 中。</span><span class="sxs-lookup"><span data-stu-id="804ca-209">Only in personal OneDrive.</span></span>
| <span data-ttu-id="804ca-210">following</span><span class="sxs-lookup"><span data-stu-id="804ca-210">following</span></span>    | <span data-ttu-id="804ca-211">[driveItem][] 集合</span><span class="sxs-lookup"><span data-stu-id="804ca-211">[driveItem][] collection</span></span>             | <span data-ttu-id="804ca-212">用户关注的项列表。</span><span class="sxs-lookup"><span data-stu-id="804ca-212">The list of items the user is following.</span></span> <span data-ttu-id="804ca-213">仅适用于 OneDrive for Business 中。</span><span class="sxs-lookup"><span data-stu-id="804ca-213">Only in OneDrive for Business.</span></span>
| <span data-ttu-id="804ca-214">items</span><span class="sxs-lookup"><span data-stu-id="804ca-214">items</span></span>        | <span data-ttu-id="804ca-215">[driveItem][] 集合</span><span class="sxs-lookup"><span data-stu-id="804ca-215">[driveItem][] collection</span></span>             | <span data-ttu-id="804ca-p117">驱动器中包含的所有项。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="804ca-p117">All items contained in the drive. Read-only. Nullable.</span></span>
| <span data-ttu-id="804ca-219">root</span><span class="sxs-lookup"><span data-stu-id="804ca-219">root</span></span>         | <span data-ttu-id="804ca-220">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="804ca-220">[driveItem][]</span></span>                        | <span data-ttu-id="804ca-p118">驱动器的根文件夹。只读。</span><span class="sxs-lookup"><span data-stu-id="804ca-p118">The root folder of the drive. Read-only.</span></span>
| <span data-ttu-id="804ca-223">special</span><span class="sxs-lookup"><span data-stu-id="804ca-223">special</span></span>      | <span data-ttu-id="804ca-224">[driveItem][] 集合</span><span class="sxs-lookup"><span data-stu-id="804ca-224">[driveItem][] collection</span></span>             | <span data-ttu-id="804ca-p119">OneDrive 中可用的公用文件夹的集合。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="804ca-p119">Collection of common folders available in OneDrive. Read-only. Nullable.</span></span>


## <a name="json-representation"></a><span data-ttu-id="804ca-228">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="804ca-228">JSON representation</span></span>

<span data-ttu-id="804ca-229">下面是 Drive 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="804ca-229">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="804ca-230">**drive** 资源派生自 [**baseItem**](baseitem.md) 并继承该资源的属性。</span><span class="sxs-lookup"><span data-stu-id="804ca-230">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "string (timestamp)",
  "description": "string",
  "driveType": "personal | business | documentLibrary",
  "following": [{"@odata.type": "microsoft.graph.driveItem"}],
  "items": [{"@odata.type": "microsoft.graph.driveItem"}],
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "string (timestamp)",
  "name": "string",
  "owner": {"@odata.type": "microsoft.graph.identitySet"},
  "quota": {"@odata.type": "microsoft.graph.quota"},
  "root": {"@odata.type": "microsoft.graph.driveItem"},
  "special": [{"@odata.type": "microsoft.graph.driveItem"}],
  "system": {"@odata.type": "microsoft.graph.systemFacet"},
  "webUrl": "string",
  "sharepointIds": {"@odata.type": "microsoft.graph.sharepointIds"}
}
```


[bundle]: bundle.md
[driveItem]: driveItem.md
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
  "suppressions": []
}
-->
