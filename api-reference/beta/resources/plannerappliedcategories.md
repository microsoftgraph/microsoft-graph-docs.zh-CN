---
title: plannerAppliedCategories 资源类型
description: '**AppliedCategoriesCollection**资源表示已应用于任务的类别 (或标签) 的集合。 它是 plannerTask 对象的一部分。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: a927adb78bc0fe1c5135281043ecbdd3afe09a60
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344609"
---
# <a name="plannerappliedcategories-resource-type"></a><span data-ttu-id="f07ff-104">plannerAppliedCategories 资源类型</span><span class="sxs-lookup"><span data-stu-id="f07ff-104">plannerAppliedCategories resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f07ff-105">**AppliedCategoriesCollection**资源表示已应用于任务的类别 (或标签) 的集合。</span><span class="sxs-lookup"><span data-stu-id="f07ff-105">The **AppliedCategoriesCollection** resource represents the collection of categories (or labels) that have been applied to a task.</span></span> <span data-ttu-id="f07ff-106">它是[plannerTask](plannertask.md)对象的一部分。</span><span class="sxs-lookup"><span data-stu-id="f07ff-106">It is part of the [plannerTask](plannertask.md) object.</span></span>
<span data-ttu-id="f07ff-107">最多可以将6个类别应用于一个任务。</span><span class="sxs-lookup"><span data-stu-id="f07ff-107">There can be up to 6 categories applied to a task.</span></span> <span data-ttu-id="f07ff-108">类别说明 (如`category1` `category2`等) 是 "[计划详细信息](plannerplandetails.md)" 对象的一部分。</span><span class="sxs-lookup"><span data-stu-id="f07ff-108">Category descriptions, e.g. `category1`, `category2` etc., are part of the [plan details](plannerplandetails.md) object.</span></span> <span data-ttu-id="f07ff-109">这是开放类型。</span><span class="sxs-lookup"><span data-stu-id="f07ff-109">This is an open type.</span></span>

## <a name="properties"></a><span data-ttu-id="f07ff-110">属性</span><span class="sxs-lookup"><span data-stu-id="f07ff-110">Properties</span></span>
<span data-ttu-id="f07ff-111">可由客户端定义打开类型的属性。</span><span class="sxs-lookup"><span data-stu-id="f07ff-111">Properties of an Open Type can be defined by the client.</span></span> <span data-ttu-id="f07ff-112">但在这种情况下, 客户端`category1`必须`category2`提供`category3`、 `category4`、 `category5` 、和/ `category6`或属性值作为属性, 当`true`对该任务应用相应的类别时, 这些属性的值为 boolean。</span><span class="sxs-lookup"><span data-stu-id="f07ff-112">In this case though, the client must provide `category1`, `category2`, `category3`, `category4`, `category5` and/or `category6` as properties with their values being the `true` boolean when the corresponding categories are applied on the task.</span></span> <span data-ttu-id="f07ff-113">示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="f07ff-113">Example is shown below.</span></span> <span data-ttu-id="f07ff-114">如果它们不适用, 则通过将属性值设置为`false`布尔值来自动删除属性。</span><span class="sxs-lookup"><span data-stu-id="f07ff-114">When they do not apply, properties are automatically removed by setting their values to the `false` boolean.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="f07ff-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f07ff-115">JSON representation</span></span>

<span data-ttu-id="f07ff-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f07ff-116">Here is a JSON representation of the resource</span></span>

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

<span data-ttu-id="f07ff-117">示例：</span><span class="sxs-lookup"><span data-stu-id="f07ff-117">Example:</span></span> 

```json
{
  "category1": true,
  "category3": true,
  "category5": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerAppliedCategories resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
