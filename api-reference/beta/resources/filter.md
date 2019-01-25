---
title: 筛选器资源类型
description: 管理表格列的筛选。
localization_priority: Normal
ms.openlocfilehash: 6adc4e378b47bcb134a640e77bf54c32a35b3be2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518889"
---
# <a name="filter-resource-type"></a><span data-ttu-id="7a54a-103">筛选器资源类型</span><span class="sxs-lookup"><span data-stu-id="7a54a-103">Filter resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a54a-104">管理表格列的筛选。</span><span class="sxs-lookup"><span data-stu-id="7a54a-104">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="7a54a-105">方法</span><span class="sxs-lookup"><span data-stu-id="7a54a-105">Methods</span></span>

| <span data-ttu-id="7a54a-106">方法</span><span class="sxs-lookup"><span data-stu-id="7a54a-106">Method</span></span>           | <span data-ttu-id="7a54a-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="7a54a-107">Return Type</span></span>    |<span data-ttu-id="7a54a-108">说明</span><span class="sxs-lookup"><span data-stu-id="7a54a-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7a54a-109">应用</span><span class="sxs-lookup"><span data-stu-id="7a54a-109">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="7a54a-110">无</span><span class="sxs-lookup"><span data-stu-id="7a54a-110">None</span></span>|<span data-ttu-id="7a54a-111">在给定列中应用给定的筛选条件。</span><span class="sxs-lookup"><span data-stu-id="7a54a-111">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="7a54a-112">清除</span><span class="sxs-lookup"><span data-stu-id="7a54a-112">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="7a54a-113">无</span><span class="sxs-lookup"><span data-stu-id="7a54a-113">None</span></span>|<span data-ttu-id="7a54a-114">清除给定列上的筛选器。</span><span class="sxs-lookup"><span data-stu-id="7a54a-114">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="7a54a-115">属性</span><span class="sxs-lookup"><span data-stu-id="7a54a-115">Properties</span></span>
<span data-ttu-id="7a54a-116">无</span><span class="sxs-lookup"><span data-stu-id="7a54a-116">None</span></span>

## <a name="relationships"></a><span data-ttu-id="7a54a-117">关系</span><span class="sxs-lookup"><span data-stu-id="7a54a-117">Relationships</span></span>
| <span data-ttu-id="7a54a-118">关系</span><span class="sxs-lookup"><span data-stu-id="7a54a-118">Relationship</span></span> | <span data-ttu-id="7a54a-119">类型</span><span class="sxs-lookup"><span data-stu-id="7a54a-119">Type</span></span>   |<span data-ttu-id="7a54a-120">说明</span><span class="sxs-lookup"><span data-stu-id="7a54a-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a54a-121">条件</span><span class="sxs-lookup"><span data-stu-id="7a54a-121">criteria</span></span>|[<span data-ttu-id="7a54a-122">FilterCriteria</span><span class="sxs-lookup"><span data-stu-id="7a54a-122">FilterCriteria</span></span>](filtercriteria.md)|<span data-ttu-id="7a54a-p101">给定列上当前应用的筛选器。只读。</span><span class="sxs-lookup"><span data-stu-id="7a54a-p101">The currently applied filter on the given column. Read-only.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/filter.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
