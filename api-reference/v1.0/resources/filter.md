---
title: 筛选器资源类型
description: 管理表格列的筛选。
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c85c8237f179fd6be2add02263c9d6d040a71849
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018303"
---
# <a name="filter-resource-type"></a><span data-ttu-id="db311-103">筛选器资源类型</span><span class="sxs-lookup"><span data-stu-id="db311-103">Filter resource type</span></span>

<span data-ttu-id="db311-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db311-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="db311-105">管理表格列的筛选。</span><span class="sxs-lookup"><span data-stu-id="db311-105">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="db311-106">方法</span><span class="sxs-lookup"><span data-stu-id="db311-106">Methods</span></span>

| <span data-ttu-id="db311-107">方法</span><span class="sxs-lookup"><span data-stu-id="db311-107">Method</span></span>           | <span data-ttu-id="db311-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="db311-108">Return Type</span></span>    |<span data-ttu-id="db311-109">说明</span><span class="sxs-lookup"><span data-stu-id="db311-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="db311-110">应用</span><span class="sxs-lookup"><span data-stu-id="db311-110">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="db311-111">无</span><span class="sxs-lookup"><span data-stu-id="db311-111">None</span></span>|<span data-ttu-id="db311-112">在给定列中应用给定的筛选条件。</span><span class="sxs-lookup"><span data-stu-id="db311-112">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="db311-113">清除</span><span class="sxs-lookup"><span data-stu-id="db311-113">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="db311-114">None</span><span class="sxs-lookup"><span data-stu-id="db311-114">None</span></span>|<span data-ttu-id="db311-115">清除给定列上的筛选器。</span><span class="sxs-lookup"><span data-stu-id="db311-115">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="db311-116">属性</span><span class="sxs-lookup"><span data-stu-id="db311-116">Properties</span></span>

| <span data-ttu-id="db311-117">名称</span><span class="sxs-lookup"><span data-stu-id="db311-117">Name</span></span> | <span data-ttu-id="db311-118">类型</span><span class="sxs-lookup"><span data-stu-id="db311-118">Type</span></span>   |<span data-ttu-id="db311-119">说明</span><span class="sxs-lookup"><span data-stu-id="db311-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db311-120">条件</span><span class="sxs-lookup"><span data-stu-id="db311-120">criteria</span></span>|[<span data-ttu-id="db311-121">WorkbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="db311-121">WorkbookFilterCriteria</span></span>](filtercriteria.md)|<span data-ttu-id="db311-122">给定列上当前应用的筛选器。</span><span class="sxs-lookup"><span data-stu-id="db311-122">The currently applied filter on the given column.</span></span> <span data-ttu-id="db311-123">只读。</span><span class="sxs-lookup"><span data-stu-id="db311-123">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="db311-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="db311-124">JSON representation</span></span>

<span data-ttu-id="db311-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="db311-125">Here is a JSON representation of the resource.</span></span>

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

