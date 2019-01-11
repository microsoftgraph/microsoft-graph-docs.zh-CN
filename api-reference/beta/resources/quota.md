---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 配额
localization_priority: Normal
ms.openlocfilehash: a63b41253569dbb3d666a76b0a7495839ef61b12
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882409"
---
# <a name="quota-resource-type"></a><span data-ttu-id="8aa59-102">配额资源类型</span><span class="sxs-lookup"><span data-stu-id="8aa59-102">quota resource type</span></span>

> <span data-ttu-id="8aa59-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8aa59-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8aa59-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8aa59-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8aa59-105">**配额**资源提供有关空间的详细信息约束[驱动器](drive.md)资源。</span><span class="sxs-lookup"><span data-stu-id="8aa59-105">The **quota** resource provides details about space constrains on a [drive](drive.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8aa59-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8aa59-106">JSON representation</span></span>

<span data-ttu-id="8aa59-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8aa59-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="8aa59-108">属性</span><span class="sxs-lookup"><span data-stu-id="8aa59-108">Properties</span></span>

| <span data-ttu-id="8aa59-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="8aa59-109">Property name</span></span> | <span data-ttu-id="8aa59-110">类型</span><span class="sxs-lookup"><span data-stu-id="8aa59-110">Type</span></span>   | <span data-ttu-id="8aa59-111">说明</span><span class="sxs-lookup"><span data-stu-id="8aa59-111">Description</span></span>                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| <span data-ttu-id="8aa59-112">total</span><span class="sxs-lookup"><span data-stu-id="8aa59-112">total</span></span>         | <span data-ttu-id="8aa59-113">Int64</span><span class="sxs-lookup"><span data-stu-id="8aa59-113">Int64</span></span>  | <span data-ttu-id="8aa59-p102">允许的总存储空间，以字节为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="8aa59-p102">Total allowed storage space, in bytes. Read-only.</span></span>                           |
| <span data-ttu-id="8aa59-116">used</span><span class="sxs-lookup"><span data-stu-id="8aa59-116">used</span></span>          | <span data-ttu-id="8aa59-117">Int64</span><span class="sxs-lookup"><span data-stu-id="8aa59-117">Int64</span></span>  | <span data-ttu-id="8aa59-p103">已使用的总空间，以字节为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="8aa59-p103">Total space used, in bytes. Read-only.</span></span>                                      |
| <span data-ttu-id="8aa59-120">remaining</span><span class="sxs-lookup"><span data-stu-id="8aa59-120">remaining</span></span>     | <span data-ttu-id="8aa59-121">Int64</span><span class="sxs-lookup"><span data-stu-id="8aa59-121">Int64</span></span>  | <span data-ttu-id="8aa59-p104">达到配额限制之前剩余的总空间，以字节为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="8aa59-p104">Total space remaining before reaching the quota limit, in bytes. Read-only.</span></span> |
| <span data-ttu-id="8aa59-124">deleted</span><span class="sxs-lookup"><span data-stu-id="8aa59-124">deleted</span></span>       | <span data-ttu-id="8aa59-125">Int64</span><span class="sxs-lookup"><span data-stu-id="8aa59-125">Int64</span></span>  | <span data-ttu-id="8aa59-p105">回收站中的文件占用的总空间，以字节为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="8aa59-p105">Total space consumed by files in the recycle bin, in bytes. Read-only.</span></span>      |
| <span data-ttu-id="8aa59-128">state</span><span class="sxs-lookup"><span data-stu-id="8aa59-128">state</span></span>         | <span data-ttu-id="8aa59-129">string</span><span class="sxs-lookup"><span data-stu-id="8aa59-129">string</span></span> | <span data-ttu-id="8aa59-p106">指示存储空间状态的枚举值。只读。</span><span class="sxs-lookup"><span data-stu-id="8aa59-p106">Enumeration value that indicates the state of the storage space. Read-only.</span></span> |
| <span data-ttu-id="8aa59-132">storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="8aa59-132">storagePlanInformation</span></span>  | [<span data-ttu-id="8aa59-133">storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="8aa59-133">storagePlanInformation</span></span>](storageplaninformation.md) | <span data-ttu-id="8aa59-134">有关驱动器的存储配额计划的信息。</span><span class="sxs-lookup"><span data-stu-id="8aa59-134">Information about the drive's storage quota plans.</span></span> <span data-ttu-id="8aa59-135">仅在个人 OneDrive。</span><span class="sxs-lookup"><span data-stu-id="8aa59-135">Only in Personal OneDrive.</span></span>|

### <a name="state-enumeration-values"></a><span data-ttu-id="8aa59-136">状态的枚举值</span><span class="sxs-lookup"><span data-stu-id="8aa59-136">State enumeration values</span></span>

| <span data-ttu-id="8aa59-137">值</span><span class="sxs-lookup"><span data-stu-id="8aa59-137">Value</span></span>      | <span data-ttu-id="8aa59-138">说明</span><span class="sxs-lookup"><span data-stu-id="8aa59-138">Description</span></span>                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | <span data-ttu-id="8aa59-139">驱动器具有充足的剩余配额。</span><span class="sxs-lookup"><span data-stu-id="8aa59-139">The drive has plenty of remaining quota left.</span></span>                                                                                                                               |
| `nearing`  | <span data-ttu-id="8aa59-140">剩余配额少于总配额空间的 10%。</span><span class="sxs-lookup"><span data-stu-id="8aa59-140">Remaining quota is less than 10% of total quota space.</span></span>                                                                                                                      |
| `critical` | <span data-ttu-id="8aa59-141">剩余配额少于总配额空间的 1%。</span><span class="sxs-lookup"><span data-stu-id="8aa59-141">Remaining quota is less than 1% of total quota space.</span></span>                                                                                                                       |
| `exceeded` | <span data-ttu-id="8aa59-p108">使用的配额已超出总配额。在驱动器低于总配额量或购买更多存储空间之前，无法向该驱动器添加新的文件或文件夹。</span><span class="sxs-lookup"><span data-stu-id="8aa59-p108">The used quota has exceeded the total quota. New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span></span> |

<!-- {
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/Quota"
} -->
