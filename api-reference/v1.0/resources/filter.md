---
title: 筛选器资源类型
description: 管理表格列的筛选。
localization_priority: Normal
ms.openlocfilehash: cc4b1b105c2049b36fa27cb88b41102366648fa8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564314"
---
# <a name="filter-resource-type"></a><span data-ttu-id="f1374-103">筛选器资源类型</span><span class="sxs-lookup"><span data-stu-id="f1374-103">Filter resource type</span></span>

<span data-ttu-id="f1374-104">管理表格列的筛选。</span><span class="sxs-lookup"><span data-stu-id="f1374-104">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="f1374-105">方法</span><span class="sxs-lookup"><span data-stu-id="f1374-105">Methods</span></span>

| <span data-ttu-id="f1374-106">方法</span><span class="sxs-lookup"><span data-stu-id="f1374-106">Method</span></span>           | <span data-ttu-id="f1374-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="f1374-107">Return Type</span></span>    |<span data-ttu-id="f1374-108">说明</span><span class="sxs-lookup"><span data-stu-id="f1374-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f1374-109">应用</span><span class="sxs-lookup"><span data-stu-id="f1374-109">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="f1374-110">无</span><span class="sxs-lookup"><span data-stu-id="f1374-110">None</span></span>|<span data-ttu-id="f1374-111">在给定列中应用给定的筛选条件。</span><span class="sxs-lookup"><span data-stu-id="f1374-111">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="f1374-112">清除</span><span class="sxs-lookup"><span data-stu-id="f1374-112">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="f1374-113">无</span><span class="sxs-lookup"><span data-stu-id="f1374-113">None</span></span>|<span data-ttu-id="f1374-114">清除给定列上的筛选器。</span><span class="sxs-lookup"><span data-stu-id="f1374-114">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="f1374-115">属性</span><span class="sxs-lookup"><span data-stu-id="f1374-115">Properties</span></span>

| <span data-ttu-id="f1374-116">名称</span><span class="sxs-lookup"><span data-stu-id="f1374-116">Name</span></span> | <span data-ttu-id="f1374-117">类型</span><span class="sxs-lookup"><span data-stu-id="f1374-117">Type</span></span>   |<span data-ttu-id="f1374-118">说明</span><span class="sxs-lookup"><span data-stu-id="f1374-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1374-119">条件</span><span class="sxs-lookup"><span data-stu-id="f1374-119">criteria</span></span>|[<span data-ttu-id="f1374-120">WorkbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="f1374-120">WorkbookFilterCriteria</span></span>](filtercriteria.md)|<span data-ttu-id="f1374-121">给定列上当前应用的筛选器。</span><span class="sxs-lookup"><span data-stu-id="f1374-121">The currently applied filter on the given column.</span></span> <span data-ttu-id="f1374-122">只读。</span><span class="sxs-lookup"><span data-stu-id="f1374-122">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f1374-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f1374-123">JSON representation</span></span>

<span data-ttu-id="f1374-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1374-124">Here is a JSON representation of the resource.</span></span>

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
