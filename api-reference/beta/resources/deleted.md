---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Deleted
localization_priority: Normal
ms.openlocfilehash: 6316f31d41e9d8e7264a671ac0317ebf9b32173f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804765"
---
# <a name="deleted-facet"></a><span data-ttu-id="55b96-102">Deleted Facet</span><span class="sxs-lookup"><span data-stu-id="55b96-102">Deleted facet</span></span>

> <span data-ttu-id="55b96-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="55b96-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="55b96-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="55b96-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="55b96-p102">**已删除的**资源指示该项已被删除。在这个 API 版本中，已删除资源值的状态（非 null）指示文件。Null（或缺少）值表示未删除该文件。</span><span class="sxs-lookup"><span data-stu-id="55b96-p102">The **Deleted** resource indicates that the item has been deleted. In this version of the API, the presence (non-null) of the resource value indicates that the file was deleted. A null (or missing) value indicates that the file is not deleted.</span></span>

<span data-ttu-id="55b96-108">有关跟踪更改和查找已删除项的详细信息，请参阅[查看项更改](../api/driveitem-delta.md)。</span><span class="sxs-lookup"><span data-stu-id="55b96-108">See [view changes for an item](../api/driveitem-delta.md) for more information on tracking changes and finding deleted items.</span></span>

## <a name="json-representation"></a><span data-ttu-id="55b96-109">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="55b96-109">JSON representation</span></span>

<span data-ttu-id="55b96-110">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="55b96-110">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="55b96-111">属性</span><span class="sxs-lookup"><span data-stu-id="55b96-111">Properties</span></span>

| <span data-ttu-id="55b96-112">属性</span><span class="sxs-lookup"><span data-stu-id="55b96-112">Property</span></span> | <span data-ttu-id="55b96-113">类型</span><span class="sxs-lookup"><span data-stu-id="55b96-113">Type</span></span>   | <span data-ttu-id="55b96-114">说明</span><span class="sxs-lookup"><span data-stu-id="55b96-114">Description</span></span>                               |
|:---------|:-------|:------------------------------------------|
| <span data-ttu-id="55b96-115">state</span><span class="sxs-lookup"><span data-stu-id="55b96-115">state</span></span>    | <span data-ttu-id="55b96-116">String</span><span class="sxs-lookup"><span data-stu-id="55b96-116">String</span></span> | <span data-ttu-id="55b96-117">表示已删除的项的状态。</span><span class="sxs-lookup"><span data-stu-id="55b96-117">Represents the state of the deleted item.</span></span> |

## <a name="remarks"></a><span data-ttu-id="55b96-118">注解</span><span class="sxs-lookup"><span data-stu-id="55b96-118">Remarks</span></span> 

<span data-ttu-id="55b96-119">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="55b96-119">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted"
} -->
