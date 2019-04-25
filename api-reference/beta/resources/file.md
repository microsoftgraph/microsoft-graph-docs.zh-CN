---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 文件
localization_priority: Normal
ms.openlocfilehash: 219398ea62b825797479bef0b7a2bf52d014c8c0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547632"
---
# <a name="file-resource-type"></a><span data-ttu-id="79cc5-102">File 资源类型</span><span class="sxs-lookup"><span data-stu-id="79cc5-102">File resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79cc5-103">**文件**资源将与文件相关的数据项分组到一个单一结构。</span><span class="sxs-lookup"><span data-stu-id="79cc5-103">The **File** resource groups file-related data items into a single structure.</span></span>

<span data-ttu-id="79cc5-p101">如果 [**DriveItem**](driveitem.md) 具有一个非 null **文件**方面，则该项表示一个文件。除了其他属性，文件还具有**内容**关系，其中包含文件字节流。</span><span class="sxs-lookup"><span data-stu-id="79cc5-p101">If a [**DriveItem**](driveitem.md) has a non-null **file** facet, the item represents an file. In addition to other properties, files have a **content** relationship which contains the byte stream of the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="79cc5-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="79cc5-106">JSON representation</span></span>

<span data-ttu-id="79cc5-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="79cc5-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="79cc5-108">属性</span><span class="sxs-lookup"><span data-stu-id="79cc5-108">Properties</span></span>

| <span data-ttu-id="79cc5-109">属性</span><span class="sxs-lookup"><span data-stu-id="79cc5-109">Property</span></span> | <span data-ttu-id="79cc5-110">类型</span><span class="sxs-lookup"><span data-stu-id="79cc5-110">Type</span></span>                    | <span data-ttu-id="79cc5-111">说明</span><span class="sxs-lookup"><span data-stu-id="79cc5-111">Description</span></span>                                                                                                                                      |
|:---------|:------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="79cc5-112">哈希</span><span class="sxs-lookup"><span data-stu-id="79cc5-112">hashes</span></span>   | [<span data-ttu-id="79cc5-113">HashesType</span><span class="sxs-lookup"><span data-stu-id="79cc5-113">HashesType</span></span>](hashes.md) | <span data-ttu-id="79cc5-p102">文件二进制内容的哈希值（如果可用）。只读。</span><span class="sxs-lookup"><span data-stu-id="79cc5-p102">Hashes of the file's binary content, if available. Read-only.</span></span>                                                                                    |
| <span data-ttu-id="79cc5-116">mimeType</span><span class="sxs-lookup"><span data-stu-id="79cc5-116">mimeType</span></span> | <span data-ttu-id="79cc5-117">string</span><span class="sxs-lookup"><span data-stu-id="79cc5-117">string</span></span>                  | <span data-ttu-id="79cc5-p103">文件的 MIME 类型。这由服务器上的逻辑决定，不能是在上载文件时提供的值。只读。</span><span class="sxs-lookup"><span data-stu-id="79cc5-p103">The MIME type for the file. This is determined by logic on the server and might not be the value provided when the file was uploaded. Read-only.</span></span> |

## <a name="remarks"></a><span data-ttu-id="79cc5-121">注解</span><span class="sxs-lookup"><span data-stu-id="79cc5-121">Remarks</span></span> 

<span data-ttu-id="79cc5-122">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="79cc5-122">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The file facet describes properties of a file",
  "keywords": "file,item,facet",
  "section": "documentation",
  "tocPath": "Facets/File",
  "suppressions": [
    "Error: /api-reference/beta/resources/file.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
