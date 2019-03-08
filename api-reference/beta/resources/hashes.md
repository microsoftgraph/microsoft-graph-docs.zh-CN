---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 希
localization_priority: Normal
ms.openlocfilehash: be7d3b27b1ef22976dc93ea5aecbc2a64031e8b4
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480115"
---
# <a name="hashes-resource-type"></a><span data-ttu-id="5fc5b-102">Hashes 资源类型</span><span class="sxs-lookup"><span data-stu-id="5fc5b-102">Hashes resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5fc5b-103">**哈希**资源将可用哈希分组到项的单个结构中。</span><span class="sxs-lookup"><span data-stu-id="5fc5b-103">The **Hashes** resource groups available hashes into a single structure for an item.</span></span>

<span data-ttu-id="5fc5b-104">**注意：** 并非所有服务均为列出的所有哈希属性提供值。</span><span class="sxs-lookup"><span data-stu-id="5fc5b-104">**Note:** Not all services provide a value for all hash properties listed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5fc5b-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5fc5b-105">JSON representation</span></span>

<span data-ttu-id="5fc5b-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5fc5b-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "sha1Hash", "crc32Hash", "quickXorHash" ],
  "@odata.type": "microsoft.graph.hashes"
}-->

```json
{
  "crc32Hash": "string (hex)",
  "sha1Hash": "string (hex)",
  "quickXorHash": "string (base64)"
}
```

## <a name="properties"></a><span data-ttu-id="5fc5b-107">属性</span><span class="sxs-lookup"><span data-stu-id="5fc5b-107">Properties</span></span>

| <span data-ttu-id="5fc5b-108">属性</span><span class="sxs-lookup"><span data-stu-id="5fc5b-108">Property</span></span>         | <span data-ttu-id="5fc5b-109">类型</span><span class="sxs-lookup"><span data-stu-id="5fc5b-109">Type</span></span>   | <span data-ttu-id="5fc5b-110">说明</span><span class="sxs-lookup"><span data-stu-id="5fc5b-110">Description</span></span>                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| <span data-ttu-id="5fc5b-111">**sha1Hash**</span><span class="sxs-lookup"><span data-stu-id="5fc5b-111">**sha1Hash**</span></span>     | <span data-ttu-id="5fc5b-112">String</span><span class="sxs-lookup"><span data-stu-id="5fc5b-112">String</span></span> | <span data-ttu-id="5fc5b-p101">文件内容的 SHA1 哈希（如果可用）。只读。</span><span class="sxs-lookup"><span data-stu-id="5fc5b-p101">SHA1 hash for the contents of the file (if available). Read-only.</span></span> |
| <span data-ttu-id="5fc5b-115">**crc32Hash**</span><span class="sxs-lookup"><span data-stu-id="5fc5b-115">**crc32Hash**</span></span>    | <span data-ttu-id="5fc5b-116">String</span><span class="sxs-lookup"><span data-stu-id="5fc5b-116">String</span></span> | <span data-ttu-id="5fc5b-p102">文件的 CRC32 值（如果可用）。只读。</span><span class="sxs-lookup"><span data-stu-id="5fc5b-p102">The CRC32 value of the file (if available). Read-only.</span></span>            |
| <span data-ttu-id="5fc5b-119">**quickXorHash**</span><span class="sxs-lookup"><span data-stu-id="5fc5b-119">**quickXorHash**</span></span> | <span data-ttu-id="5fc5b-120">String</span><span class="sxs-lookup"><span data-stu-id="5fc5b-120">String</span></span> | <span data-ttu-id="5fc5b-p103">文件的专有哈希，可用于确定文件内容是否更改（如果存在）。只读。</span><span class="sxs-lookup"><span data-stu-id="5fc5b-p103">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available). Read-only.</span></span> |

<span data-ttu-id="5fc5b-p104">**注意：** 在某些情况下，哈希值不可用。如果出现这种情况，将在下载项后对项上的哈希值进行更新。</span><span class="sxs-lookup"><span data-stu-id="5fc5b-p104">**Note:** In some cases hash values may not be available. If this is the case, the hash values on an item will be updated after the item is downloaded.</span></span>

## <a name="remarks"></a><span data-ttu-id="5fc5b-125">注解</span><span class="sxs-lookup"><span data-stu-id="5fc5b-125">Remarks</span></span>

<span data-ttu-id="5fc5b-126">在 OneDrive for Business 和 SharePoint Server 2016 中，**sha1Hash** 和 **crc32Hash** 不可用。</span><span class="sxs-lookup"><span data-stu-id="5fc5b-126">In OneDrive for Business and SharePoint Server 2016, **sha1Hash** and **crc32Hash** are not available.</span></span>

<span data-ttu-id="5fc5b-127">在 OneDrive 个人版中，**quickXorHash** 不可用。</span><span class="sxs-lookup"><span data-stu-id="5fc5b-127">In OneDrive Personal, **quickXorHash** is not available.</span></span>

<span data-ttu-id="5fc5b-128">若要计算文件的 **quickXorHash**，请参阅 [QuickXorHash 代码片段](https://dev.onedrive.com/snippets/quickxorhash.htm)。</span><span class="sxs-lookup"><span data-stu-id="5fc5b-128">To calculate **quickXorHash** for a file, refer to the [QuickXorHash snippet](https://dev.onedrive.com/snippets/quickxorhash.htm).</span></span>

<span data-ttu-id="5fc5b-129">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="5fc5b-129">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes",
  "suppressions": [
    "Error: /api-reference/beta/resources/hashes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
