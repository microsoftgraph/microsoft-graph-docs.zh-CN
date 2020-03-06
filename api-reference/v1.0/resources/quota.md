---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 配额
localization_priority: Normal
description: 配额资源提供有关 驱动器 资源上的空间限制的详细信息。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 53aad1392e66f610f85f30ae088dc6f8ca04df73
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533934"
---
# <a name="quota-resource-type"></a><span data-ttu-id="d328c-103">Quota 资源类型</span><span class="sxs-lookup"><span data-stu-id="d328c-103">Quota resource type</span></span>

<span data-ttu-id="d328c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d328c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d328c-105">**配额**资源提供有关 [驱动器](drive.md) 资源上的空间限制的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d328c-105">The **quota** resource provides details about space constrains on a [Drive](drive.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d328c-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d328c-106">JSON representation</span></span>

<span data-ttu-id="d328c-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d328c-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="d328c-108">属性</span><span class="sxs-lookup"><span data-stu-id="d328c-108">Properties</span></span>

| <span data-ttu-id="d328c-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="d328c-109">Property name</span></span> | <span data-ttu-id="d328c-110">类型</span><span class="sxs-lookup"><span data-stu-id="d328c-110">Type</span></span>   | <span data-ttu-id="d328c-111">说明</span><span class="sxs-lookup"><span data-stu-id="d328c-111">Description</span></span>                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| <span data-ttu-id="d328c-112">total</span><span class="sxs-lookup"><span data-stu-id="d328c-112">total</span></span>         | <span data-ttu-id="d328c-113">Int64</span><span class="sxs-lookup"><span data-stu-id="d328c-113">Int64</span></span>  | <span data-ttu-id="d328c-p101">允许的总存储空间，以字节为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="d328c-p101">Total allowed storage space, in bytes. Read-only.</span></span>                           |
| <span data-ttu-id="d328c-116">used</span><span class="sxs-lookup"><span data-stu-id="d328c-116">used</span></span>          | <span data-ttu-id="d328c-117">Int64</span><span class="sxs-lookup"><span data-stu-id="d328c-117">Int64</span></span>  | <span data-ttu-id="d328c-p102">已使用的总空间，以字节为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="d328c-p102">Total space used, in bytes. Read-only.</span></span>                                      |
| <span data-ttu-id="d328c-120">remaining</span><span class="sxs-lookup"><span data-stu-id="d328c-120">remaining</span></span>     | <span data-ttu-id="d328c-121">Int64</span><span class="sxs-lookup"><span data-stu-id="d328c-121">Int64</span></span>  | <span data-ttu-id="d328c-p103">达到配额限制之前剩余的总空间，以字节为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="d328c-p103">Total space remaining before reaching the quota limit, in bytes. Read-only.</span></span> |
| <span data-ttu-id="d328c-124">deleted</span><span class="sxs-lookup"><span data-stu-id="d328c-124">deleted</span></span>       | <span data-ttu-id="d328c-125">Int64</span><span class="sxs-lookup"><span data-stu-id="d328c-125">Int64</span></span>  | <span data-ttu-id="d328c-p104">回收站中的文件占用的总空间，以字节为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="d328c-p104">Total space consumed by files in the recycle bin, in bytes. Read-only.</span></span>      |
| <span data-ttu-id="d328c-128">state</span><span class="sxs-lookup"><span data-stu-id="d328c-128">state</span></span>         | <span data-ttu-id="d328c-129">string</span><span class="sxs-lookup"><span data-stu-id="d328c-129">string</span></span> | <span data-ttu-id="d328c-p105">指示存储空间状态的枚举值。只读。</span><span class="sxs-lookup"><span data-stu-id="d328c-p105">Enumeration value that indicates the state of the storage space. Read-only.</span></span> |

## <a name="state-enumeration"></a><span data-ttu-id="d328c-132">状态枚举</span><span class="sxs-lookup"><span data-stu-id="d328c-132">State Enumeration</span></span>

| <span data-ttu-id="d328c-133">值</span><span class="sxs-lookup"><span data-stu-id="d328c-133">Value</span></span>      | <span data-ttu-id="d328c-134">说明</span><span class="sxs-lookup"><span data-stu-id="d328c-134">Description</span></span>                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | <span data-ttu-id="d328c-135">驱动器具有充足的剩余配额。</span><span class="sxs-lookup"><span data-stu-id="d328c-135">The drive has plenty of remaining quota left.</span></span>                                                                                                                               |
| `nearing`  | <span data-ttu-id="d328c-136">剩余配额少于总配额空间的 10%。</span><span class="sxs-lookup"><span data-stu-id="d328c-136">Remaining quota is less than 10% of total quota space.</span></span>                                                                                                                      |
| `critical` | <span data-ttu-id="d328c-137">剩余配额少于总配额空间的 1%。</span><span class="sxs-lookup"><span data-stu-id="d328c-137">Remaining quota is less than 1% of total quota space.</span></span>                                                                                                                       |
| `exceeded` | <span data-ttu-id="d328c-p106">使用的配额已超出总配额。在驱动器低于总配额量或购买更多存储空间之前，无法向该驱动器添加新的文件或文件夹。</span><span class="sxs-lookup"><span data-stu-id="d328c-p106">The used quota has exceeded the total quota. New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span></span> |

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
