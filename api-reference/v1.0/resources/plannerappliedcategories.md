---
title: plannerAppliedCategories 资源类型
description: '**AppliedCategoriesCollection**资源代表已应用于任务类别 （或标签） 的集合。 它是 plannerTask 对象的一部分。'
localization_priority: Normal
ms.openlocfilehash: 5601c3b0d49e7504c16a8ee517b60f3c98c84fee
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814777"
---
# <a name="plannerappliedcategories-resource-type"></a><span data-ttu-id="3e660-104">plannerAppliedCategories 资源类型</span><span class="sxs-lookup"><span data-stu-id="3e660-104">plannerAppliedCategories resource type</span></span>


<span data-ttu-id="3e660-p102">**AppliedCategoriesCollection** 资源表示已应用于任务的类别（或标签）的集合。她是 [plannerTask](plannertask.md) 对象的组成部分。最多可向一个任务应用 6 个类别。类别说明，例如 `category1`、`category2` 等，是[计划详细信息](plannerplandetails.md)对象的组成部分。它是开放类型。</span><span class="sxs-lookup"><span data-stu-id="3e660-p102">The **AppliedCategoriesCollection** resource represents the collection of categories (or labels) that have been applied to a task. It is part of the [plannerTask](plannertask.md) object. There can be up to 6 categories applied to a task. Category descriptions, e.g. `category1`, `category2` etc., are part of the [plan details](plannerplandetails.md) object. This is an open type.</span></span>

## <a name="properties"></a><span data-ttu-id="3e660-110">属性</span><span class="sxs-lookup"><span data-stu-id="3e660-110">Properties</span></span>
<span data-ttu-id="3e660-p103">开放类型的属性可以由客户端定义。但是在这种情况下，在任务上应用相应的类别时客户端必须将 `category1`、`category2`、`category3`、`category4`、`category5` 和/或 `category6` 作为属性，且其值要为 `true` 布尔值。下面是一个示例。不应用这些类别时，则将属性值设置为 `false` 布尔值来自动删除属性。</span><span class="sxs-lookup"><span data-stu-id="3e660-p103">Properties of an Open Type can be defined by the client. In this case though, the client must provide `category1`, `category2`, `category3`, `category4`, `category5` and/or `category6` as properties with their values being the `true` boolean when the corresponding categories are applied on the task. Example is shown below. When they do not apply, properties are automatically removed by setting their values to the `false` boolean.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="3e660-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3e660-115">JSON representation</span></span>

<span data-ttu-id="3e660-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e660-116">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "String-value" ],
  "@odata.type": "microsoft.graph.plannerAppliedCategories"
}-->

```json
{
  "String-value": true
}
```

<span data-ttu-id="3e660-117">示例：</span><span class="sxs-lookup"><span data-stu-id="3e660-117">Example:</span></span> 

```json
{
  "category1": true,
  "category3": true,
  "category5": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAppliedCategories resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
