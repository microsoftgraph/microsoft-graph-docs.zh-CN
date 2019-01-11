---
title: filterClause 资源类型
description: 代表单个断言候选对象必须满足的要求，并计算到`true`（对象满足断言） 或`false`（对象不满足声明）。
localization_priority: Normal
ms.openlocfilehash: 89807a6086f661388c8d5b1d5f82bfe973c3af39
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833857"
---
# <a name="filterclause-resource-type"></a><span data-ttu-id="0c4fc-103">filterClause 资源类型</span><span class="sxs-lookup"><span data-stu-id="0c4fc-103">filterClause resource type</span></span>

> <span data-ttu-id="0c4fc-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0c4fc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c4fc-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0c4fc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0c4fc-106">代表单个断言候选对象必须满足的要求，并计算到`true`（对象满足断言） 或`false`（对象不满足声明）。</span><span class="sxs-lookup"><span data-stu-id="0c4fc-106">Represents a single assertion that a candidate object must satisfy, and is evaluated to either `true` (object satisfies the assertion) or `false` (object does not satisfy the assertion).</span></span>

## <a name="properties"></a><span data-ttu-id="0c4fc-107">属性</span><span class="sxs-lookup"><span data-stu-id="0c4fc-107">Properties</span></span>
| <span data-ttu-id="0c4fc-108">属性</span><span class="sxs-lookup"><span data-stu-id="0c4fc-108">Property</span></span>     | <span data-ttu-id="0c4fc-109">类型</span><span class="sxs-lookup"><span data-stu-id="0c4fc-109">Type</span></span>   |<span data-ttu-id="0c4fc-110">Description</span><span class="sxs-lookup"><span data-stu-id="0c4fc-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c4fc-111">operatorName</span><span class="sxs-lookup"><span data-stu-id="0c4fc-111">operatorName</span></span>|<span data-ttu-id="0c4fc-112">字符串</span><span class="sxs-lookup"><span data-stu-id="0c4fc-112">String</span></span>|<span data-ttu-id="0c4fc-113">要应用于的源和目标操作数的运算符的名称。</span><span class="sxs-lookup"><span data-stu-id="0c4fc-113">Name of the operator to be applied to the source and target operands.</span></span> <span data-ttu-id="0c4fc-114">必须是受支持运算符之一。</span><span class="sxs-lookup"><span data-stu-id="0c4fc-114">Must be one of the supported operators.</span></span> <span data-ttu-id="0c4fc-115">可以发现受支持的运算符。</span><span class="sxs-lookup"><span data-stu-id="0c4fc-115">Supported operators can be discovered.</span></span>|
|<span data-ttu-id="0c4fc-116">sourceOperandName</span><span class="sxs-lookup"><span data-stu-id="0c4fc-116">sourceOperandName</span></span>|<span data-ttu-id="0c4fc-117">字符串</span><span class="sxs-lookup"><span data-stu-id="0c4fc-117">String</span></span>|<span data-ttu-id="0c4fc-118">源操作数 （正在测试的操作数） 的名称。</span><span class="sxs-lookup"><span data-stu-id="0c4fc-118">Name of source operand (the operand being tested).</span></span> <span data-ttu-id="0c4fc-119">源操作数名称必须匹配源对象上的属性名称之一。</span><span class="sxs-lookup"><span data-stu-id="0c4fc-119">The source operand name must match one of the attribute names on the source object.</span></span>|
|<span data-ttu-id="0c4fc-120">targetOperand</span><span class="sxs-lookup"><span data-stu-id="0c4fc-120">targetOperand</span></span>|[<span data-ttu-id="0c4fc-121">filterOperand</span><span class="sxs-lookup"><span data-stu-id="0c4fc-121">filterOperand</span></span>](synchronization-filteroperand.md)|<span data-ttu-id="0c4fc-122">将对照测试源操作数的值。</span><span class="sxs-lookup"><span data-stu-id="0c4fc-122">Values that the source operand will be tested against.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0c4fc-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0c4fc-123">JSON representation</span></span>

<span data-ttu-id="0c4fc-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0c4fc-124">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "filterClause resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
