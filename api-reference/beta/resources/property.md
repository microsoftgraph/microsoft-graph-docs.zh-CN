---
title: 属性资源类型
description: Microsoft 搜索连接的架构属性定义。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 087afe3e753ab68369899c0f0db07e93319e3687
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870150"
---
# <a name="property-resource-type"></a><span data-ttu-id="7d87c-103">属性资源类型</span><span class="sxs-lookup"><span data-stu-id="7d87c-103">property resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d87c-104">Microsoft 搜索[连接](externalconnection.md)的[架构](schema.md)属性定义。</span><span class="sxs-lookup"><span data-stu-id="7d87c-104">A [schema](schema.md) property definition for a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="7d87c-105">属性</span><span class="sxs-lookup"><span data-stu-id="7d87c-105">Properties</span></span>

| <span data-ttu-id="7d87c-106">属性</span><span class="sxs-lookup"><span data-stu-id="7d87c-106">Property</span></span>      | <span data-ttu-id="7d87c-107">类型</span><span class="sxs-lookup"><span data-stu-id="7d87c-107">Type</span></span>    | <span data-ttu-id="7d87c-108">说明</span><span class="sxs-lookup"><span data-stu-id="7d87c-108">Description</span></span>                                        |
|:--------------|:--------|:---------------------------------------------------|
| <span data-ttu-id="7d87c-109">isQueryable</span><span class="sxs-lookup"><span data-stu-id="7d87c-109">isQueryable</span></span>   | <span data-ttu-id="7d87c-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d87c-110">Boolean</span></span> | <span data-ttu-id="7d87c-111">指定属性是否为可查询属性。</span><span class="sxs-lookup"><span data-stu-id="7d87c-111">Specifies if the property is queryable.</span></span> <span data-ttu-id="7d87c-112">可查询属性可在[关键字查询语言（KQL）查询](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)中使用。</span><span class="sxs-lookup"><span data-stu-id="7d87c-112">Queryable properties can be used in [Keyword Query Language (KQL) queries](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference).</span></span> <span data-ttu-id="7d87c-113">可选。</span><span class="sxs-lookup"><span data-stu-id="7d87c-113">Optional.</span></span>  |
| <span data-ttu-id="7d87c-114">isRetrievable</span><span class="sxs-lookup"><span data-stu-id="7d87c-114">isRetrievable</span></span> | <span data-ttu-id="7d87c-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d87c-115">Boolean</span></span> | <span data-ttu-id="7d87c-116">指定属性是否可检索。</span><span class="sxs-lookup"><span data-stu-id="7d87c-116">Specifies if the property is retrievable.</span></span> <span data-ttu-id="7d87c-117">当搜索 API 返回项目时，将在结果集中返回可检索的属性。</span><span class="sxs-lookup"><span data-stu-id="7d87c-117">Retrievable properties are returned in the result set when items are returned by the search API.</span></span> <span data-ttu-id="7d87c-118">可检索属性也可用于添加到用于呈现搜索结果的显示模板。</span><span class="sxs-lookup"><span data-stu-id="7d87c-118">Retrievable properties are also available to add to the display template used to render search results.</span></span> <span data-ttu-id="7d87c-119">可选。</span><span class="sxs-lookup"><span data-stu-id="7d87c-119">Optional.</span></span> |
| <span data-ttu-id="7d87c-120">isSearchable</span><span class="sxs-lookup"><span data-stu-id="7d87c-120">isSearchable</span></span>  | <span data-ttu-id="7d87c-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d87c-121">Boolean</span></span> | <span data-ttu-id="7d87c-122">指定属性是否可搜索。</span><span class="sxs-lookup"><span data-stu-id="7d87c-122">Specifies if the property is searchable.</span></span> <span data-ttu-id="7d87c-123">仅可搜索的`String`类型`StringCollection`或属性的属性。</span><span class="sxs-lookup"><span data-stu-id="7d87c-123">Only properties of type `String` or `StringCollection` can be searchable.</span></span> <span data-ttu-id="7d87c-124">不可搜索的属性不会添加到搜索索引中。</span><span class="sxs-lookup"><span data-stu-id="7d87c-124">Non-searchable properties are not added to the search index.</span></span> <span data-ttu-id="7d87c-125">可选。</span><span class="sxs-lookup"><span data-stu-id="7d87c-125">Optional.</span></span> |
| <span data-ttu-id="7d87c-126">name</span><span class="sxs-lookup"><span data-stu-id="7d87c-126">name</span></span>          | <span data-ttu-id="7d87c-127">String</span><span class="sxs-lookup"><span data-stu-id="7d87c-127">String</span></span>  | <span data-ttu-id="7d87c-128">属性的名称。</span><span class="sxs-lookup"><span data-stu-id="7d87c-128">The name of the property.</span></span> <span data-ttu-id="7d87c-129">最多32个字符。</span><span class="sxs-lookup"><span data-stu-id="7d87c-129">Maximum 32 characters.</span></span> <span data-ttu-id="7d87c-130">不得包含控制字符、空白或以下任何内容`:`：、 `;` `,` `(` `)` `[` `]` `{` `}` `%` `$` `+` `!` `^`、、、、、、、、、、、、、、、、、、、、、、、、、、。 `|` `` ` `` `*` `=` `&` `?` `@` `#` `\` `~` `'` `"` `<` `>`</span><span class="sxs-lookup"><span data-stu-id="7d87c-130">Must not contain control characters, whitespace, or any of the following: `:`, `;`, `,`, `(`, `)`, `[`, `]`, `{`, `}`, `%`, `$`, `+`, `!`, `*`, `=`, `&`, `?`, `@`, `#`, `\`, `~`, `'`, `"`, `<`, `>`, `|`, `` ` ``, `^`.</span></span> <span data-ttu-id="7d87c-131">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="7d87c-131">Required.</span></span>                |
| <span data-ttu-id="7d87c-132">type</span><span class="sxs-lookup"><span data-stu-id="7d87c-132">type</span></span>          | <span data-ttu-id="7d87c-133">String</span><span class="sxs-lookup"><span data-stu-id="7d87c-133">String</span></span>  | <span data-ttu-id="7d87c-134">属性的数据类型。</span><span class="sxs-lookup"><span data-stu-id="7d87c-134">The data type of the property.</span></span> <span data-ttu-id="7d87c-135">可取值为：`String`、`Int64`、`Double`、`DateTime`、`Boolean`、`StringCollection`、`Int64Collection`、`DoubleCollection`、`DateTimeCollection`。</span><span class="sxs-lookup"><span data-stu-id="7d87c-135">Possible values are: `String`, `Int64`, `Double`, `DateTime`, `Boolean`, `StringCollection`, `Int64Collection`, `DoubleCollection`, `DateTimeCollection`.</span></span> <span data-ttu-id="7d87c-136">必需。</span><span class="sxs-lookup"><span data-stu-id="7d87c-136">Required.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7d87c-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7d87c-137">JSON representation</span></span>

<span data-ttu-id="7d87c-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7d87c-138">The following is a JSON representation of the resource.</span></span>

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
