---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Deleted
localization_priority: Normal
ms.openlocfilehash: d52ca0a9815e46ebc11a653be381ac65f3cd209e
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482180"
---
# <a name="deleted-facet"></a><span data-ttu-id="5241e-102">Deleted Facet</span><span class="sxs-lookup"><span data-stu-id="5241e-102">Deleted facet</span></span>

<span data-ttu-id="5241e-p101">**已删除的**资源指示该项已被删除。在这个 API 版本中，已删除资源值的状态（非 null）指示文件。Null（或缺少）值表示未删除该文件。</span><span class="sxs-lookup"><span data-stu-id="5241e-p101">The **Deleted** resource indicates that the item has been deleted. In this version of the API, the presence (non-null) of the resource value indicates that the file was deleted. A null (or missing) value indicates that the file is not deleted.</span></span>

<span data-ttu-id="5241e-106">有关跟踪更改和查找已删除项的详细信息，请参阅[查看项更改](../api/driveitem-delta.md)。</span><span class="sxs-lookup"><span data-stu-id="5241e-106">See [view changes for an item](../api/driveitem-delta.md) for more information on tracking changes and finding deleted items.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5241e-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5241e-107">JSON representation</span></span>

<span data-ttu-id="5241e-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5241e-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="5241e-109">属性</span><span class="sxs-lookup"><span data-stu-id="5241e-109">Properties</span></span>

| <span data-ttu-id="5241e-110">属性</span><span class="sxs-lookup"><span data-stu-id="5241e-110">Property</span></span> | <span data-ttu-id="5241e-111">类型</span><span class="sxs-lookup"><span data-stu-id="5241e-111">Type</span></span>   | <span data-ttu-id="5241e-112">说明</span><span class="sxs-lookup"><span data-stu-id="5241e-112">Description</span></span>                               |
|:---------|:-------|:------------------------------------------|
| <span data-ttu-id="5241e-113">state</span><span class="sxs-lookup"><span data-stu-id="5241e-113">state</span></span>    | <span data-ttu-id="5241e-114">String</span><span class="sxs-lookup"><span data-stu-id="5241e-114">String</span></span> | <span data-ttu-id="5241e-115">表示已删除的项的状态。</span><span class="sxs-lookup"><span data-stu-id="5241e-115">Represents the state of the deleted item.</span></span> |

## <a name="remarks"></a><span data-ttu-id="5241e-116">注解</span><span class="sxs-lookup"><span data-stu-id="5241e-116">Remarks</span></span> 

<span data-ttu-id="5241e-117">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="5241e-117">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted"
} -->
