---
author: JeremyKelley
description: 配额资源提供有关驱动器资源上的空间限制的详细信息。
ms.date: 09/10/2017
title: 配额
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 8421998d9815efcd23417aadde8ef29e28050647
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521283"
---
# <a name="quota-resource-type"></a><span data-ttu-id="3d8b5-103">配额资源类型</span><span class="sxs-lookup"><span data-stu-id="3d8b5-103">quota resource type</span></span>

<span data-ttu-id="3d8b5-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="3d8b5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d8b5-105">**配额**资源提供有关[驱动器](drive.md)资源上的空间限制的详细信息。</span><span class="sxs-lookup"><span data-stu-id="3d8b5-105">The **quota** resource provides details about space constrains on a [drive](drive.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d8b5-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3d8b5-106">JSON representation</span></span>

<span data-ttu-id="3d8b5-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3d8b5-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="3d8b5-108">属性</span><span class="sxs-lookup"><span data-stu-id="3d8b5-108">Properties</span></span>

| <span data-ttu-id="3d8b5-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="3d8b5-109">Property name</span></span> | <span data-ttu-id="3d8b5-110">类型</span><span class="sxs-lookup"><span data-stu-id="3d8b5-110">Type</span></span>   | <span data-ttu-id="3d8b5-111">说明</span><span class="sxs-lookup"><span data-stu-id="3d8b5-111">Description</span></span>                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| <span data-ttu-id="3d8b5-112">total</span><span class="sxs-lookup"><span data-stu-id="3d8b5-112">total</span></span>         | <span data-ttu-id="3d8b5-113">Int64</span><span class="sxs-lookup"><span data-stu-id="3d8b5-113">Int64</span></span>  | <span data-ttu-id="3d8b5-p101">允许的总存储空间，以字节为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="3d8b5-p101">Total allowed storage space, in bytes. Read-only.</span></span>                           |
| <span data-ttu-id="3d8b5-116">used</span><span class="sxs-lookup"><span data-stu-id="3d8b5-116">used</span></span>          | <span data-ttu-id="3d8b5-117">Int64</span><span class="sxs-lookup"><span data-stu-id="3d8b5-117">Int64</span></span>  | <span data-ttu-id="3d8b5-p102">已使用的总空间，以字节为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="3d8b5-p102">Total space used, in bytes. Read-only.</span></span>                                      |
| <span data-ttu-id="3d8b5-120">remaining</span><span class="sxs-lookup"><span data-stu-id="3d8b5-120">remaining</span></span>     | <span data-ttu-id="3d8b5-121">Int64</span><span class="sxs-lookup"><span data-stu-id="3d8b5-121">Int64</span></span>  | <span data-ttu-id="3d8b5-p103">达到配额限制之前剩余的总空间，以字节为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="3d8b5-p103">Total space remaining before reaching the quota limit, in bytes. Read-only.</span></span> |
| <span data-ttu-id="3d8b5-124">deleted</span><span class="sxs-lookup"><span data-stu-id="3d8b5-124">deleted</span></span>       | <span data-ttu-id="3d8b5-125">Int64</span><span class="sxs-lookup"><span data-stu-id="3d8b5-125">Int64</span></span>  | <span data-ttu-id="3d8b5-p104">回收站中的文件占用的总空间，以字节为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="3d8b5-p104">Total space consumed by files in the recycle bin, in bytes. Read-only.</span></span>      |
| <span data-ttu-id="3d8b5-128">state</span><span class="sxs-lookup"><span data-stu-id="3d8b5-128">state</span></span>         | <span data-ttu-id="3d8b5-129">string</span><span class="sxs-lookup"><span data-stu-id="3d8b5-129">string</span></span> | <span data-ttu-id="3d8b5-p105">指示存储空间状态的枚举值。只读。</span><span class="sxs-lookup"><span data-stu-id="3d8b5-p105">Enumeration value that indicates the state of the storage space. Read-only.</span></span> |
| <span data-ttu-id="3d8b5-132">storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="3d8b5-132">storagePlanInformation</span></span>  | [<span data-ttu-id="3d8b5-133">storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="3d8b5-133">storagePlanInformation</span></span>](storageplaninformation.md) | <span data-ttu-id="3d8b5-134">有关驱动器的存储配额计划的信息。</span><span class="sxs-lookup"><span data-stu-id="3d8b5-134">Information about the drive's storage quota plans.</span></span> <span data-ttu-id="3d8b5-135">仅在个人 OneDrive 中。</span><span class="sxs-lookup"><span data-stu-id="3d8b5-135">Only in Personal OneDrive.</span></span>|

### <a name="state-enumeration-values"></a><span data-ttu-id="3d8b5-136">状态枚举值</span><span class="sxs-lookup"><span data-stu-id="3d8b5-136">State enumeration values</span></span>

| <span data-ttu-id="3d8b5-137">值</span><span class="sxs-lookup"><span data-stu-id="3d8b5-137">Value</span></span>      | <span data-ttu-id="3d8b5-138">说明</span><span class="sxs-lookup"><span data-stu-id="3d8b5-138">Description</span></span>                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | <span data-ttu-id="3d8b5-139">驱动器具有充足的剩余配额。</span><span class="sxs-lookup"><span data-stu-id="3d8b5-139">The drive has plenty of remaining quota left.</span></span>                                                                                                                               |
| `nearing`  | <span data-ttu-id="3d8b5-140">剩余配额少于总配额空间的 10%。</span><span class="sxs-lookup"><span data-stu-id="3d8b5-140">Remaining quota is less than 10% of total quota space.</span></span>                                                                                                                      |
| `critical` | <span data-ttu-id="3d8b5-141">剩余配额少于总配额空间的 1%。</span><span class="sxs-lookup"><span data-stu-id="3d8b5-141">Remaining quota is less than 1% of total quota space.</span></span>                                                                                                                       |
| `exceeded` | <span data-ttu-id="3d8b5-p107">使用的配额已超出总配额。在驱动器低于总配额量或购买更多存储空间之前，无法向该驱动器添加新的文件或文件夹。</span><span class="sxs-lookup"><span data-stu-id="3d8b5-p107">The used quota has exceeded the total quota. New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span></span> |

<!--
{
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/Quota",
  "suppressions": []
}
-->
