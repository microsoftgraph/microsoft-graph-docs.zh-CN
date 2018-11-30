---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 哈希
ms.openlocfilehash: 2387af83450f667aa4732cc46d7d3cf2111579f0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041771"
---
# <a name="hashes-resource-type"></a><span data-ttu-id="79cc2-102">Hashes 资源类型</span><span class="sxs-lookup"><span data-stu-id="79cc2-102">Hashes resource type</span></span>

> <span data-ttu-id="79cc2-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="79cc2-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="79cc2-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="79cc2-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="79cc2-105">**哈希**资源将可用哈希分组到项的单个结构中。</span><span class="sxs-lookup"><span data-stu-id="79cc2-105">The **Hashes** resource groups available hashes into a single structure for an item.</span></span>

<span data-ttu-id="79cc2-106">**注意：** 并非所有服务均为列出的所有哈希属性提供值。</span><span class="sxs-lookup"><span data-stu-id="79cc2-106">**Note:** Not all services provide a value for all hash properties listed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="79cc2-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="79cc2-107">JSON representation</span></span>

<span data-ttu-id="79cc2-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="79cc2-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="79cc2-109">属性</span><span class="sxs-lookup"><span data-stu-id="79cc2-109">Properties</span></span>

| <span data-ttu-id="79cc2-110">属性</span><span class="sxs-lookup"><span data-stu-id="79cc2-110">Property</span></span>         | <span data-ttu-id="79cc2-111">类型</span><span class="sxs-lookup"><span data-stu-id="79cc2-111">Type</span></span>   | <span data-ttu-id="79cc2-112">说明</span><span class="sxs-lookup"><span data-stu-id="79cc2-112">Description</span></span>                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| <span data-ttu-id="79cc2-113">**sha1Hash**</span><span class="sxs-lookup"><span data-stu-id="79cc2-113">**sha1Hash**</span></span>     | <span data-ttu-id="79cc2-114">String</span><span class="sxs-lookup"><span data-stu-id="79cc2-114">String</span></span> | <span data-ttu-id="79cc2-p102">文件内容的 SHA1 哈希（如果可用）。只读。</span><span class="sxs-lookup"><span data-stu-id="79cc2-p102">SHA1 hash for the contents of the file (if available). Read-only.</span></span> |
| <span data-ttu-id="79cc2-117">**crc32Hash**</span><span class="sxs-lookup"><span data-stu-id="79cc2-117">**crc32Hash**</span></span>    | <span data-ttu-id="79cc2-118">String</span><span class="sxs-lookup"><span data-stu-id="79cc2-118">String</span></span> | <span data-ttu-id="79cc2-p103">文件的 CRC32 值（如果可用）。只读。</span><span class="sxs-lookup"><span data-stu-id="79cc2-p103">The CRC32 value of the file (if available). Read-only.</span></span>            |
| <span data-ttu-id="79cc2-121">**quickXorHash**</span><span class="sxs-lookup"><span data-stu-id="79cc2-121">**quickXorHash**</span></span> | <span data-ttu-id="79cc2-122">String</span><span class="sxs-lookup"><span data-stu-id="79cc2-122">String</span></span> | <span data-ttu-id="79cc2-p104">文件的专有哈希，可用于确定文件内容是否更改（如果存在）。只读。</span><span class="sxs-lookup"><span data-stu-id="79cc2-p104">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available). Read-only.</span></span> |

<span data-ttu-id="79cc2-p105">**注意：** 在某些情况下，哈希值不可用。如果出现这种情况，将在下载项后对项上的哈希值进行更新。</span><span class="sxs-lookup"><span data-stu-id="79cc2-p105">**Note:** In some cases hash values may not be available. If this is the case, the hash values on an item will be updated after the item is downloaded.</span></span>

## <a name="remarks"></a><span data-ttu-id="79cc2-127">注解</span><span class="sxs-lookup"><span data-stu-id="79cc2-127">Remarks</span></span>

<span data-ttu-id="79cc2-128">在 OneDrive for Business 和 SharePoint Server 2016 中，**sha1Hash** 和 **crc32Hash** 不可用。</span><span class="sxs-lookup"><span data-stu-id="79cc2-128">In OneDrive for Business and SharePoint Server 2016, **sha1Hash** and **crc32Hash** are not available.</span></span>

<span data-ttu-id="79cc2-129">在 OneDrive 个人版中，**quickXorHash** 不可用。</span><span class="sxs-lookup"><span data-stu-id="79cc2-129">In OneDrive Personal, **quickXorHash** is not available.</span></span>

<span data-ttu-id="79cc2-130">若要计算文件的 **quickXorHash**，请参阅 [QuickXorHash 代码片段](https://dev.onedrive.com/snippets/quickxorhash.htm)。</span><span class="sxs-lookup"><span data-stu-id="79cc2-130">To calculate **quickXorHash** for a file, refer to the [QuickXorHash snippet](https://dev.onedrive.com/snippets/quickxorhash.htm).</span></span>

<span data-ttu-id="79cc2-131">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="79cc2-131">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes"
} -->
