---
title: 属性资源类型
description: 连接架构属性Microsoft 搜索定义。
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 6159126581d2a95cc45596a29cddff8642c5838f
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467218"
---
# <a name="property-resource-type"></a><span data-ttu-id="e6e79-103">属性资源类型</span><span class="sxs-lookup"><span data-stu-id="e6e79-103">property resource type</span></span>

<span data-ttu-id="e6e79-104">命名空间：microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="e6e79-104">Namespace: microsoft.graph.externalConnectors</span></span>



<span data-ttu-id="e6e79-105">连接[架构](externalconnectors-schema.md)的架构Microsoft 搜索[定义](externalconnectors-externalconnection.md)。</span><span class="sxs-lookup"><span data-stu-id="e6e79-105">A [schema](externalconnectors-schema.md) property definition for a Microsoft Search [connection](externalconnectors-externalconnection.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e6e79-106">属性</span><span class="sxs-lookup"><span data-stu-id="e6e79-106">Properties</span></span>
|<span data-ttu-id="e6e79-107">属性</span><span class="sxs-lookup"><span data-stu-id="e6e79-107">Property</span></span>|<span data-ttu-id="e6e79-108">类型</span><span class="sxs-lookup"><span data-stu-id="e6e79-108">Type</span></span>|<span data-ttu-id="e6e79-109">说明</span><span class="sxs-lookup"><span data-stu-id="e6e79-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6e79-110">aliases</span><span class="sxs-lookup"><span data-stu-id="e6e79-110">aliases</span></span>|<span data-ttu-id="e6e79-111">字符串集合</span><span class="sxs-lookup"><span data-stu-id="e6e79-111">String collection</span></span>|<span data-ttu-id="e6e79-112">属性的一组别名或友好名称。</span><span class="sxs-lookup"><span data-stu-id="e6e79-112">A set of aliases or a friendly names for the property.</span></span> <span data-ttu-id="e6e79-113">最多 32 个字符。</span><span class="sxs-lookup"><span data-stu-id="e6e79-113">Maximum 32 characters.</span></span> <span data-ttu-id="e6e79-114">每个字符串不得包含控制字符、空格或以下任何字符： `:` 、 、 `;` `,` 、 `(` `)` 、 `[` `]` 、 `{` 、 `}` 、 `%` `$` `+` `!` 、 `*` `=` `&` `?` `@` `#` `\` `~` `'` `"` `<` `>` `|` `` ` `` `^` 。</span><span class="sxs-lookup"><span data-stu-id="e6e79-114">Each string must not contain control characters, whitespace, or any of the following: `:`, `;`, `,`, `(`, `)`, `[`, `]`, `{`, `}`, `%`, `$`, `+`, `!`, `*`, `=`, `&`, `?`, `@`, `#`, `\`, `~`, `'`, `"`, `<`, `>`, `|`, `` ` ``, `^`.</span></span> <span data-ttu-id="e6e79-115">可选。</span><span class="sxs-lookup"><span data-stu-id="e6e79-115">Optional.</span></span>|
|<span data-ttu-id="e6e79-116">isQueryable</span><span class="sxs-lookup"><span data-stu-id="e6e79-116">isQueryable</span></span>|<span data-ttu-id="e6e79-117">布尔</span><span class="sxs-lookup"><span data-stu-id="e6e79-117">Boolean</span></span>|<span data-ttu-id="e6e79-118">指定属性是否可查询。</span><span class="sxs-lookup"><span data-stu-id="e6e79-118">Specifies if the property is queryable.</span></span> <span data-ttu-id="e6e79-119">可查询属性可用于关键字查询语言 [ (KQL) 查询](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)。</span><span class="sxs-lookup"><span data-stu-id="e6e79-119">Queryable properties can be used in [Keyword Query Language (KQL) queries](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference).</span></span> <span data-ttu-id="e6e79-120">可选。</span><span class="sxs-lookup"><span data-stu-id="e6e79-120">Optional.</span></span>|
|<span data-ttu-id="e6e79-121">isRefinable</span><span class="sxs-lookup"><span data-stu-id="e6e79-121">isRefinable</span></span>|<span data-ttu-id="e6e79-122">布尔</span><span class="sxs-lookup"><span data-stu-id="e6e79-122">Boolean</span></span>|<span data-ttu-id="e6e79-123">指定属性是否可精简。</span><span class="sxs-lookup"><span data-stu-id="e6e79-123">Specifies if the property is refinable.</span></span>  <span data-ttu-id="e6e79-124">可精简属性可用于筛选搜索[API](search-api-overview.md)中的搜索结果，在用户体验中Microsoft 搜索精简程序控件。</span><span class="sxs-lookup"><span data-stu-id="e6e79-124">Refinable properties can be used to filter search results in the [Search API](search-api-overview.md) and add a refiner control in the Microsoft Search user experience.</span></span> <span data-ttu-id="e6e79-125">可选。</span><span class="sxs-lookup"><span data-stu-id="e6e79-125">Optional.</span></span>|
|<span data-ttu-id="e6e79-126">isRetrievable</span><span class="sxs-lookup"><span data-stu-id="e6e79-126">isRetrievable</span></span>|<span data-ttu-id="e6e79-127">布尔</span><span class="sxs-lookup"><span data-stu-id="e6e79-127">Boolean</span></span>|<span data-ttu-id="e6e79-128">指定属性是否可检索。</span><span class="sxs-lookup"><span data-stu-id="e6e79-128">Specifies if the property is retrievable.</span></span> <span data-ttu-id="e6e79-129">当搜索 API 返回项目结果集可检索属性将返回在搜索记录中。</span><span class="sxs-lookup"><span data-stu-id="e6e79-129">Retrievable properties are returned in the result set when items are returned by the search API.</span></span> <span data-ttu-id="e6e79-130">还可将可检索属性添加到用于呈现搜索结果的显示模板。</span><span class="sxs-lookup"><span data-stu-id="e6e79-130">Retrievable properties are also available to add to the display template used to render search results.</span></span> <span data-ttu-id="e6e79-131">可选。</span><span class="sxs-lookup"><span data-stu-id="e6e79-131">Optional.</span></span>|
|<span data-ttu-id="e6e79-132">isSearchable</span><span class="sxs-lookup"><span data-stu-id="e6e79-132">isSearchable</span></span>|<span data-ttu-id="e6e79-133">布尔</span><span class="sxs-lookup"><span data-stu-id="e6e79-133">Boolean</span></span>|<span data-ttu-id="e6e79-134">指定属性是否可搜索。</span><span class="sxs-lookup"><span data-stu-id="e6e79-134">Specifies if the property is searchable.</span></span> <span data-ttu-id="e6e79-135">仅类型或 `String` `StringCollection` 可搜索的属性。</span><span class="sxs-lookup"><span data-stu-id="e6e79-135">Only properties of type `String` or `StringCollection` can be searchable.</span></span> <span data-ttu-id="e6e79-136">不可搜索的属性不会添加到搜索索引。</span><span class="sxs-lookup"><span data-stu-id="e6e79-136">Non-searchable properties are not added to the search index.</span></span> <span data-ttu-id="e6e79-137">可选。</span><span class="sxs-lookup"><span data-stu-id="e6e79-137">Optional.</span></span>|
|<span data-ttu-id="e6e79-138">labels</span><span class="sxs-lookup"><span data-stu-id="e6e79-138">labels</span></span>|<span data-ttu-id="e6e79-139">microsoft.graph.externalConnectors.label 集合</span><span class="sxs-lookup"><span data-stu-id="e6e79-139">microsoft.graph.externalConnectors.label collection</span></span>|<span data-ttu-id="e6e79-140">指定针对属性添加的一个或多个已知标记。</span><span class="sxs-lookup"><span data-stu-id="e6e79-140">Specifies one or more well-known tags added against a property.</span></span> <span data-ttu-id="e6e79-141">标签Microsoft 搜索了解连接中数据的语义。</span><span class="sxs-lookup"><span data-stu-id="e6e79-141">Labels help Microsoft Search understand the semantics of the data in the connection.</span></span> <span data-ttu-id="e6e79-142">添加适当的标签可增强搜索体验 (例如，提高相关性) 。</span><span class="sxs-lookup"><span data-stu-id="e6e79-142">Adding appropriate labels would result in an enhanced search experience (e.g. better relevance).</span></span> <span data-ttu-id="e6e79-143">支持的标签 `title` `url` `createdBy` ：、、、、、、、 `lastModifiedBy` `authors` 和 `createdDateTime` `lastModifiedDateTime` `fileName` `fileExtension` 。</span><span class="sxs-lookup"><span data-stu-id="e6e79-143">Supported labels: `title`, `url`, `createdBy`, `lastModifiedBy`, `authors`, `createdDateTime`, `lastModifiedDateTime`, `fileName` and `fileExtension`.</span></span> <span data-ttu-id="e6e79-144">可选。</span><span class="sxs-lookup"><span data-stu-id="e6e79-144">Optional.</span></span>|
|<span data-ttu-id="e6e79-145">name</span><span class="sxs-lookup"><span data-stu-id="e6e79-145">name</span></span>|<span data-ttu-id="e6e79-146">String</span><span class="sxs-lookup"><span data-stu-id="e6e79-146">String</span></span>|<span data-ttu-id="e6e79-147">属性的名称。</span><span class="sxs-lookup"><span data-stu-id="e6e79-147">The name of the property.</span></span> <span data-ttu-id="e6e79-148">最多 32 个字符。</span><span class="sxs-lookup"><span data-stu-id="e6e79-148">Maximum 32 characters.</span></span> <span data-ttu-id="e6e79-149">不得包含控制字符、空格或以下任何 `:` 字符：、 `;` `,` `(` `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=` `&` `?` `@` `#` `\` `~` `'` `"` `<` `>` `|` `` ` `` `^`</span><span class="sxs-lookup"><span data-stu-id="e6e79-149">Must not contain control characters, whitespace, or any of the following: `:`, `;`, `,`, `(`, `)`, `[`, `]`, `{`, `}`, `%`, `$`, `+`, `!`, `*`, `=`, `&`, `?`, `@`, `#`, `\`, `~`, `'`, `"`, `<`, `>`, `|`, `` ` ``, `^`.</span></span> <span data-ttu-id="e6e79-150">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="e6e79-150">Required.</span></span>|
|<span data-ttu-id="e6e79-151">type</span><span class="sxs-lookup"><span data-stu-id="e6e79-151">type</span></span>|<span data-ttu-id="e6e79-152">microsoft.graph.externalConnectors.propertyType</span><span class="sxs-lookup"><span data-stu-id="e6e79-152">microsoft.graph.externalConnectors.propertyType</span></span>|<span data-ttu-id="e6e79-153">属性的数据类型。</span><span class="sxs-lookup"><span data-stu-id="e6e79-153">The data type of the property.</span></span> <span data-ttu-id="e6e79-154">可取值为：`string`、`int64`、`double`、`dateTime`、`boolean`、`stringCollection`、`int64Collection`、`doubleCollection`、`dateTimeCollection`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="e6e79-154">Possible values are: `string`, `int64`, `double`, `dateTime`, `boolean`, `stringCollection`, `int64Collection`, `doubleCollection`, `dateTimeCollection`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6e79-155">关系</span><span class="sxs-lookup"><span data-stu-id="e6e79-155">Relationships</span></span>
<span data-ttu-id="e6e79-156">无。</span><span class="sxs-lookup"><span data-stu-id="e6e79-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6e79-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e6e79-157">JSON representation</span></span>
<span data-ttu-id="e6e79-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6e79-158">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalConnectors.property"
}
-->
``` json
{
  "name": "String",
  "type": "String",
  "isSearchable": "Boolean",
  "isRetrievable": "Boolean",
  "isQueryable": "Boolean",
  "isRefinable": "Boolean",
  "aliases": [
    "String"
  ],
  "labels": [
    "String"
  ]
}
```

