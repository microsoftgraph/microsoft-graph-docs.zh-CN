---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
localization_priority: Normal
ms.openlocfilehash: abe6fc277f94eb1f66f50f25b894bc41fd038a9b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570818"
---
# <a name="hashes-resource-type"></a><span data-ttu-id="dd738-101">Hashes 资源类型</span><span class="sxs-lookup"><span data-stu-id="dd738-101">Hashes resource type</span></span>

<span data-ttu-id="dd738-102">**哈希**资源将可用哈希分组到项的单个结构中。</span><span class="sxs-lookup"><span data-stu-id="dd738-102">The **Hashes** resource groups available hashes into a single structure for an item.</span></span>

<span data-ttu-id="dd738-103">**注意：** 并非所有服务均为列出的所有哈希属性提供值。</span><span class="sxs-lookup"><span data-stu-id="dd738-103">**Note:** Not all services provide a value for all hash properties listed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dd738-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dd738-104">JSON representation</span></span>

<span data-ttu-id="dd738-105">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd738-105">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="dd738-106">属性</span><span class="sxs-lookup"><span data-stu-id="dd738-106">Properties</span></span>

| <span data-ttu-id="dd738-107">属性</span><span class="sxs-lookup"><span data-stu-id="dd738-107">Property</span></span>         | <span data-ttu-id="dd738-108">类型</span><span class="sxs-lookup"><span data-stu-id="dd738-108">Type</span></span>   | <span data-ttu-id="dd738-109">说明</span><span class="sxs-lookup"><span data-stu-id="dd738-109">Description</span></span>                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| <span data-ttu-id="dd738-110">**sha1Hash**</span><span class="sxs-lookup"><span data-stu-id="dd738-110">**sha1Hash**</span></span>     | <span data-ttu-id="dd738-111">String</span><span class="sxs-lookup"><span data-stu-id="dd738-111">String</span></span> | <span data-ttu-id="dd738-p101">文件内容的 SHA1 哈希（如果可用）。只读。</span><span class="sxs-lookup"><span data-stu-id="dd738-p101">SHA1 hash for the contents of the file (if available). Read-only.</span></span> |
| <span data-ttu-id="dd738-114">**crc32Hash**</span><span class="sxs-lookup"><span data-stu-id="dd738-114">**crc32Hash**</span></span>    | <span data-ttu-id="dd738-115">String</span><span class="sxs-lookup"><span data-stu-id="dd738-115">String</span></span> | <span data-ttu-id="dd738-116">文件的 CRC32 值, 以小字节序 (如果可用) 为单位。</span><span class="sxs-lookup"><span data-stu-id="dd738-116">The CRC32 value of the file in little endian (if available).</span></span> <span data-ttu-id="dd738-117">只读。</span><span class="sxs-lookup"><span data-stu-id="dd738-117">Read-only.</span></span>            |
| <span data-ttu-id="dd738-118">**quickXorHash**</span><span class="sxs-lookup"><span data-stu-id="dd738-118">**quickXorHash**</span></span> | <span data-ttu-id="dd738-119">String</span><span class="sxs-lookup"><span data-stu-id="dd738-119">String</span></span> | <span data-ttu-id="dd738-p103">文件的专有哈希，可用于确定文件内容是否更改（如果存在）。只读。</span><span class="sxs-lookup"><span data-stu-id="dd738-p103">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available). Read-only.</span></span> |

<span data-ttu-id="dd738-p104">**注意：** 在某些情况下，哈希值不可用。如果出现这种情况，将在下载项后对项上的哈希值进行更新。</span><span class="sxs-lookup"><span data-stu-id="dd738-p104">**Note:** In some cases hash values may not be available. If this is the case, the hash values on an item will be updated after the item is downloaded.</span></span>

## <a name="remarks"></a><span data-ttu-id="dd738-124">注解</span><span class="sxs-lookup"><span data-stu-id="dd738-124">Remarks</span></span>

<span data-ttu-id="dd738-125">在 OneDrive for Business 和 SharePoint Server 2016 中，**sha1Hash** 和 **crc32Hash** 不可用。</span><span class="sxs-lookup"><span data-stu-id="dd738-125">In OneDrive for Business and SharePoint Server 2016, **sha1Hash** and **crc32Hash** are not available.</span></span>

<span data-ttu-id="dd738-126">在 OneDrive 个人版中，**quickXorHash** 不可用。</span><span class="sxs-lookup"><span data-stu-id="dd738-126">In OneDrive Personal, **quickXorHash** is not available.</span></span>

<span data-ttu-id="dd738-127">若要计算文件的 **quickXorHash**，请参阅 [QuickXorHash 代码片段](https://dev.onedrive.com/snippets/quickxorhash.htm)。</span><span class="sxs-lookup"><span data-stu-id="dd738-127">To calculate **quickXorHash** for a file, refer to the [QuickXorHash snippet](https://dev.onedrive.com/snippets/quickxorhash.htm).</span></span>
<span data-ttu-id="dd738-128">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="dd738-128">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes"
} -->
