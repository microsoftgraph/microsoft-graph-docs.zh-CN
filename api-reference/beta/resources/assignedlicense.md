---
title: assignedLicense 资源类型
description: 表示分配给用户的许可证。 **用户实体的 assignedLicenses** 属性是 **assignedLicense 的集合**。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: jpettere
ms.openlocfilehash: 4014198d211c2955866b1a56d80377e19ba4a38f
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721850"
---
# <a name="assignedlicense-resource-type"></a><span data-ttu-id="fd258-104">assignedLicense 资源类型</span><span class="sxs-lookup"><span data-stu-id="fd258-104">assignedLicense resource type</span></span>

<span data-ttu-id="fd258-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd258-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd258-106">表示分配给用户的许可证。</span><span class="sxs-lookup"><span data-stu-id="fd258-106">Represents a license assigned to a user.</span></span> <span data-ttu-id="fd258-107">**用户实体的 assignedLicenses** 属性是 **assignedLicense 的集合**。 [](user.md)</span><span class="sxs-lookup"><span data-stu-id="fd258-107">The **assignedLicenses** property of the [user](user.md) entity is a collection of **assignedLicense**.</span></span>

## <a name="properties"></a><span data-ttu-id="fd258-108">属性</span><span class="sxs-lookup"><span data-stu-id="fd258-108">Properties</span></span>
| <span data-ttu-id="fd258-109">属性</span><span class="sxs-lookup"><span data-stu-id="fd258-109">Property</span></span>     | <span data-ttu-id="fd258-110">类型</span><span class="sxs-lookup"><span data-stu-id="fd258-110">Type</span></span>   |<span data-ttu-id="fd258-111">说明</span><span class="sxs-lookup"><span data-stu-id="fd258-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd258-112">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="fd258-112">disabledPlans</span></span>|<span data-ttu-id="fd258-113">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="fd258-113">Guid collection</span></span>|<span data-ttu-id="fd258-114">已禁用的计划的唯一标识符的集合。</span><span class="sxs-lookup"><span data-stu-id="fd258-114">A collection of the unique identifiers for plans that have been disabled.</span></span>|
|<span data-ttu-id="fd258-115">skuId</span><span class="sxs-lookup"><span data-stu-id="fd258-115">skuId</span></span>|<span data-ttu-id="fd258-116">Guid</span><span class="sxs-lookup"><span data-stu-id="fd258-116">Guid</span></span>|<span data-ttu-id="fd258-117">此 SKU 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="fd258-117">The unique identifier for the SKU.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fd258-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fd258-118">JSON representation</span></span>

<span data-ttu-id="fd258-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fd258-119">Here is a JSON representation of the resource</span></span>

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


