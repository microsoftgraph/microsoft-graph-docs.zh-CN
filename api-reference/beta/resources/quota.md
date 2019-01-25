---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 配额
localization_priority: Normal
ms.openlocfilehash: ce07852592317568254217c7e869f1da7f296a2e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525484"
---
# <a name="quota-resource-type"></a><span data-ttu-id="112b1-102">配额资源类型</span><span class="sxs-lookup"><span data-stu-id="112b1-102">quota resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="112b1-103">**配额**资源提供有关 [驱动器](drive.md) 资源上的空间限制的详细信息。</span><span class="sxs-lookup"><span data-stu-id="112b1-103">The **quota** resource provides details about space constrains on a [drive](drive.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="112b1-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="112b1-104">JSON representation</span></span>

<span data-ttu-id="112b1-105">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="112b1-105">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="112b1-106">属性</span><span class="sxs-lookup"><span data-stu-id="112b1-106">Properties</span></span>

| <span data-ttu-id="112b1-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="112b1-107">Property name</span></span> | <span data-ttu-id="112b1-108">类型</span><span class="sxs-lookup"><span data-stu-id="112b1-108">Type</span></span>   | <span data-ttu-id="112b1-109">说明</span><span class="sxs-lookup"><span data-stu-id="112b1-109">Description</span></span>                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| <span data-ttu-id="112b1-110">total</span><span class="sxs-lookup"><span data-stu-id="112b1-110">total</span></span>         | <span data-ttu-id="112b1-111">Int64</span><span class="sxs-lookup"><span data-stu-id="112b1-111">Int64</span></span>  | <span data-ttu-id="112b1-p101">允许的总存储空间，以字节为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="112b1-p101">Total allowed storage space, in bytes. Read-only.</span></span>                           |
| <span data-ttu-id="112b1-114">used</span><span class="sxs-lookup"><span data-stu-id="112b1-114">used</span></span>          | <span data-ttu-id="112b1-115">Int64</span><span class="sxs-lookup"><span data-stu-id="112b1-115">Int64</span></span>  | <span data-ttu-id="112b1-p102">已使用的总空间，以字节为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="112b1-p102">Total space used, in bytes. Read-only.</span></span>                                      |
| <span data-ttu-id="112b1-118">remaining</span><span class="sxs-lookup"><span data-stu-id="112b1-118">remaining</span></span>     | <span data-ttu-id="112b1-119">Int64</span><span class="sxs-lookup"><span data-stu-id="112b1-119">Int64</span></span>  | <span data-ttu-id="112b1-p103">达到配额限制之前剩余的总空间，以字节为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="112b1-p103">Total space remaining before reaching the quota limit, in bytes. Read-only.</span></span> |
| <span data-ttu-id="112b1-122">deleted</span><span class="sxs-lookup"><span data-stu-id="112b1-122">deleted</span></span>       | <span data-ttu-id="112b1-123">Int64</span><span class="sxs-lookup"><span data-stu-id="112b1-123">Int64</span></span>  | <span data-ttu-id="112b1-p104">回收站中的文件占用的总空间，以字节为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="112b1-p104">Total space consumed by files in the recycle bin, in bytes. Read-only.</span></span>      |
| <span data-ttu-id="112b1-126">state</span><span class="sxs-lookup"><span data-stu-id="112b1-126">state</span></span>         | <span data-ttu-id="112b1-127">string</span><span class="sxs-lookup"><span data-stu-id="112b1-127">string</span></span> | <span data-ttu-id="112b1-p105">指示存储空间状态的枚举值。只读。</span><span class="sxs-lookup"><span data-stu-id="112b1-p105">Enumeration value that indicates the state of the storage space. Read-only.</span></span> |
| <span data-ttu-id="112b1-130">storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="112b1-130">storagePlanInformation</span></span>  | [<span data-ttu-id="112b1-131">storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="112b1-131">storagePlanInformation</span></span>](storageplaninformation.md) | <span data-ttu-id="112b1-132">有关驱动器的存储配额计划的信息。</span><span class="sxs-lookup"><span data-stu-id="112b1-132">Information about the drive's storage quota plans.</span></span> <span data-ttu-id="112b1-133">仅在个人 OneDrive。</span><span class="sxs-lookup"><span data-stu-id="112b1-133">Only in Personal OneDrive.</span></span>|

### <a name="state-enumeration-values"></a><span data-ttu-id="112b1-134">状态的枚举值</span><span class="sxs-lookup"><span data-stu-id="112b1-134">State enumeration values</span></span>

| <span data-ttu-id="112b1-135">值</span><span class="sxs-lookup"><span data-stu-id="112b1-135">Value</span></span>      | <span data-ttu-id="112b1-136">说明</span><span class="sxs-lookup"><span data-stu-id="112b1-136">Description</span></span>                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | <span data-ttu-id="112b1-137">驱动器具有充足的剩余配额。</span><span class="sxs-lookup"><span data-stu-id="112b1-137">The drive has plenty of remaining quota left.</span></span>                                                                                                                               |
| `nearing`  | <span data-ttu-id="112b1-138">剩余配额少于总配额空间的 10%。</span><span class="sxs-lookup"><span data-stu-id="112b1-138">Remaining quota is less than 10% of total quota space.</span></span>                                                                                                                      |
| `critical` | <span data-ttu-id="112b1-139">剩余配额少于总配额空间的 1%。</span><span class="sxs-lookup"><span data-stu-id="112b1-139">Remaining quota is less than 1% of total quota space.</span></span>                                                                                                                       |
| `exceeded` | <span data-ttu-id="112b1-p107">使用的配额已超出总配额。在驱动器低于总配额量或购买更多存储空间之前，无法向该驱动器添加新的文件或文件夹。</span><span class="sxs-lookup"><span data-stu-id="112b1-p107">The used quota has exceeded the total quota. New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased.</span></span> |

<!--
{
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/Quota",
  "suppressions": [
    "Error: /api-reference/beta/resources/quota.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
