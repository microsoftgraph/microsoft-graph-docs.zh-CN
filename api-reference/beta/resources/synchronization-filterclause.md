---
title: filterClause 资源类型
description: 表示候选对象必须满足的单个断言, 并计算为`true` (object 满足断言) 或`false` (对象不满足断言)。
localization_priority: Normal
ms.openlocfilehash: 62623cee5b2991acbe162561940adb1afd3574a1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582036"
---
# <a name="filterclause-resource-type"></a><span data-ttu-id="f66bf-103">filterClause 资源类型</span><span class="sxs-lookup"><span data-stu-id="f66bf-103">filterClause resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f66bf-104">表示候选对象必须满足的单个断言, 并计算为`true` (object 满足断言) 或`false` (对象不满足断言)。</span><span class="sxs-lookup"><span data-stu-id="f66bf-104">Represents a single assertion that a candidate object must satisfy, and is evaluated to either `true` (object satisfies the assertion) or `false` (object does not satisfy the assertion).</span></span>

## <a name="properties"></a><span data-ttu-id="f66bf-105">属性</span><span class="sxs-lookup"><span data-stu-id="f66bf-105">Properties</span></span>
| <span data-ttu-id="f66bf-106">属性</span><span class="sxs-lookup"><span data-stu-id="f66bf-106">Property</span></span>     | <span data-ttu-id="f66bf-107">类型</span><span class="sxs-lookup"><span data-stu-id="f66bf-107">Type</span></span>   |<span data-ttu-id="f66bf-108">说明</span><span class="sxs-lookup"><span data-stu-id="f66bf-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f66bf-109">operatorName</span><span class="sxs-lookup"><span data-stu-id="f66bf-109">operatorName</span></span>|<span data-ttu-id="f66bf-110">String</span><span class="sxs-lookup"><span data-stu-id="f66bf-110">String</span></span>|<span data-ttu-id="f66bf-111">要应用于源和目标操作数的运算符的名称。</span><span class="sxs-lookup"><span data-stu-id="f66bf-111">Name of the operator to be applied to the source and target operands.</span></span> <span data-ttu-id="f66bf-112">必须是受支持的运算符之一。</span><span class="sxs-lookup"><span data-stu-id="f66bf-112">Must be one of the supported operators.</span></span> <span data-ttu-id="f66bf-113">可以发现受支持的运算符。</span><span class="sxs-lookup"><span data-stu-id="f66bf-113">Supported operators can be discovered.</span></span>|
|<span data-ttu-id="f66bf-114">sourceOperandName</span><span class="sxs-lookup"><span data-stu-id="f66bf-114">sourceOperandName</span></span>|<span data-ttu-id="f66bf-115">String</span><span class="sxs-lookup"><span data-stu-id="f66bf-115">String</span></span>|<span data-ttu-id="f66bf-116">源操作数的名称 (所测试的操作数)。</span><span class="sxs-lookup"><span data-stu-id="f66bf-116">Name of source operand (the operand being tested).</span></span> <span data-ttu-id="f66bf-117">源操作数名称必须与源对象上的某个属性名称相匹配。</span><span class="sxs-lookup"><span data-stu-id="f66bf-117">The source operand name must match one of the attribute names on the source object.</span></span>|
|<span data-ttu-id="f66bf-118">targetOperand</span><span class="sxs-lookup"><span data-stu-id="f66bf-118">targetOperand</span></span>|[<span data-ttu-id="f66bf-119">filterOperand</span><span class="sxs-lookup"><span data-stu-id="f66bf-119">filterOperand</span></span>](synchronization-filteroperand.md)|<span data-ttu-id="f66bf-120">将对源操作数进行测试的值。</span><span class="sxs-lookup"><span data-stu-id="f66bf-120">Values that the source operand will be tested against.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f66bf-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f66bf-121">JSON representation</span></span>

<span data-ttu-id="f66bf-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f66bf-122">The following is a JSON representation of the resource.</span></span>

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
