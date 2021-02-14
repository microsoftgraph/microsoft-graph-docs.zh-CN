---
author: JeremyKelley
ms.date: 09/10/2017
title: Deleted
localization_priority: Normal
description: 已删除资源指示该项已被删除。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3743a343b9928eda4a888cff06a3ff1b7525f9c9
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239609"
---
# <a name="deleted-facet"></a><span data-ttu-id="5716d-103">Deleted Facet</span><span class="sxs-lookup"><span data-stu-id="5716d-103">Deleted facet</span></span>

<span data-ttu-id="5716d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5716d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5716d-p101">**已删除的** 资源指示该项已被删除。在这个 API 版本中，已删除资源值的状态（非 null）指示文件。Null（或缺少）值表示未删除该文件。</span><span class="sxs-lookup"><span data-stu-id="5716d-p101">The **Deleted** resource indicates that the item has been deleted. In this version of the API, the presence (non-null) of the resource value indicates that the file was deleted. A null (or missing) value indicates that the file is not deleted.</span></span>

<span data-ttu-id="5716d-108">有关跟踪更改和查找已删除项的详细信息，请参阅[查看项更改](../api/driveitem-delta.md)。</span><span class="sxs-lookup"><span data-stu-id="5716d-108">See [view changes for an item](../api/driveitem-delta.md) for more information on tracking changes and finding deleted items.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5716d-109">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5716d-109">JSON representation</span></span>

<span data-ttu-id="5716d-110">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5716d-110">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="5716d-111">属性</span><span class="sxs-lookup"><span data-stu-id="5716d-111">Properties</span></span>

| <span data-ttu-id="5716d-112">属性</span><span class="sxs-lookup"><span data-stu-id="5716d-112">Property</span></span> | <span data-ttu-id="5716d-113">类型</span><span class="sxs-lookup"><span data-stu-id="5716d-113">Type</span></span>   | <span data-ttu-id="5716d-114">说明</span><span class="sxs-lookup"><span data-stu-id="5716d-114">Description</span></span>                               |
|:---------|:-------|:------------------------------------------|
| <span data-ttu-id="5716d-115">state</span><span class="sxs-lookup"><span data-stu-id="5716d-115">state</span></span>    | <span data-ttu-id="5716d-116">String</span><span class="sxs-lookup"><span data-stu-id="5716d-116">String</span></span> | <span data-ttu-id="5716d-117">表示已删除的项的状态。</span><span class="sxs-lookup"><span data-stu-id="5716d-117">Represents the state of the deleted item.</span></span> |

## <a name="remarks"></a><span data-ttu-id="5716d-118">注解</span><span class="sxs-lookup"><span data-stu-id="5716d-118">Remarks</span></span> 

<span data-ttu-id="5716d-119">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="5716d-119">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted"
} -->

