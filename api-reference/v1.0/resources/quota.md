---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 配额
localization_priority: Normal
description: 配额资源提供有关 驱动器 资源上的空间限制的详细信息。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ee93ddfe54e785ea8a8fa245ab3828c548928cc0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034956"
---
# <a name="quota-resource-type"></a><span data-ttu-id="8eee5-103">Quota 资源类型</span><span class="sxs-lookup"><span data-stu-id="8eee5-103">Quota resource type</span></span>

<span data-ttu-id="8eee5-104">**配额**资源提供有关 [驱动器](drive.md) 资源上的空间限制的详细信息。</span><span class="sxs-lookup"><span data-stu-id="8eee5-104">The **quota** resource provides details about space constrains on a [Drive](drive.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8eee5-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8eee5-105">JSON representation</span></span>

<span data-ttu-id="8eee5-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8eee5-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.quota"
}-->

```json
{
  "deleted": 1024,
  "remaining": 1024,
  "state": "normal | nearing | critical | exceeded",
  "total": 1024,
  "used": 1024
}
```

## <a name="properties"></a><span data-ttu-id="8eee5-107">属性</span><span class="sxs-lookup"><span data-stu-id="8eee5-107">Properties</span></span>

| <span data-ttu-id="8eee5-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="8eee5-108">Property name</span></span> | <span data-ttu-id="8eee5-109">类型</span><span class="sxs-lookup"><span data-stu-id="8eee5-109">Type</span></span>   | <span data-ttu-id="8eee5-110">说明</span><span class="sxs-lookup"><span data-stu-id="8eee5-110">Description</span></span>                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| <span data-ttu-id="8eee5-111">total</span><span class="sxs-lookup"><span data-stu-id="8eee5-111">total</span></span>         | <span data-ttu-id="8eee5-112">Int64</span><span class="sxs-lookup"><span data-stu-id="8eee5-112">Int64</span></span>  | <span data-ttu-id="8eee5-p101">允许的总存储空间，以字节为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="8eee5-p101">Total allowed storage space, in bytes. Read-only.</span></span>                           |
| <span data-ttu-id="8eee5-115">used</span><span class="sxs-lookup"><span data-stu-id="8eee5-115">used</span></span>          | <span data-ttu-id="8eee5-116">Int64</span><span class="sxs-lookup"><span data-stu-id="8eee5-116">Int64</span></span>  | <span data-ttu-id="8eee5-p102">已使用的总空间，以字节为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="8eee5-p102">Total space used, in bytes. Read-only.</span></span>                                      |
| <span data-ttu-id="8eee5-119">remaining</span><span class="sxs-lookup"><span data-stu-id="8eee5-119">remaining</span></span>     | <span data-ttu-id="8eee5-120">Int64</span><span class="sxs-lookup"><span data-stu-id="8eee5-120">Int64</span></span>  | <span data-ttu-id="8eee5-p103">达到配额限制之前剩余的总空间，以字节为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="8eee5-p103">Total space remaining before reaching the quota limit, in bytes. Read-only.</span></span> |
| <span data-ttu-id="8eee5-123">deleted</span><span class="sxs-lookup"><span data-stu-id="8eee5-123">deleted</span></span>       | <span data-ttu-id="8eee5-124">Int64</span><span class="sxs-lookup"><span data-stu-id="8eee5-124">Int64</span></span>  | <span data-ttu-id="8eee5-p104">回收站中的文件占用的总空间，以字节为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="8eee5-p104">Total space consumed by files in the recycle bin, in bytes. Read-only.</span></span>      |
| <span data-ttu-id="8eee5-127">state</span><span class="sxs-lookup"><span data-stu-id="8eee5-127">state</span></span>         | <span data-ttu-id="8eee5-128">string</span><span class="sxs-lookup"><span data-stu-id="8eee5-128">string</span></span> | <span data-ttu-id="8eee5-p105">指示存储空间状态的枚举值。只读。</span><span class="sxs-lookup"><span data-stu-id="8eee5-p105">Enumeration value that indicates the state of the storage space. Read-only.</span></span> |

## <a name="state-enumeration"></a><span data-ttu-id="8eee5-131">状态枚举</span><span class="sxs-lookup"><span data-stu-id="8eee5-131">State Enumeration</span></span>

| <span data-ttu-id="8eee5-132">值</span><span class="sxs-lookup"><span data-stu-id="8eee5-132">Value</span></span>      | <span data-ttu-id="8eee5-133">说明</span><span class="sxs-lookup"><span data-stu-id="8eee5-133">Description</span></span>                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | <span data-ttu-id="8eee5-134">驱动器具有充足的剩余配额。</span><span class="sxs-lookup"><span data-stu-id="8eee5-134">The drive has plenty of remaining quota left.</span></span>                                                                                                                               |
| `nearing`  | <span data-ttu-id="8eee5-135">剩余配额少于总配额空间的 10%。</span><span class="sxs-lookup"><span data-stu-id="8eee5-135">Remaining quota is less than 10% of total quota space.</span></span>                                                                                                                      |
| `critical` | <span data-ttu-id="8eee5-136">剩余配额少于总配额空间的 1%。</span><span class="sxs-lookup"><span data-stu-id="8eee5-136">Remaining quota is less than 1% of total quota space.</span></span>                                                                                                                       |
| `exceeded` | <span data-ttu-id="8eee5-p106">使用的配额已超出总配额。在驱动器低于总配额量或购买更多存储空间之前，无法向该驱动器添加新的文件或文件夹。</span><span class="sxs-lookup"><span data-stu-id="8eee5-p106">The used quota has exceeded the total quota. New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span></span> |

<!-- {
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/quota.md:
      Found potential enums in resource example that weren't defined in a table:(normal, nearing,critical,exceeded) are in resource, but () are in table"
  ],
  "tocPath": "Facets/Quota"
} -->
