---
title: expressionInputObject 资源类型
description: '代表要用作输入的测试数据时[synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md)操作执行表达式求值。'
ms.openlocfilehash: 06b7344f7e6418db0557f2b12dfa7e964b9d5ab7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048330"
---
# <a name="expressioninputobject-resource-type"></a><span data-ttu-id="a3202-103">expressionInputObject 资源类型</span><span class="sxs-lookup"><span data-stu-id="a3202-103">expressionInputObject resource type</span></span>

> <span data-ttu-id="a3202-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a3202-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a3202-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a3202-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a3202-106">代表要用作输入的测试数据时[synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md)操作执行表达式求值。</span><span class="sxs-lookup"><span data-stu-id="a3202-106">Represents an object to be used as input test data when the [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) action performs an expression evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="a3202-107">属性</span><span class="sxs-lookup"><span data-stu-id="a3202-107">Properties</span></span>
| <span data-ttu-id="a3202-108">属性</span><span class="sxs-lookup"><span data-stu-id="a3202-108">Property</span></span>     | <span data-ttu-id="a3202-109">类型</span><span class="sxs-lookup"><span data-stu-id="a3202-109">Type</span></span>   |<span data-ttu-id="a3202-110">说明</span><span class="sxs-lookup"><span data-stu-id="a3202-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a3202-111">definition</span><span class="sxs-lookup"><span data-stu-id="a3202-111">definition</span></span>|[<span data-ttu-id="a3202-112">objectDefinition</span><span class="sxs-lookup"><span data-stu-id="a3202-112">objectDefinition</span></span>](synchronization-objectdefinition.md)|<span data-ttu-id="a3202-113">测试对象的定义。</span><span class="sxs-lookup"><span data-stu-id="a3202-113">Definition of the test object.</span></span>|
|<span data-ttu-id="a3202-114">properties</span><span class="sxs-lookup"><span data-stu-id="a3202-114">properties</span></span>|<span data-ttu-id="a3202-115">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md)集合</span><span class="sxs-lookup"><span data-stu-id="a3202-115">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md) collection</span></span>|<span data-ttu-id="a3202-116">测试对象的属性值。</span><span class="sxs-lookup"><span data-stu-id="a3202-116">Property values of the test object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a3202-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a3202-117">JSON representation</span></span>

<span data-ttu-id="a3202-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3202-118">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "expressionInputObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->