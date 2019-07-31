---
title: expressionInputObject 资源类型
description: '表示当[synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md)操作执行表达式评估时用作输入测试数据的对象。'
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 113c38e540b8c41fb3d3156b27f6f5e1f1df42f2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007947"
---
# <a name="expressioninputobject-resource-type"></a><span data-ttu-id="3b404-103">expressionInputObject 资源类型</span><span class="sxs-lookup"><span data-stu-id="3b404-103">expressionInputObject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b404-104">表示在[parseExpression](../api/synchronization-synchronizationschema-parseexpression.md)操作执行表达式评估时用作输入测试数据的对象。</span><span class="sxs-lookup"><span data-stu-id="3b404-104">Represents an object to be used as input test data when the [parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) action performs an expression evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="3b404-105">属性</span><span class="sxs-lookup"><span data-stu-id="3b404-105">Properties</span></span>
| <span data-ttu-id="3b404-106">属性</span><span class="sxs-lookup"><span data-stu-id="3b404-106">Property</span></span>     | <span data-ttu-id="3b404-107">类型</span><span class="sxs-lookup"><span data-stu-id="3b404-107">Type</span></span>   |<span data-ttu-id="3b404-108">说明</span><span class="sxs-lookup"><span data-stu-id="3b404-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b404-109">定义</span><span class="sxs-lookup"><span data-stu-id="3b404-109">definition</span></span>|[<span data-ttu-id="3b404-110">objectDefinition</span><span class="sxs-lookup"><span data-stu-id="3b404-110">objectDefinition</span></span>](synchronization-objectdefinition.md)|<span data-ttu-id="3b404-111">Test 对象的定义。</span><span class="sxs-lookup"><span data-stu-id="3b404-111">Definition of the test object.</span></span>|
|<span data-ttu-id="3b404-112">properties</span><span class="sxs-lookup"><span data-stu-id="3b404-112">properties</span></span>|<span data-ttu-id="3b404-113">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md)集合</span><span class="sxs-lookup"><span data-stu-id="3b404-113">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md) collection</span></span>|<span data-ttu-id="3b404-114">Test 对象的属性值。</span><span class="sxs-lookup"><span data-stu-id="3b404-114">Property values of the test object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3b404-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3b404-115">JSON representation</span></span>

<span data-ttu-id="3b404-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3b404-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.expressionInputObject"
}-->

```json
{
  "definition": {"@odata.type": "microsoft.graph.objectDefinition"},
  "properties": [{"@odata.type": "microsoft.graph.stringKeyObjectValuePair"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "expressionInputObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
