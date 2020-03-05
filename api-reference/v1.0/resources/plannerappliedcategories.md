---
title: plannerAppliedCategories 资源类型
description: '**AppliedCategoriesCollection**资源表示已应用于任务的类别（或标签）的集合。 它是 plannerTask 对象的一部分。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 61b5b8d6f883ed3e7799acd312cb71c68dd07780
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447155"
---
# <a name="plannerappliedcategories-resource-type"></a><span data-ttu-id="d88d7-104">plannerAppliedCategories 资源类型</span><span class="sxs-lookup"><span data-stu-id="d88d7-104">plannerAppliedCategories resource type</span></span>

<span data-ttu-id="d88d7-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d88d7-105">Namespace: microsoft.graph</span></span>


<span data-ttu-id="d88d7-106">**AppliedCategoriesCollection**资源表示已应用于任务的类别（或标签）的集合。</span><span class="sxs-lookup"><span data-stu-id="d88d7-106">The **AppliedCategoriesCollection** resource represents the collection of categories (or labels) that have been applied to a task.</span></span> <span data-ttu-id="d88d7-107">它是[plannerTask](plannertask.md)对象的一部分。</span><span class="sxs-lookup"><span data-stu-id="d88d7-107">It is part of the [plannerTask](plannertask.md) object.</span></span>
<span data-ttu-id="d88d7-108">最多可以将6个类别应用于一个任务。</span><span class="sxs-lookup"><span data-stu-id="d88d7-108">There can be up to 6 categories applied to a task.</span></span> <span data-ttu-id="d88d7-109">类别说明（如`category1` `category2`等）是 "[计划详细信息](plannerplandetails.md)" 对象的一部分。</span><span class="sxs-lookup"><span data-stu-id="d88d7-109">Category descriptions, e.g. `category1`, `category2` etc., are part of the [plan details](plannerplandetails.md) object.</span></span> <span data-ttu-id="d88d7-110">这是开放类型。</span><span class="sxs-lookup"><span data-stu-id="d88d7-110">This is an open type.</span></span>

## <a name="properties"></a><span data-ttu-id="d88d7-111">属性</span><span class="sxs-lookup"><span data-stu-id="d88d7-111">Properties</span></span>
<span data-ttu-id="d88d7-112">可由客户端定义打开类型的属性。</span><span class="sxs-lookup"><span data-stu-id="d88d7-112">Properties of an Open Type can be defined by the client.</span></span> <span data-ttu-id="d88d7-113">但在这种情况下，客户端`category1`必须`category2`提供`category3`、 `category4`、 `category5` 、和/ `category6`或属性值作为属性，当`true`对该任务应用相应的类别时，这些属性的值为 boolean。</span><span class="sxs-lookup"><span data-stu-id="d88d7-113">In this case though, the client must provide `category1`, `category2`, `category3`, `category4`, `category5` and/or `category6` as properties with their values being the `true` boolean when the corresponding categories are applied on the task.</span></span> <span data-ttu-id="d88d7-114">示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="d88d7-114">Example is shown below.</span></span> <span data-ttu-id="d88d7-115">如果它们不适用，则通过将属性值设置为`false`布尔值来自动删除属性。</span><span class="sxs-lookup"><span data-stu-id="d88d7-115">When they do not apply, properties are automatically removed by setting their values to the `false` boolean.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="d88d7-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d88d7-116">JSON representation</span></span>

<span data-ttu-id="d88d7-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d88d7-117">Here is a JSON representation of the resource</span></span>

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

<span data-ttu-id="d88d7-118">示例：</span><span class="sxs-lookup"><span data-stu-id="d88d7-118">Example:</span></span> 

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
