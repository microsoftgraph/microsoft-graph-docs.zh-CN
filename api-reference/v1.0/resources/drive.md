---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Drive
ms.openlocfilehash: 0b178967f7eb8da8bdf8584bb13a7d4f9950392b
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="drive-resource-type"></a><span data-ttu-id="7ce26-102">Drive 资源类型</span><span class="sxs-lookup"><span data-stu-id="7ce26-102">Drive resource type</span></span>

<span data-ttu-id="7ce26-103">驱动器资源是表示用户的 OneDrive 或 SharePoint 中文档库的顶级对象。</span><span class="sxs-lookup"><span data-stu-id="7ce26-103">The drive resource is the top level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="7ce26-p101">OneDrive 用户必须始终具有至少一个可用驱动器，即默认驱动器。没有 OneDrive 许可证的用户不能拥有可用的默认驱动器。</span><span class="sxs-lookup"><span data-stu-id="7ce26-p101">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ce26-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7ce26-106">JSON representation</span></span>

<span data-ttu-id="7ce26-107">下面是 Drive 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ce26-107">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="7ce26-108">**drive** 资源派生自 [**baseItem**](baseitem.md) 并继承该资源的属性。</span><span class="sxs-lookup"><span data-stu-id="7ce26-108">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.drive",
       "keyProperty": "id", 
       "optionalProperties": [ "activities", "createdBy", "createdDateTime", "description", "lastModifiedBy", "lastModifiedDateTime", "name", "webUrl", "items", "root", "special", "system"] } -->

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
  "special": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "system": { "@odata.type": "microsoft.graph.systemFacet" },
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="7ce26-109">属性</span><span class="sxs-lookup"><span data-stu-id="7ce26-109">Properties</span></span>

| <span data-ttu-id="7ce26-110">属性</span><span class="sxs-lookup"><span data-stu-id="7ce26-110">Property</span></span>             | <span data-ttu-id="7ce26-111">类型</span><span class="sxs-lookup"><span data-stu-id="7ce26-111">Type</span></span>                          | <span data-ttu-id="7ce26-112">说明</span><span class="sxs-lookup"><span data-stu-id="7ce26-112">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="7ce26-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="7ce26-113">createdBy</span></span>            | <span data-ttu-id="7ce26-114">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="7ce26-114">[identitySet][]</span></span>               | <span data-ttu-id="7ce26-p102">识别创建项目的用户、设备或应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="7ce26-p102">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="7ce26-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7ce26-117">createdDateTime</span></span>      | <span data-ttu-id="7ce26-118">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ce26-118">dateTimeOffset</span></span>                | <span data-ttu-id="7ce26-p103">创建项的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="7ce26-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="7ce26-121">说明</span><span class="sxs-lookup"><span data-stu-id="7ce26-121">description</span></span>          | <span data-ttu-id="7ce26-122">String</span><span class="sxs-lookup"><span data-stu-id="7ce26-122">String</span></span>                        | <span data-ttu-id="7ce26-123">提供驱动器的用户可见说明。</span><span class="sxs-lookup"><span data-stu-id="7ce26-123">Provide a user-visible description of the drive.</span></span> <span data-ttu-id="7ce26-124">读写。</span><span class="sxs-lookup"><span data-stu-id="7ce26-124">Read-write.</span></span>
| <span data-ttu-id="7ce26-125">driveType</span><span class="sxs-lookup"><span data-stu-id="7ce26-125">driveType</span></span>            | <span data-ttu-id="7ce26-126">String</span><span class="sxs-lookup"><span data-stu-id="7ce26-126">String</span></span>                        | <span data-ttu-id="7ce26-p105">说明了由该资源表示的驱动器的类型。OneDrive 个人版驱动器将返回 `personal`。OneDrive for Business 将返回 `business`。SharePoint 文档库将返回 `documentLibrary`。只读。</span><span class="sxs-lookup"><span data-stu-id="7ce26-p105">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="7ce26-132">id</span><span class="sxs-lookup"><span data-stu-id="7ce26-132">id</span></span>                   | <span data-ttu-id="7ce26-133">String</span><span class="sxs-lookup"><span data-stu-id="7ce26-133">String</span></span>                        | <span data-ttu-id="7ce26-p106">驱动器唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="7ce26-p106">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="7ce26-136">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="7ce26-136">lastModifiedBy</span></span>       | <span data-ttu-id="7ce26-137">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="7ce26-137">[identitySet][]</span></span>               | <span data-ttu-id="7ce26-p107">上次修改项目的用户、设备和应用程序的标识。只读。</span><span class="sxs-lookup"><span data-stu-id="7ce26-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="7ce26-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7ce26-140">lastModifiedDateTime</span></span> | <span data-ttu-id="7ce26-141">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ce26-141">dateTimeOffset</span></span>                | <span data-ttu-id="7ce26-p108">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="7ce26-p108">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="7ce26-144">name</span><span class="sxs-lookup"><span data-stu-id="7ce26-144">name</span></span>                 | <span data-ttu-id="7ce26-145">string</span><span class="sxs-lookup"><span data-stu-id="7ce26-145">string</span></span>                        | <span data-ttu-id="7ce26-p109">项目名称。读写。</span><span class="sxs-lookup"><span data-stu-id="7ce26-p109">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="7ce26-148">所有者</span><span class="sxs-lookup"><span data-stu-id="7ce26-148">owner</span></span>                | [<span data-ttu-id="7ce26-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="7ce26-149">identitySet</span></span>](identityset.md) | <span data-ttu-id="7ce26-p110">可选。拥有此驱动器的用户帐户。只读。</span><span class="sxs-lookup"><span data-stu-id="7ce26-p110">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="7ce26-153">配额</span><span class="sxs-lookup"><span data-stu-id="7ce26-153">quota</span></span>                | [<span data-ttu-id="7ce26-154">配额</span><span class="sxs-lookup"><span data-stu-id="7ce26-154">quota</span></span>](quota.md)             | <span data-ttu-id="7ce26-p111">可选。有关驱动器的存储空间配额的信息。只读。</span><span class="sxs-lookup"><span data-stu-id="7ce26-p111">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="7ce26-158">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="7ce26-158">sharepointIds</span></span>        | <span data-ttu-id="7ce26-159">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="7ce26-159">[sharepointIds][]</span></span>             | <span data-ttu-id="7ce26-p112">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="7ce26-p112">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="7ce26-162">system</span><span class="sxs-lookup"><span data-stu-id="7ce26-162">System</span></span>               | <span data-ttu-id="7ce26-163">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="7ce26-163">[systemFacet][]</span></span>               | <span data-ttu-id="7ce26-164">如果存在，则表示这是系统管理的驱动器。</span><span class="sxs-lookup"><span data-stu-id="7ce26-164">If present, indicates that this is a system-managed drive.</span></span> <span data-ttu-id="7ce26-165">只读。</span><span class="sxs-lookup"><span data-stu-id="7ce26-165">Read-only.</span></span>
| <span data-ttu-id="7ce26-166">WebUrl</span><span class="sxs-lookup"><span data-stu-id="7ce26-166">webUrl</span></span>               | <span data-ttu-id="7ce26-167">string (url)</span><span class="sxs-lookup"><span data-stu-id="7ce26-167">string (url)</span></span>                  | <span data-ttu-id="7ce26-p114">在浏览器中显示此资源的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="7ce26-p114">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a><span data-ttu-id="7ce26-173">关系</span><span class="sxs-lookup"><span data-stu-id="7ce26-173">Relationships</span></span>

| <span data-ttu-id="7ce26-174">关系</span><span class="sxs-lookup"><span data-stu-id="7ce26-174">Relationship</span></span> | <span data-ttu-id="7ce26-175">类型</span><span class="sxs-lookup"><span data-stu-id="7ce26-175">Type</span></span>                                 | <span data-ttu-id="7ce26-176">说明</span><span class="sxs-lookup"><span data-stu-id="7ce26-176">Description</span></span>
|:-------------|:-------------------------------------|:-----------------------
| <span data-ttu-id="7ce26-177">项目</span><span class="sxs-lookup"><span data-stu-id="7ce26-177">items</span></span>        | <span data-ttu-id="7ce26-178">[driveitem](driveitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7ce26-178">[driveitem](driveitem.md) collection</span></span> | <span data-ttu-id="7ce26-p115">驱动器中包含的所有项。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="7ce26-p115">All items contained in the drive. Read-only. Nullable.</span></span>
| <span data-ttu-id="7ce26-182">root</span><span class="sxs-lookup"><span data-stu-id="7ce26-182">root</span></span>         | [<span data-ttu-id="7ce26-183">driveitem</span><span class="sxs-lookup"><span data-stu-id="7ce26-183">driveitem</span></span>](driveitem.md)            | <span data-ttu-id="7ce26-p116">驱动器的根文件夹。只读。</span><span class="sxs-lookup"><span data-stu-id="7ce26-p116">The root folder of the drive. Read-only.</span></span>
| <span data-ttu-id="7ce26-186">special</span><span class="sxs-lookup"><span data-stu-id="7ce26-186">special</span></span>      | <span data-ttu-id="7ce26-187">[driveitem](driveitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7ce26-187">[driveitem](driveitem.md) collection</span></span> | <span data-ttu-id="7ce26-p117">OneDrive 中可用的公用文件夹的集合。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="7ce26-p117">Collection of common folders available in OneDrive. Read-only. Nullable.</span></span>

## <a name="methods"></a><span data-ttu-id="7ce26-191">方法</span><span class="sxs-lookup"><span data-stu-id="7ce26-191">Methods</span></span>

|                        <span data-ttu-id="7ce26-192">常见任务</span><span class="sxs-lookup"><span data-stu-id="7ce26-192">Common task</span></span>                         |         <span data-ttu-id="7ce26-193">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="7ce26-193">HTTP method</span></span>         |
| :--------------------------------------------------------- | :-------------------------- |
| <span data-ttu-id="7ce26-194">[获取其他驱动器的驱动器元数据][drive-get]</span><span class="sxs-lookup"><span data-stu-id="7ce26-194">[Get Drive metadata of another Drive][drive-get]</span></span>           | `GET /drives/{drive-id}`    |
| <span data-ttu-id="7ce26-195">[获取用户默认驱动器的根文件夹][item-get]</span><span class="sxs-lookup"><span data-stu-id="7ce26-195">[Get root folder for user's default Drive][item-get]</span></span>       | `GET /drive/root`           |
| <span data-ttu-id="7ce26-196">[列出驱动器下的子项][item-children]</span><span class="sxs-lookup"><span data-stu-id="7ce26-196">[List children under the Drive][item-children]</span></span>             | `GET /drive/root/children`  |
| <span data-ttu-id="7ce26-197">[列出驱动器中所有项的变更][item-changes]</span><span class="sxs-lookup"><span data-stu-id="7ce26-197">[List changes for all Items in the Drive][item-changes]</span></span>    | `GET /drive/root/delta`     |
| <span data-ttu-id="7ce26-198">[搜索驱动器中的项][item-search]</span><span class="sxs-lookup"><span data-stu-id="7ce26-198">[Search for Items in the Drive][item-search]</span></span>               | `GET /drive/root/search`    |
| [<span data-ttu-id="7ce26-199">访问特殊文件夹</span><span class="sxs-lookup"><span data-stu-id="7ce26-199">Access special folder</span></span>](../api/drive_get_specialfolder.md) | `GET /drive/special/{name}` |

<span data-ttu-id="7ce26-200">在上表中，各示例使用的是 `/drive`，但其他路径也同样有效。</span><span class="sxs-lookup"><span data-stu-id="7ce26-200">In the previous table, the examples use , but  is valid too.</span></span>

[item-resource]: driveitem.md
[identity-set]: identityset.md
[quota-facet]: quota.md
[drive-resource]: drive.md
[drive-get]: ../api/drive_get.md
[item-get]: ../api/driveitem_get.md
[item-changes]: ../api/driveitem_delta.md
[item-search]: ../api/driveitem_search.md
[item-children]: ../api/driveitem_list_children.md


<!-- {
  "type": "#page.annotation",
  "description": "Drive is a top level object for OneDrive API that provides access to the contents of a drive. ",
  "keywords": "drive,objects,resources",
  "section": "documentation",
  "tocPath": "Drives",
  "tocBookmarks": { "Resources/Drive": "#" }
} -->
