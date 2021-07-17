---
title: 属性资源类型
description: 连接架构属性Microsoft 搜索定义。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 68dfe94d81f4ae5347322ba17c02eb3dab5c15d7
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467663"
---
# <a name="property-resource-type"></a><span data-ttu-id="a4f98-103">属性资源类型</span><span class="sxs-lookup"><span data-stu-id="a4f98-103">property resource type</span></span>

<span data-ttu-id="a4f98-104">命名空间：microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="a4f98-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4f98-105">连接[架构](externalconnectors-schema.md)的架构Microsoft 搜索[定义](externalconnectors-externalconnection.md)。</span><span class="sxs-lookup"><span data-stu-id="a4f98-105">A [schema](externalconnectors-schema.md) property definition for a Microsoft Search [connection](externalconnectors-externalconnection.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a4f98-106">属性</span><span class="sxs-lookup"><span data-stu-id="a4f98-106">Properties</span></span>

| <span data-ttu-id="a4f98-107">属性</span><span class="sxs-lookup"><span data-stu-id="a4f98-107">Property</span></span>      | <span data-ttu-id="a4f98-108">类型</span><span class="sxs-lookup"><span data-stu-id="a4f98-108">Type</span></span>              | <span data-ttu-id="a4f98-109">说明</span><span class="sxs-lookup"><span data-stu-id="a4f98-109">Description</span></span>                                        |
|:--------------|:------------------|:---------------------------------------------------|
| <span data-ttu-id="a4f98-110">aliases</span><span class="sxs-lookup"><span data-stu-id="a4f98-110">aliases</span></span>       | <span data-ttu-id="a4f98-111">字符串集合</span><span class="sxs-lookup"><span data-stu-id="a4f98-111">String collection</span></span> | <span data-ttu-id="a4f98-112">属性的一组别名或友好名称。</span><span class="sxs-lookup"><span data-stu-id="a4f98-112">A set of aliases or a friendly names for the property.</span></span> <span data-ttu-id="a4f98-113">最多 32 个字符。</span><span class="sxs-lookup"><span data-stu-id="a4f98-113">Maximum 32 characters.</span></span> <span data-ttu-id="a4f98-114">每个字符串不得包含控制字符、空格或以下任何字符： `:` 、 、 `;` `,` 、 `(` `)` 、 `[` `]` 、 `{` 、 `}` 、 `%` `$` `+` `!` 、 `*` `=` `&` `?` `@` `#` `\` `~` `'` `"` `<` `>` `|` `` ` `` `^` 。</span><span class="sxs-lookup"><span data-stu-id="a4f98-114">Each string must not contain control characters, whitespace, or any of the following: `:`, `;`, `,`, `(`, `)`, `[`, `]`, `{`, `}`, `%`, `$`, `+`, `!`, `*`, `=`, `&`, `?`, `@`, `#`, `\`, `~`, `'`, `"`, `<`, `>`, `|`, `` ` ``, `^`.</span></span> <span data-ttu-id="a4f98-115">可选。</span><span class="sxs-lookup"><span data-stu-id="a4f98-115">Optional.</span></span>  |
| <span data-ttu-id="a4f98-116">isQueryable</span><span class="sxs-lookup"><span data-stu-id="a4f98-116">isQueryable</span></span>   | <span data-ttu-id="a4f98-117">boolean</span><span class="sxs-lookup"><span data-stu-id="a4f98-117">boolean</span></span>           | <span data-ttu-id="a4f98-118">指定属性是否可查询。</span><span class="sxs-lookup"><span data-stu-id="a4f98-118">Specifies if the property is queryable.</span></span> <span data-ttu-id="a4f98-119">可查询属性可用于关键字查询语言 [ (KQL) 查询](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)。</span><span class="sxs-lookup"><span data-stu-id="a4f98-119">Queryable properties can be used in [Keyword Query Language (KQL) queries](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference).</span></span> <span data-ttu-id="a4f98-120">可选。</span><span class="sxs-lookup"><span data-stu-id="a4f98-120">Optional.</span></span>  |
| <span data-ttu-id="a4f98-121">isRefinable</span><span class="sxs-lookup"><span data-stu-id="a4f98-121">isRefinable</span></span>   | <span data-ttu-id="a4f98-122">boolean</span><span class="sxs-lookup"><span data-stu-id="a4f98-122">boolean</span></span>           | <span data-ttu-id="a4f98-123">指定属性是否可精简。</span><span class="sxs-lookup"><span data-stu-id="a4f98-123">Specifies if the property is refinable.</span></span>  <span data-ttu-id="a4f98-124">可精简属性可用于筛选搜索[API](search-api-overview.md)中的搜索结果，在用户体验中Microsoft 搜索精简程序控件。</span><span class="sxs-lookup"><span data-stu-id="a4f98-124">Refinable properties can be used to filter search results in the [Search API](search-api-overview.md) and add a refiner control in the Microsoft Search user experience.</span></span> <span data-ttu-id="a4f98-125">可选。</span><span class="sxs-lookup"><span data-stu-id="a4f98-125">Optional.</span></span>  |
| <span data-ttu-id="a4f98-126">isRetrievable</span><span class="sxs-lookup"><span data-stu-id="a4f98-126">isRetrievable</span></span> | <span data-ttu-id="a4f98-127">boolean</span><span class="sxs-lookup"><span data-stu-id="a4f98-127">boolean</span></span>           | <span data-ttu-id="a4f98-128">指定属性是否可检索。</span><span class="sxs-lookup"><span data-stu-id="a4f98-128">Specifies if the property is retrievable.</span></span> <span data-ttu-id="a4f98-129">当搜索 API 返回项目结果集可检索属性将返回在搜索记录中。</span><span class="sxs-lookup"><span data-stu-id="a4f98-129">Retrievable properties are returned in the result set when items are returned by the search API.</span></span> <span data-ttu-id="a4f98-130">还可将可检索属性添加到用于呈现搜索结果的显示模板。</span><span class="sxs-lookup"><span data-stu-id="a4f98-130">Retrievable properties are also available to add to the display template used to render search results.</span></span> <span data-ttu-id="a4f98-131">可选。</span><span class="sxs-lookup"><span data-stu-id="a4f98-131">Optional.</span></span> |
| <span data-ttu-id="a4f98-132">isSearchable</span><span class="sxs-lookup"><span data-stu-id="a4f98-132">isSearchable</span></span>  | <span data-ttu-id="a4f98-133">boolean</span><span class="sxs-lookup"><span data-stu-id="a4f98-133">boolean</span></span>           | <span data-ttu-id="a4f98-134">指定属性是否可搜索。</span><span class="sxs-lookup"><span data-stu-id="a4f98-134">Specifies if the property is searchable.</span></span> <span data-ttu-id="a4f98-135">仅类型或 `string` `stringCollection` 可搜索的属性。</span><span class="sxs-lookup"><span data-stu-id="a4f98-135">Only properties of type `string` or `stringCollection` can be searchable.</span></span> <span data-ttu-id="a4f98-136">不可搜索的属性不会添加到搜索索引。</span><span class="sxs-lookup"><span data-stu-id="a4f98-136">Non-searchable properties are not added to the search index.</span></span> <span data-ttu-id="a4f98-137">可选。</span><span class="sxs-lookup"><span data-stu-id="a4f98-137">Optional.</span></span> |
| <span data-ttu-id="a4f98-138">labels</span><span class="sxs-lookup"><span data-stu-id="a4f98-138">labels</span></span>        | <span data-ttu-id="a4f98-139">字符串集合</span><span class="sxs-lookup"><span data-stu-id="a4f98-139">String collection</span></span> | <span data-ttu-id="a4f98-140">指定针对属性添加的一个或多个已知标记。</span><span class="sxs-lookup"><span data-stu-id="a4f98-140">Specifies one or more well-known tags added against a property.</span></span> <span data-ttu-id="a4f98-141">标签Microsoft 搜索了解连接中数据的语义。</span><span class="sxs-lookup"><span data-stu-id="a4f98-141">Labels help Microsoft Search understand the semantics of the data in the connection.</span></span> <span data-ttu-id="a4f98-142">添加适当的标签可增强搜索体验 (例如，提高相关性) 。</span><span class="sxs-lookup"><span data-stu-id="a4f98-142">Adding appropriate labels would result in an enhanced search experience (e.g. better relevance).</span></span> <span data-ttu-id="a4f98-143">支持的标签 `title` `url` `createdBy` ：、、、、、、、 `lastModifiedBy` `authors` 和 `createdDateTime` `lastModifiedDateTime` `fileName` `fileExtension` `iconUrl` `containerName` `containerUrl` 。</span><span class="sxs-lookup"><span data-stu-id="a4f98-143">Supported labels: `title`, `url`, `createdBy`, `lastModifiedBy`, `authors`, `createdDateTime`, `lastModifiedDateTime`, `fileName`, `fileExtension`, `iconUrl`, `containerName`, and `containerUrl`.</span></span> <span data-ttu-id="a4f98-144">可选。</span><span class="sxs-lookup"><span data-stu-id="a4f98-144">Optional.</span></span> |
| <span data-ttu-id="a4f98-145">name</span><span class="sxs-lookup"><span data-stu-id="a4f98-145">name</span></span>          | <span data-ttu-id="a4f98-146">String</span><span class="sxs-lookup"><span data-stu-id="a4f98-146">String</span></span>            | <span data-ttu-id="a4f98-147">属性的名称。</span><span class="sxs-lookup"><span data-stu-id="a4f98-147">The name of the property.</span></span> <span data-ttu-id="a4f98-148">最多 32 个字符。</span><span class="sxs-lookup"><span data-stu-id="a4f98-148">Maximum 32 characters.</span></span> <span data-ttu-id="a4f98-149">不得包含控制字符、空格或以下任何 `:` 字符：、 `;` `,` `(` `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=` `&` `?` `@` `#` `\` `~` `'` `"` `<` `>` `|` `` ` `` `^`</span><span class="sxs-lookup"><span data-stu-id="a4f98-149">Must not contain control characters, whitespace, or any of the following: `:`, `;`, `,`, `(`, `)`, `[`, `]`, `{`, `}`, `%`, `$`, `+`, `!`, `*`, `=`, `&`, `?`, `@`, `#`, `\`, `~`, `'`, `"`, `<`, `>`, `|`, `` ` ``, `^`.</span></span> <span data-ttu-id="a4f98-150">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="a4f98-150">Required.</span></span>                |
| <span data-ttu-id="a4f98-151">type</span><span class="sxs-lookup"><span data-stu-id="a4f98-151">type</span></span>          | <span data-ttu-id="a4f98-152">String</span><span class="sxs-lookup"><span data-stu-id="a4f98-152">String</span></span>            | <span data-ttu-id="a4f98-153">属性的数据类型。</span><span class="sxs-lookup"><span data-stu-id="a4f98-153">The data type of the property.</span></span> <span data-ttu-id="a4f98-154">可取值为：`string`、`int64`、`double`、`dateTime`、`boolean`、`stringCollection`、`int64Collection`、`doubleCollection`、`dateTimeCollection`。</span><span class="sxs-lookup"><span data-stu-id="a4f98-154">Possible values are: `string`, `int64`, `double`, `dateTime`, `boolean`, `stringCollection`, `int64Collection`, `doubleCollection`, `dateTimeCollection`.</span></span> <span data-ttu-id="a4f98-155">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="a4f98-155">Required.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a4f98-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a4f98-156">JSON representation</span></span>

<span data-ttu-id="a4f98-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a4f98-157">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnectors.property",
  "baseType": null
}-->

```json
{
  "aliases": [ "String" ],
  "isQueryable": true,
  "isRefinable": true,
  "isRetrievable": true,
  "isSearchable": true,
  "labels": [ "string" ],
  "name": "string",
  "type": "string"
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
