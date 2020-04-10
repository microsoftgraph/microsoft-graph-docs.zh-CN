---
title: filterClause 资源类型
description: 表示候选对象必须满足的单个断言。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6688f26353bed9e92f60a93b688b1679e70bd75f
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218427"
---
# <a name="filterclause-resource-type"></a><span data-ttu-id="7f252-103">filterClause 资源类型</span><span class="sxs-lookup"><span data-stu-id="7f252-103">filterClause resource type</span></span>

<span data-ttu-id="7f252-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f252-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f252-105">表示候选对象必须满足的单个断言，并计算为`true` （object 满足断言）或`false` （对象不满足断言）。</span><span class="sxs-lookup"><span data-stu-id="7f252-105">Represents a single assertion that a candidate object must satisfy, and is evaluated to either `true` (object satisfies the assertion) or `false` (object does not satisfy the assertion).</span></span>

## <a name="properties"></a><span data-ttu-id="7f252-106">属性</span><span class="sxs-lookup"><span data-stu-id="7f252-106">Properties</span></span>
| <span data-ttu-id="7f252-107">属性</span><span class="sxs-lookup"><span data-stu-id="7f252-107">Property</span></span>     | <span data-ttu-id="7f252-108">类型</span><span class="sxs-lookup"><span data-stu-id="7f252-108">Type</span></span>   |<span data-ttu-id="7f252-109">说明</span><span class="sxs-lookup"><span data-stu-id="7f252-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f252-110">operatorName</span><span class="sxs-lookup"><span data-stu-id="7f252-110">operatorName</span></span>|<span data-ttu-id="7f252-111">字符串</span><span class="sxs-lookup"><span data-stu-id="7f252-111">String</span></span>|<span data-ttu-id="7f252-112">要应用于源和目标操作数的运算符的名称。</span><span class="sxs-lookup"><span data-stu-id="7f252-112">Name of the operator to be applied to the source and target operands.</span></span> <span data-ttu-id="7f252-113">必须是受支持的运算符之一。</span><span class="sxs-lookup"><span data-stu-id="7f252-113">Must be one of the supported operators.</span></span> <span data-ttu-id="7f252-114">可以发现受支持的运算符。</span><span class="sxs-lookup"><span data-stu-id="7f252-114">Supported operators can be discovered.</span></span>|
|<span data-ttu-id="7f252-115">sourceOperandName</span><span class="sxs-lookup"><span data-stu-id="7f252-115">sourceOperandName</span></span>|<span data-ttu-id="7f252-116">字符串</span><span class="sxs-lookup"><span data-stu-id="7f252-116">String</span></span>|<span data-ttu-id="7f252-117">源操作数的名称（所测试的操作数）。</span><span class="sxs-lookup"><span data-stu-id="7f252-117">Name of source operand (the operand being tested).</span></span> <span data-ttu-id="7f252-118">源操作数名称必须与源对象上的某个属性名称相匹配。</span><span class="sxs-lookup"><span data-stu-id="7f252-118">The source operand name must match one of the attribute names on the source object.</span></span>|
|<span data-ttu-id="7f252-119">targetOperand</span><span class="sxs-lookup"><span data-stu-id="7f252-119">targetOperand</span></span>|[<span data-ttu-id="7f252-120">filterOperand</span><span class="sxs-lookup"><span data-stu-id="7f252-120">filterOperand</span></span>](synchronization-filteroperand.md)|<span data-ttu-id="7f252-121">将对源操作数进行测试的值。</span><span class="sxs-lookup"><span data-stu-id="7f252-121">Values that the source operand will be tested against.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7f252-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7f252-122">JSON representation</span></span>

<span data-ttu-id="7f252-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7f252-123">The following is a JSON representation of the resource.</span></span>

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
