---
author: JeremyKelley
description: 表示网站、列表或 contentType 中的列。
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 982b9751f522d34a5cdf1dd329262486d35bfb0a
ms.sourcegitcommit: 73bbf84e6f5dbc8c3db8ed2c48cc5ab9ae3cff78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2021
ms.locfileid: "53456469"
---
# <a name="columndefinition-resource-type"></a><span data-ttu-id="abb7c-103">columnDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="abb7c-103">columnDefinition resource type</span></span>

<span data-ttu-id="abb7c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abb7c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abb7c-105">表示网站、[列表或][] [contentType][][中的][]列。</span><span class="sxs-lookup"><span data-stu-id="abb7c-105">Represents a column in a [site][], [list][] or [contentType][].</span></span>

## <a name="methods"></a><span data-ttu-id="abb7c-106">方法</span><span class="sxs-lookup"><span data-stu-id="abb7c-106">Methods</span></span>
|<span data-ttu-id="abb7c-107">方法</span><span class="sxs-lookup"><span data-stu-id="abb7c-107">Method</span></span>|<span data-ttu-id="abb7c-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="abb7c-108">Return type</span></span>|<span data-ttu-id="abb7c-109">说明</span><span class="sxs-lookup"><span data-stu-id="abb7c-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="abb7c-110">列出网站中的列</span><span class="sxs-lookup"><span data-stu-id="abb7c-110">List columns in a site</span></span>](../api/site-list-columns.md)|<span data-ttu-id="abb7c-111">[columnDefinition](../resources/columndefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="abb7c-111">[columnDefinition](../resources/columndefinition.md) collection</span></span>|<span data-ttu-id="abb7c-112">获取网站中的 [columnDefinition](../resources/columndefinition.md) 对象及其属性 [的列表](../resources/site.md)。</span><span class="sxs-lookup"><span data-stu-id="abb7c-112">Get a list of the [columnDefinition](../resources/columndefinition.md) objects and their properties in a [site](../resources/site.md).</span></span>|
|[<span data-ttu-id="abb7c-113">列出列表中的列</span><span class="sxs-lookup"><span data-stu-id="abb7c-113">List columns in a list</span></span>](../api/list-list-columns.md)|<span data-ttu-id="abb7c-114">[columnDefinition](../resources/columndefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="abb7c-114">[columnDefinition](../resources/columndefinition.md) collection</span></span>|<span data-ttu-id="abb7c-115">在列表中获取 [columnDefinition](../resources/columndefinition.md) 对象及其属性 [的列表](../resources/list.md)。</span><span class="sxs-lookup"><span data-stu-id="abb7c-115">Get a list of the [columnDefinition](../resources/columndefinition.md) objects and their properties in a [list](../resources/list.md).</span></span>|
|[<span data-ttu-id="abb7c-116">列出内容类型中的列</span><span class="sxs-lookup"><span data-stu-id="abb7c-116">List columns in a content type</span></span>](../api/contenttype-list-columns.md)|<span data-ttu-id="abb7c-117">[columnDefinition](../resources/columndefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="abb7c-117">[columnDefinition](../resources/columndefinition.md) collection</span></span>|<span data-ttu-id="abb7c-118">获取内容类型中的 [columnDefinition](../resources/columndefinition.md) 对象及其 [属性的列表](../resources/contenttype.md)。</span><span class="sxs-lookup"><span data-stu-id="abb7c-118">Get a list of the [columnDefinition](../resources/columndefinition.md) objects and their properties in a [content type](../resources/contenttype.md).</span></span>|
|[<span data-ttu-id="abb7c-119">为网站创建 columnDefinition</span><span class="sxs-lookup"><span data-stu-id="abb7c-119">Create columnDefinition for a site</span></span>](../api/site-post-columns.md)|[<span data-ttu-id="abb7c-120">columnDefinition</span><span class="sxs-lookup"><span data-stu-id="abb7c-120">columnDefinition</span></span>](../resources/columndefinition.md)|<span data-ttu-id="abb7c-121">在网站 [中创建新的 columnDefinition](../resources/columndefinition.md) [对象](../resources/site.md)。</span><span class="sxs-lookup"><span data-stu-id="abb7c-121">Create a new [columnDefinition](../resources/columndefinition.md) object in a [site](../resources/site.md).</span></span>|
|[<span data-ttu-id="abb7c-122">为列表创建 columnDefinition</span><span class="sxs-lookup"><span data-stu-id="abb7c-122">Create columnDefinition for a list</span></span>](../api/list-post-columns.md)|[<span data-ttu-id="abb7c-123">columnDefinition</span><span class="sxs-lookup"><span data-stu-id="abb7c-123">columnDefinition</span></span>](../resources/columndefinition.md)|<span data-ttu-id="abb7c-124">在列表中 [创建新的 columnDefinition](../resources/columndefinition.md) [对象](../resources/list.md)。</span><span class="sxs-lookup"><span data-stu-id="abb7c-124">Create a new [columnDefinition](../resources/columndefinition.md) object in a [list](../resources/list.md).</span></span>|
|[<span data-ttu-id="abb7c-125">为内容类型创建 columnDefinition</span><span class="sxs-lookup"><span data-stu-id="abb7c-125">Create columnDefinition for a content type</span></span>](../api/contenttype-post-columns.md)|[<span data-ttu-id="abb7c-126">columnDefinition</span><span class="sxs-lookup"><span data-stu-id="abb7c-126">columnDefinition</span></span>](../resources/columndefinition.md)|<span data-ttu-id="abb7c-127">在内容类型 [中创建新的 columnDefinition](../resources/columndefinition.md) [对象](../resources/contenttype.md)。</span><span class="sxs-lookup"><span data-stu-id="abb7c-127">Create a new [columnDefinition](../resources/columndefinition.md) object in a [content type](../resources/contenttype.md).</span></span>|
|[<span data-ttu-id="abb7c-128">获取 columnDefinition</span><span class="sxs-lookup"><span data-stu-id="abb7c-128">Get columnDefinition</span></span>](../api/columndefinition-get.md)|[<span data-ttu-id="abb7c-129">columnDefinition</span><span class="sxs-lookup"><span data-stu-id="abb7c-129">columnDefinition</span></span>](../resources/columndefinition.md)|<span data-ttu-id="abb7c-130">读取 [columnDefinition 对象的属性和](../resources/columndefinition.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="abb7c-130">Read the properties and relationships of a [columnDefinition](../resources/columndefinition.md) object.</span></span>|
|[<span data-ttu-id="abb7c-131">更新 columnDefinition</span><span class="sxs-lookup"><span data-stu-id="abb7c-131">Update columnDefinition</span></span>](../api/columndefinition-update.md)|[<span data-ttu-id="abb7c-132">columnDefinition</span><span class="sxs-lookup"><span data-stu-id="abb7c-132">columnDefinition</span></span>](../resources/columndefinition.md)|<span data-ttu-id="abb7c-133">更新 [columnDefinition 对象](../resources/columndefinition.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="abb7c-133">Update the properties of a [columnDefinition](../resources/columndefinition.md) object.</span></span>|
|[<span data-ttu-id="abb7c-134">删除 columnDefinition</span><span class="sxs-lookup"><span data-stu-id="abb7c-134">Delete columnDefinition</span></span>](../api/columndefinition-delete.md)|<span data-ttu-id="abb7c-135">无</span><span class="sxs-lookup"><span data-stu-id="abb7c-135">None</span></span>|<span data-ttu-id="abb7c-136">删除 [columnDefinition](../resources/columndefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="abb7c-136">Deletes a [columnDefinition](../resources/columndefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="abb7c-137">属性</span><span class="sxs-lookup"><span data-stu-id="abb7c-137">Properties</span></span>

<span data-ttu-id="abb7c-138">列可以包含各种类型的数据。</span><span class="sxs-lookup"><span data-stu-id="abb7c-138">Columns can hold data of various types.</span></span>
<span data-ttu-id="abb7c-139">以下属性表示列存储的数据类型以及该数据的其他设置。</span><span class="sxs-lookup"><span data-stu-id="abb7c-139">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="abb7c-140">与类型相关的属性 (布尔、计算、选项、货币、dateTime、lookup、number、personOrGroup、text) 是互斥的 -列只能指定其中一个。</span><span class="sxs-lookup"><span data-stu-id="abb7c-140">The type-related properties (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="abb7c-141">属性名称</span><span class="sxs-lookup"><span data-stu-id="abb7c-141">Property name</span></span>           | <span data-ttu-id="abb7c-142">类型</span><span class="sxs-lookup"><span data-stu-id="abb7c-142">Type</span></span>    | <span data-ttu-id="abb7c-143">说明</span><span class="sxs-lookup"><span data-stu-id="abb7c-143">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="abb7c-144">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="abb7c-144">**columnGroup**</span></span>         | <span data-ttu-id="abb7c-145">string</span><span class="sxs-lookup"><span data-stu-id="abb7c-145">string</span></span>  | <span data-ttu-id="abb7c-146">对于网站列，此列所属的组的名称。</span><span class="sxs-lookup"><span data-stu-id="abb7c-146">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="abb7c-147">可以帮助组织相关的列。</span><span class="sxs-lookup"><span data-stu-id="abb7c-147">Helps organize related columns.</span></span>
| <span data-ttu-id="abb7c-148">**说明**</span><span class="sxs-lookup"><span data-stu-id="abb7c-148">**description**</span></span>         | <span data-ttu-id="abb7c-149">string</span><span class="sxs-lookup"><span data-stu-id="abb7c-149">string</span></span>  | <span data-ttu-id="abb7c-150">面向用户的列描述。</span><span class="sxs-lookup"><span data-stu-id="abb7c-150">The user-facing description of the column.</span></span>
| <span data-ttu-id="abb7c-151">**displayName**</span><span class="sxs-lookup"><span data-stu-id="abb7c-151">**displayName**</span></span>         | <span data-ttu-id="abb7c-152">string</span><span class="sxs-lookup"><span data-stu-id="abb7c-152">string</span></span>  | <span data-ttu-id="abb7c-153">面向用户的列名称。</span><span class="sxs-lookup"><span data-stu-id="abb7c-153">The user-facing name of the column.</span></span>
| <span data-ttu-id="abb7c-154">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="abb7c-154">**enforceUniqueValues**</span></span> | <span data-ttu-id="abb7c-155">布尔</span><span class="sxs-lookup"><span data-stu-id="abb7c-155">Boolean</span></span> | <span data-ttu-id="abb7c-156">如果 `true` 为 ，则没有两个列表项对此列具有相同的值。</span><span class="sxs-lookup"><span data-stu-id="abb7c-156">If `true`, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="abb7c-157">**hidden**</span><span class="sxs-lookup"><span data-stu-id="abb7c-157">**hidden**</span></span>              | <span data-ttu-id="abb7c-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="abb7c-158">Boolean</span></span> | <span data-ttu-id="abb7c-159">指定列是否显示在用户界面中。</span><span class="sxs-lookup"><span data-stu-id="abb7c-159">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="abb7c-160">**id**</span><span class="sxs-lookup"><span data-stu-id="abb7c-160">**id**</span></span>                  | <span data-ttu-id="abb7c-161">string</span><span class="sxs-lookup"><span data-stu-id="abb7c-161">string</span></span>  | <span data-ttu-id="abb7c-162">列的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="abb7c-162">The unique identifier for the column.</span></span>
| <span data-ttu-id="abb7c-163">**indexed**</span><span class="sxs-lookup"><span data-stu-id="abb7c-163">**indexed**</span></span>             | <span data-ttu-id="abb7c-164">布尔</span><span class="sxs-lookup"><span data-stu-id="abb7c-164">Boolean</span></span> | <span data-ttu-id="abb7c-165">指定列值是否可用于排序和搜索。</span><span class="sxs-lookup"><span data-stu-id="abb7c-165">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="abb7c-166">**名称**</span><span class="sxs-lookup"><span data-stu-id="abb7c-166">**name**</span></span>                | <span data-ttu-id="abb7c-167">string</span><span class="sxs-lookup"><span data-stu-id="abb7c-167">string</span></span>  | <span data-ttu-id="abb7c-168">在 [listItem][] 上的 [fields][] 中显示的面向 API 的列名称。</span><span class="sxs-lookup"><span data-stu-id="abb7c-168">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="abb7c-169">对于面向用户的名称，请参阅 **displayName**。</span><span class="sxs-lookup"><span data-stu-id="abb7c-169">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="abb7c-170">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="abb7c-170">**readOnly**</span></span>            | <span data-ttu-id="abb7c-171">布尔</span><span class="sxs-lookup"><span data-stu-id="abb7c-171">Boolean</span></span>    | <span data-ttu-id="abb7c-172">指定是否可以修改列值。</span><span class="sxs-lookup"><span data-stu-id="abb7c-172">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="abb7c-173">**required**</span><span class="sxs-lookup"><span data-stu-id="abb7c-173">**required**</span></span>            | <span data-ttu-id="abb7c-174">布尔</span><span class="sxs-lookup"><span data-stu-id="abb7c-174">Boolean</span></span> | <span data-ttu-id="abb7c-175">指定列值是否可选。</span><span class="sxs-lookup"><span data-stu-id="abb7c-175">Specifies whether the column value isn't optional.</span></span>
| <span data-ttu-id="abb7c-176">**boolean**</span><span class="sxs-lookup"><span data-stu-id="abb7c-176">**boolean**</span></span>       | <span data-ttu-id="abb7c-177">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="abb7c-177">[booleanColumn][]</span></span>       | <span data-ttu-id="abb7c-178">此列存储布尔值。</span><span class="sxs-lookup"><span data-stu-id="abb7c-178">This column stores boolean values.</span></span>
| <span data-ttu-id="abb7c-179">**calculated**</span><span class="sxs-lookup"><span data-stu-id="abb7c-179">**calculated**</span></span>    | <span data-ttu-id="abb7c-180">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="abb7c-180">[calculatedColumn][]</span></span>    | <span data-ttu-id="abb7c-181">根据其他列计算此列的数据。</span><span class="sxs-lookup"><span data-stu-id="abb7c-181">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="abb7c-182">**choice**</span><span class="sxs-lookup"><span data-stu-id="abb7c-182">**choice**</span></span>        | <span data-ttu-id="abb7c-183">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="abb7c-183">[choiceColumn][]</span></span>        | <span data-ttu-id="abb7c-184">此列存储所选列表中的数据。</span><span class="sxs-lookup"><span data-stu-id="abb7c-184">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="abb7c-185">**currency**</span><span class="sxs-lookup"><span data-stu-id="abb7c-185">**currency**</span></span>      | <span data-ttu-id="abb7c-186">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="abb7c-186">[currencyColumn][]</span></span>      | <span data-ttu-id="abb7c-187">此列存储货币值。</span><span class="sxs-lookup"><span data-stu-id="abb7c-187">This column stores currency values.</span></span>
| <span data-ttu-id="abb7c-188">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="abb7c-188">**dateTime**</span></span>      | <span data-ttu-id="abb7c-189">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="abb7c-189">[dateTimeColumn][]</span></span>      | <span data-ttu-id="abb7c-190">此列存储日期时间值。</span><span class="sxs-lookup"><span data-stu-id="abb7c-190">This column stores DateTime values.</span></span>
| <span data-ttu-id="abb7c-191">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="abb7c-191">**defaultValue**</span></span>  | <span data-ttu-id="abb7c-192">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="abb7c-192">[defaultColumnValue][]</span></span>  | <span data-ttu-id="abb7c-193">此列的默认值。</span><span class="sxs-lookup"><span data-stu-id="abb7c-193">The default value for this column.</span></span>
| <span data-ttu-id="abb7c-194">**地理位置**</span><span class="sxs-lookup"><span data-stu-id="abb7c-194">**geolocation**</span></span>   | <span data-ttu-id="abb7c-195">[geolocationColumn][]</span><span class="sxs-lookup"><span data-stu-id="abb7c-195">[geolocationColumn][]</span></span>   | <span data-ttu-id="abb7c-196">此列存储地理位置。</span><span class="sxs-lookup"><span data-stu-id="abb7c-196">This column stores a geolocation.</span></span>
| <span data-ttu-id="abb7c-197">**lookup**</span><span class="sxs-lookup"><span data-stu-id="abb7c-197">**lookup**</span></span>        | <span data-ttu-id="abb7c-198">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="abb7c-198">[lookupColumn][]</span></span>        | <span data-ttu-id="abb7c-199">从网站中的另一个源查找此列的数据。</span><span class="sxs-lookup"><span data-stu-id="abb7c-199">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="abb7c-200">**number**</span><span class="sxs-lookup"><span data-stu-id="abb7c-200">**number**</span></span>        | <span data-ttu-id="abb7c-201">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="abb7c-201">[numberColumn][]</span></span>        | <span data-ttu-id="abb7c-202">此列存储数值。</span><span class="sxs-lookup"><span data-stu-id="abb7c-202">This column stores number values.</span></span>
| <span data-ttu-id="abb7c-203">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="abb7c-203">**personOrGroup**</span></span> | <span data-ttu-id="abb7c-204">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="abb7c-204">[personOrGroupColumn][]</span></span> | <span data-ttu-id="abb7c-205">此列存储个人或组值。</span><span class="sxs-lookup"><span data-stu-id="abb7c-205">This column stores Person or Group values.</span></span>
| <span data-ttu-id="abb7c-206">**text**</span><span class="sxs-lookup"><span data-stu-id="abb7c-206">**text**</span></span>          | <span data-ttu-id="abb7c-207">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="abb7c-207">[textColumn][]</span></span>          | <span data-ttu-id="abb7c-208">此列存储文本值。</span><span class="sxs-lookup"><span data-stu-id="abb7c-208">This column stores text values.</span></span>
| <span data-ttu-id="abb7c-209">**isDeletable**</span><span class="sxs-lookup"><span data-stu-id="abb7c-209">**isDeletable**</span></span>       | <span data-ttu-id="abb7c-210">布尔</span><span class="sxs-lookup"><span data-stu-id="abb7c-210">Boolean</span></span> | <span data-ttu-id="abb7c-211">指示是否可以删除此列。</span><span class="sxs-lookup"><span data-stu-id="abb7c-211">Indicates whether this column can be deleted.</span></span>
| <span data-ttu-id="abb7c-212">**propagateChanges**</span><span class="sxs-lookup"><span data-stu-id="abb7c-212">**propagateChanges**</span></span>     | <span data-ttu-id="abb7c-213">布尔</span><span class="sxs-lookup"><span data-stu-id="abb7c-213">Boolean</span></span> | <span data-ttu-id="abb7c-214">如果 `true` 为 ，则对此列所做的更改将传播到实现该列的列表。</span><span class="sxs-lookup"><span data-stu-id="abb7c-214">If `true`, changes to this column will be propagated to lists that implement the column.</span></span> 
| <span data-ttu-id="abb7c-215">**isReorderable**</span><span class="sxs-lookup"><span data-stu-id="abb7c-215">**isReorderable**</span></span>         | <span data-ttu-id="abb7c-216">布尔</span><span class="sxs-lookup"><span data-stu-id="abb7c-216">Boolean</span></span> | <span data-ttu-id="abb7c-217">指示是否可以对列中的值进行重新排序。</span><span class="sxs-lookup"><span data-stu-id="abb7c-217">Indicates whether values in the column can be reordered.</span></span> <span data-ttu-id="abb7c-218">只读。</span><span class="sxs-lookup"><span data-stu-id="abb7c-218">Read-only.</span></span>
| <span data-ttu-id="abb7c-219">**isSealed**</span><span class="sxs-lookup"><span data-stu-id="abb7c-219">**isSealed**</span></span>              | <span data-ttu-id="abb7c-220">布尔</span><span class="sxs-lookup"><span data-stu-id="abb7c-220">Boolean</span></span> | <span data-ttu-id="abb7c-221">指定是否可以更改列。</span><span class="sxs-lookup"><span data-stu-id="abb7c-221">Specifies whether the column can be changed.</span></span>
| <span data-ttu-id="abb7c-222">**validation**</span><span class="sxs-lookup"><span data-stu-id="abb7c-222">**validation**</span></span>   |  <span data-ttu-id="abb7c-223">[columnValidation][]</span><span class="sxs-lookup"><span data-stu-id="abb7c-223">[columnValidation][]</span></span>    | <span data-ttu-id="abb7c-224">此列存储该列的验证公式和消息。</span><span class="sxs-lookup"><span data-stu-id="abb7c-224">This column stores validation formula and message for the column.</span></span> 
| <span data-ttu-id="abb7c-225">**hyperlinkOrPicture**</span><span class="sxs-lookup"><span data-stu-id="abb7c-225">**hyperlinkOrPicture**</span></span>  | <span data-ttu-id="abb7c-226">[hyperlinkOrPictureColumn][]</span><span class="sxs-lookup"><span data-stu-id="abb7c-226">[hyperlinkOrPictureColumn][]</span></span> | <span data-ttu-id="abb7c-227">此列存储超链接或图片值。</span><span class="sxs-lookup"><span data-stu-id="abb7c-227">This column stores hyperlink or picture values.</span></span> 
| <span data-ttu-id="abb7c-228">**term**</span><span class="sxs-lookup"><span data-stu-id="abb7c-228">**term**</span></span>     | <span data-ttu-id="abb7c-229">[termColumn][]</span><span class="sxs-lookup"><span data-stu-id="abb7c-229">[termColumn][]</span></span> | <span data-ttu-id="abb7c-230">此列存储分类术语。</span><span class="sxs-lookup"><span data-stu-id="abb7c-230">This column stores taxonomy terms.</span></span>
| <span data-ttu-id="abb7c-231">**sourceContentType**</span><span class="sxs-lookup"><span data-stu-id="abb7c-231">**sourceContentType**</span></span>   |<span data-ttu-id="abb7c-232">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="abb7c-232">[contentTypeInfo][]</span></span>  | <span data-ttu-id="abb7c-233">从其继承此列的 ContentType。</span><span class="sxs-lookup"><span data-stu-id="abb7c-233">ContentType from which this column is inherited from.</span></span> <span data-ttu-id="abb7c-234">仅用于提取 contentTypes 列。</span><span class="sxs-lookup"><span data-stu-id="abb7c-234">Used only to fetch contentTypes columns.</span></span>
| <span data-ttu-id="abb7c-235">**thumbnail**</span><span class="sxs-lookup"><span data-stu-id="abb7c-235">**thumbnail**</span></span>           |<span data-ttu-id="abb7c-236">[thumbnailColumn][]</span><span class="sxs-lookup"><span data-stu-id="abb7c-236">[thumbnailColumn][]</span></span>      | <span data-ttu-id="abb7c-237">此列存储缩略图值。</span><span class="sxs-lookup"><span data-stu-id="abb7c-237">This column stores thumbnail values.</span></span>
| <span data-ttu-id="abb7c-238">**type**</span><span class="sxs-lookup"><span data-stu-id="abb7c-238">**type**</span></span>         | <span data-ttu-id="abb7c-239">columnTypes</span><span class="sxs-lookup"><span data-stu-id="abb7c-239">columnTypes</span></span>  | <span data-ttu-id="abb7c-240">对于网站栏，列的类型。</span><span class="sxs-lookup"><span data-stu-id="abb7c-240">For site columns, the type of column.</span></span> <span data-ttu-id="abb7c-241">只读。</span><span class="sxs-lookup"><span data-stu-id="abb7c-241">Read-only.</span></span>
| <span data-ttu-id="abb7c-242">**contentApprovalStatus**</span><span class="sxs-lookup"><span data-stu-id="abb7c-242">**contentApprovalStatus**</span></span>| <span data-ttu-id="abb7c-243">[contentApprovalStatusColumn][]</span><span class="sxs-lookup"><span data-stu-id="abb7c-243">[contentApprovalStatusColumn][]</span></span>     | <span data-ttu-id="abb7c-244">此列存储内容审批状态。</span><span class="sxs-lookup"><span data-stu-id="abb7c-244">This column stores content approval status.</span></span>

## <a name="relationships"></a><span data-ttu-id="abb7c-245">关系</span><span class="sxs-lookup"><span data-stu-id="abb7c-245">Relationships</span></span>

| <span data-ttu-id="abb7c-246">属性名称</span><span class="sxs-lookup"><span data-stu-id="abb7c-246">Property name</span></span>   | <span data-ttu-id="abb7c-247">类型</span><span class="sxs-lookup"><span data-stu-id="abb7c-247">Type</span></span>                      | <span data-ttu-id="abb7c-248">说明</span><span class="sxs-lookup"><span data-stu-id="abb7c-248">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="abb7c-249">**sourceColumn**</span><span class="sxs-lookup"><span data-stu-id="abb7c-249">**sourceColumn**</span></span> | <span data-ttu-id="abb7c-250">[columnDefinition][]</span><span class="sxs-lookup"><span data-stu-id="abb7c-250">[columnDefinition][]</span></span> | <span data-ttu-id="abb7c-251">内容类型列的源列。</span><span class="sxs-lookup"><span data-stu-id="abb7c-251">The source column for content type column.</span></span>

><span data-ttu-id="abb7c-252">**注意：** 这些属性对应于 [SPFieldType SharePoint。][]</span><span class="sxs-lookup"><span data-stu-id="abb7c-252">**Note:** These properties correspond to the SharePoint [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="abb7c-253">请注意，最常见的字段类型在上表中表示。</span><span class="sxs-lookup"><span data-stu-id="abb7c-253">Note that the most common field types are represented in the previous table.</span></span> <span data-ttu-id="abb7c-254">但是，此 beta API 仍缺少一些。</span><span class="sxs-lookup"><span data-stu-id="abb7c-254">However, this beta API is still missing some.</span></span>
<span data-ttu-id="abb7c-255">在这些情况下，不会填充列类型 facet，列将仅具有其基本属性。</span><span class="sxs-lookup"><span data-stu-id="abb7c-255">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="json-representation"></a><span data-ttu-id="abb7c-256">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="abb7c-256">JSON representation</span></span>

<span data-ttu-id="abb7c-257">下面是 columnDefinition 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="abb7c-257">Here is a JSON representation of a columnDefinition resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.columnDefinition"
}-->

```json
{
  "columnGroup": "string",
  "description": "description",
  "displayName": "friendly name",
  "enforceUniqueValues": true,
  "hidden": false,
  "id": "string",
  "indexed": true,
  "name": "staticNameForApi",
  "readOnly": false,
  "required": false,
  "boolean": { "@odata.type": "microsoft.graph.booleanColumn" },
  "calculated": { "@odata.type": "microsoft.graph.calculatedColumn" },
  "choice": { "@odata.type": "microsoft.graph.choiceColumn" },
  "currency": { "@odata.type": "microsoft.graph.currencyColumn" },
  "dateTime": { "@odata.type": "microsoft.graph.dateTimeColumn" },
  "defaultValue": { "@odata.type": "microsoft.graph.defaultColumnValue" },
  "geolocation": { "@odata.type": "microsoft.graph.geolocationColumn" },
  "lookup": { "@odata.type": "microsoft.graph.lookupColumn" },
  "number": { "@odata.type": "microsoft.graph.numberColumn" },
  "personOrGroup": { "@odata.type": "microsoft.graph.personOrGroupColumn" },
  "text": { "@odata.type": "microsoft.graph.textColumn" },
  "isDeletable" : false,
  "propagateChanges": false,
  "isReorderable": false,
  "isSealed": false,
  "validation": { "@odata.type": "microsoft.graph.columnValidation" },
  "hyperlinkOrPicture": { "@odata.type": "microsoft.graph.hyperlinkOrPictureColumn" },
  "term": { "@odata.type": "microsoft.graph.termColumn" },
  "sourceContentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },
  "thumbnail": { "@odata.type": "microsoft.graph.thumbnailColumn" },
  "type": { "@odata.type": "microsoft.graph.columnTypes" },
  "contentApprovalStatus": { "@odata.type": "microsoft.graph.contentApprovalStatusColumn" }
}
```

## <a name="remarks"></a><span data-ttu-id="abb7c-258">备注</span><span class="sxs-lookup"><span data-stu-id="abb7c-258">Remarks</span></span>

<span data-ttu-id="abb7c-259">默认情况下，不显示 `hidden` 列的 ColumnDefinitions 和字段值。</span><span class="sxs-lookup"><span data-stu-id="abb7c-259">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="abb7c-260">若要在列出 **columnDefinitions** 时看到这些内容，请在 `$select` 语句中添加 `hidden`。</span><span class="sxs-lookup"><span data-stu-id="abb7c-260">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="abb7c-261">若要在 [listItems][listItem] 上显示 **字段** 值时看到这些内容，请在 `$select` 语句中添加名称所需的列。</span><span class="sxs-lookup"><span data-stu-id="abb7c-261">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

[booleanColumn]: booleancolumn.md
[calculatedColumn]: calculatedcolumn.md
[choiceColumn]: choicecolumn.md
[columnDefinition]: columnDefinition.md
[contentType]: contenttype.md
[currencyColumn]: currencycolumn.md
[dateTimeColumn]: datetimecolumn.md
[defaultColumnValue]: defaultcolumnvalue.md
[geolocationColumn]: geolocationcolumn.md
[列表]: list.md
[list]: list.md
[lookupColumn]: lookupcolumn.md
[numberColumn]: numbercolumn.md
[personOrGroupColumn]: personorgroupcolumn.md
[网站]: site.md
[site]: site.md
[textColumn]: textcolumn.md
[fieldValueSet]: fieldvalueset.md
[fields]: fieldvalueset.md
[listItem]: listitem.md
[termColumn]: termColumn.md
[contentApprovalStatusColumn]: contentApprovalStatusColumn.md
[thumbnailColumn]: thumbnailColumn.md
[hyperlinkOrPictureColumn]: hyperlinkOrPictureColumn.md
[columnValidation]: columnValidation.md
[contentTypeInfo]: contentTypeInfo.md

<span data-ttu-id="abb7c-285">
  [SPFieldType]: /previous-versions/office/sharepoint-server/ms428806(v=office.15)</span><span class="sxs-lookup"><span data-stu-id="abb7c-285">[SPFieldType]: /previous-versions/office/sharepoint-server/ms428806(v=office.15)</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition",
  "suppressions": []
}
-->
