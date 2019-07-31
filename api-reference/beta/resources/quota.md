---
author: JeremyKelley
description: 配额资源提供有关驱动器资源上的空间限制的详细信息。
ms.date: 09/10/2017
title: 配额
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 83e842872694a1f708bf37ab800fa73673255647
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008794"
---
# <a name="quota-resource-type"></a><span data-ttu-id="51594-103">配额资源类型</span><span class="sxs-lookup"><span data-stu-id="51594-103">quota resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51594-104">**配额**资源提供有关[驱动器](drive.md)资源上的空间限制的详细信息。</span><span class="sxs-lookup"><span data-stu-id="51594-104">The **quota** resource provides details about space constrains on a [drive](drive.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="51594-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="51594-105">JSON representation</span></span>

<span data-ttu-id="51594-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51594-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="51594-107">属性</span><span class="sxs-lookup"><span data-stu-id="51594-107">Properties</span></span>

| <span data-ttu-id="51594-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="51594-108">Property name</span></span> | <span data-ttu-id="51594-109">类型</span><span class="sxs-lookup"><span data-stu-id="51594-109">Type</span></span>   | <span data-ttu-id="51594-110">说明</span><span class="sxs-lookup"><span data-stu-id="51594-110">Description</span></span>                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| <span data-ttu-id="51594-111">total</span><span class="sxs-lookup"><span data-stu-id="51594-111">total</span></span>         | <span data-ttu-id="51594-112">Int64</span><span class="sxs-lookup"><span data-stu-id="51594-112">Int64</span></span>  | <span data-ttu-id="51594-p101">允许的总存储空间，以字节为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="51594-p101">Total allowed storage space, in bytes. Read-only.</span></span>                           |
| <span data-ttu-id="51594-115">used</span><span class="sxs-lookup"><span data-stu-id="51594-115">used</span></span>          | <span data-ttu-id="51594-116">Int64</span><span class="sxs-lookup"><span data-stu-id="51594-116">Int64</span></span>  | <span data-ttu-id="51594-p102">已使用的总空间，以字节为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="51594-p102">Total space used, in bytes. Read-only.</span></span>                                      |
| <span data-ttu-id="51594-119">remaining</span><span class="sxs-lookup"><span data-stu-id="51594-119">remaining</span></span>     | <span data-ttu-id="51594-120">Int64</span><span class="sxs-lookup"><span data-stu-id="51594-120">Int64</span></span>  | <span data-ttu-id="51594-p103">达到配额限制之前剩余的总空间，以字节为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="51594-p103">Total space remaining before reaching the quota limit, in bytes. Read-only.</span></span> |
| <span data-ttu-id="51594-123">deleted</span><span class="sxs-lookup"><span data-stu-id="51594-123">deleted</span></span>       | <span data-ttu-id="51594-124">Int64</span><span class="sxs-lookup"><span data-stu-id="51594-124">Int64</span></span>  | <span data-ttu-id="51594-p104">回收站中的文件占用的总空间，以字节为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="51594-p104">Total space consumed by files in the recycle bin, in bytes. Read-only.</span></span>      |
| <span data-ttu-id="51594-127">state</span><span class="sxs-lookup"><span data-stu-id="51594-127">state</span></span>         | <span data-ttu-id="51594-128">string</span><span class="sxs-lookup"><span data-stu-id="51594-128">string</span></span> | <span data-ttu-id="51594-p105">指示存储空间状态的枚举值。只读。</span><span class="sxs-lookup"><span data-stu-id="51594-p105">Enumeration value that indicates the state of the storage space. Read-only.</span></span> |
| <span data-ttu-id="51594-131">storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="51594-131">storagePlanInformation</span></span>  | [<span data-ttu-id="51594-132">storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="51594-132">storagePlanInformation</span></span>](storageplaninformation.md) | <span data-ttu-id="51594-133">有关驱动器的存储配额计划的信息。</span><span class="sxs-lookup"><span data-stu-id="51594-133">Information about the drive's storage quota plans.</span></span> <span data-ttu-id="51594-134">仅在个人 OneDrive 中。</span><span class="sxs-lookup"><span data-stu-id="51594-134">Only in Personal OneDrive.</span></span>|

### <a name="state-enumeration-values"></a><span data-ttu-id="51594-135">状态枚举值</span><span class="sxs-lookup"><span data-stu-id="51594-135">State enumeration values</span></span>

| <span data-ttu-id="51594-136">值</span><span class="sxs-lookup"><span data-stu-id="51594-136">Value</span></span>      | <span data-ttu-id="51594-137">说明</span><span class="sxs-lookup"><span data-stu-id="51594-137">Description</span></span>                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | <span data-ttu-id="51594-138">驱动器具有充足的剩余配额。</span><span class="sxs-lookup"><span data-stu-id="51594-138">The drive has plenty of remaining quota left.</span></span>                                                                                                                               |
| `nearing`  | <span data-ttu-id="51594-139">剩余配额少于总配额空间的 10%。</span><span class="sxs-lookup"><span data-stu-id="51594-139">Remaining quota is less than 10% of total quota space.</span></span>                                                                                                                      |
| `critical` | <span data-ttu-id="51594-140">剩余配额少于总配额空间的 1%。</span><span class="sxs-lookup"><span data-stu-id="51594-140">Remaining quota is less than 1% of total quota space.</span></span>                                                                                                                       |
| `exceeded` | <span data-ttu-id="51594-p107">使用的配额已超出总配额。在驱动器低于总配额量或购买更多存储空间之前，无法向该驱动器添加新的文件或文件夹。</span><span class="sxs-lookup"><span data-stu-id="51594-p107">The used quota has exceeded the total quota. New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span></span> |

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
