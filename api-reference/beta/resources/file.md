---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: File
ms.openlocfilehash: bd0cd6ea5f5ee2225392aa61c2dda9b30e2ffbca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047528"
---
# <a name="file-resource-type"></a><span data-ttu-id="a48c8-102">File 资源类型</span><span class="sxs-lookup"><span data-stu-id="a48c8-102">File resource type</span></span>

> <span data-ttu-id="a48c8-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a48c8-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a48c8-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a48c8-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a48c8-105">**文件**资源将与文件相关的数据项分组到一个单一结构。</span><span class="sxs-lookup"><span data-stu-id="a48c8-105">The **File** resource groups file-related data items into a single structure.</span></span>

<span data-ttu-id="a48c8-p102">如果 [**DriveItem**](driveitem.md) 具有一个非 null **文件**方面，则该项表示一个文件。除了其他属性，文件还具有**内容**关系，其中包含文件字节流。</span><span class="sxs-lookup"><span data-stu-id="a48c8-p102">If a [**DriveItem**](driveitem.md) has a non-null **file** facet, the item represents an file. In addition to other properties, files have a **content** relationship which contains the byte stream of the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a48c8-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a48c8-108">JSON representation</span></span>

<span data-ttu-id="a48c8-109">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a48c8-109">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="a48c8-110">属性</span><span class="sxs-lookup"><span data-stu-id="a48c8-110">Properties</span></span>

| <span data-ttu-id="a48c8-111">属性</span><span class="sxs-lookup"><span data-stu-id="a48c8-111">Property</span></span> | <span data-ttu-id="a48c8-112">类型</span><span class="sxs-lookup"><span data-stu-id="a48c8-112">Type</span></span>                    | <span data-ttu-id="a48c8-113">说明</span><span class="sxs-lookup"><span data-stu-id="a48c8-113">Description</span></span>                                                                                                                                      |
|:---------|:------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="a48c8-114">哈希</span><span class="sxs-lookup"><span data-stu-id="a48c8-114">hashes</span></span>   | [<span data-ttu-id="a48c8-115">HashesType</span><span class="sxs-lookup"><span data-stu-id="a48c8-115">HashesType</span></span>](hashes.md) | <span data-ttu-id="a48c8-p103">文件二进制内容的哈希值（如果可用）。只读。</span><span class="sxs-lookup"><span data-stu-id="a48c8-p103">Hashes of the file's binary content, if available. Read-only.</span></span>                                                                                    |
| <span data-ttu-id="a48c8-118">mimeType</span><span class="sxs-lookup"><span data-stu-id="a48c8-118">mimeType</span></span> | <span data-ttu-id="a48c8-119">string</span><span class="sxs-lookup"><span data-stu-id="a48c8-119">string</span></span>                  | <span data-ttu-id="a48c8-p104">文件的 MIME 类型。这由服务器上的逻辑决定，不能是在上载文件时提供的值。只读。</span><span class="sxs-lookup"><span data-stu-id="a48c8-p104">The MIME type for the file. This is determined by logic on the server and might not be the value provided when the file was uploaded. Read-only.</span></span> |

## <a name="remarks"></a><span data-ttu-id="a48c8-123">注解</span><span class="sxs-lookup"><span data-stu-id="a48c8-123">Remarks</span></span> 

<span data-ttu-id="a48c8-124">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="a48c8-124">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The file facet describes properties of a file",
  "keywords": "file,item,facet",
  "section": "documentation",
  "tocPath": "Facets/File"
} -->
