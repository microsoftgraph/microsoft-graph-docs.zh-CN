---
title: SortField 资源类型
description: 表示排序操作中的条件。
localization_priority: Normal
ms.openlocfilehash: 2c1b9a272fd024455d1297c5f59ca7684283e1a1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825968"
---
# <a name="sortfield-resource-type"></a><span data-ttu-id="c7bdc-103">SortField 资源类型</span><span class="sxs-lookup"><span data-stu-id="c7bdc-103">SortField resource type</span></span>

<span data-ttu-id="c7bdc-104">表示排序操作中的条件。</span><span class="sxs-lookup"><span data-stu-id="c7bdc-104">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="c7bdc-105">属性</span><span class="sxs-lookup"><span data-stu-id="c7bdc-105">Properties</span></span>
| <span data-ttu-id="c7bdc-106">属性</span><span class="sxs-lookup"><span data-stu-id="c7bdc-106">Property</span></span>     | <span data-ttu-id="c7bdc-107">类型</span><span class="sxs-lookup"><span data-stu-id="c7bdc-107">Type</span></span>   |<span data-ttu-id="c7bdc-108">说明</span><span class="sxs-lookup"><span data-stu-id="c7bdc-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c7bdc-109">ascending</span><span class="sxs-lookup"><span data-stu-id="c7bdc-109">ascending</span></span>|<span data-ttu-id="c7bdc-110">boolean</span><span class="sxs-lookup"><span data-stu-id="c7bdc-110">boolean</span></span>|<span data-ttu-id="c7bdc-111">表示是否以升序方式进行排序。</span><span class="sxs-lookup"><span data-stu-id="c7bdc-111">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="c7bdc-112">color</span><span class="sxs-lookup"><span data-stu-id="c7bdc-112">color</span></span>|<span data-ttu-id="c7bdc-113">string</span><span class="sxs-lookup"><span data-stu-id="c7bdc-113">string</span></span>|<span data-ttu-id="c7bdc-114">表示按字体或单元格颜色进行排序时，条件的目标颜色。</span><span class="sxs-lookup"><span data-stu-id="c7bdc-114">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="c7bdc-115">dataOption</span><span class="sxs-lookup"><span data-stu-id="c7bdc-115">dataOption</span></span>|<span data-ttu-id="c7bdc-116">string</span><span class="sxs-lookup"><span data-stu-id="c7bdc-116">string</span></span>|<span data-ttu-id="c7bdc-117">代表用于此字段的其他排序选项。</span><span class="sxs-lookup"><span data-stu-id="c7bdc-117">Represents additional sorting options for this field.</span></span> <span data-ttu-id="c7bdc-118">可能的值为： `Normal`， `TextAsNumber`。</span><span class="sxs-lookup"><span data-stu-id="c7bdc-118">The possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="c7bdc-119">Key</span><span class="sxs-lookup"><span data-stu-id="c7bdc-119">key</span></span>|<span data-ttu-id="c7bdc-120">int</span><span class="sxs-lookup"><span data-stu-id="c7bdc-120">int</span></span>|<span data-ttu-id="c7bdc-p102">表示条件所在的列（或行，具体取决于排序方向）。表示与第一列（或行）的偏移量。</span><span class="sxs-lookup"><span data-stu-id="c7bdc-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="c7bdc-123">sortOn</span><span class="sxs-lookup"><span data-stu-id="c7bdc-123">sortOn</span></span>|<span data-ttu-id="c7bdc-124">string</span><span class="sxs-lookup"><span data-stu-id="c7bdc-124">string</span></span>|<span data-ttu-id="c7bdc-125">表示此条件的排序的类型。</span><span class="sxs-lookup"><span data-stu-id="c7bdc-125">Represents the type of sorting of this condition.</span></span> <span data-ttu-id="c7bdc-126">可能的值为： `Value`， `CellColor`， `FontColor`， `Icon`。</span><span class="sxs-lookup"><span data-stu-id="c7bdc-126">The possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|
|<span data-ttu-id="c7bdc-127">icon</span><span class="sxs-lookup"><span data-stu-id="c7bdc-127">icon</span></span>|[<span data-ttu-id="c7bdc-128">WorkbookIcon</span><span class="sxs-lookup"><span data-stu-id="c7bdc-128">WorkbookIcon</span></span>](icon.md)|<span data-ttu-id="c7bdc-129">表示对单元格图标进行排序时，条件的目标图标。</span><span class="sxs-lookup"><span data-stu-id="c7bdc-129">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c7bdc-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c7bdc-130">JSON representation</span></span>

<span data-ttu-id="c7bdc-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c7bdc-131">Here is a JSON representation of the resource.</span></span>

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
