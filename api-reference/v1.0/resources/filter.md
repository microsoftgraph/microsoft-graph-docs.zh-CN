---
title: 筛选器资源类型
description: 管理表格列的筛选。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3f58e1f5207fc3b4aebe2fdfb780735c0c5d209d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032478"
---
# <a name="filter-resource-type"></a><span data-ttu-id="b7c34-103">筛选器资源类型</span><span class="sxs-lookup"><span data-stu-id="b7c34-103">Filter resource type</span></span>

<span data-ttu-id="b7c34-104">管理表格列的筛选。</span><span class="sxs-lookup"><span data-stu-id="b7c34-104">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="b7c34-105">方法</span><span class="sxs-lookup"><span data-stu-id="b7c34-105">Methods</span></span>

| <span data-ttu-id="b7c34-106">方法</span><span class="sxs-lookup"><span data-stu-id="b7c34-106">Method</span></span>           | <span data-ttu-id="b7c34-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="b7c34-107">Return Type</span></span>    |<span data-ttu-id="b7c34-108">说明</span><span class="sxs-lookup"><span data-stu-id="b7c34-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b7c34-109">应用</span><span class="sxs-lookup"><span data-stu-id="b7c34-109">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="b7c34-110">无</span><span class="sxs-lookup"><span data-stu-id="b7c34-110">None</span></span>|<span data-ttu-id="b7c34-111">在给定列中应用给定的筛选条件。</span><span class="sxs-lookup"><span data-stu-id="b7c34-111">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="b7c34-112">清除</span><span class="sxs-lookup"><span data-stu-id="b7c34-112">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="b7c34-113">None</span><span class="sxs-lookup"><span data-stu-id="b7c34-113">None</span></span>|<span data-ttu-id="b7c34-114">清除给定列上的筛选器。</span><span class="sxs-lookup"><span data-stu-id="b7c34-114">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="b7c34-115">属性</span><span class="sxs-lookup"><span data-stu-id="b7c34-115">Properties</span></span>

| <span data-ttu-id="b7c34-116">名称</span><span class="sxs-lookup"><span data-stu-id="b7c34-116">Name</span></span> | <span data-ttu-id="b7c34-117">类型</span><span class="sxs-lookup"><span data-stu-id="b7c34-117">Type</span></span>   |<span data-ttu-id="b7c34-118">说明</span><span class="sxs-lookup"><span data-stu-id="b7c34-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7c34-119">条件</span><span class="sxs-lookup"><span data-stu-id="b7c34-119">criteria</span></span>|[<span data-ttu-id="b7c34-120">WorkbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="b7c34-120">WorkbookFilterCriteria</span></span>](filtercriteria.md)|<span data-ttu-id="b7c34-121">给定列上当前应用的筛选器。</span><span class="sxs-lookup"><span data-stu-id="b7c34-121">The currently applied filter on the given column.</span></span> <span data-ttu-id="b7c34-122">只读。</span><span class="sxs-lookup"><span data-stu-id="b7c34-122">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b7c34-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b7c34-123">JSON representation</span></span>

<span data-ttu-id="b7c34-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b7c34-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilter"
}-->

```json
{
  "criteria": {"@odata.type": "microsoft.graph.workbookFilterCriteria" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
