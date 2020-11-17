---
author: JeremyKelley
ms.author: JeremyKelley
title: 驱动器资源类型
description: 表示用户的 OneDrive 或 SharePoint 中文档库的驱动器资源。
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 74ef4a5f8c2e67a81ad02ca0844d7f15dba972e8
ms.sourcegitcommit: eafb1629e52450dab0da6a1fb6d1ddfa878777c6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2020
ms.locfileid: "49081829"
---
# <a name="drive-resource-type"></a><span data-ttu-id="adcd9-103">驱动器资源类型</span><span class="sxs-lookup"><span data-stu-id="adcd9-103">drive resource type</span></span>

<span data-ttu-id="adcd9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="adcd9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="adcd9-105">驱动器资源是表示用户的 OneDrive 或其 SharePoint 中文档库的顶级对象。</span><span class="sxs-lookup"><span data-stu-id="adcd9-105">The drive resource is the top-level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="adcd9-p101">OneDrive 用户必须始终具有至少一个可用驱动器，即默认驱动器。没有 OneDrive 许可证的用户不能拥有可用的默认驱动器。</span><span class="sxs-lookup"><span data-stu-id="adcd9-p101">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="methods"></a><span data-ttu-id="adcd9-108">方法</span><span class="sxs-lookup"><span data-stu-id="adcd9-108">Methods</span></span>

|                        <span data-ttu-id="adcd9-109">方法</span><span class="sxs-lookup"><span data-stu-id="adcd9-109">Method</span></span>                              |         <span data-ttu-id="adcd9-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="adcd9-110">Return type</span></span>         | <span data-ttu-id="adcd9-111">说明</span><span class="sxs-lookup"><span data-stu-id="adcd9-111">Description</span></span> |
| :--------------------------------------------------------- | :-------------------------- |-------------|
| <span data-ttu-id="adcd9-112">[获取驱动器][drive-get]</span><span class="sxs-lookup"><span data-stu-id="adcd9-112">[Get drive][drive-get]</span></span>                                     | <span data-ttu-id="adcd9-113">驱动器</span><span class="sxs-lookup"><span data-stu-id="adcd9-113">drive</span></span>                       | <span data-ttu-id="adcd9-114">获取有关驱动器的元数据</span><span class="sxs-lookup"><span data-stu-id="adcd9-114">Get metadata about a drive</span></span> |
| <span data-ttu-id="adcd9-115">[获取驱动器根][item-get]</span><span class="sxs-lookup"><span data-stu-id="adcd9-115">[Get drive root][item-get]</span></span>                                 | <span data-ttu-id="adcd9-116">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="adcd9-116">[driveItem][]</span></span>               | <span data-ttu-id="adcd9-117">获取驱动器的根文件夹</span><span class="sxs-lookup"><span data-stu-id="adcd9-117">Get root folder of a drive</span></span> |
| <span data-ttu-id="adcd9-118">[列出活动][drive-activities]</span><span class="sxs-lookup"><span data-stu-id="adcd9-118">[List activities][drive-activities]</span></span>                        | <span data-ttu-id="adcd9-119">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="adcd9-119">[itemActivity][] collection</span></span> | <span data-ttu-id="adcd9-120">列出在驱动器下发生的活动</span><span class="sxs-lookup"><span data-stu-id="adcd9-120">List activities that occurred under the drive</span></span> |
| <span data-ttu-id="adcd9-121">[列出关注的项][drive-following]</span><span class="sxs-lookup"><span data-stu-id="adcd9-121">[List followed items][drive-following]</span></span>                     | <span data-ttu-id="adcd9-122">[driveItem][] 集合</span><span class="sxs-lookup"><span data-stu-id="adcd9-122">[driveItem][] collection</span></span>    | <span data-ttu-id="adcd9-123">列出用户的关注 driveItems</span><span class="sxs-lookup"><span data-stu-id="adcd9-123">List the user's followed driveItems</span></span> |
| <span data-ttu-id="adcd9-124">[列出子项][item-children]</span><span class="sxs-lookup"><span data-stu-id="adcd9-124">[List children][item-children]</span></span>                             | <span data-ttu-id="adcd9-125">[driveItem][] 集合</span><span class="sxs-lookup"><span data-stu-id="adcd9-125">[driveItem][] collection</span></span>    | <span data-ttu-id="adcd9-126">列出驱动器根文件夹的子项</span><span class="sxs-lookup"><span data-stu-id="adcd9-126">List children of the root folder of a drive</span></span> |
| <span data-ttu-id="adcd9-127">[列出变更][item-changes]</span><span class="sxs-lookup"><span data-stu-id="adcd9-127">[List changes][item-changes]</span></span>                               | <span data-ttu-id="adcd9-128">[driveItem][] 集合</span><span class="sxs-lookup"><span data-stu-id="adcd9-128">[driveItem][] collection</span></span>    | <span data-ttu-id="adcd9-129">列出驱动器中所有 DriveItem 的变更</span><span class="sxs-lookup"><span data-stu-id="adcd9-129">List changes for all driveItems in the Drive</span></span> |
| <span data-ttu-id="adcd9-130">[搜索][item-search]</span><span class="sxs-lookup"><span data-stu-id="adcd9-130">[Search][item-search]</span></span>                                      | <span data-ttu-id="adcd9-131">[driveItem][] 集合</span><span class="sxs-lookup"><span data-stu-id="adcd9-131">[driveItem][] collection</span></span>    | <span data-ttu-id="adcd9-132">搜索驱动器中的 DriveItem</span><span class="sxs-lookup"><span data-stu-id="adcd9-132">Search for driveItems in a drive</span></span> |
| [<span data-ttu-id="adcd9-133">获取特殊文件夹</span><span class="sxs-lookup"><span data-stu-id="adcd9-133">Get special folder</span></span>](../api/drive-get-specialfolder.md)    | <span data-ttu-id="adcd9-134">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="adcd9-134">[driveItem][]</span></span>               | <span data-ttu-id="adcd9-135">通过特殊文件夹的规范名称访问它</span><span class="sxs-lookup"><span data-stu-id="adcd9-135">Access a special folder by its canonical name</span></span> |


## <a name="properties"></a><span data-ttu-id="adcd9-136">属性</span><span class="sxs-lookup"><span data-stu-id="adcd9-136">Properties</span></span>

| <span data-ttu-id="adcd9-137">属性</span><span class="sxs-lookup"><span data-stu-id="adcd9-137">Property</span></span>             | <span data-ttu-id="adcd9-138">类型</span><span class="sxs-lookup"><span data-stu-id="adcd9-138">Type</span></span>                          | <span data-ttu-id="adcd9-139">说明</span><span class="sxs-lookup"><span data-stu-id="adcd9-139">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="adcd9-140">createdBy</span><span class="sxs-lookup"><span data-stu-id="adcd9-140">createdBy</span></span>            | <span data-ttu-id="adcd9-141">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="adcd9-141">[identitySet][]</span></span>               | <span data-ttu-id="adcd9-p102">识别创建项目的用户、设备或应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="adcd9-p102">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="adcd9-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="adcd9-144">createdDateTime</span></span>      | <span data-ttu-id="adcd9-145">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="adcd9-145">dateTimeOffset</span></span>                | <span data-ttu-id="adcd9-p103">创建项的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="adcd9-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="adcd9-148">description</span><span class="sxs-lookup"><span data-stu-id="adcd9-148">description</span></span>          | <span data-ttu-id="adcd9-149">String</span><span class="sxs-lookup"><span data-stu-id="adcd9-149">String</span></span>                        | <span data-ttu-id="adcd9-150">提供驱动器的用户可见说明。</span><span class="sxs-lookup"><span data-stu-id="adcd9-150">Provide a user-visible description of the drive.</span></span> <span data-ttu-id="adcd9-151">读写。</span><span class="sxs-lookup"><span data-stu-id="adcd9-151">Read-write.</span></span>
| <span data-ttu-id="adcd9-152">driveType</span><span class="sxs-lookup"><span data-stu-id="adcd9-152">driveType</span></span>            | <span data-ttu-id="adcd9-153">String</span><span class="sxs-lookup"><span data-stu-id="adcd9-153">String</span></span>                        | <span data-ttu-id="adcd9-p105">说明了由该资源表示的驱动器的类型。OneDrive 个人版驱动器将返回 `personal`。OneDrive for Business 将返回 `business`。SharePoint 文档库将返回 `documentLibrary`。只读。</span><span class="sxs-lookup"><span data-stu-id="adcd9-p105">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="adcd9-159">id</span><span class="sxs-lookup"><span data-stu-id="adcd9-159">id</span></span>                   | <span data-ttu-id="adcd9-160">String</span><span class="sxs-lookup"><span data-stu-id="adcd9-160">String</span></span>                        | <span data-ttu-id="adcd9-p106">驱动器唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="adcd9-p106">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="adcd9-163">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="adcd9-163">lastModifiedBy</span></span>       | <span data-ttu-id="adcd9-164">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="adcd9-164">[identitySet][]</span></span>               | <span data-ttu-id="adcd9-p107">上次修改项目的用户、设备和应用程序的标识。只读。</span><span class="sxs-lookup"><span data-stu-id="adcd9-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="adcd9-167">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="adcd9-167">lastModifiedDateTime</span></span> | <span data-ttu-id="adcd9-168">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="adcd9-168">dateTimeOffset</span></span>                | <span data-ttu-id="adcd9-p108">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="adcd9-p108">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="adcd9-171">name</span><span class="sxs-lookup"><span data-stu-id="adcd9-171">name</span></span>                 | <span data-ttu-id="adcd9-172">string</span><span class="sxs-lookup"><span data-stu-id="adcd9-172">string</span></span>                        | <span data-ttu-id="adcd9-p109">项目名称。读写。</span><span class="sxs-lookup"><span data-stu-id="adcd9-p109">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="adcd9-175">所有者</span><span class="sxs-lookup"><span data-stu-id="adcd9-175">owner</span></span>                | [<span data-ttu-id="adcd9-176">identitySet</span><span class="sxs-lookup"><span data-stu-id="adcd9-176">identitySet</span></span>](identityset.md) | <span data-ttu-id="adcd9-p110">可选。拥有此驱动器的用户帐户。只读。</span><span class="sxs-lookup"><span data-stu-id="adcd9-p110">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="adcd9-180">配额</span><span class="sxs-lookup"><span data-stu-id="adcd9-180">quota</span></span>                | [<span data-ttu-id="adcd9-181">配额</span><span class="sxs-lookup"><span data-stu-id="adcd9-181">quota</span></span>](quota.md)             | <span data-ttu-id="adcd9-p111">可选。有关驱动器的存储空间配额的信息。只读。</span><span class="sxs-lookup"><span data-stu-id="adcd9-p111">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="adcd9-185">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="adcd9-185">sharepointIds</span></span>        | <span data-ttu-id="adcd9-186">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="adcd9-186">[sharepointIds][]</span></span>             | <span data-ttu-id="adcd9-p112">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="adcd9-p112">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="adcd9-189">system</span><span class="sxs-lookup"><span data-stu-id="adcd9-189">system</span></span>               | <span data-ttu-id="adcd9-190">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="adcd9-190">[systemFacet][]</span></span>               | <span data-ttu-id="adcd9-191">如果存在，则表示这是系统管理的驱动器。</span><span class="sxs-lookup"><span data-stu-id="adcd9-191">If present, indicates that this is a system-managed drive.</span></span> <span data-ttu-id="adcd9-192">只读。</span><span class="sxs-lookup"><span data-stu-id="adcd9-192">Read-only.</span></span>
| <span data-ttu-id="adcd9-193">WebUrl</span><span class="sxs-lookup"><span data-stu-id="adcd9-193">webUrl</span></span>               | <span data-ttu-id="adcd9-194">string (url)</span><span class="sxs-lookup"><span data-stu-id="adcd9-194">string (url)</span></span>                  | <span data-ttu-id="adcd9-p114">在浏览器中显示此资源的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="adcd9-p114">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a><span data-ttu-id="adcd9-200">关系</span><span class="sxs-lookup"><span data-stu-id="adcd9-200">Relationships</span></span>

| <span data-ttu-id="adcd9-201">关系</span><span class="sxs-lookup"><span data-stu-id="adcd9-201">Relationship</span></span> | <span data-ttu-id="adcd9-202">类型</span><span class="sxs-lookup"><span data-stu-id="adcd9-202">Type</span></span>                                 | <span data-ttu-id="adcd9-203">说明</span><span class="sxs-lookup"><span data-stu-id="adcd9-203">Description</span></span>
|:-------------|:-------------------------------------|:-----------------------
| <span data-ttu-id="adcd9-204">activities</span><span class="sxs-lookup"><span data-stu-id="adcd9-204">activities</span></span>   | <span data-ttu-id="adcd9-205">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="adcd9-205">[itemActivity][] collection</span></span>          | <span data-ttu-id="adcd9-206">最近发生在此驱动器下的活动的列表。</span><span class="sxs-lookup"><span data-stu-id="adcd9-206">The list of recent activities that took place under this drive.</span></span>
| <span data-ttu-id="adcd9-207">捆绑</span><span class="sxs-lookup"><span data-stu-id="adcd9-207">bundles</span></span>      | <span data-ttu-id="adcd9-208">[driveItem][] 集合</span><span class="sxs-lookup"><span data-stu-id="adcd9-208">[driveItem][] collection</span></span>             | <span data-ttu-id="adcd9-209">[捆绑][bundle] (相册和多选共享项目集) 的集合。</span><span class="sxs-lookup"><span data-stu-id="adcd9-209">Collection of [bundles][bundle] (albums and multi-select-shared sets of items).</span></span> <span data-ttu-id="adcd9-210">只在个人的 OneDrive 中。</span><span class="sxs-lookup"><span data-stu-id="adcd9-210">Only in personal OneDrive.</span></span>
| <span data-ttu-id="adcd9-211">following</span><span class="sxs-lookup"><span data-stu-id="adcd9-211">following</span></span>    | <span data-ttu-id="adcd9-212">[driveItem][] 集合</span><span class="sxs-lookup"><span data-stu-id="adcd9-212">[driveItem][] collection</span></span>             | <span data-ttu-id="adcd9-213">用户关注的项列表。</span><span class="sxs-lookup"><span data-stu-id="adcd9-213">The list of items the user is following.</span></span> <span data-ttu-id="adcd9-214">仅适用于 OneDrive for Business 中。</span><span class="sxs-lookup"><span data-stu-id="adcd9-214">Only in OneDrive for Business.</span></span>
| <span data-ttu-id="adcd9-215">items</span><span class="sxs-lookup"><span data-stu-id="adcd9-215">items</span></span>        | <span data-ttu-id="adcd9-216">[driveItem][] 集合</span><span class="sxs-lookup"><span data-stu-id="adcd9-216">[driveItem][] collection</span></span>             | <span data-ttu-id="adcd9-p117">驱动器中包含的所有项。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="adcd9-p117">All items contained in the drive. Read-only. Nullable.</span></span>
| <span data-ttu-id="adcd9-220">root</span><span class="sxs-lookup"><span data-stu-id="adcd9-220">root</span></span>         | <span data-ttu-id="adcd9-221">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="adcd9-221">[driveItem][]</span></span>                        | <span data-ttu-id="adcd9-p118">驱动器的根文件夹。只读。</span><span class="sxs-lookup"><span data-stu-id="adcd9-p118">The root folder of the drive. Read-only.</span></span>
| <span data-ttu-id="adcd9-224">special</span><span class="sxs-lookup"><span data-stu-id="adcd9-224">special</span></span>      | <span data-ttu-id="adcd9-225">[driveItem][] 集合</span><span class="sxs-lookup"><span data-stu-id="adcd9-225">[driveItem][] collection</span></span>             | <span data-ttu-id="adcd9-p119">OneDrive 中可用的公用文件夹的集合。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="adcd9-p119">Collection of common folders available in OneDrive. Read-only. Nullable.</span></span>


## <a name="json-representation"></a><span data-ttu-id="adcd9-229">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="adcd9-229">JSON representation</span></span>

<span data-ttu-id="adcd9-230">下面是 Drive 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="adcd9-230">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="adcd9-231">**drive** 资源派生自 [**baseItem**](baseitem.md) 并继承该资源的属性。</span><span class="sxs-lookup"><span data-stu-id="adcd9-231">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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


