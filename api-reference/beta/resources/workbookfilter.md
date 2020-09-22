---
title: workbookFilter 资源类型
description: 管理表格列的筛选。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: ruoyingl
ms.openlocfilehash: a86c7bc0f9448ded2fbee40c4639cfb6d54f5f57
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079669"
---
# <a name="workbookfilter-resource-type"></a><span data-ttu-id="f6560-103">workbookFilter 资源类型</span><span class="sxs-lookup"><span data-stu-id="f6560-103">workbookFilter resource type</span></span>

<span data-ttu-id="f6560-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6560-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6560-105">管理表格列的筛选。</span><span class="sxs-lookup"><span data-stu-id="f6560-105">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="f6560-106">方法</span><span class="sxs-lookup"><span data-stu-id="f6560-106">Methods</span></span>

| <span data-ttu-id="f6560-107">方法</span><span class="sxs-lookup"><span data-stu-id="f6560-107">Method</span></span>           | <span data-ttu-id="f6560-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="f6560-108">Return Type</span></span>    |<span data-ttu-id="f6560-109">说明</span><span class="sxs-lookup"><span data-stu-id="f6560-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f6560-110">应用</span><span class="sxs-lookup"><span data-stu-id="f6560-110">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="f6560-111">无</span><span class="sxs-lookup"><span data-stu-id="f6560-111">None</span></span>|<span data-ttu-id="f6560-112">在给定列中应用给定的筛选条件。</span><span class="sxs-lookup"><span data-stu-id="f6560-112">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="f6560-113">清除</span><span class="sxs-lookup"><span data-stu-id="f6560-113">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="f6560-114">None</span><span class="sxs-lookup"><span data-stu-id="f6560-114">None</span></span>|<span data-ttu-id="f6560-115">清除给定列上的筛选器。</span><span class="sxs-lookup"><span data-stu-id="f6560-115">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="f6560-116">属性</span><span class="sxs-lookup"><span data-stu-id="f6560-116">Properties</span></span>
<span data-ttu-id="f6560-117">无</span><span class="sxs-lookup"><span data-stu-id="f6560-117">None</span></span>

## <a name="relationships"></a><span data-ttu-id="f6560-118">关系</span><span class="sxs-lookup"><span data-stu-id="f6560-118">Relationships</span></span>
| <span data-ttu-id="f6560-119">关系</span><span class="sxs-lookup"><span data-stu-id="f6560-119">Relationship</span></span> | <span data-ttu-id="f6560-120">类型</span><span class="sxs-lookup"><span data-stu-id="f6560-120">Type</span></span>   |<span data-ttu-id="f6560-121">说明</span><span class="sxs-lookup"><span data-stu-id="f6560-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f6560-122">条件</span><span class="sxs-lookup"><span data-stu-id="f6560-122">criteria</span></span>|[<span data-ttu-id="f6560-123">workbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="f6560-123">workbookFilterCriteria</span></span>](workbookfiltercriteria.md)|<span data-ttu-id="f6560-124">给定列上当前应用的筛选器。</span><span class="sxs-lookup"><span data-stu-id="f6560-124">The currently applied filter on the given column.</span></span> <span data-ttu-id="f6560-125">只读。</span><span class="sxs-lookup"><span data-stu-id="f6560-125">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="f6560-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f6560-126">JSON representation</span></span>

<span data-ttu-id="f6560-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f6560-127">Here is a JSON representation of the resource.</span></span>

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


