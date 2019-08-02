---
title: SortField 资源类型
description: 表示排序操作中的条件。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 33c2d37f46d4fdfdaef4bc5b6d92557668bf9d70
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034053"
---
# <a name="sortfield-resource-type"></a><span data-ttu-id="e4f1d-103">SortField 资源类型</span><span class="sxs-lookup"><span data-stu-id="e4f1d-103">SortField resource type</span></span>

<span data-ttu-id="e4f1d-104">表示排序操作中的条件。</span><span class="sxs-lookup"><span data-stu-id="e4f1d-104">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="e4f1d-105">属性</span><span class="sxs-lookup"><span data-stu-id="e4f1d-105">Properties</span></span>
| <span data-ttu-id="e4f1d-106">属性</span><span class="sxs-lookup"><span data-stu-id="e4f1d-106">Property</span></span>     | <span data-ttu-id="e4f1d-107">类型</span><span class="sxs-lookup"><span data-stu-id="e4f1d-107">Type</span></span>   |<span data-ttu-id="e4f1d-108">说明</span><span class="sxs-lookup"><span data-stu-id="e4f1d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4f1d-109">ascending</span><span class="sxs-lookup"><span data-stu-id="e4f1d-109">ascending</span></span>|<span data-ttu-id="e4f1d-110">boolean</span><span class="sxs-lookup"><span data-stu-id="e4f1d-110">boolean</span></span>|<span data-ttu-id="e4f1d-111">表示是否以升序方式进行排序。</span><span class="sxs-lookup"><span data-stu-id="e4f1d-111">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="e4f1d-112">color</span><span class="sxs-lookup"><span data-stu-id="e4f1d-112">color</span></span>|<span data-ttu-id="e4f1d-113">字符串</span><span class="sxs-lookup"><span data-stu-id="e4f1d-113">string</span></span>|<span data-ttu-id="e4f1d-114">表示按字体或单元格颜色进行排序时，条件的目标颜色。</span><span class="sxs-lookup"><span data-stu-id="e4f1d-114">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="e4f1d-115">dataOption</span><span class="sxs-lookup"><span data-stu-id="e4f1d-115">dataOption</span></span>|<span data-ttu-id="e4f1d-116">string</span><span class="sxs-lookup"><span data-stu-id="e4f1d-116">string</span></span>|<span data-ttu-id="e4f1d-117">表示此字段的其他排序选项。</span><span class="sxs-lookup"><span data-stu-id="e4f1d-117">Represents additional sorting options for this field.</span></span> <span data-ttu-id="e4f1d-118">可能的值为: `Normal`、 `TextAsNumber`。</span><span class="sxs-lookup"><span data-stu-id="e4f1d-118">The possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="e4f1d-119">Key</span><span class="sxs-lookup"><span data-stu-id="e4f1d-119">key</span></span>|<span data-ttu-id="e4f1d-120">int</span><span class="sxs-lookup"><span data-stu-id="e4f1d-120">int</span></span>|<span data-ttu-id="e4f1d-p102">表示条件所在的列（或行，具体取决于排序方向）。表示与第一列（或行）的偏移量。</span><span class="sxs-lookup"><span data-stu-id="e4f1d-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="e4f1d-123">sortOn</span><span class="sxs-lookup"><span data-stu-id="e4f1d-123">sortOn</span></span>|<span data-ttu-id="e4f1d-124">string</span><span class="sxs-lookup"><span data-stu-id="e4f1d-124">string</span></span>|<span data-ttu-id="e4f1d-125">表示此条件的排序类型。</span><span class="sxs-lookup"><span data-stu-id="e4f1d-125">Represents the type of sorting of this condition.</span></span> <span data-ttu-id="e4f1d-126">可能的值包括 `Value`、`CellColor`、`FontColor`、`Icon`。</span><span class="sxs-lookup"><span data-stu-id="e4f1d-126">The possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|
|<span data-ttu-id="e4f1d-127">图标</span><span class="sxs-lookup"><span data-stu-id="e4f1d-127">icon</span></span>|[<span data-ttu-id="e4f1d-128">WorkbookIcon</span><span class="sxs-lookup"><span data-stu-id="e4f1d-128">WorkbookIcon</span></span>](icon.md)|<span data-ttu-id="e4f1d-129">表示对单元格图标进行排序时，条件的目标图标。</span><span class="sxs-lookup"><span data-stu-id="e4f1d-129">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e4f1d-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e4f1d-130">JSON representation</span></span>

<span data-ttu-id="e4f1d-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4f1d-131">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookSortField"
}-->

```json
{
  "ascending": true,
  "color": "string",
  "dataOption": "string",
  "key": 1024,
  "sortOn": "string",
  "icon": { "@odata.type": "microsoft.graph.workbookIcon" }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "SortField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
