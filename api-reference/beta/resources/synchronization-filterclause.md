---
title: filterClause 资源类型
description: 代表单个断言候选对象必须满足的要求，并计算到`true`（对象满足断言） 或`false`（对象不满足声明）。
localization_priority: Normal
ms.openlocfilehash: 62623cee5b2991acbe162561940adb1afd3574a1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523867"
---
# <a name="filterclause-resource-type"></a><span data-ttu-id="adbfd-103">filterClause 资源类型</span><span class="sxs-lookup"><span data-stu-id="adbfd-103">filterClause resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="adbfd-104">代表单个断言候选对象必须满足的要求，并计算到`true`（对象满足断言） 或`false`（对象不满足声明）。</span><span class="sxs-lookup"><span data-stu-id="adbfd-104">Represents a single assertion that a candidate object must satisfy, and is evaluated to either `true` (object satisfies the assertion) or `false` (object does not satisfy the assertion).</span></span>

## <a name="properties"></a><span data-ttu-id="adbfd-105">属性</span><span class="sxs-lookup"><span data-stu-id="adbfd-105">Properties</span></span>
| <span data-ttu-id="adbfd-106">属性</span><span class="sxs-lookup"><span data-stu-id="adbfd-106">Property</span></span>     | <span data-ttu-id="adbfd-107">类型</span><span class="sxs-lookup"><span data-stu-id="adbfd-107">Type</span></span>   |<span data-ttu-id="adbfd-108">说明</span><span class="sxs-lookup"><span data-stu-id="adbfd-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="adbfd-109">operatorName</span><span class="sxs-lookup"><span data-stu-id="adbfd-109">operatorName</span></span>|<span data-ttu-id="adbfd-110">String</span><span class="sxs-lookup"><span data-stu-id="adbfd-110">String</span></span>|<span data-ttu-id="adbfd-111">要应用于的源和目标操作数的运算符的名称。</span><span class="sxs-lookup"><span data-stu-id="adbfd-111">Name of the operator to be applied to the source and target operands.</span></span> <span data-ttu-id="adbfd-112">必须是受支持运算符之一。</span><span class="sxs-lookup"><span data-stu-id="adbfd-112">Must be one of the supported operators.</span></span> <span data-ttu-id="adbfd-113">可以发现受支持的运算符。</span><span class="sxs-lookup"><span data-stu-id="adbfd-113">Supported operators can be discovered.</span></span>|
|<span data-ttu-id="adbfd-114">sourceOperandName</span><span class="sxs-lookup"><span data-stu-id="adbfd-114">sourceOperandName</span></span>|<span data-ttu-id="adbfd-115">String</span><span class="sxs-lookup"><span data-stu-id="adbfd-115">String</span></span>|<span data-ttu-id="adbfd-116">源操作数 （正在测试的操作数） 的名称。</span><span class="sxs-lookup"><span data-stu-id="adbfd-116">Name of source operand (the operand being tested).</span></span> <span data-ttu-id="adbfd-117">源操作数名称必须匹配源对象上的属性名称之一。</span><span class="sxs-lookup"><span data-stu-id="adbfd-117">The source operand name must match one of the attribute names on the source object.</span></span>|
|<span data-ttu-id="adbfd-118">targetOperand</span><span class="sxs-lookup"><span data-stu-id="adbfd-118">targetOperand</span></span>|[<span data-ttu-id="adbfd-119">filterOperand</span><span class="sxs-lookup"><span data-stu-id="adbfd-119">filterOperand</span></span>](synchronization-filteroperand.md)|<span data-ttu-id="adbfd-120">将对照测试源操作数的值。</span><span class="sxs-lookup"><span data-stu-id="adbfd-120">Values that the source operand will be tested against.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="adbfd-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="adbfd-121">JSON representation</span></span>

<span data-ttu-id="adbfd-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="adbfd-122">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-filterclause.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
