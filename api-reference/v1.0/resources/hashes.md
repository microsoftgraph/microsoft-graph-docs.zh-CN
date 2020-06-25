---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
localization_priority: Normal
title: Hashes 资源类型
description: 哈希资源将可用哈希分组到项的单个结构中。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: da326576b148fdaee79ebfc3df2d7832bfeee4e5
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863738"
---
# <a name="hashes-resource-type"></a><span data-ttu-id="a0afc-103">Hashes 资源类型</span><span class="sxs-lookup"><span data-stu-id="a0afc-103">Hashes resource type</span></span>

<span data-ttu-id="a0afc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0afc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a0afc-105">**哈希**资源将可用哈希分组到项的单个结构中。</span><span class="sxs-lookup"><span data-stu-id="a0afc-105">The **Hashes** resource groups available hashes into a single structure for an item.</span></span>

<span data-ttu-id="a0afc-106">**注意：** 并非所有服务均为列出的所有哈希属性提供值。</span><span class="sxs-lookup"><span data-stu-id="a0afc-106">**Note:** Not all services provide a value for all hash properties listed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a0afc-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a0afc-107">JSON representation</span></span>

<span data-ttu-id="a0afc-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0afc-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="a0afc-109">属性</span><span class="sxs-lookup"><span data-stu-id="a0afc-109">Properties</span></span>

| <span data-ttu-id="a0afc-110">属性</span><span class="sxs-lookup"><span data-stu-id="a0afc-110">Property</span></span>         | <span data-ttu-id="a0afc-111">类型</span><span class="sxs-lookup"><span data-stu-id="a0afc-111">Type</span></span>   | <span data-ttu-id="a0afc-112">说明</span><span class="sxs-lookup"><span data-stu-id="a0afc-112">Description</span></span>                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| <span data-ttu-id="a0afc-113">**sha1Hash**</span><span class="sxs-lookup"><span data-stu-id="a0afc-113">**sha1Hash**</span></span>     | <span data-ttu-id="a0afc-114">String</span><span class="sxs-lookup"><span data-stu-id="a0afc-114">String</span></span> | <span data-ttu-id="a0afc-115">SHA1 hash for the contents of the file (if available).</span><span class="sxs-lookup"><span data-stu-id="a0afc-115">SHA1 hash for the contents of the file (if available).</span></span> <span data-ttu-id="a0afc-116">Read-only.</span><span class="sxs-lookup"><span data-stu-id="a0afc-116">Read-only.</span></span> |
| <span data-ttu-id="a0afc-117">**sha256Hash**</span><span class="sxs-lookup"><span data-stu-id="a0afc-117">**sha256Hash**</span></span>   | <span data-ttu-id="a0afc-118">String</span><span class="sxs-lookup"><span data-stu-id="a0afc-118">String</span></span> | <span data-ttu-id="a0afc-119">文件内容的 SHA256 哈希值（如果有）。</span><span class="sxs-lookup"><span data-stu-id="a0afc-119">SHA256 hash for the contents of the file (if available).</span></span> <span data-ttu-id="a0afc-120">只读。</span><span class="sxs-lookup"><span data-stu-id="a0afc-120">Read-only.</span></span> |
| <span data-ttu-id="a0afc-121">**crc32Hash**</span><span class="sxs-lookup"><span data-stu-id="a0afc-121">**crc32Hash**</span></span>    | <span data-ttu-id="a0afc-122">String</span><span class="sxs-lookup"><span data-stu-id="a0afc-122">String</span></span> | <span data-ttu-id="a0afc-123">文件的 CRC32 值，以小字节序（如果可用）为单位。</span><span class="sxs-lookup"><span data-stu-id="a0afc-123">The CRC32 value of the file in little endian (if available).</span></span> <span data-ttu-id="a0afc-124">只读。</span><span class="sxs-lookup"><span data-stu-id="a0afc-124">Read-only.</span></span>            |
| <span data-ttu-id="a0afc-125">**quickXorHash**</span><span class="sxs-lookup"><span data-stu-id="a0afc-125">**quickXorHash**</span></span> | <span data-ttu-id="a0afc-126">String</span><span class="sxs-lookup"><span data-stu-id="a0afc-126">String</span></span> | <span data-ttu-id="a0afc-127">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available).</span><span class="sxs-lookup"><span data-stu-id="a0afc-127">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available).</span></span> <span data-ttu-id="a0afc-128">Read-only.</span><span class="sxs-lookup"><span data-stu-id="a0afc-128">Read-only.</span></span> |

<span data-ttu-id="a0afc-129">**Note:** In some cases hash values may not be available.</span><span class="sxs-lookup"><span data-stu-id="a0afc-129">**Note:** In some cases hash values may not be available.</span></span> <span data-ttu-id="a0afc-130">If this is the case, the hash values on an item will be updated after the item is downloaded.</span><span class="sxs-lookup"><span data-stu-id="a0afc-130">If this is the case, the hash values on an item will be updated after the item is downloaded.</span></span>

## <a name="remarks"></a><span data-ttu-id="a0afc-131">注解</span><span class="sxs-lookup"><span data-stu-id="a0afc-131">Remarks</span></span>

<span data-ttu-id="a0afc-132">在 OneDrive for Business 和 SharePoint Server 2016 中， **sha1Hash**和**Crc32Hash**，并且**sha256Hash**不可用。</span><span class="sxs-lookup"><span data-stu-id="a0afc-132">In OneDrive for Business and SharePoint Server 2016, **sha1Hash** and **crc32Hash**, and **sha256Hash** are not available.</span></span>

<span data-ttu-id="a0afc-133">在 OneDrive 个人版中，**quickXorHash** 不可用。</span><span class="sxs-lookup"><span data-stu-id="a0afc-133">In OneDrive Personal, **quickXorHash** is not available.</span></span>

<span data-ttu-id="a0afc-134">若要计算文件的 **quickXorHash**，请参阅 [QuickXorHash 代码片段](https://dev.onedrive.com/snippets/quickxorhash.htm)。</span><span class="sxs-lookup"><span data-stu-id="a0afc-134">To calculate **quickXorHash** for a file, refer to the [QuickXorHash snippet](https://dev.onedrive.com/snippets/quickxorhash.htm).</span></span>
<span data-ttu-id="a0afc-135">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="a0afc-135">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes"
} -->
