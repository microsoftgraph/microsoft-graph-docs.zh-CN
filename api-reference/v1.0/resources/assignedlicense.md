---
title: assignedLicense 资源类型
description: 表示分配给用户的许可证。 **user 实体的 assignedLicenses** 属性是 **assignedLicense 的集合**。
localization_priority: Normal
author: jpettere
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d6cb848506d7f78b652f3d094c7b74c4cade6543
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720807"
---
# <a name="assignedlicense-resource-type"></a><span data-ttu-id="327c3-104">assignedLicense 资源类型</span><span class="sxs-lookup"><span data-stu-id="327c3-104">assignedLicense resource type</span></span>

<span data-ttu-id="327c3-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="327c3-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="327c3-106">表示分配给用户的许可证。</span><span class="sxs-lookup"><span data-stu-id="327c3-106">Represents a license assigned to a user.</span></span> <span data-ttu-id="327c3-107">**user 实体的 assignedLicenses** 属性是 **assignedLicense 的集合**。 [](user.md)</span><span class="sxs-lookup"><span data-stu-id="327c3-107">The **assignedLicenses** property of the [user](user.md) entity is a collection of **assignedLicense**.</span></span>

## <a name="properties"></a><span data-ttu-id="327c3-108">属性</span><span class="sxs-lookup"><span data-stu-id="327c3-108">Properties</span></span>
| <span data-ttu-id="327c3-109">属性</span><span class="sxs-lookup"><span data-stu-id="327c3-109">Property</span></span>     | <span data-ttu-id="327c3-110">类型</span><span class="sxs-lookup"><span data-stu-id="327c3-110">Type</span></span>   |<span data-ttu-id="327c3-111">说明</span><span class="sxs-lookup"><span data-stu-id="327c3-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="327c3-112">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="327c3-112">disabledPlans</span></span>|<span data-ttu-id="327c3-113">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="327c3-113">Guid collection</span></span>|<span data-ttu-id="327c3-114">已禁用的计划的唯一标识符的集合。</span><span class="sxs-lookup"><span data-stu-id="327c3-114">A collection of the unique identifiers for plans that have been disabled.</span></span>|
|<span data-ttu-id="327c3-115">skuId</span><span class="sxs-lookup"><span data-stu-id="327c3-115">skuId</span></span>|<span data-ttu-id="327c3-116">Guid</span><span class="sxs-lookup"><span data-stu-id="327c3-116">Guid</span></span>|<span data-ttu-id="327c3-117">此 SKU 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="327c3-117">The unique identifier for the SKU.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="327c3-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="327c3-118">JSON representation</span></span>

<span data-ttu-id="327c3-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="327c3-119">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "assignedLicense resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

