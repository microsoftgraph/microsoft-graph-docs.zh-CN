---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
localization_priority: Normal
title: Hashes 资源类型
description: 哈希资源将可用哈希分组到项的单个结构中。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 807b2155114d0fa689de5dab60b2e21d7745ef99
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48062923"
---
# <a name="hashes-resource-type"></a><span data-ttu-id="61a17-103">Hashes 资源类型</span><span class="sxs-lookup"><span data-stu-id="61a17-103">Hashes resource type</span></span>

<span data-ttu-id="61a17-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61a17-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="61a17-105">**哈希**资源将可用哈希分组到项的单个结构中。</span><span class="sxs-lookup"><span data-stu-id="61a17-105">The **Hashes** resource groups available hashes into a single structure for an item.</span></span>

<span data-ttu-id="61a17-106">**注意：** 并非所有服务均为列出的所有哈希属性提供值。</span><span class="sxs-lookup"><span data-stu-id="61a17-106">**Note:** Not all services provide a value for all hash properties listed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="61a17-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="61a17-107">JSON representation</span></span>

<span data-ttu-id="61a17-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="61a17-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="61a17-109">属性</span><span class="sxs-lookup"><span data-stu-id="61a17-109">Properties</span></span>

| <span data-ttu-id="61a17-110">属性</span><span class="sxs-lookup"><span data-stu-id="61a17-110">Property</span></span>         | <span data-ttu-id="61a17-111">类型</span><span class="sxs-lookup"><span data-stu-id="61a17-111">Type</span></span>   | <span data-ttu-id="61a17-112">说明</span><span class="sxs-lookup"><span data-stu-id="61a17-112">Description</span></span>                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| <span data-ttu-id="61a17-113">**sha1Hash**</span><span class="sxs-lookup"><span data-stu-id="61a17-113">**sha1Hash**</span></span>     | <span data-ttu-id="61a17-114">String</span><span class="sxs-lookup"><span data-stu-id="61a17-114">String</span></span> | <span data-ttu-id="61a17-p101">文件内容的 SHA1 哈希（如果可用）。只读。</span><span class="sxs-lookup"><span data-stu-id="61a17-p101">SHA1 hash for the contents of the file (if available). Read-only.</span></span> |
| <span data-ttu-id="61a17-117">**sha256Hash**</span><span class="sxs-lookup"><span data-stu-id="61a17-117">**sha256Hash**</span></span>   | <span data-ttu-id="61a17-118">String</span><span class="sxs-lookup"><span data-stu-id="61a17-118">String</span></span> | <span data-ttu-id="61a17-119">如果可用) ，则为文件的内容 (SHA256 哈希。</span><span class="sxs-lookup"><span data-stu-id="61a17-119">SHA256 hash for the contents of the file (if available).</span></span> <span data-ttu-id="61a17-120">只读。</span><span class="sxs-lookup"><span data-stu-id="61a17-120">Read-only.</span></span> |
| <span data-ttu-id="61a17-121">**crc32Hash**</span><span class="sxs-lookup"><span data-stu-id="61a17-121">**crc32Hash**</span></span>    | <span data-ttu-id="61a17-122">String</span><span class="sxs-lookup"><span data-stu-id="61a17-122">String</span></span> | <span data-ttu-id="61a17-123">如果可用) ，则 CRC32 的文件的值以小 endian (。</span><span class="sxs-lookup"><span data-stu-id="61a17-123">The CRC32 value of the file in little endian (if available).</span></span> <span data-ttu-id="61a17-124">只读。</span><span class="sxs-lookup"><span data-stu-id="61a17-124">Read-only.</span></span>            |
| <span data-ttu-id="61a17-125">**quickXorHash**</span><span class="sxs-lookup"><span data-stu-id="61a17-125">**quickXorHash**</span></span> | <span data-ttu-id="61a17-126">String</span><span class="sxs-lookup"><span data-stu-id="61a17-126">String</span></span> | <span data-ttu-id="61a17-p104">文件的专有哈希，可用于确定文件内容是否更改（如果存在）。只读。</span><span class="sxs-lookup"><span data-stu-id="61a17-p104">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available). Read-only.</span></span> |

<span data-ttu-id="61a17-p105">**注意：** 在某些情况下，哈希值不可用。如果出现这种情况，将在下载项后对项上的哈希值进行更新。</span><span class="sxs-lookup"><span data-stu-id="61a17-p105">**Note:** In some cases hash values may not be available. If this is the case, the hash values on an item will be updated after the item is downloaded.</span></span>

## <a name="remarks"></a><span data-ttu-id="61a17-131">注解</span><span class="sxs-lookup"><span data-stu-id="61a17-131">Remarks</span></span>

<span data-ttu-id="61a17-132">在 OneDrive for Business 和 SharePoint Server 2016 中， **sha1Hash** 和 **Crc32Hash**，并且 **sha256Hash** 不可用。</span><span class="sxs-lookup"><span data-stu-id="61a17-132">In OneDrive for Business and SharePoint Server 2016, **sha1Hash** and **crc32Hash**, and **sha256Hash** are not available.</span></span>

<span data-ttu-id="61a17-133">在 OneDrive 个人版中，**quickXorHash** 不可用。</span><span class="sxs-lookup"><span data-stu-id="61a17-133">In OneDrive Personal, **quickXorHash** is not available.</span></span>

<span data-ttu-id="61a17-134">若要计算文件的 **quickXorHash**，请参阅 [QuickXorHash 代码片段](https://dev.onedrive.com/snippets/quickxorhash.htm)。</span><span class="sxs-lookup"><span data-stu-id="61a17-134">To calculate **quickXorHash** for a file, refer to the [QuickXorHash snippet](https://dev.onedrive.com/snippets/quickxorhash.htm).</span></span>
<span data-ttu-id="61a17-135">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="61a17-135">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes"
} -->

