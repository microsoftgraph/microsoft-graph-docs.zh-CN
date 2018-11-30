---
title: plannerAppliedCategories 资源类型
description: '**AppliedCategoriesCollection**资源代表已应用于任务类别 （或标签） 的集合。 它是 plannerTask 对象的一部分。'
ms.openlocfilehash: 0bb7987c3da62f2302b08ab43fa00d09763e0c1d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047819"
---
# <a name="plannerappliedcategories-resource-type"></a><span data-ttu-id="f5b5a-104">plannerAppliedCategories 资源类型</span><span class="sxs-lookup"><span data-stu-id="f5b5a-104">plannerAppliedCategories resource type</span></span>

> <span data-ttu-id="f5b5a-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f5b5a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5b5a-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f5b5a-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f5b5a-p103">**AppliedCategoriesCollection** 资源表示已应用于任务的类别（或标签）的集合。她是 [plannerTask](plannertask.md) 对象的组成部分。最多可向一个任务应用 6 个类别。类别说明，例如 `category1`、`category2` 等，是[计划详细信息](plannerplandetails.md)对象的组成部分。它是开放类型。</span><span class="sxs-lookup"><span data-stu-id="f5b5a-p103">The **AppliedCategoriesCollection** resource represents the collection of categories (or labels) that have been applied to a task. It is part of the [plannerTask](plannertask.md) object. There can be up to 6 categories applied to a task. Category descriptions, e.g. `category1`, `category2` etc., are part of the [plan details](plannerplandetails.md) object. This is an open type.</span></span>

## <a name="properties"></a><span data-ttu-id="f5b5a-112">属性</span><span class="sxs-lookup"><span data-stu-id="f5b5a-112">Properties</span></span>
<span data-ttu-id="f5b5a-p104">开放类型的属性可以由客户端定义。但是在这种情况下，在任务上应用相应的类别时客户端必须将 `category1`、`category2`、`category3`、`category4`、`category5` 和/或 `category6` 作为属性，且其值要为 `true` 布尔值。下面是一个示例。不应用这些类别时，则将属性值设置为 `false` 布尔值来自动删除属性。</span><span class="sxs-lookup"><span data-stu-id="f5b5a-p104">Properties of an Open Type can be defined by the client. In this case though, the client must provide `category1`, `category2`, `category3`, `category4`, `category5` and/or `category6` as properties with their values being the `true` boolean when the corresponding categories are applied on the task. Example is shown below. When they do not apply, properties are automatically removed by setting their values to the `false` boolean.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="f5b5a-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f5b5a-117">JSON representation</span></span>

<span data-ttu-id="f5b5a-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f5b5a-118">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAppliedCategories"
}-->

```json
{
  "String-value": true
}
```

<span data-ttu-id="f5b5a-119">示例：</span><span class="sxs-lookup"><span data-stu-id="f5b5a-119">Example:</span></span> 

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