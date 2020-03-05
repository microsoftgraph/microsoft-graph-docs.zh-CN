---
title: expressionInputObject 资源类型
description: 表示当[synchronizationSchema： parseExpression](../api/synchronization_synchronizationschema_parseexpression.md)操作执行表达式评估时用作输入测试数据的对象。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 107dd80187f7b00439ec248be513d921bc64888e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520203"
---
# <a name="expressioninputobject-resource-type"></a><span data-ttu-id="a3630-103">expressionInputObject 资源类型</span><span class="sxs-lookup"><span data-stu-id="a3630-103">expressionInputObject resource type</span></span>

<span data-ttu-id="a3630-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="a3630-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3630-105">表示在[parseExpression](../api/synchronization-synchronizationschema-parseexpression.md)操作执行表达式评估时用作输入测试数据的对象。</span><span class="sxs-lookup"><span data-stu-id="a3630-105">Represents an object to be used as input test data when the [parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) action performs an expression evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="a3630-106">属性</span><span class="sxs-lookup"><span data-stu-id="a3630-106">Properties</span></span>
| <span data-ttu-id="a3630-107">属性</span><span class="sxs-lookup"><span data-stu-id="a3630-107">Property</span></span>     | <span data-ttu-id="a3630-108">类型</span><span class="sxs-lookup"><span data-stu-id="a3630-108">Type</span></span>   |<span data-ttu-id="a3630-109">说明</span><span class="sxs-lookup"><span data-stu-id="a3630-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a3630-110">定义</span><span class="sxs-lookup"><span data-stu-id="a3630-110">definition</span></span>|[<span data-ttu-id="a3630-111">objectDefinition</span><span class="sxs-lookup"><span data-stu-id="a3630-111">objectDefinition</span></span>](synchronization-objectdefinition.md)|<span data-ttu-id="a3630-112">Test 对象的定义。</span><span class="sxs-lookup"><span data-stu-id="a3630-112">Definition of the test object.</span></span>|
|<span data-ttu-id="a3630-113">properties</span><span class="sxs-lookup"><span data-stu-id="a3630-113">properties</span></span>|<span data-ttu-id="a3630-114">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md)集合</span><span class="sxs-lookup"><span data-stu-id="a3630-114">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md) collection</span></span>|<span data-ttu-id="a3630-115">Test 对象的属性值。</span><span class="sxs-lookup"><span data-stu-id="a3630-115">Property values of the test object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a3630-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a3630-116">JSON representation</span></span>

<span data-ttu-id="a3630-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3630-117">The following is a JSON representation of the resource.</span></span>

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
