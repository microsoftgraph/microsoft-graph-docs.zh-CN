---
title: filterClause 资源类型
description: 表示候选对象必须满足的单个断言。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: fc633f6e25373713679da30a5b319ab8ae99fb04
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131920"
---
# <a name="filterclause-resource-type"></a><span data-ttu-id="061de-103">filterClause 资源类型</span><span class="sxs-lookup"><span data-stu-id="061de-103">filterClause resource type</span></span>

<span data-ttu-id="061de-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="061de-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="061de-105">表示候选对象必须满足的单个断言，并计算为 (对象满足断言) 或 (对象不满足断言 `true` `false`) 。</span><span class="sxs-lookup"><span data-stu-id="061de-105">Represents a single assertion that a candidate object must satisfy, and is evaluated to either `true` (object satisfies the assertion) or `false` (object does not satisfy the assertion).</span></span>

## <a name="properties"></a><span data-ttu-id="061de-106">属性</span><span class="sxs-lookup"><span data-stu-id="061de-106">Properties</span></span>
| <span data-ttu-id="061de-107">属性</span><span class="sxs-lookup"><span data-stu-id="061de-107">Property</span></span>     | <span data-ttu-id="061de-108">类型</span><span class="sxs-lookup"><span data-stu-id="061de-108">Type</span></span>   |<span data-ttu-id="061de-109">说明</span><span class="sxs-lookup"><span data-stu-id="061de-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="061de-110">operatorName</span><span class="sxs-lookup"><span data-stu-id="061de-110">operatorName</span></span>|<span data-ttu-id="061de-111">字符串</span><span class="sxs-lookup"><span data-stu-id="061de-111">String</span></span>|<span data-ttu-id="061de-112">要应用于源操作数和目标操作数的运算符的名称。</span><span class="sxs-lookup"><span data-stu-id="061de-112">Name of the operator to be applied to the source and target operands.</span></span> <span data-ttu-id="061de-113">必须是受支持的运算符之一。</span><span class="sxs-lookup"><span data-stu-id="061de-113">Must be one of the supported operators.</span></span> <span data-ttu-id="061de-114">可以发现支持的运算符。</span><span class="sxs-lookup"><span data-stu-id="061de-114">Supported operators can be discovered.</span></span>|
|<span data-ttu-id="061de-115">sourceOperandName</span><span class="sxs-lookup"><span data-stu-id="061de-115">sourceOperandName</span></span>|<span data-ttu-id="061de-116">字符串</span><span class="sxs-lookup"><span data-stu-id="061de-116">String</span></span>|<span data-ttu-id="061de-117">要测试 (操作数的源操作数) 。</span><span class="sxs-lookup"><span data-stu-id="061de-117">Name of source operand (the operand being tested).</span></span> <span data-ttu-id="061de-118">源操作数名称必须与源对象上的某个属性名称匹配。</span><span class="sxs-lookup"><span data-stu-id="061de-118">The source operand name must match one of the attribute names on the source object.</span></span>|
|<span data-ttu-id="061de-119">targetOperand</span><span class="sxs-lookup"><span data-stu-id="061de-119">targetOperand</span></span>|[<span data-ttu-id="061de-120">filterOperand</span><span class="sxs-lookup"><span data-stu-id="061de-120">filterOperand</span></span>](synchronization-filteroperand.md)|<span data-ttu-id="061de-121">将针对其测试源操作数值。</span><span class="sxs-lookup"><span data-stu-id="061de-121">Values that the source operand will be tested against.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="061de-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="061de-122">JSON representation</span></span>

<span data-ttu-id="061de-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="061de-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterClause"
}-->

```json
{
  "operatorName": "String",
  "sourceOperandName": "String",
  "targetOperand": {"@odata.type": "microsoft.graph.filterOperand"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "filterClause resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


