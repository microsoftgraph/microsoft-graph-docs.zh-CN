---
title: 属性资源类型
description: Microsoft 搜索连接的架构属性定义。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: df535b89d238f31185ff187b207671337d05fd75
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939086"
---
# <a name="property-resource-type"></a><span data-ttu-id="1ba30-103">属性资源类型</span><span class="sxs-lookup"><span data-stu-id="1ba30-103">property resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ba30-104">Microsoft 搜索[连接](externalconnection.md)的[架构](schema.md)属性定义。</span><span class="sxs-lookup"><span data-stu-id="1ba30-104">A [schema](schema.md) property definition for a Microsoft Search [connection](externalconnection.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1ba30-105">属性</span><span class="sxs-lookup"><span data-stu-id="1ba30-105">Properties</span></span>

| <span data-ttu-id="1ba30-106">属性</span><span class="sxs-lookup"><span data-stu-id="1ba30-106">Property</span></span>      | <span data-ttu-id="1ba30-107">类型</span><span class="sxs-lookup"><span data-stu-id="1ba30-107">Type</span></span>    | <span data-ttu-id="1ba30-108">描述</span><span class="sxs-lookup"><span data-stu-id="1ba30-108">Description</span></span>                                        |
|:--------------|:--------|:---------------------------------------------------|
| <span data-ttu-id="1ba30-109">isQueryable</span><span class="sxs-lookup"><span data-stu-id="1ba30-109">isQueryable</span></span>   | <span data-ttu-id="1ba30-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ba30-110">Boolean</span></span> | <span data-ttu-id="1ba30-111">指定属性是否为可查询属性。</span><span class="sxs-lookup"><span data-stu-id="1ba30-111">Specifies if the property is queryable.</span></span> <span data-ttu-id="1ba30-112">可查询属性可在[关键字查询语言（KQL）查询](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)中使用。</span><span class="sxs-lookup"><span data-stu-id="1ba30-112">Queryable properties can be used in [Keyword Query Language (KQL) queries](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference).</span></span> <span data-ttu-id="1ba30-113">可选。</span><span class="sxs-lookup"><span data-stu-id="1ba30-113">Optional.</span></span>  |
| <span data-ttu-id="1ba30-114">isRetrievable</span><span class="sxs-lookup"><span data-stu-id="1ba30-114">isRetrievable</span></span> | <span data-ttu-id="1ba30-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ba30-115">Boolean</span></span> | <span data-ttu-id="1ba30-116">指定属性是否可检索。</span><span class="sxs-lookup"><span data-stu-id="1ba30-116">Specifies if the property is retrievable.</span></span> <span data-ttu-id="1ba30-117">当搜索 API 返回项目时，将在结果集中返回可检索的属性。</span><span class="sxs-lookup"><span data-stu-id="1ba30-117">Retrievable properties are returned in the result set when items are returned by the search API.</span></span> <span data-ttu-id="1ba30-118">可检索属性也可用于添加到用于呈现搜索结果的显示模板。</span><span class="sxs-lookup"><span data-stu-id="1ba30-118">Retrievable properties are also available to add to the display template used to render search results.</span></span> <span data-ttu-id="1ba30-119">可选。</span><span class="sxs-lookup"><span data-stu-id="1ba30-119">Optional.</span></span> |
| <span data-ttu-id="1ba30-120">isSearchable</span><span class="sxs-lookup"><span data-stu-id="1ba30-120">isSearchable</span></span>  | <span data-ttu-id="1ba30-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ba30-121">Boolean</span></span> | <span data-ttu-id="1ba30-122">指定属性是否可搜索。</span><span class="sxs-lookup"><span data-stu-id="1ba30-122">Specifies if the property is searchable.</span></span> <span data-ttu-id="1ba30-123">仅可搜索的`String`类型`Collection(String)`或属性的属性。</span><span class="sxs-lookup"><span data-stu-id="1ba30-123">Only properties of type `String` or `Collection(String)` can be searchable.</span></span> <span data-ttu-id="1ba30-124">不可搜索的属性不会添加到搜索索引中。</span><span class="sxs-lookup"><span data-stu-id="1ba30-124">Non-searchable properties are not added to the search index.</span></span> <span data-ttu-id="1ba30-125">可选。</span><span class="sxs-lookup"><span data-stu-id="1ba30-125">Optional.</span></span> |
| <span data-ttu-id="1ba30-126">name</span><span class="sxs-lookup"><span data-stu-id="1ba30-126">name</span></span>          | <span data-ttu-id="1ba30-127">String</span><span class="sxs-lookup"><span data-stu-id="1ba30-127">String</span></span>  | <span data-ttu-id="1ba30-128">属性的名称。</span><span class="sxs-lookup"><span data-stu-id="1ba30-128">The name of the property.</span></span> <span data-ttu-id="1ba30-129">最多32个字符。</span><span class="sxs-lookup"><span data-stu-id="1ba30-129">Maximum 32 characters.</span></span> <span data-ttu-id="1ba30-130">不得包含`:`控制字符、空白或以下任何内容：、 `;`、 `,` `(` `)` `[` `]` `{` `}` `%` `$` `+` `!` `*`、、、、、、、、、、、、、 `=``&`, `?`, `@`, `#`, `\`, `~`, `'`, `"`, `<`, `>`, `|`, `` ` ``, `^`.</span><span class="sxs-lookup"><span data-stu-id="1ba30-130">Must not contain control characters, whitespace, or any of the following: `:`, `;`, `,`, `(`, `)`, `[`, `]`, `{`, `}`, `%`, `$`, `+`, `!`, `*`, `=`, `&`, `?`, `@`, `#`, `\`, `~`, `'`, `"`, `<`, `>`, `|`, `` ` ``, `^`.</span></span> <span data-ttu-id="1ba30-131">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="1ba30-131">Required.</span></span>                |
| <span data-ttu-id="1ba30-132">type</span><span class="sxs-lookup"><span data-stu-id="1ba30-132">type</span></span>          | <span data-ttu-id="1ba30-133">字符串</span><span class="sxs-lookup"><span data-stu-id="1ba30-133">String</span></span>  | <span data-ttu-id="1ba30-134">属性的数据类型。</span><span class="sxs-lookup"><span data-stu-id="1ba30-134">The data type of the property.</span></span> <span data-ttu-id="1ba30-135">可取值为：`String`、`Int64`、`Double`、`DateTime`、`Boolean`、`Collection(String)`、`Collection(Int64)`、`Collection(Double)`、`Collection(DateTime)`。</span><span class="sxs-lookup"><span data-stu-id="1ba30-135">Possible values are: `String`, `Int64`, `Double`, `DateTime`, `Boolean`, `Collection(String)`, `Collection(Int64)`, `Collection(Double)`, `Collection(DateTime)`.</span></span> <span data-ttu-id="1ba30-136">必填。</span><span class="sxs-lookup"><span data-stu-id="1ba30-136">Required.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1ba30-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1ba30-137">JSON representation</span></span>

<span data-ttu-id="1ba30-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1ba30-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.property",
  "baseType": null
}-->

```json
{
  "isQueryable": true,
  "isRetrievable": true,
  "isSearchable": true,
  "name": "String",
  "type": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "property resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
