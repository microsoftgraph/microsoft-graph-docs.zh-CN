---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Deleted
localization_priority: Normal
ms.openlocfilehash: 06fe9835ef4b31d7a48bad955b17872142a94b2d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535283"
---
# <a name="deleted-facet"></a><span data-ttu-id="aa5f2-102">Deleted Facet</span><span class="sxs-lookup"><span data-stu-id="aa5f2-102">Deleted facet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa5f2-p101">**已删除的**资源指示该项已被删除。在这个 API 版本中，已删除资源值的状态（非 null）指示文件。Null（或缺少）值表示未删除该文件。</span><span class="sxs-lookup"><span data-stu-id="aa5f2-p101">The **Deleted** resource indicates that the item has been deleted. In this version of the API, the presence (non-null) of the resource value indicates that the file was deleted. A null (or missing) value indicates that the file is not deleted.</span></span>

<span data-ttu-id="aa5f2-106">有关跟踪更改和查找已删除项的详细信息，请参阅[查看项更改](../api/driveitem-delta.md)。</span><span class="sxs-lookup"><span data-stu-id="aa5f2-106">See [view changes for an item](../api/driveitem-delta.md) for more information on tracking changes and finding deleted items.</span></span>

## <a name="json-representation"></a><span data-ttu-id="aa5f2-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aa5f2-107">JSON representation</span></span>

<span data-ttu-id="aa5f2-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aa5f2-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="aa5f2-109">属性</span><span class="sxs-lookup"><span data-stu-id="aa5f2-109">Properties</span></span>

| <span data-ttu-id="aa5f2-110">属性</span><span class="sxs-lookup"><span data-stu-id="aa5f2-110">Property</span></span> | <span data-ttu-id="aa5f2-111">类型</span><span class="sxs-lookup"><span data-stu-id="aa5f2-111">Type</span></span>   | <span data-ttu-id="aa5f2-112">说明</span><span class="sxs-lookup"><span data-stu-id="aa5f2-112">Description</span></span>                               |
|:---------|:-------|:------------------------------------------|
| <span data-ttu-id="aa5f2-113">state</span><span class="sxs-lookup"><span data-stu-id="aa5f2-113">state</span></span>    | <span data-ttu-id="aa5f2-114">String</span><span class="sxs-lookup"><span data-stu-id="aa5f2-114">String</span></span> | <span data-ttu-id="aa5f2-115">表示已删除的项的状态。</span><span class="sxs-lookup"><span data-stu-id="aa5f2-115">Represents the state of the deleted item.</span></span> |

## <a name="remarks"></a><span data-ttu-id="aa5f2-116">注解</span><span class="sxs-lookup"><span data-stu-id="aa5f2-116">Remarks</span></span> 

<span data-ttu-id="aa5f2-117">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="aa5f2-117">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


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
