---
title: 属性资源类型
description: Microsoft 搜索连接的架构属性定义。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9862170dfcca0960ebd319089da70cca93782875
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "44990262"
---
# <a name="property-resource-type"></a><span data-ttu-id="ff66d-103">属性资源类型</span><span class="sxs-lookup"><span data-stu-id="ff66d-103">property resource type</span></span>

<span data-ttu-id="ff66d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff66d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff66d-105">Microsoft 搜索[连接](externalconnection.md)的[架构](schema.md)属性定义。</span><span class="sxs-lookup"><span data-stu-id="ff66d-105">A [schema](schema.md) property definition for a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="ff66d-106">属性</span><span class="sxs-lookup"><span data-stu-id="ff66d-106">Properties</span></span>

| <span data-ttu-id="ff66d-107">属性</span><span class="sxs-lookup"><span data-stu-id="ff66d-107">Property</span></span>      | <span data-ttu-id="ff66d-108">类型</span><span class="sxs-lookup"><span data-stu-id="ff66d-108">Type</span></span>              | <span data-ttu-id="ff66d-109">说明</span><span class="sxs-lookup"><span data-stu-id="ff66d-109">Description</span></span>                                        |
|:--------------|:------------------|:---------------------------------------------------|
| <span data-ttu-id="ff66d-110">别名</span><span class="sxs-lookup"><span data-stu-id="ff66d-110">aliases</span></span>       | <span data-ttu-id="ff66d-111">String collection</span><span class="sxs-lookup"><span data-stu-id="ff66d-111">String collection</span></span> | <span data-ttu-id="ff66d-112">一组别名或属性的友好名称。</span><span class="sxs-lookup"><span data-stu-id="ff66d-112">A set of aliases or a friendly names for the property.</span></span> <span data-ttu-id="ff66d-113">最多32个字符。</span><span class="sxs-lookup"><span data-stu-id="ff66d-113">Maximum 32 characters.</span></span> <span data-ttu-id="ff66d-114">每个字符串不得包含控制字符、空白或以下任何内容：、、、、、、、、、、、、、、、、、、、、、、、、、、 `:` `;` `,` `(` `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=` `&` `?` `@` `#` `\` `~` `'` `"` `<` `>` `|` `` ` `` `^` 。</span><span class="sxs-lookup"><span data-stu-id="ff66d-114">Each string must not contain control characters, whitespace, or any of the following: `:`, `;`, `,`, `(`, `)`, `[`, `]`, `{`, `}`, `%`, `$`, `+`, `!`, `*`, `=`, `&`, `?`, `@`, `#`, `\`, `~`, `'`, `"`, `<`, `>`, `|`, `` ` ``, `^`.</span></span> <span data-ttu-id="ff66d-115">可选。</span><span class="sxs-lookup"><span data-stu-id="ff66d-115">Optional.</span></span>  |
| <span data-ttu-id="ff66d-116">isQueryable</span><span class="sxs-lookup"><span data-stu-id="ff66d-116">isQueryable</span></span>   | <span data-ttu-id="ff66d-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff66d-117">Boolean</span></span>           | <span data-ttu-id="ff66d-118">指定属性是否为可查询属性。</span><span class="sxs-lookup"><span data-stu-id="ff66d-118">Specifies if the property is queryable.</span></span> <span data-ttu-id="ff66d-119">可查询属性可在[关键字查询语言（KQL）查询](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)中使用。</span><span class="sxs-lookup"><span data-stu-id="ff66d-119">Queryable properties can be used in [Keyword Query Language (KQL) queries](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference).</span></span> <span data-ttu-id="ff66d-120">可选。</span><span class="sxs-lookup"><span data-stu-id="ff66d-120">Optional.</span></span>  |
| <span data-ttu-id="ff66d-121">isRefinable</span><span class="sxs-lookup"><span data-stu-id="ff66d-121">isRefinable</span></span>   | <span data-ttu-id="ff66d-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff66d-122">Boolean</span></span>           | <span data-ttu-id="ff66d-123">指定属性是否为可精简。</span><span class="sxs-lookup"><span data-stu-id="ff66d-123">Specifies if the property is refinable.</span></span>  <span data-ttu-id="ff66d-124">可精简属性可用于筛选[搜索 API](search-api-overview.md)中的搜索结果，并在 Microsoft search 用户体验中添加精简条件控件。</span><span class="sxs-lookup"><span data-stu-id="ff66d-124">Refinable properties can be used to filter search results in the [Search API](search-api-overview.md) and add a refiner control in the Microsoft Search user experience.</span></span> <span data-ttu-id="ff66d-125">可选。</span><span class="sxs-lookup"><span data-stu-id="ff66d-125">Optional.</span></span>  |
| <span data-ttu-id="ff66d-126">isRetrievable</span><span class="sxs-lookup"><span data-stu-id="ff66d-126">isRetrievable</span></span> | <span data-ttu-id="ff66d-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff66d-127">Boolean</span></span>           | <span data-ttu-id="ff66d-128">指定属性是否可检索。</span><span class="sxs-lookup"><span data-stu-id="ff66d-128">Specifies if the property is retrievable.</span></span> <span data-ttu-id="ff66d-129">当搜索 API 返回项目时，将在结果集中返回可检索的属性。</span><span class="sxs-lookup"><span data-stu-id="ff66d-129">Retrievable properties are returned in the result set when items are returned by the search API.</span></span> <span data-ttu-id="ff66d-130">可检索属性也可用于添加到用于呈现搜索结果的显示模板。</span><span class="sxs-lookup"><span data-stu-id="ff66d-130">Retrievable properties are also available to add to the display template used to render search results.</span></span> <span data-ttu-id="ff66d-131">可选。</span><span class="sxs-lookup"><span data-stu-id="ff66d-131">Optional.</span></span> |
| <span data-ttu-id="ff66d-132">isSearchable</span><span class="sxs-lookup"><span data-stu-id="ff66d-132">isSearchable</span></span>  | <span data-ttu-id="ff66d-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff66d-133">Boolean</span></span>           | <span data-ttu-id="ff66d-134">指定属性是否可搜索。</span><span class="sxs-lookup"><span data-stu-id="ff66d-134">Specifies if the property is searchable.</span></span> <span data-ttu-id="ff66d-135">仅可搜索的类型或属性的属性 `String` `StringCollection` 。</span><span class="sxs-lookup"><span data-stu-id="ff66d-135">Only properties of type `String` or `StringCollection` can be searchable.</span></span> <span data-ttu-id="ff66d-136">不可搜索的属性不会添加到搜索索引中。</span><span class="sxs-lookup"><span data-stu-id="ff66d-136">Non-searchable properties are not added to the search index.</span></span> <span data-ttu-id="ff66d-137">可选。</span><span class="sxs-lookup"><span data-stu-id="ff66d-137">Optional.</span></span> |
| <span data-ttu-id="ff66d-138">标题</span><span class="sxs-lookup"><span data-stu-id="ff66d-138">labels</span></span>        | <span data-ttu-id="ff66d-139">String collection</span><span class="sxs-lookup"><span data-stu-id="ff66d-139">String collection</span></span> | <span data-ttu-id="ff66d-140">指定针对属性添加的一个或多个已知标记。</span><span class="sxs-lookup"><span data-stu-id="ff66d-140">Specifies one or more well-known tags added against a property.</span></span> <span data-ttu-id="ff66d-141">标签可帮助 Microsoft 搜索了解连接中的数据的语义。</span><span class="sxs-lookup"><span data-stu-id="ff66d-141">Labels help Microsoft Search understand the semantics of the data in the connection.</span></span> <span data-ttu-id="ff66d-142">添加适当的标签将导致增强的搜索体验（如更好的相关性）。</span><span class="sxs-lookup"><span data-stu-id="ff66d-142">Adding appropriate labels would result in an enhanced search experience (e.g. better relevance).</span></span> <span data-ttu-id="ff66d-143">支持的标签：、、、、、、 `title` `url` `createdBy` `lastModifiedBy` `authors` `createdDateTime` `lastModifiedDateTime` `fileName` 和 `fileExtension` 。</span><span class="sxs-lookup"><span data-stu-id="ff66d-143">Supported labels: `title`, `url`, `createdBy`, `lastModifiedBy`, `authors`, `createdDateTime`, `lastModifiedDateTime`, `fileName` and `fileExtension`.</span></span> <span data-ttu-id="ff66d-144">可选。</span><span class="sxs-lookup"><span data-stu-id="ff66d-144">Optional.</span></span> |
| <span data-ttu-id="ff66d-145">name</span><span class="sxs-lookup"><span data-stu-id="ff66d-145">name</span></span>          | <span data-ttu-id="ff66d-146">String</span><span class="sxs-lookup"><span data-stu-id="ff66d-146">String</span></span>            | <span data-ttu-id="ff66d-147">属性的名称。</span><span class="sxs-lookup"><span data-stu-id="ff66d-147">The name of the property.</span></span> <span data-ttu-id="ff66d-148">最多32个字符。</span><span class="sxs-lookup"><span data-stu-id="ff66d-148">Maximum 32 characters.</span></span> <span data-ttu-id="ff66d-149">不得包含控制字符、空白或以下任何内容：、、、、、、、、、、、、、、、、、、、、、、、、、、、 `:` `;` `,` `(` `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=` `&` `?` `@` `#` `\` `~` `'` `"` `<` `>` `|` `` ` `` `^` 。</span><span class="sxs-lookup"><span data-stu-id="ff66d-149">Must not contain control characters, whitespace, or any of the following: `:`, `;`, `,`, `(`, `)`, `[`, `]`, `{`, `}`, `%`, `$`, `+`, `!`, `*`, `=`, `&`, `?`, `@`, `#`, `\`, `~`, `'`, `"`, `<`, `>`, `|`, `` ` ``, `^`.</span></span> <span data-ttu-id="ff66d-150">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="ff66d-150">Required.</span></span>                |
| <span data-ttu-id="ff66d-151">type</span><span class="sxs-lookup"><span data-stu-id="ff66d-151">type</span></span>          | <span data-ttu-id="ff66d-152">String</span><span class="sxs-lookup"><span data-stu-id="ff66d-152">String</span></span>            | <span data-ttu-id="ff66d-153">属性的数据类型。</span><span class="sxs-lookup"><span data-stu-id="ff66d-153">The data type of the property.</span></span> <span data-ttu-id="ff66d-154">可取值为：`String`、`Int64`、`Double`、`DateTime`、`Boolean`、`StringCollection`、`Int64Collection`、`DoubleCollection`、`DateTimeCollection`。</span><span class="sxs-lookup"><span data-stu-id="ff66d-154">Possible values are: `String`, `Int64`, `Double`, `DateTime`, `Boolean`, `StringCollection`, `Int64Collection`, `DoubleCollection`, `DateTimeCollection`.</span></span> <span data-ttu-id="ff66d-155">必需。</span><span class="sxs-lookup"><span data-stu-id="ff66d-155">Required.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ff66d-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ff66d-156">JSON representation</span></span>

<span data-ttu-id="ff66d-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff66d-157">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.property",
  "baseType": null
}-->

```json
{
  "aliases": [ "String" ],
  "isQueryable": true,
  "isRefinable": true,
  "isRetrievable": true,
  "isSearchable": true,
  "labels": [ "String" ],
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
