---
title: expressionInputObject 资源类型
description: 表示在 synchronizationSchema parseExpression 操作执行表达式评估时用作输入测试数据的对象。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e9727f50b05eb8cdb5319883dd0058a91d9383cc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968351"
---
# <a name="expressioninputobject-resource-type"></a><span data-ttu-id="982ba-103">expressionInputObject 资源类型</span><span class="sxs-lookup"><span data-stu-id="982ba-103">expressionInputObject resource type</span></span>

<span data-ttu-id="982ba-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="982ba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="982ba-105">表示在 [parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) 操作执行表达式评估时用作输入测试数据的对象。</span><span class="sxs-lookup"><span data-stu-id="982ba-105">Represents an object to be used as input test data when the [parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) action performs an expression evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="982ba-106">属性</span><span class="sxs-lookup"><span data-stu-id="982ba-106">Properties</span></span>
| <span data-ttu-id="982ba-107">属性</span><span class="sxs-lookup"><span data-stu-id="982ba-107">Property</span></span>     | <span data-ttu-id="982ba-108">类型</span><span class="sxs-lookup"><span data-stu-id="982ba-108">Type</span></span>   |<span data-ttu-id="982ba-109">说明</span><span class="sxs-lookup"><span data-stu-id="982ba-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="982ba-110">定义</span><span class="sxs-lookup"><span data-stu-id="982ba-110">definition</span></span>|[<span data-ttu-id="982ba-111">objectDefinition</span><span class="sxs-lookup"><span data-stu-id="982ba-111">objectDefinition</span></span>](synchronization-objectdefinition.md)|<span data-ttu-id="982ba-112">Test 对象的定义。</span><span class="sxs-lookup"><span data-stu-id="982ba-112">Definition of the test object.</span></span>|
|<span data-ttu-id="982ba-113">properties</span><span class="sxs-lookup"><span data-stu-id="982ba-113">properties</span></span>|<span data-ttu-id="982ba-114">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="982ba-114">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md) collection</span></span>|<span data-ttu-id="982ba-115">Test 对象的属性值。</span><span class="sxs-lookup"><span data-stu-id="982ba-115">Property values of the test object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="982ba-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="982ba-116">JSON representation</span></span>

<span data-ttu-id="982ba-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="982ba-117">The following is a JSON representation of the resource.</span></span>

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


