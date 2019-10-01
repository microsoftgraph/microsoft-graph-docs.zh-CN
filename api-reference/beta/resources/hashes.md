---
author: JeremyKelley
description: 哈希资源将可用哈希分组到项的单个结构中。
ms.date: 09/10/2017
title: 希
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: b620170cf05e8e04cb4368874ea20d29c5440298
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333246"
---
# <a name="hashes-resource-type"></a><span data-ttu-id="54b33-103">哈希资源类型</span><span class="sxs-lookup"><span data-stu-id="54b33-103">hashes resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54b33-104">将可用哈希分组到一个项的单个结构中。</span><span class="sxs-lookup"><span data-stu-id="54b33-104">Groups available hashes into a single structure for an item.</span></span>

> [!NOTE]
> <span data-ttu-id="54b33-105">并非所有服务都为列出的所有哈希属性提供值。</span><span class="sxs-lookup"><span data-stu-id="54b33-105">Not all services provide a value for all hash properties listed.</span></span> <span data-ttu-id="54b33-106">在 OneDrive for Business 和 SharePoint Server 2016 中， **sha1Hash**、 **crc32Hash**和**sha256Hash**不可用。</span><span class="sxs-lookup"><span data-stu-id="54b33-106">In OneDrive for Business and SharePoint Server 2016, **sha1Hash**, **crc32Hash**, and **sha256Hash** are not available.</span></span> <span data-ttu-id="54b33-107">在 OneDrive 个人版中，**quickXorHash** 不可用。</span><span class="sxs-lookup"><span data-stu-id="54b33-107">In OneDrive Personal, **quickXorHash** is not available.</span></span>

## <a name="properties"></a><span data-ttu-id="54b33-108">属性</span><span class="sxs-lookup"><span data-stu-id="54b33-108">Properties</span></span>

| <span data-ttu-id="54b33-109">属性</span><span class="sxs-lookup"><span data-stu-id="54b33-109">Property</span></span>         | <span data-ttu-id="54b33-110">类型</span><span class="sxs-lookup"><span data-stu-id="54b33-110">Type</span></span>   | <span data-ttu-id="54b33-111">说明</span><span class="sxs-lookup"><span data-stu-id="54b33-111">Description</span></span>                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| <span data-ttu-id="54b33-112">**sha1Hash**</span><span class="sxs-lookup"><span data-stu-id="54b33-112">**sha1Hash**</span></span>     | <span data-ttu-id="54b33-113">String</span><span class="sxs-lookup"><span data-stu-id="54b33-113">String</span></span> | <span data-ttu-id="54b33-p102">文件内容的 SHA1 哈希（如果可用）。只读。</span><span class="sxs-lookup"><span data-stu-id="54b33-p102">SHA1 hash for the contents of the file (if available). Read-only.</span></span> |
| <span data-ttu-id="54b33-116">**sha256Hash**</span><span class="sxs-lookup"><span data-stu-id="54b33-116">**sha256Hash**</span></span>   | <span data-ttu-id="54b33-117">String</span><span class="sxs-lookup"><span data-stu-id="54b33-117">String</span></span> | <span data-ttu-id="54b33-118">文件内容的 SHA256 哈希值（如果有）。</span><span class="sxs-lookup"><span data-stu-id="54b33-118">SHA256 hash for the contents of the file (if available).</span></span> <span data-ttu-id="54b33-119">只读。</span><span class="sxs-lookup"><span data-stu-id="54b33-119">Read-only.</span></span> |
| <span data-ttu-id="54b33-120">**crc32Hash**</span><span class="sxs-lookup"><span data-stu-id="54b33-120">**crc32Hash**</span></span>    | <span data-ttu-id="54b33-121">String</span><span class="sxs-lookup"><span data-stu-id="54b33-121">String</span></span> | <span data-ttu-id="54b33-p104">文件的 CRC32 值（如果可用）。只读。</span><span class="sxs-lookup"><span data-stu-id="54b33-p104">The CRC32 value of the file (if available). Read-only.</span></span>            |
| <span data-ttu-id="54b33-124">**quickXorHash**</span><span class="sxs-lookup"><span data-stu-id="54b33-124">**quickXorHash**</span></span> | <span data-ttu-id="54b33-125">String</span><span class="sxs-lookup"><span data-stu-id="54b33-125">String</span></span> | <span data-ttu-id="54b33-p105">文件的专有哈希，可用于确定文件内容是否更改（如果存在）。只读。</span><span class="sxs-lookup"><span data-stu-id="54b33-p105">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available). Read-only.</span></span> |

> <span data-ttu-id="54b33-128">**注意：** 在哈希值不可用的情况下，项目的哈希值将在项目下载后进行更新。</span><span class="sxs-lookup"><span data-stu-id="54b33-128">**Note:** In cases where the hash values are not available, the hash values on an item will be updated after the item is downloaded.</span></span>

## <a name="json-representation"></a><span data-ttu-id="54b33-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="54b33-129">JSON representation</span></span>

<span data-ttu-id="54b33-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="54b33-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "sha1Hash", "crc32Hash", "quickXorHash" ],
  "@odata.type": "microsoft.graph.hashes"
}-->

```json
{
  "crc32Hash": "string (hex)",
  "sha1Hash": "string (hex)",
  "sha256Hash": "string (hex)",
  "quickXorHash": "string (base64)"
}
```

## <a name="see-also"></a><span data-ttu-id="54b33-131">另请参阅</span><span class="sxs-lookup"><span data-stu-id="54b33-131">See also</span></span>

- <span data-ttu-id="54b33-132">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="54b33-132">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
- <span data-ttu-id="54b33-133">若要计算文件的 **quickXorHash**，请参阅 [QuickXorHash 代码片段](https://dev.onedrive.com/snippets/quickxorhash.htm)。</span><span class="sxs-lookup"><span data-stu-id="54b33-133">To calculate **quickXorHash** for a file, refer to the [QuickXorHash snippet](https://dev.onedrive.com/snippets/quickxorhash.htm).</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes",
  "suppressions": []
}
-->
