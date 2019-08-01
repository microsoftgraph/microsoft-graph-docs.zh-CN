---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Deleted
localization_priority: Normal
description: 已删除资源指示该项已被删除。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d1f5c07c60c8de4890a2a4ac334df04a59b7339c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029517"
---
# <a name="deleted-facet"></a><span data-ttu-id="f77eb-103">Deleted Facet</span><span class="sxs-lookup"><span data-stu-id="f77eb-103">Deleted facet</span></span>

<span data-ttu-id="f77eb-p101">**已删除的**资源指示该项已被删除。在这个 API 版本中，已删除资源值的状态（非 null）指示文件。Null（或缺少）值表示未删除该文件。</span><span class="sxs-lookup"><span data-stu-id="f77eb-p101">The **Deleted** resource indicates that the item has been deleted. In this version of the API, the presence (non-null) of the resource value indicates that the file was deleted. A null (or missing) value indicates that the file is not deleted.</span></span>

<span data-ttu-id="f77eb-107">有关跟踪更改和查找已删除项的详细信息，请参阅[查看项更改](../api/driveitem-delta.md)。</span><span class="sxs-lookup"><span data-stu-id="f77eb-107">See [view changes for an item](../api/driveitem-delta.md) for more information on tracking changes and finding deleted items.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f77eb-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f77eb-108">JSON representation</span></span>

<span data-ttu-id="f77eb-109">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f77eb-109">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="f77eb-110">属性</span><span class="sxs-lookup"><span data-stu-id="f77eb-110">Properties</span></span>

| <span data-ttu-id="f77eb-111">属性</span><span class="sxs-lookup"><span data-stu-id="f77eb-111">Property</span></span> | <span data-ttu-id="f77eb-112">类型</span><span class="sxs-lookup"><span data-stu-id="f77eb-112">Type</span></span>   | <span data-ttu-id="f77eb-113">说明</span><span class="sxs-lookup"><span data-stu-id="f77eb-113">Description</span></span>                               |
|:---------|:-------|:------------------------------------------|
| <span data-ttu-id="f77eb-114">state</span><span class="sxs-lookup"><span data-stu-id="f77eb-114">state</span></span>    | <span data-ttu-id="f77eb-115">String</span><span class="sxs-lookup"><span data-stu-id="f77eb-115">String</span></span> | <span data-ttu-id="f77eb-116">表示已删除的项的状态。</span><span class="sxs-lookup"><span data-stu-id="f77eb-116">Represents the state of the deleted item.</span></span> |

## <a name="remarks"></a><span data-ttu-id="f77eb-117">注解</span><span class="sxs-lookup"><span data-stu-id="f77eb-117">Remarks</span></span> 

<span data-ttu-id="f77eb-118">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="f77eb-118">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted"
} -->
