---
author: JeremyKelley
description: 已删除资源指示该项已被删除。
ms.date: 09/10/2017
title: Deleted
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6f42f5cea70e4dd4304a12130aaa34376fde226d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049869"
---
# <a name="deleted-facet"></a><span data-ttu-id="97f4a-103">Deleted Facet</span><span class="sxs-lookup"><span data-stu-id="97f4a-103">Deleted facet</span></span>

<span data-ttu-id="97f4a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97f4a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97f4a-p101">**已删除的**资源指示该项已被删除。在这个 API 版本中，已删除资源值的状态（非 null）指示文件。Null（或缺少）值表示未删除该文件。</span><span class="sxs-lookup"><span data-stu-id="97f4a-p101">The **Deleted** resource indicates that the item has been deleted. In this version of the API, the presence (non-null) of the resource value indicates that the file was deleted. A null (or missing) value indicates that the file is not deleted.</span></span>

<span data-ttu-id="97f4a-108">有关跟踪更改和查找已删除项的详细信息，请参阅[查看项更改](../api/driveitem-delta.md)。</span><span class="sxs-lookup"><span data-stu-id="97f4a-108">See [view changes for an item](../api/driveitem-delta.md) for more information on tracking changes and finding deleted items.</span></span>

## <a name="json-representation"></a><span data-ttu-id="97f4a-109">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="97f4a-109">JSON representation</span></span>

<span data-ttu-id="97f4a-110">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97f4a-110">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  "state"
  ],
  "@odata.type": "microsoft.graph.deleted"
}-->
```json
{
  "state": "string"
}
```
## <a name="properties"></a><span data-ttu-id="97f4a-111">属性</span><span class="sxs-lookup"><span data-stu-id="97f4a-111">Properties</span></span>

| <span data-ttu-id="97f4a-112">属性</span><span class="sxs-lookup"><span data-stu-id="97f4a-112">Property</span></span> | <span data-ttu-id="97f4a-113">类型</span><span class="sxs-lookup"><span data-stu-id="97f4a-113">Type</span></span>   | <span data-ttu-id="97f4a-114">说明</span><span class="sxs-lookup"><span data-stu-id="97f4a-114">Description</span></span>                               |
|:---------|:-------|:------------------------------------------|
| <span data-ttu-id="97f4a-115">state</span><span class="sxs-lookup"><span data-stu-id="97f4a-115">state</span></span>    | <span data-ttu-id="97f4a-116">String</span><span class="sxs-lookup"><span data-stu-id="97f4a-116">String</span></span> | <span data-ttu-id="97f4a-117">表示已删除的项的状态。</span><span class="sxs-lookup"><span data-stu-id="97f4a-117">Represents the state of the deleted item.</span></span> |

## <a name="remarks"></a><span data-ttu-id="97f4a-118">注解</span><span class="sxs-lookup"><span data-stu-id="97f4a-118">Remarks</span></span> 

<span data-ttu-id="97f4a-119">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="97f4a-119">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted",
  "suppressions": []
}
-->


