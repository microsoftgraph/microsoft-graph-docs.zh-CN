---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 文件
localization_priority: Normal
description: 文件资源将与文件相关的数据项分组到一个单一结构。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c316e3b09f00ffebd7ebfab5e47b49c7df3980d3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532958"
---
# <a name="file-resource-type"></a><span data-ttu-id="03a14-103">File 资源类型</span><span class="sxs-lookup"><span data-stu-id="03a14-103">File resource type</span></span>

<span data-ttu-id="03a14-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03a14-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="03a14-105">**文件**资源将与文件相关的数据项分组到一个单一结构。</span><span class="sxs-lookup"><span data-stu-id="03a14-105">The **File** resource groups file-related data items into a single structure.</span></span>

<span data-ttu-id="03a14-p101">如果 [**DriveItem**](driveitem.md) 具有一个非 null **文件**方面，则该项表示一个文件。除了其他属性，文件还具有**内容**关系，其中包含文件字节流。</span><span class="sxs-lookup"><span data-stu-id="03a14-p101">If a [**DriveItem**](driveitem.md) has a non-null **file** facet, the item represents an file. In addition to other properties, files have a **content** relationship which contains the byte stream of the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="03a14-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="03a14-108">JSON representation</span></span>

<span data-ttu-id="03a14-109">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03a14-109">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.file"
}-->

```json
{
  "hashes": {"@odata.type": "microsoft.graph.hashes"},
  "mimeType": "string"
}
```

## <a name="properties"></a><span data-ttu-id="03a14-110">属性</span><span class="sxs-lookup"><span data-stu-id="03a14-110">Properties</span></span>

| <span data-ttu-id="03a14-111">属性</span><span class="sxs-lookup"><span data-stu-id="03a14-111">Property</span></span> | <span data-ttu-id="03a14-112">类型</span><span class="sxs-lookup"><span data-stu-id="03a14-112">Type</span></span>                    | <span data-ttu-id="03a14-113">说明</span><span class="sxs-lookup"><span data-stu-id="03a14-113">Description</span></span>                                                                                                                                      |
|:---------|:------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="03a14-114">哈希</span><span class="sxs-lookup"><span data-stu-id="03a14-114">hashes</span></span>   | [<span data-ttu-id="03a14-115">哈希</span><span class="sxs-lookup"><span data-stu-id="03a14-115">Hashes</span></span>](hashes.md) | <span data-ttu-id="03a14-p102">文件二进制内容的哈希值（如果可用）。只读。</span><span class="sxs-lookup"><span data-stu-id="03a14-p102">Hashes of the file's binary content, if available. Read-only.</span></span>                                                                                    |
| <span data-ttu-id="03a14-118">mimeType</span><span class="sxs-lookup"><span data-stu-id="03a14-118">mimeType</span></span> | <span data-ttu-id="03a14-119">string</span><span class="sxs-lookup"><span data-stu-id="03a14-119">string</span></span>                  | <span data-ttu-id="03a14-p103">文件的 MIME 类型。这由服务器上的逻辑决定，不能是在上载文件时提供的值。只读。</span><span class="sxs-lookup"><span data-stu-id="03a14-p103">The MIME type for the file. This is determined by logic on the server and might not be the value provided when the file was uploaded. Read-only.</span></span> |

## <a name="remarks"></a><span data-ttu-id="03a14-123">注解</span><span class="sxs-lookup"><span data-stu-id="03a14-123">Remarks</span></span> 

<span data-ttu-id="03a14-124">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="03a14-124">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The file facet describes properties of a file",
  "keywords": "file,item,facet",
  "section": "documentation",
  "tocPath": "Facets/File"
} -->
