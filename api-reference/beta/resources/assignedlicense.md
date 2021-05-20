---
title: assignedLicense 资源类型
description: 表示分配给用户的许可证。**用户** 实体的 AssignedLicenses 属性是一个 **assignedLicense** 集合。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: jpettere
ms.openlocfilehash: 9d957f2bfa5c7c9e4390e5c4df06d084a3e49e6f
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547247"
---
# <a name="assignedlicense-resource-type"></a><span data-ttu-id="83ee3-104">assignedLicense 资源类型</span><span class="sxs-lookup"><span data-stu-id="83ee3-104">assignedLicense resource type</span></span>

<span data-ttu-id="83ee3-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83ee3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83ee3-p102">表示分配给用户的许可证。**用户** 实体的 [AssignedLicenses](user.md) 属性是一个 **assignedLicense** 集合。</span><span class="sxs-lookup"><span data-stu-id="83ee3-p102">Represents a license assigned to a user. The **assignedLicenses** property of the [user](user.md) entity is a collection of **assignedLicense**.</span></span>

## <a name="properties"></a><span data-ttu-id="83ee3-108">属性</span><span class="sxs-lookup"><span data-stu-id="83ee3-108">Properties</span></span>
| <span data-ttu-id="83ee3-109">属性</span><span class="sxs-lookup"><span data-stu-id="83ee3-109">Property</span></span>     | <span data-ttu-id="83ee3-110">类型</span><span class="sxs-lookup"><span data-stu-id="83ee3-110">Type</span></span>   |<span data-ttu-id="83ee3-111">说明</span><span class="sxs-lookup"><span data-stu-id="83ee3-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="83ee3-112">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="83ee3-112">disabledPlans</span></span>|<span data-ttu-id="83ee3-113">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="83ee3-113">Guid collection</span></span>|<span data-ttu-id="83ee3-114">已禁用的计划的唯一标识符的集合。</span><span class="sxs-lookup"><span data-stu-id="83ee3-114">A collection of the unique identifiers for plans that have been disabled.</span></span>|
|<span data-ttu-id="83ee3-115">skuId</span><span class="sxs-lookup"><span data-stu-id="83ee3-115">skuId</span></span>|<span data-ttu-id="83ee3-116">Guid</span><span class="sxs-lookup"><span data-stu-id="83ee3-116">Guid</span></span>|<span data-ttu-id="83ee3-117">此 SKU 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="83ee3-117">The unique identifier for the SKU.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="83ee3-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="83ee3-118">JSON representation</span></span>

<span data-ttu-id="83ee3-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83ee3-119">Here is a JSON representation of the resource</span></span>

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


