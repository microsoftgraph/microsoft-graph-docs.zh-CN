---
title: 属性资源类型
description: Microsoft 搜索连接的架构属性定义。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 48a61c9f26a7f5b90e41fc2cd36334d4061449dc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521381"
---
# <a name="property-resource-type"></a><span data-ttu-id="84ae9-103">属性资源类型</span><span class="sxs-lookup"><span data-stu-id="84ae9-103">property resource type</span></span>

<span data-ttu-id="84ae9-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="84ae9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84ae9-105">Microsoft 搜索[连接](externalconnection.md)的[架构](schema.md)属性定义。</span><span class="sxs-lookup"><span data-stu-id="84ae9-105">A [schema](schema.md) property definition for a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="84ae9-106">属性</span><span class="sxs-lookup"><span data-stu-id="84ae9-106">Properties</span></span>

| <span data-ttu-id="84ae9-107">属性</span><span class="sxs-lookup"><span data-stu-id="84ae9-107">Property</span></span>      | <span data-ttu-id="84ae9-108">类型</span><span class="sxs-lookup"><span data-stu-id="84ae9-108">Type</span></span>    | <span data-ttu-id="84ae9-109">说明</span><span class="sxs-lookup"><span data-stu-id="84ae9-109">Description</span></span>                                        |
|:--------------|:--------|:---------------------------------------------------|
| <span data-ttu-id="84ae9-110">isQueryable</span><span class="sxs-lookup"><span data-stu-id="84ae9-110">isQueryable</span></span>   | <span data-ttu-id="84ae9-111">布尔</span><span class="sxs-lookup"><span data-stu-id="84ae9-111">Boolean</span></span> | <span data-ttu-id="84ae9-112">指定属性是否为可查询属性。</span><span class="sxs-lookup"><span data-stu-id="84ae9-112">Specifies if the property is queryable.</span></span> <span data-ttu-id="84ae9-113">可查询属性可在[关键字查询语言（KQL）查询](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)中使用。</span><span class="sxs-lookup"><span data-stu-id="84ae9-113">Queryable properties can be used in [Keyword Query Language (KQL) queries](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference).</span></span> <span data-ttu-id="84ae9-114">可选。</span><span class="sxs-lookup"><span data-stu-id="84ae9-114">Optional.</span></span>  |
| <span data-ttu-id="84ae9-115">isRetrievable</span><span class="sxs-lookup"><span data-stu-id="84ae9-115">isRetrievable</span></span> | <span data-ttu-id="84ae9-116">布尔</span><span class="sxs-lookup"><span data-stu-id="84ae9-116">Boolean</span></span> | <span data-ttu-id="84ae9-117">指定属性是否可检索。</span><span class="sxs-lookup"><span data-stu-id="84ae9-117">Specifies if the property is retrievable.</span></span> <span data-ttu-id="84ae9-118">当搜索 API 返回项目时，将在结果集中返回可检索的属性。</span><span class="sxs-lookup"><span data-stu-id="84ae9-118">Retrievable properties are returned in the result set when items are returned by the search API.</span></span> <span data-ttu-id="84ae9-119">可检索属性也可用于添加到用于呈现搜索结果的显示模板。</span><span class="sxs-lookup"><span data-stu-id="84ae9-119">Retrievable properties are also available to add to the display template used to render search results.</span></span> <span data-ttu-id="84ae9-120">可选。</span><span class="sxs-lookup"><span data-stu-id="84ae9-120">Optional.</span></span> |
| <span data-ttu-id="84ae9-121">isSearchable</span><span class="sxs-lookup"><span data-stu-id="84ae9-121">isSearchable</span></span>  | <span data-ttu-id="84ae9-122">布尔</span><span class="sxs-lookup"><span data-stu-id="84ae9-122">Boolean</span></span> | <span data-ttu-id="84ae9-123">指定属性是否可搜索。</span><span class="sxs-lookup"><span data-stu-id="84ae9-123">Specifies if the property is searchable.</span></span> <span data-ttu-id="84ae9-124">仅可搜索的`String`类型`StringCollection`或属性的属性。</span><span class="sxs-lookup"><span data-stu-id="84ae9-124">Only properties of type `String` or `StringCollection` can be searchable.</span></span> <span data-ttu-id="84ae9-125">不可搜索的属性不会添加到搜索索引中。</span><span class="sxs-lookup"><span data-stu-id="84ae9-125">Non-searchable properties are not added to the search index.</span></span> <span data-ttu-id="84ae9-126">可选。</span><span class="sxs-lookup"><span data-stu-id="84ae9-126">Optional.</span></span> |
| <span data-ttu-id="84ae9-127">name</span><span class="sxs-lookup"><span data-stu-id="84ae9-127">name</span></span>          | <span data-ttu-id="84ae9-128">String</span><span class="sxs-lookup"><span data-stu-id="84ae9-128">String</span></span>  | <span data-ttu-id="84ae9-129">属性的名称。</span><span class="sxs-lookup"><span data-stu-id="84ae9-129">The name of the property.</span></span> <span data-ttu-id="84ae9-130">最多32个字符。</span><span class="sxs-lookup"><span data-stu-id="84ae9-130">Maximum 32 characters.</span></span> <span data-ttu-id="84ae9-131">不得包含控制字符、空白或以下任何内容`:`：、 `;` `,` `(` `)` `[` `]` `{` `}` `%` `$` `+` `!` `^`、、、、、、、、、、、、、、、、、、、、、、、、、、。 `|` `` ` `` `*` `=` `&` `?` `@` `#` `\` `~` `'` `"` `<` `>`</span><span class="sxs-lookup"><span data-stu-id="84ae9-131">Must not contain control characters, whitespace, or any of the following: `:`, `;`, `,`, `(`, `)`, `[`, `]`, `{`, `}`, `%`, `$`, `+`, `!`, `*`, `=`, `&`, `?`, `@`, `#`, `\`, `~`, `'`, `"`, `<`, `>`, `|`, `` ` ``, `^`.</span></span> <span data-ttu-id="84ae9-132">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="84ae9-132">Required.</span></span>                |
| <span data-ttu-id="84ae9-133">type</span><span class="sxs-lookup"><span data-stu-id="84ae9-133">type</span></span>          | <span data-ttu-id="84ae9-134">String</span><span class="sxs-lookup"><span data-stu-id="84ae9-134">String</span></span>  | <span data-ttu-id="84ae9-135">属性的数据类型。</span><span class="sxs-lookup"><span data-stu-id="84ae9-135">The data type of the property.</span></span> <span data-ttu-id="84ae9-136">可取值为：`String`、`Int64`、`Double`、`DateTime`、`Boolean`、`StringCollection`、`Int64Collection`、`DoubleCollection`、`DateTimeCollection`。</span><span class="sxs-lookup"><span data-stu-id="84ae9-136">Possible values are: `String`, `Int64`, `Double`, `DateTime`, `Boolean`, `StringCollection`, `Int64Collection`, `DoubleCollection`, `DateTimeCollection`.</span></span> <span data-ttu-id="84ae9-137">必填。</span><span class="sxs-lookup"><span data-stu-id="84ae9-137">Required.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="84ae9-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="84ae9-138">JSON representation</span></span>

<span data-ttu-id="84ae9-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84ae9-139">The following is a JSON representation of the resource.</span></span>

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
