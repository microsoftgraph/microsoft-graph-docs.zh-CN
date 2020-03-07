---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
localization_priority: Normal
title: Hashes 资源类型
description: 哈希资源将可用哈希分组到项的单个结构中。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: cb852ad01394ac463cb3d23ed404a7956bbf1eea
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532911"
---
# <a name="hashes-resource-type"></a><span data-ttu-id="f9a93-103">Hashes 资源类型</span><span class="sxs-lookup"><span data-stu-id="f9a93-103">Hashes resource type</span></span>

<span data-ttu-id="f9a93-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9a93-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f9a93-105">**哈希**资源将可用哈希分组到项的单个结构中。</span><span class="sxs-lookup"><span data-stu-id="f9a93-105">The **Hashes** resource groups available hashes into a single structure for an item.</span></span>

<span data-ttu-id="f9a93-106">**注意：** 并非所有服务均为列出的所有哈希属性提供值。</span><span class="sxs-lookup"><span data-stu-id="f9a93-106">**Note:** Not all services provide a value for all hash properties listed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f9a93-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f9a93-107">JSON representation</span></span>

<span data-ttu-id="f9a93-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f9a93-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="f9a93-109">属性</span><span class="sxs-lookup"><span data-stu-id="f9a93-109">Properties</span></span>

| <span data-ttu-id="f9a93-110">属性</span><span class="sxs-lookup"><span data-stu-id="f9a93-110">Property</span></span>         | <span data-ttu-id="f9a93-111">类型</span><span class="sxs-lookup"><span data-stu-id="f9a93-111">Type</span></span>   | <span data-ttu-id="f9a93-112">说明</span><span class="sxs-lookup"><span data-stu-id="f9a93-112">Description</span></span>                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| <span data-ttu-id="f9a93-113">**sha1Hash**</span><span class="sxs-lookup"><span data-stu-id="f9a93-113">**sha1Hash**</span></span>     | <span data-ttu-id="f9a93-114">String</span><span class="sxs-lookup"><span data-stu-id="f9a93-114">String</span></span> | <span data-ttu-id="f9a93-p101">文件内容的 SHA1 哈希（如果可用）。只读。</span><span class="sxs-lookup"><span data-stu-id="f9a93-p101">SHA1 hash for the contents of the file (if available). Read-only.</span></span> |
| <span data-ttu-id="f9a93-117">**crc32Hash**</span><span class="sxs-lookup"><span data-stu-id="f9a93-117">**crc32Hash**</span></span>    | <span data-ttu-id="f9a93-118">String</span><span class="sxs-lookup"><span data-stu-id="f9a93-118">String</span></span> | <span data-ttu-id="f9a93-119">文件的 CRC32 值，以小字节序（如果可用）为单位。</span><span class="sxs-lookup"><span data-stu-id="f9a93-119">The CRC32 value of the file in little endian (if available).</span></span> <span data-ttu-id="f9a93-120">只读。</span><span class="sxs-lookup"><span data-stu-id="f9a93-120">Read-only.</span></span>            |
| <span data-ttu-id="f9a93-121">**quickXorHash**</span><span class="sxs-lookup"><span data-stu-id="f9a93-121">**quickXorHash**</span></span> | <span data-ttu-id="f9a93-122">String</span><span class="sxs-lookup"><span data-stu-id="f9a93-122">String</span></span> | <span data-ttu-id="f9a93-p103">文件的专有哈希，可用于确定文件内容是否更改（如果存在）。只读。</span><span class="sxs-lookup"><span data-stu-id="f9a93-p103">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available). Read-only.</span></span> |

<span data-ttu-id="f9a93-p104">**注意：** 在某些情况下，哈希值不可用。如果出现这种情况，将在下载项后对项上的哈希值进行更新。</span><span class="sxs-lookup"><span data-stu-id="f9a93-p104">**Note:** In some cases hash values may not be available. If this is the case, the hash values on an item will be updated after the item is downloaded.</span></span>

## <a name="remarks"></a><span data-ttu-id="f9a93-127">注解</span><span class="sxs-lookup"><span data-stu-id="f9a93-127">Remarks</span></span>

<span data-ttu-id="f9a93-128">在 OneDrive for Business 和 SharePoint Server 2016 中，**sha1Hash** 和 **crc32Hash** 不可用。</span><span class="sxs-lookup"><span data-stu-id="f9a93-128">In OneDrive for Business and SharePoint Server 2016, **sha1Hash** and **crc32Hash** are not available.</span></span>

<span data-ttu-id="f9a93-129">在 OneDrive 个人版中，**quickXorHash** 不可用。</span><span class="sxs-lookup"><span data-stu-id="f9a93-129">In OneDrive Personal, **quickXorHash** is not available.</span></span>

<span data-ttu-id="f9a93-130">若要计算文件的 **quickXorHash**，请参阅 [QuickXorHash 代码片段](https://dev.onedrive.com/snippets/quickxorhash.htm)。</span><span class="sxs-lookup"><span data-stu-id="f9a93-130">To calculate **quickXorHash** for a file, refer to the [QuickXorHash snippet](https://dev.onedrive.com/snippets/quickxorhash.htm).</span></span>
<span data-ttu-id="f9a93-131">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="f9a93-131">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes"
} -->
