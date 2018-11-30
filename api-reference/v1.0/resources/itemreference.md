---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ItemReference
ms.openlocfilehash: abd8b438e6c4e364a7a4b010d0808255425fa4df
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="itemreference-resource-type"></a><span data-ttu-id="4c4eb-102">ItemReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="4c4eb-102">ItemReference resource type</span></span>

<span data-ttu-id="4c4eb-103">**ItemReference** 资源提供了通过 API 查找 [DriveItem](driveitem.md) 的必要信息。</span><span class="sxs-lookup"><span data-stu-id="4c4eb-103">The **ItemReference** resource provides information necessary to address a [DriveItem](driveitem.md) via the API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4c4eb-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4c4eb-104">JSON representation</span></span>

<span data-ttu-id="4c4eb-105">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4c4eb-105">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="4c4eb-106">属性</span><span class="sxs-lookup"><span data-stu-id="4c4eb-106">Properties</span></span>

| <span data-ttu-id="4c4eb-107">属性</span><span class="sxs-lookup"><span data-stu-id="4c4eb-107">Property</span></span>      | <span data-ttu-id="4c4eb-108">类型</span><span class="sxs-lookup"><span data-stu-id="4c4eb-108">Type</span></span>              | <span data-ttu-id="4c4eb-109">说明</span><span class="sxs-lookup"><span data-stu-id="4c4eb-109">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="4c4eb-110">driveId</span><span class="sxs-lookup"><span data-stu-id="4c4eb-110">driveId</span></span>       | <span data-ttu-id="4c4eb-111">String</span><span class="sxs-lookup"><span data-stu-id="4c4eb-111">String</span></span>            | <span data-ttu-id="4c4eb-p101">包含项的驱动器实例的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="4c4eb-p101">Unique identifier of the drive instance that contains the item. Read-only.</span></span>
| <span data-ttu-id="4c4eb-114">driveType</span><span class="sxs-lookup"><span data-stu-id="4c4eb-114">driveType</span></span>     | <span data-ttu-id="4c4eb-115">String</span><span class="sxs-lookup"><span data-stu-id="4c4eb-115">String</span></span>            | <span data-ttu-id="4c4eb-116">标识驱动器的类型。</span><span class="sxs-lookup"><span data-stu-id="4c4eb-116">Identifies the type of form region.</span></span> <span data-ttu-id="4c4eb-117">请参阅 [drive][] 资源查看其值。</span><span class="sxs-lookup"><span data-stu-id="4c4eb-117">See [drive][] resource for values.</span></span>
| <span data-ttu-id="4c4eb-118">id</span><span class="sxs-lookup"><span data-stu-id="4c4eb-118">id</span></span>            | <span data-ttu-id="4c4eb-119">String</span><span class="sxs-lookup"><span data-stu-id="4c4eb-119">String</span></span>            | <span data-ttu-id="4c4eb-p103">项在驱动器中的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="4c4eb-p103">Unique identifier of the item in the drive. Read-only.</span></span>
| <span data-ttu-id="4c4eb-122">name</span><span class="sxs-lookup"><span data-stu-id="4c4eb-122">name</span></span>          | <span data-ttu-id="4c4eb-123">字符串</span><span class="sxs-lookup"><span data-stu-id="4c4eb-123">String</span></span>            | <span data-ttu-id="4c4eb-p104">所引用的项的名称。只读。</span><span class="sxs-lookup"><span data-stu-id="4c4eb-p104">The name of the item being referenced. Read-only.</span></span>
| <span data-ttu-id="4c4eb-126">路径</span><span class="sxs-lookup"><span data-stu-id="4c4eb-126">path</span></span>          | <span data-ttu-id="4c4eb-127">String</span><span class="sxs-lookup"><span data-stu-id="4c4eb-127">String</span></span>            | <span data-ttu-id="4c4eb-p105">可用于导航到该项的路径。只读。</span><span class="sxs-lookup"><span data-stu-id="4c4eb-p105">Path that can be used to navigate to the item. Read-only.</span></span>
| <span data-ttu-id="4c4eb-130">shareId</span><span class="sxs-lookup"><span data-stu-id="4c4eb-130">shareId</span></span>       | <span data-ttu-id="4c4eb-131">String</span><span class="sxs-lookup"><span data-stu-id="4c4eb-131">String</span></span>            | <span data-ttu-id="4c4eb-132">可通过 [Shares][] API 访问共享资源的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4c4eb-132">A unique identifier for a shared resource that can be accessed via the [Shares][] API.</span></span>
| <span data-ttu-id="4c4eb-133">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="4c4eb-133">sharepointIds</span></span> | <span data-ttu-id="4c4eb-134">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="4c4eb-134">[sharepointIds][]</span></span> | <span data-ttu-id="4c4eb-p106">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="4c4eb-p106">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>

[drive]: ../resources/drive.md
[sharepointIds]: ../resources/sharepointids.md
[Shares]: ../api/shares_get.md

## <a name="remarks"></a><span data-ttu-id="4c4eb-140">备注</span><span class="sxs-lookup"><span data-stu-id="4c4eb-140">Remarks</span></span>

<span data-ttu-id="4c4eb-141">为了从 **itemReference** 资源中找到 **driveItem**，请构建以下格式的 URL：</span><span class="sxs-lookup"><span data-stu-id="4c4eb-141">To address a **driveItem** from an **itemReference** resource, construct a URL of the format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/drives/{driveId}/items/{id}
```

<span data-ttu-id="4c4eb-142">**path** 值是相对于目标驱动器的 API 路径，例如：`/drive/root:/Documents/myfile.docx`。</span><span class="sxs-lookup"><span data-stu-id="4c4eb-142">The **path** value is an API path relative to the target drive, for example: `/drive/root:/Documents/myfile.docx`.</span></span>

<span data-ttu-id="4c4eb-143">要检索人工可读路径中的痕迹，可以放心地忽略路径字符串中的第一个 `:` 之前的所有内容。</span><span class="sxs-lookup"><span data-stu-id="4c4eb-143">To retrieve the human-readable path for a breadcrumb, you can safely ignore everything up to the first `:` in the path string.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ItemReference returns a pointer to another item.",
  "section": "documentation",
  "tocPath": "Resources/ItemReference"
} -->
