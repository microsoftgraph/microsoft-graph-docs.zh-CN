---
title: 筛选器资源类型
description: 管理表格列的筛选。
ms.openlocfilehash: df896d10b1e8734015d38b92b5824e3e3652e3a6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046068"
---
# <a name="filter-resource-type"></a><span data-ttu-id="8eaf6-103">筛选器资源类型</span><span class="sxs-lookup"><span data-stu-id="8eaf6-103">Filter resource type</span></span>

> <span data-ttu-id="8eaf6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8eaf6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8eaf6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8eaf6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8eaf6-106">管理表格列的筛选。</span><span class="sxs-lookup"><span data-stu-id="8eaf6-106">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="8eaf6-107">方法</span><span class="sxs-lookup"><span data-stu-id="8eaf6-107">Methods</span></span>

| <span data-ttu-id="8eaf6-108">方法</span><span class="sxs-lookup"><span data-stu-id="8eaf6-108">Method</span></span>           | <span data-ttu-id="8eaf6-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="8eaf6-109">Return Type</span></span>    |<span data-ttu-id="8eaf6-110">说明</span><span class="sxs-lookup"><span data-stu-id="8eaf6-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8eaf6-111">应用</span><span class="sxs-lookup"><span data-stu-id="8eaf6-111">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="8eaf6-112">无</span><span class="sxs-lookup"><span data-stu-id="8eaf6-112">None</span></span>|<span data-ttu-id="8eaf6-113">在给定列中应用给定的筛选条件。</span><span class="sxs-lookup"><span data-stu-id="8eaf6-113">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="8eaf6-114">Clear</span><span class="sxs-lookup"><span data-stu-id="8eaf6-114">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="8eaf6-115">无</span><span class="sxs-lookup"><span data-stu-id="8eaf6-115">None</span></span>|<span data-ttu-id="8eaf6-116">清除给定列上的筛选器。</span><span class="sxs-lookup"><span data-stu-id="8eaf6-116">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="8eaf6-117">属性</span><span class="sxs-lookup"><span data-stu-id="8eaf6-117">Properties</span></span>
<span data-ttu-id="8eaf6-118">无</span><span class="sxs-lookup"><span data-stu-id="8eaf6-118">None</span></span>

## <a name="relationships"></a><span data-ttu-id="8eaf6-119">Relationships</span><span class="sxs-lookup"><span data-stu-id="8eaf6-119">Relationships</span></span>
| <span data-ttu-id="8eaf6-120">关系</span><span class="sxs-lookup"><span data-stu-id="8eaf6-120">Relationship</span></span> | <span data-ttu-id="8eaf6-121">类型</span><span class="sxs-lookup"><span data-stu-id="8eaf6-121">Type</span></span>   |<span data-ttu-id="8eaf6-122">说明</span><span class="sxs-lookup"><span data-stu-id="8eaf6-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8eaf6-123">条件</span><span class="sxs-lookup"><span data-stu-id="8eaf6-123">criteria</span></span>|[<span data-ttu-id="8eaf6-124">FilterCriteria</span><span class="sxs-lookup"><span data-stu-id="8eaf6-124">FilterCriteria</span></span>](filtercriteria.md)|<span data-ttu-id="8eaf6-p102">给定列上当前应用的筛选器。只读。</span><span class="sxs-lookup"><span data-stu-id="8eaf6-p102">The currently applied filter on the given column. Read-only.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->