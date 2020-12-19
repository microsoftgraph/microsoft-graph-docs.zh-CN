---
author: JeremyKelley
ms.date: 09/10/2017
title: ItemReference
localization_priority: Normal
description: ItemReference 资源提供通过 API 寻址 DriveItem 所需的必要信息。
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: dd24f0d1fc0a5f5db576f5eea89b8205ff55b2b7
ms.sourcegitcommit: 0d4377b0153bc339ab7b3b1a6ee4d52848b622d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2020
ms.locfileid: "49714254"
---
# <a name="itemreference-resource-type"></a><span data-ttu-id="d24e4-103">ItemReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="d24e4-103">ItemReference resource type</span></span>

<span data-ttu-id="d24e4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d24e4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d24e4-105">**ItemReference** 资源提供了通过 API 查找 [DriveItem](driveitem.md) 的必要信息。</span><span class="sxs-lookup"><span data-stu-id="d24e4-105">The **ItemReference** resource provides information necessary to address a [DriveItem](driveitem.md) via the API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d24e4-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d24e4-106">JSON representation</span></span>

<span data-ttu-id="d24e4-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d24e4-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "path", "shareId", "sharepointIds" ],
  "@odata.type": "microsoft.graph.itemReference"
}-->

```json
{
  "driveId": "string",
  "driveType": "personal | business | documentLibrary",
  "id": "string",
  "name": "string",
  "path": "string",
  "shareId": "string",
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "siteId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="d24e4-108">属性</span><span class="sxs-lookup"><span data-stu-id="d24e4-108">Properties</span></span>

| <span data-ttu-id="d24e4-109">属性</span><span class="sxs-lookup"><span data-stu-id="d24e4-109">Property</span></span>      | <span data-ttu-id="d24e4-110">类型</span><span class="sxs-lookup"><span data-stu-id="d24e4-110">Type</span></span>              | <span data-ttu-id="d24e4-111">说明</span><span class="sxs-lookup"><span data-stu-id="d24e4-111">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="d24e4-112">driveId</span><span class="sxs-lookup"><span data-stu-id="d24e4-112">driveId</span></span>       | <span data-ttu-id="d24e4-113">String</span><span class="sxs-lookup"><span data-stu-id="d24e4-113">String</span></span>            | <span data-ttu-id="d24e4-p101">包含项的驱动器实例的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="d24e4-p101">Unique identifier of the drive instance that contains the item. Read-only.</span></span>
| <span data-ttu-id="d24e4-116">driveType</span><span class="sxs-lookup"><span data-stu-id="d24e4-116">driveType</span></span>     | <span data-ttu-id="d24e4-117">String</span><span class="sxs-lookup"><span data-stu-id="d24e4-117">String</span></span>            | <span data-ttu-id="d24e4-118">标识驱动器的类型。</span><span class="sxs-lookup"><span data-stu-id="d24e4-118">Identifies the type of drive.</span></span> <span data-ttu-id="d24e4-119">请参阅 [drive][] 资源查看其值。</span><span class="sxs-lookup"><span data-stu-id="d24e4-119">See [drive][] resource for values.</span></span>
| <span data-ttu-id="d24e4-120">id</span><span class="sxs-lookup"><span data-stu-id="d24e4-120">id</span></span>            | <span data-ttu-id="d24e4-121">String</span><span class="sxs-lookup"><span data-stu-id="d24e4-121">String</span></span>            | <span data-ttu-id="d24e4-p103">项在驱动器中的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="d24e4-p103">Unique identifier of the item in the drive. Read-only.</span></span>
| <span data-ttu-id="d24e4-124">name</span><span class="sxs-lookup"><span data-stu-id="d24e4-124">name</span></span>          | <span data-ttu-id="d24e4-125">String</span><span class="sxs-lookup"><span data-stu-id="d24e4-125">String</span></span>            | <span data-ttu-id="d24e4-p104">所引用的项的名称。只读。</span><span class="sxs-lookup"><span data-stu-id="d24e4-p104">The name of the item being referenced. Read-only.</span></span>
| <span data-ttu-id="d24e4-128">路径</span><span class="sxs-lookup"><span data-stu-id="d24e4-128">path</span></span>          | <span data-ttu-id="d24e4-129">String</span><span class="sxs-lookup"><span data-stu-id="d24e4-129">String</span></span>            | <span data-ttu-id="d24e4-p105">可用于导航到该项的路径。只读。</span><span class="sxs-lookup"><span data-stu-id="d24e4-p105">Path that can be used to navigate to the item. Read-only.</span></span>
| <span data-ttu-id="d24e4-132">shareId</span><span class="sxs-lookup"><span data-stu-id="d24e4-132">shareId</span></span>       | <span data-ttu-id="d24e4-133">String</span><span class="sxs-lookup"><span data-stu-id="d24e4-133">String</span></span>            | <span data-ttu-id="d24e4-134">可通过 [Shares][] API 访问的共享资源的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d24e4-134">A unique identifier for a shared resource that can be accessed via the [Shares][] API.</span></span>
| <span data-ttu-id="d24e4-135">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="d24e4-135">sharepointIds</span></span> | <span data-ttu-id="d24e4-136">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="d24e4-136">[sharepointIds][]</span></span> | <span data-ttu-id="d24e4-p106">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="d24e4-p106">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="d24e4-139">siteId</span><span class="sxs-lookup"><span data-stu-id="d24e4-139">siteId</span></span>        | <span data-ttu-id="d24e4-140">String</span><span class="sxs-lookup"><span data-stu-id="d24e4-140">String</span></span>            | <span data-ttu-id="d24e4-141">对于 OneDrive for Business 和 SharePoint，此属性表示包含 driveItem 资源的父文档库的网站的 ID。</span><span class="sxs-lookup"><span data-stu-id="d24e4-141">For OneDrive for Business and SharePoint, this property represents the ID of the site that contains the parent document library of the driveItem resource.</span></span> <span data-ttu-id="d24e4-142">该值与该网站资源的 ID [属性][] 相同。</span><span class="sxs-lookup"><span data-stu-id="d24e4-142">The value is the same as the id property of that [site][] resource.</span></span> <span data-ttu-id="d24e4-143">它是一 [个不透明的字符串，由网站的三个](/graph/api/resources/site#id-property) 标识符组成。</span><span class="sxs-lookup"><span data-stu-id="d24e4-143">It is an [opaque string that consists of three identifiers](/graph/api/resources/site#id-property) of the site.</span></span> <br><span data-ttu-id="d24e4-144">对于 OneDrive，不填充此属性。</span><span class="sxs-lookup"><span data-stu-id="d24e4-144">For OneDrive, this property is not populated.</span></span>

[drive]: ../resources/drive.md
[sharepointIds]: ../resources/sharepointids.md
[Shares]: ../api/shares-get.md
[网站]: ../resources/site.md
[site]: ../resources/site.md

## <a name="remarks"></a><span data-ttu-id="d24e4-149">注解</span><span class="sxs-lookup"><span data-stu-id="d24e4-149">Remarks</span></span>

<span data-ttu-id="d24e4-150">为了从 **itemReference** 资源中找到 **driveItem**，请构建以下格式的 URL：</span><span class="sxs-lookup"><span data-stu-id="d24e4-150">To address a **driveItem** from an **itemReference** resource, construct a URL of the format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/drives/{driveId}/items/{id}
```

<span data-ttu-id="d24e4-151">**path** 值是相对于目标驱动器的 API 路径，例如：`/drive/root:/Documents/myfile.docx`。</span><span class="sxs-lookup"><span data-stu-id="d24e4-151">The **path** value is an API path relative to the target drive, for example: `/drive/root:/Documents/myfile.docx`.</span></span>

<span data-ttu-id="d24e4-152">要检索人工可读路径中的痕迹，可以放心地忽略路径字符串中的第一个 `:` 之前的所有内容。</span><span class="sxs-lookup"><span data-stu-id="d24e4-152">To retrieve the human-readable path for a breadcrumb, you can safely ignore everything up to the first `:` in the path string.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ItemReference returns a pointer to another item.",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/itemreference.md:
      Found potential enums in resource example that weren't defined in a table:(personal,business,documentLibrary) are in resource, but () are in table"
  ],
  "tocPath": "Resources/ItemReference"
} -->

