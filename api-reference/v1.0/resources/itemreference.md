---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ItemReference
localization_priority: Normal
description: ItemReference 资源提供通过 API 寻址 DriveItem 所需的必要信息。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f7d8f6d524b605b544785b0379a273d4c022c9c9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036524"
---
# <a name="itemreference-resource-type"></a><span data-ttu-id="b4bcf-103">ItemReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="b4bcf-103">ItemReference resource type</span></span>

<span data-ttu-id="b4bcf-104">**ItemReference** 资源提供了通过 API 查找 [DriveItem](driveitem.md) 的必要信息。</span><span class="sxs-lookup"><span data-stu-id="b4bcf-104">The **ItemReference** resource provides information necessary to address a [DriveItem](driveitem.md) via the API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4bcf-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b4bcf-105">JSON representation</span></span>

<span data-ttu-id="b4bcf-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b4bcf-106">Here is a JSON representation of the resource</span></span>

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
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" }
}
```

## <a name="properties"></a><span data-ttu-id="b4bcf-107">属性</span><span class="sxs-lookup"><span data-stu-id="b4bcf-107">Properties</span></span>

| <span data-ttu-id="b4bcf-108">属性</span><span class="sxs-lookup"><span data-stu-id="b4bcf-108">Property</span></span>      | <span data-ttu-id="b4bcf-109">类型</span><span class="sxs-lookup"><span data-stu-id="b4bcf-109">Type</span></span>              | <span data-ttu-id="b4bcf-110">说明</span><span class="sxs-lookup"><span data-stu-id="b4bcf-110">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="b4bcf-111">driveId</span><span class="sxs-lookup"><span data-stu-id="b4bcf-111">driveId</span></span>       | <span data-ttu-id="b4bcf-112">字符串</span><span class="sxs-lookup"><span data-stu-id="b4bcf-112">String</span></span>            | <span data-ttu-id="b4bcf-p101">包含项的驱动器实例的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="b4bcf-p101">Unique identifier of the drive instance that contains the item. Read-only.</span></span>
| <span data-ttu-id="b4bcf-115">driveType</span><span class="sxs-lookup"><span data-stu-id="b4bcf-115">driveType</span></span>     | <span data-ttu-id="b4bcf-116">String</span><span class="sxs-lookup"><span data-stu-id="b4bcf-116">String</span></span>            | <span data-ttu-id="b4bcf-117">标识驱动器的类型。</span><span class="sxs-lookup"><span data-stu-id="b4bcf-117">Identifies the type of drive.</span></span> <span data-ttu-id="b4bcf-118">请参阅 [drive][] 资源查看其值。</span><span class="sxs-lookup"><span data-stu-id="b4bcf-118">See [drive][] resource for values.</span></span>
| <span data-ttu-id="b4bcf-119">id</span><span class="sxs-lookup"><span data-stu-id="b4bcf-119">id</span></span>            | <span data-ttu-id="b4bcf-120">String</span><span class="sxs-lookup"><span data-stu-id="b4bcf-120">String</span></span>            | <span data-ttu-id="b4bcf-p103">项在驱动器中的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="b4bcf-p103">Unique identifier of the item in the drive. Read-only.</span></span>
| <span data-ttu-id="b4bcf-123">name</span><span class="sxs-lookup"><span data-stu-id="b4bcf-123">name</span></span>          | <span data-ttu-id="b4bcf-124">字符串</span><span class="sxs-lookup"><span data-stu-id="b4bcf-124">String</span></span>            | <span data-ttu-id="b4bcf-p104">所引用的项的名称。只读。</span><span class="sxs-lookup"><span data-stu-id="b4bcf-p104">The name of the item being referenced. Read-only.</span></span>
| <span data-ttu-id="b4bcf-127">路径</span><span class="sxs-lookup"><span data-stu-id="b4bcf-127">path</span></span>          | <span data-ttu-id="b4bcf-128">String</span><span class="sxs-lookup"><span data-stu-id="b4bcf-128">String</span></span>            | <span data-ttu-id="b4bcf-p105">可用于导航到该项的路径。只读。</span><span class="sxs-lookup"><span data-stu-id="b4bcf-p105">Path that can be used to navigate to the item. Read-only.</span></span>
| <span data-ttu-id="b4bcf-131">shareId</span><span class="sxs-lookup"><span data-stu-id="b4bcf-131">shareId</span></span>       | <span data-ttu-id="b4bcf-132">String</span><span class="sxs-lookup"><span data-stu-id="b4bcf-132">String</span></span>            | <span data-ttu-id="b4bcf-133">可通过 [Shares][] API 访问的共享资源的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b4bcf-133">A unique identifier for a shared resource that can be accessed via the [Shares][] API.</span></span>
| <span data-ttu-id="b4bcf-134">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="b4bcf-134">sharepointIds</span></span> | <span data-ttu-id="b4bcf-135">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="b4bcf-135">[sharepointIds][]</span></span> | <span data-ttu-id="b4bcf-p106">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="b4bcf-p106">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>

[drive]: ../resources/drive.md
[sharepointIds]: ../resources/sharepointids.md
[Shares]: ../api/shares-get.md

## <a name="remarks"></a><span data-ttu-id="b4bcf-141">注解</span><span class="sxs-lookup"><span data-stu-id="b4bcf-141">Remarks</span></span>

<span data-ttu-id="b4bcf-142">为了从 **itemReference** 资源中找到 **driveItem**，请构建以下格式的 URL：</span><span class="sxs-lookup"><span data-stu-id="b4bcf-142">To address a **driveItem** from an **itemReference** resource, construct a URL of the format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/drives/{driveId}/items/{id}
```

<span data-ttu-id="b4bcf-143">**path** 值是相对于目标驱动器的 API 路径，例如：`/drive/root:/Documents/myfile.docx`。</span><span class="sxs-lookup"><span data-stu-id="b4bcf-143">The **path** value is an API path relative to the target drive, for example: `/drive/root:/Documents/myfile.docx`.</span></span>

<span data-ttu-id="b4bcf-144">要检索人工可读路径中的痕迹，可以放心地忽略路径字符串中的第一个 `:` 之前的所有内容。</span><span class="sxs-lookup"><span data-stu-id="b4bcf-144">To retrieve the human-readable path for a breadcrumb, you can safely ignore everything up to the first `:` in the path string.</span></span>

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
