---
title: assignedLicense 资源类型
description: 表示分配给用户的许可证。 user 实体的**assignedLicenses**属性是**assignedLicense**的集合。
localization_priority: Normal
ms.openlocfilehash: 619ce666c86abfd669fefc11b22760e7ac250ff5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328521"
---
# <a name="assignedlicense-resource-type"></a><span data-ttu-id="8d61f-104">assignedLicense 资源类型</span><span class="sxs-lookup"><span data-stu-id="8d61f-104">assignedLicense resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d61f-105">表示分配给用户的许可证。</span><span class="sxs-lookup"><span data-stu-id="8d61f-105">Represents a license assigned to a user.</span></span> <span data-ttu-id="8d61f-106">[user](user.md)实体的**assignedLicenses**属性是**assignedLicense**的集合。</span><span class="sxs-lookup"><span data-stu-id="8d61f-106">The **assignedLicenses** property of the [user](user.md) entity is a collection of **assignedLicense**.</span></span>

## <a name="properties"></a><span data-ttu-id="8d61f-107">属性</span><span class="sxs-lookup"><span data-stu-id="8d61f-107">Properties</span></span>
| <span data-ttu-id="8d61f-108">属性</span><span class="sxs-lookup"><span data-stu-id="8d61f-108">Property</span></span>     | <span data-ttu-id="8d61f-109">类型</span><span class="sxs-lookup"><span data-stu-id="8d61f-109">Type</span></span>   |<span data-ttu-id="8d61f-110">说明</span><span class="sxs-lookup"><span data-stu-id="8d61f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d61f-111">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="8d61f-111">disabledPlans</span></span>|<span data-ttu-id="8d61f-112">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="8d61f-112">Guid collection</span></span>|<span data-ttu-id="8d61f-113">已禁用的计划的唯一标识符的集合。</span><span class="sxs-lookup"><span data-stu-id="8d61f-113">A collection of the unique identifiers for plans that have been disabled.</span></span>|
|<span data-ttu-id="8d61f-114">skuId</span><span class="sxs-lookup"><span data-stu-id="8d61f-114">skuId</span></span>|<span data-ttu-id="8d61f-115">Guid</span><span class="sxs-lookup"><span data-stu-id="8d61f-115">Guid</span></span>|<span data-ttu-id="8d61f-116">此 SKU 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8d61f-116">The unique identifier for the SKU.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8d61f-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8d61f-117">JSON representation</span></span>

<span data-ttu-id="8d61f-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8d61f-118">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedLicense"
}-->

```json
{
  "disabledPlans": ["guid"],
  "skuId": "guid"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "assignedLicense resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
