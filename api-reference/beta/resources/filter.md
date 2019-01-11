---
title: 筛选器资源类型
description: 管理表格列的筛选。
localization_priority: Normal
ms.openlocfilehash: 5bbc4eff85f40e116ea513c27fa2966dd28a5493
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852785"
---
# <a name="filter-resource-type"></a><span data-ttu-id="b6e18-103">筛选器资源类型</span><span class="sxs-lookup"><span data-stu-id="b6e18-103">Filter resource type</span></span>

> <span data-ttu-id="b6e18-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b6e18-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b6e18-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b6e18-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b6e18-106">管理表格列的筛选。</span><span class="sxs-lookup"><span data-stu-id="b6e18-106">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="b6e18-107">方法</span><span class="sxs-lookup"><span data-stu-id="b6e18-107">Methods</span></span>

| <span data-ttu-id="b6e18-108">方法</span><span class="sxs-lookup"><span data-stu-id="b6e18-108">Method</span></span>           | <span data-ttu-id="b6e18-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="b6e18-109">Return Type</span></span>    |<span data-ttu-id="b6e18-110">说明</span><span class="sxs-lookup"><span data-stu-id="b6e18-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b6e18-111">应用</span><span class="sxs-lookup"><span data-stu-id="b6e18-111">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="b6e18-112">无</span><span class="sxs-lookup"><span data-stu-id="b6e18-112">None</span></span>|<span data-ttu-id="b6e18-113">在给定列中应用给定的筛选条件。</span><span class="sxs-lookup"><span data-stu-id="b6e18-113">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="b6e18-114">Clear</span><span class="sxs-lookup"><span data-stu-id="b6e18-114">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="b6e18-115">无</span><span class="sxs-lookup"><span data-stu-id="b6e18-115">None</span></span>|<span data-ttu-id="b6e18-116">清除给定列上的筛选器。</span><span class="sxs-lookup"><span data-stu-id="b6e18-116">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="b6e18-117">属性</span><span class="sxs-lookup"><span data-stu-id="b6e18-117">Properties</span></span>
<span data-ttu-id="b6e18-118">无</span><span class="sxs-lookup"><span data-stu-id="b6e18-118">None</span></span>

## <a name="relationships"></a><span data-ttu-id="b6e18-119">Relationships</span><span class="sxs-lookup"><span data-stu-id="b6e18-119">Relationships</span></span>
| <span data-ttu-id="b6e18-120">关系</span><span class="sxs-lookup"><span data-stu-id="b6e18-120">Relationship</span></span> | <span data-ttu-id="b6e18-121">类型</span><span class="sxs-lookup"><span data-stu-id="b6e18-121">Type</span></span>   |<span data-ttu-id="b6e18-122">说明</span><span class="sxs-lookup"><span data-stu-id="b6e18-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b6e18-123">条件</span><span class="sxs-lookup"><span data-stu-id="b6e18-123">criteria</span></span>|[<span data-ttu-id="b6e18-124">FilterCriteria</span><span class="sxs-lookup"><span data-stu-id="b6e18-124">FilterCriteria</span></span>](filtercriteria.md)|<span data-ttu-id="b6e18-p102">给定列上当前应用的筛选器。只读。</span><span class="sxs-lookup"><span data-stu-id="b6e18-p102">The currently applied filter on the given column. Read-only.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
