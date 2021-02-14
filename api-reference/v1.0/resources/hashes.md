---
author: JeremyKelley
ms.date: 09/10/2017
localization_priority: Normal
title: Hashes 资源类型
description: 哈希资源将可用哈希分组到项的单个结构中。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9b45d872966bc8eba3ef3d622b5b0e37c83122b6
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240001"
---
# <a name="hashes-resource-type"></a><span data-ttu-id="9b7ff-103">Hashes 资源类型</span><span class="sxs-lookup"><span data-stu-id="9b7ff-103">Hashes resource type</span></span>

<span data-ttu-id="9b7ff-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b7ff-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9b7ff-105">**哈希** 资源将可用哈希分组到项的单个结构中。</span><span class="sxs-lookup"><span data-stu-id="9b7ff-105">The **Hashes** resource groups available hashes into a single structure for an item.</span></span>

<span data-ttu-id="9b7ff-106">**注意：** 并非所有服务均为列出的所有哈希属性提供值。</span><span class="sxs-lookup"><span data-stu-id="9b7ff-106">**Note:** Not all services provide a value for all hash properties listed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b7ff-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9b7ff-107">JSON representation</span></span>

<span data-ttu-id="9b7ff-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9b7ff-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="9b7ff-109">属性</span><span class="sxs-lookup"><span data-stu-id="9b7ff-109">Properties</span></span>

| <span data-ttu-id="9b7ff-110">属性</span><span class="sxs-lookup"><span data-stu-id="9b7ff-110">Property</span></span>         | <span data-ttu-id="9b7ff-111">类型</span><span class="sxs-lookup"><span data-stu-id="9b7ff-111">Type</span></span>   | <span data-ttu-id="9b7ff-112">说明</span><span class="sxs-lookup"><span data-stu-id="9b7ff-112">Description</span></span>                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| <span data-ttu-id="9b7ff-113">**sha1Hash**</span><span class="sxs-lookup"><span data-stu-id="9b7ff-113">**sha1Hash**</span></span>     | <span data-ttu-id="9b7ff-114">String</span><span class="sxs-lookup"><span data-stu-id="9b7ff-114">String</span></span> | <span data-ttu-id="9b7ff-p101">文件内容的 SHA1 哈希（如果可用）。只读。</span><span class="sxs-lookup"><span data-stu-id="9b7ff-p101">SHA1 hash for the contents of the file (if available). Read-only.</span></span> |
| <span data-ttu-id="9b7ff-117">**sha256Hash**</span><span class="sxs-lookup"><span data-stu-id="9b7ff-117">**sha256Hash**</span></span>   | <span data-ttu-id="9b7ff-118">String</span><span class="sxs-lookup"><span data-stu-id="9b7ff-118">String</span></span> | <span data-ttu-id="9b7ff-119">文件内容的 SHA256 哈希 (（如果) ）。</span><span class="sxs-lookup"><span data-stu-id="9b7ff-119">SHA256 hash for the contents of the file (if available).</span></span> <span data-ttu-id="9b7ff-120">只读。</span><span class="sxs-lookup"><span data-stu-id="9b7ff-120">Read-only.</span></span> |
| <span data-ttu-id="9b7ff-121">**crc32Hash**</span><span class="sxs-lookup"><span data-stu-id="9b7ff-121">**crc32Hash**</span></span>    | <span data-ttu-id="9b7ff-122">String</span><span class="sxs-lookup"><span data-stu-id="9b7ff-122">String</span></span> | <span data-ttu-id="9b7ff-123">文件的 CRC32 值（如果可用， (以) 。</span><span class="sxs-lookup"><span data-stu-id="9b7ff-123">The CRC32 value of the file in little endian (if available).</span></span> <span data-ttu-id="9b7ff-124">只读。</span><span class="sxs-lookup"><span data-stu-id="9b7ff-124">Read-only.</span></span>            |
| <span data-ttu-id="9b7ff-125">**quickXorHash**</span><span class="sxs-lookup"><span data-stu-id="9b7ff-125">**quickXorHash**</span></span> | <span data-ttu-id="9b7ff-126">String</span><span class="sxs-lookup"><span data-stu-id="9b7ff-126">String</span></span> | <span data-ttu-id="9b7ff-p104">文件的专有哈希，可用于确定文件内容是否更改（如果存在）。只读。</span><span class="sxs-lookup"><span data-stu-id="9b7ff-p104">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available). Read-only.</span></span> |

<span data-ttu-id="9b7ff-p105">**注意：** 在某些情况下，哈希值不可用。如果出现这种情况，将在下载项后对项上的哈希值进行更新。</span><span class="sxs-lookup"><span data-stu-id="9b7ff-p105">**Note:** In some cases hash values may not be available. If this is the case, the hash values on an item will be updated after the item is downloaded.</span></span>

## <a name="remarks"></a><span data-ttu-id="9b7ff-131">注解</span><span class="sxs-lookup"><span data-stu-id="9b7ff-131">Remarks</span></span>

<span data-ttu-id="9b7ff-132">在 OneDrive for Business 和 SharePoint Server 2016 中 **，sha1Hash** 和 **crc32Hash** 和 **sha256Hash** 不可用。</span><span class="sxs-lookup"><span data-stu-id="9b7ff-132">In OneDrive for Business and SharePoint Server 2016, **sha1Hash** and **crc32Hash**, and **sha256Hash** are not available.</span></span>

<span data-ttu-id="9b7ff-133">在 OneDrive 个人版中，**quickXorHash** 不可用。</span><span class="sxs-lookup"><span data-stu-id="9b7ff-133">In OneDrive Personal, **quickXorHash** is not available.</span></span>

<span data-ttu-id="9b7ff-134">若要计算文件的 **quickXorHash**，请参阅 [QuickXorHash 代码片段](https://dev.onedrive.com/snippets/quickxorhash.htm)。</span><span class="sxs-lookup"><span data-stu-id="9b7ff-134">To calculate **quickXorHash** for a file, refer to the [QuickXorHash snippet](https://dev.onedrive.com/snippets/quickxorhash.htm).</span></span>
<span data-ttu-id="9b7ff-135">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="9b7ff-135">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes"
} -->

