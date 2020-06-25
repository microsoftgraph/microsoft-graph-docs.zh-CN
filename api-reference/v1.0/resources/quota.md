---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 配额
localization_priority: Normal
description: 配额资源提供有关 驱动器 资源上的空间限制的详细信息。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 293daf950beb5cdf3cbd791a1e8bf0d4b92a220b
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44864208"
---
# <a name="quota-resource-type"></a><span data-ttu-id="b27b9-103">Quota 资源类型</span><span class="sxs-lookup"><span data-stu-id="b27b9-103">Quota resource type</span></span>

<span data-ttu-id="b27b9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b27b9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b27b9-105">**配额**资源提供有关 [驱动器](drive.md) 资源上的空间限制的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b27b9-105">The **quota** resource provides details about space constrains on a [Drive](drive.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b27b9-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b27b9-106">JSON representation</span></span>

<span data-ttu-id="b27b9-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b27b9-107">Here is a JSON representation of the resource.</span></span>

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
  "storagePlanInformation": {
    "upgradeAvailable": true
  },
  "total": 1024,
  "used": 1024
}
```

## <a name="properties"></a><span data-ttu-id="b27b9-108">属性</span><span class="sxs-lookup"><span data-stu-id="b27b9-108">Properties</span></span>

| <span data-ttu-id="b27b9-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="b27b9-109">Property name</span></span> | <span data-ttu-id="b27b9-110">类型</span><span class="sxs-lookup"><span data-stu-id="b27b9-110">Type</span></span>   | <span data-ttu-id="b27b9-111">说明</span><span class="sxs-lookup"><span data-stu-id="b27b9-111">Description</span></span>                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| <span data-ttu-id="b27b9-112">total</span><span class="sxs-lookup"><span data-stu-id="b27b9-112">total</span></span>         | <span data-ttu-id="b27b9-113">Int64</span><span class="sxs-lookup"><span data-stu-id="b27b9-113">Int64</span></span>  | <span data-ttu-id="b27b9-114">Total allowed storage space, in bytes.</span><span class="sxs-lookup"><span data-stu-id="b27b9-114">Total allowed storage space, in bytes.</span></span> <span data-ttu-id="b27b9-115">Read-only.</span><span class="sxs-lookup"><span data-stu-id="b27b9-115">Read-only.</span></span>                           |
| <span data-ttu-id="b27b9-116">used</span><span class="sxs-lookup"><span data-stu-id="b27b9-116">used</span></span>          | <span data-ttu-id="b27b9-117">Int64</span><span class="sxs-lookup"><span data-stu-id="b27b9-117">Int64</span></span>  | <span data-ttu-id="b27b9-118">Total space used, in bytes.</span><span class="sxs-lookup"><span data-stu-id="b27b9-118">Total space used, in bytes.</span></span> <span data-ttu-id="b27b9-119">Read-only.</span><span class="sxs-lookup"><span data-stu-id="b27b9-119">Read-only.</span></span>                                      |
| <span data-ttu-id="b27b9-120">remaining</span><span class="sxs-lookup"><span data-stu-id="b27b9-120">remaining</span></span>     | <span data-ttu-id="b27b9-121">Int64</span><span class="sxs-lookup"><span data-stu-id="b27b9-121">Int64</span></span>  | <span data-ttu-id="b27b9-122">Total space remaining before reaching the quota limit, in bytes.</span><span class="sxs-lookup"><span data-stu-id="b27b9-122">Total space remaining before reaching the quota limit, in bytes.</span></span> <span data-ttu-id="b27b9-123">Read-only.</span><span class="sxs-lookup"><span data-stu-id="b27b9-123">Read-only.</span></span> |
| <span data-ttu-id="b27b9-124">deleted</span><span class="sxs-lookup"><span data-stu-id="b27b9-124">deleted</span></span>       | <span data-ttu-id="b27b9-125">Int64</span><span class="sxs-lookup"><span data-stu-id="b27b9-125">Int64</span></span>  | <span data-ttu-id="b27b9-126">Total space consumed by files in the recycle bin, in bytes.</span><span class="sxs-lookup"><span data-stu-id="b27b9-126">Total space consumed by files in the recycle bin, in bytes.</span></span> <span data-ttu-id="b27b9-127">Read-only.</span><span class="sxs-lookup"><span data-stu-id="b27b9-127">Read-only.</span></span>      |
| <span data-ttu-id="b27b9-128">state</span><span class="sxs-lookup"><span data-stu-id="b27b9-128">state</span></span>         | <span data-ttu-id="b27b9-129">string</span><span class="sxs-lookup"><span data-stu-id="b27b9-129">string</span></span> | <span data-ttu-id="b27b9-130">Enumeration value that indicates the state of the storage space.</span><span class="sxs-lookup"><span data-stu-id="b27b9-130">Enumeration value that indicates the state of the storage space.</span></span> <span data-ttu-id="b27b9-131">Read-only.</span><span class="sxs-lookup"><span data-stu-id="b27b9-131">Read-only.</span></span> |
| <span data-ttu-id="b27b9-132">storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="b27b9-132">storagePlanInformation</span></span>  | [<span data-ttu-id="b27b9-133">storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="b27b9-133">storagePlanInformation</span></span>](storageplaninformation.md) | <span data-ttu-id="b27b9-134">有关驱动器的存储配额计划的信息。</span><span class="sxs-lookup"><span data-stu-id="b27b9-134">Information about the drive's storage quota plans.</span></span> <span data-ttu-id="b27b9-135">仅在个人 OneDrive 中。</span><span class="sxs-lookup"><span data-stu-id="b27b9-135">Only in Personal OneDrive.</span></span>|

## <a name="state-enumeration"></a><span data-ttu-id="b27b9-136">状态枚举</span><span class="sxs-lookup"><span data-stu-id="b27b9-136">State Enumeration</span></span>

| <span data-ttu-id="b27b9-137">值</span><span class="sxs-lookup"><span data-stu-id="b27b9-137">Value</span></span>      | <span data-ttu-id="b27b9-138">说明</span><span class="sxs-lookup"><span data-stu-id="b27b9-138">Description</span></span>                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | <span data-ttu-id="b27b9-139">驱动器具有充足的剩余配额。</span><span class="sxs-lookup"><span data-stu-id="b27b9-139">The drive has plenty of remaining quota left.</span></span>                                                                                                                               |
| `nearing`  | <span data-ttu-id="b27b9-140">剩余配额少于总配额空间的 10%。</span><span class="sxs-lookup"><span data-stu-id="b27b9-140">Remaining quota is less than 10% of total quota space.</span></span>                                                                                                                      |
| `critical` | <span data-ttu-id="b27b9-141">剩余配额少于总配额空间的 1%。</span><span class="sxs-lookup"><span data-stu-id="b27b9-141">Remaining quota is less than 1% of total quota space.</span></span>                                                                                                                       |
| `exceeded` | <span data-ttu-id="b27b9-142">The used quota has exceeded the total quota.</span><span class="sxs-lookup"><span data-stu-id="b27b9-142">The used quota has exceeded the total quota.</span></span> <span data-ttu-id="b27b9-143">New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span><span class="sxs-lookup"><span data-stu-id="b27b9-143">New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span></span> |

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
