---
title: expressionEvaluationDetails 资源类型
description: 表示表达式的详细信息、结果和属性详细信息。
localization_priority: Normal
author: yyuank
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 347e356bda19228ea8b3738b5bf8b72f57da95f7
ms.sourcegitcommit: 62c900af626e46439d949462f09061cc5c41d6ff
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/16/2020
ms.locfileid: "44272825"
---
# <a name="expressionevaluationdetails-resource-type"></a><span data-ttu-id="ff00f-103">expressionEvaluationDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="ff00f-103">expressionEvaluationDetails resource type</span></span>

<span data-ttu-id="ff00f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff00f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff00f-105">表示表达式的详细信息、结果和属性详细信息。</span><span class="sxs-lookup"><span data-stu-id="ff00f-105">Represents the expression details, result, and property details.</span></span>

## <a name="properties"></a><span data-ttu-id="ff00f-106">属性</span><span class="sxs-lookup"><span data-stu-id="ff00f-106">Properties</span></span>

| <span data-ttu-id="ff00f-107">属性</span><span class="sxs-lookup"><span data-stu-id="ff00f-107">Property</span></span>     | <span data-ttu-id="ff00f-108">类型</span><span class="sxs-lookup"><span data-stu-id="ff00f-108">Type</span></span>        | <span data-ttu-id="ff00f-109">Description</span><span class="sxs-lookup"><span data-stu-id="ff00f-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ff00f-110">表达式</span><span class="sxs-lookup"><span data-stu-id="ff00f-110">expression</span></span> | <span data-ttu-id="ff00f-111">String</span><span class="sxs-lookup"><span data-stu-id="ff00f-111">String</span></span> | <span data-ttu-id="ff00f-112">表示已计算的表达式。</span><span class="sxs-lookup"><span data-stu-id="ff00f-112">Represents expression which has been evaluated.</span></span> |
| <span data-ttu-id="ff00f-113">expressionEvaluationDetails</span><span class="sxs-lookup"><span data-stu-id="ff00f-113">expressionEvaluationDetails</span></span> | <span data-ttu-id="ff00f-114">expressionEvaluationDetails 集合</span><span class="sxs-lookup"><span data-stu-id="ff00f-114">expressionEvaluationDetails collection</span></span> | <span data-ttu-id="ff00f-115">表示表达式计算的详细信息。</span><span class="sxs-lookup"><span data-stu-id="ff00f-115">Represents the details of the evaluation of the expression.</span></span> |
| <span data-ttu-id="ff00f-116">expressionResult</span><span class="sxs-lookup"><span data-stu-id="ff00f-116">expressionResult</span></span> | <span data-ttu-id="ff00f-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff00f-117">Boolean</span></span> | <span data-ttu-id="ff00f-118">表示当前表达式的结果的值。</span><span class="sxs-lookup"><span data-stu-id="ff00f-118">Represents the value of the result of the current expression.</span></span> |
| <span data-ttu-id="ff00f-119">propertyToEvaluate</span><span class="sxs-lookup"><span data-stu-id="ff00f-119">propertyToEvaluate</span></span> | [<span data-ttu-id="ff00f-120">propertyToEvaluate</span><span class="sxs-lookup"><span data-stu-id="ff00f-120">propertyToEvaluate</span></span>](propertytoevaluate.md) | <span data-ttu-id="ff00f-121">定义属性的名称和该属性的值。</span><span class="sxs-lookup"><span data-stu-id="ff00f-121">Defines the name of the property and the value of that property.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ff00f-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ff00f-122">JSON representation</span></span>

<span data-ttu-id="ff00f-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff00f-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.expressionEvaluationDetails",
  "baseType": null
}-->

```json
{
  "expression": "String",
  "expressionEvaluationDetails": [{"@odata.type": "microsoft.graph.expressionEvaluationDetails"}],
  "expressionResult": true,
  "propertyToEvaluate": {"@odata.type": "microsoft.graph.propertyToEvaluate"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "expressionEvaluationDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
