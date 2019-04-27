---
title: workbookFilter 资源类型
description: 管理表格列的筛选。
localization_priority: Normal
ms.openlocfilehash: 79ded0bfca0ace3b2d7c1bcdb4cd8dd2696802a4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348618"
---
# <a name="workbookfilter-resource-type"></a><span data-ttu-id="d66e0-103">workbookFilter 资源类型</span><span class="sxs-lookup"><span data-stu-id="d66e0-103">workbookFilter resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d66e0-104">管理表格列的筛选。</span><span class="sxs-lookup"><span data-stu-id="d66e0-104">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="d66e0-105">方法</span><span class="sxs-lookup"><span data-stu-id="d66e0-105">Methods</span></span>

| <span data-ttu-id="d66e0-106">方法</span><span class="sxs-lookup"><span data-stu-id="d66e0-106">Method</span></span>           | <span data-ttu-id="d66e0-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="d66e0-107">Return Type</span></span>    |<span data-ttu-id="d66e0-108">说明</span><span class="sxs-lookup"><span data-stu-id="d66e0-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d66e0-109">应用</span><span class="sxs-lookup"><span data-stu-id="d66e0-109">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="d66e0-110">无</span><span class="sxs-lookup"><span data-stu-id="d66e0-110">None</span></span>|<span data-ttu-id="d66e0-111">在给定列中应用给定的筛选条件。</span><span class="sxs-lookup"><span data-stu-id="d66e0-111">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="d66e0-112">清除</span><span class="sxs-lookup"><span data-stu-id="d66e0-112">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="d66e0-113">None</span><span class="sxs-lookup"><span data-stu-id="d66e0-113">None</span></span>|<span data-ttu-id="d66e0-114">清除给定列上的筛选器。</span><span class="sxs-lookup"><span data-stu-id="d66e0-114">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="d66e0-115">属性</span><span class="sxs-lookup"><span data-stu-id="d66e0-115">Properties</span></span>
<span data-ttu-id="d66e0-116">无</span><span class="sxs-lookup"><span data-stu-id="d66e0-116">None</span></span>

## <a name="relationships"></a><span data-ttu-id="d66e0-117">关系</span><span class="sxs-lookup"><span data-stu-id="d66e0-117">Relationships</span></span>
| <span data-ttu-id="d66e0-118">关系</span><span class="sxs-lookup"><span data-stu-id="d66e0-118">Relationship</span></span> | <span data-ttu-id="d66e0-119">类型</span><span class="sxs-lookup"><span data-stu-id="d66e0-119">Type</span></span>   |<span data-ttu-id="d66e0-120">说明</span><span class="sxs-lookup"><span data-stu-id="d66e0-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d66e0-121">条件</span><span class="sxs-lookup"><span data-stu-id="d66e0-121">criteria</span></span>|[<span data-ttu-id="d66e0-122">workbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="d66e0-122">workbookFilterCriteria</span></span>](workbookfiltercriteria.md)|<span data-ttu-id="d66e0-123">给定列上当前应用的筛选器。</span><span class="sxs-lookup"><span data-stu-id="d66e0-123">The currently applied filter on the given column.</span></span> <span data-ttu-id="d66e0-124">只读。</span><span class="sxs-lookup"><span data-stu-id="d66e0-124">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="d66e0-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d66e0-125">JSON representation</span></span>

<span data-ttu-id="d66e0-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d66e0-126">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
     "legacyId"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookFilter"
}-->

```json
{
    "criteria": {"@odata.type": "microsoft.graph.workbookFilterCriteria"}
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
