---
title: SortField 资源类型
description: 表示排序操作中的条件。
localization_priority: Normal
ms.openlocfilehash: 2c1b9a272fd024455d1297c5f59ca7684283e1a1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561297"
---
# <a name="sortfield-resource-type"></a><span data-ttu-id="9c173-103">SortField 资源类型</span><span class="sxs-lookup"><span data-stu-id="9c173-103">SortField resource type</span></span>

<span data-ttu-id="9c173-104">表示排序操作中的条件。</span><span class="sxs-lookup"><span data-stu-id="9c173-104">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="9c173-105">属性</span><span class="sxs-lookup"><span data-stu-id="9c173-105">Properties</span></span>
| <span data-ttu-id="9c173-106">属性</span><span class="sxs-lookup"><span data-stu-id="9c173-106">Property</span></span>     | <span data-ttu-id="9c173-107">类型</span><span class="sxs-lookup"><span data-stu-id="9c173-107">Type</span></span>   |<span data-ttu-id="9c173-108">说明</span><span class="sxs-lookup"><span data-stu-id="9c173-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c173-109">ascending</span><span class="sxs-lookup"><span data-stu-id="9c173-109">ascending</span></span>|<span data-ttu-id="9c173-110">boolean</span><span class="sxs-lookup"><span data-stu-id="9c173-110">boolean</span></span>|<span data-ttu-id="9c173-111">表示是否以升序方式进行排序。</span><span class="sxs-lookup"><span data-stu-id="9c173-111">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="9c173-112">color</span><span class="sxs-lookup"><span data-stu-id="9c173-112">color</span></span>|<span data-ttu-id="9c173-113">字符串</span><span class="sxs-lookup"><span data-stu-id="9c173-113">string</span></span>|<span data-ttu-id="9c173-114">表示按字体或单元格颜色进行排序时，条件的目标颜色。</span><span class="sxs-lookup"><span data-stu-id="9c173-114">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="9c173-115">dataOption</span><span class="sxs-lookup"><span data-stu-id="9c173-115">dataOption</span></span>|<span data-ttu-id="9c173-116">string</span><span class="sxs-lookup"><span data-stu-id="9c173-116">string</span></span>|<span data-ttu-id="9c173-117">表示此字段的其他排序选项。</span><span class="sxs-lookup"><span data-stu-id="9c173-117">Represents additional sorting options for this field.</span></span> <span data-ttu-id="9c173-118">可能的值为: `Normal`、 `TextAsNumber`。</span><span class="sxs-lookup"><span data-stu-id="9c173-118">The possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="9c173-119">Key</span><span class="sxs-lookup"><span data-stu-id="9c173-119">key</span></span>|<span data-ttu-id="9c173-120">int</span><span class="sxs-lookup"><span data-stu-id="9c173-120">int</span></span>|<span data-ttu-id="9c173-p102">表示条件所在的列（或行，具体取决于排序方向）。表示与第一列（或行）的偏移量。</span><span class="sxs-lookup"><span data-stu-id="9c173-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="9c173-123">sortOn</span><span class="sxs-lookup"><span data-stu-id="9c173-123">sortOn</span></span>|<span data-ttu-id="9c173-124">string</span><span class="sxs-lookup"><span data-stu-id="9c173-124">string</span></span>|<span data-ttu-id="9c173-125">表示此条件的排序类型。</span><span class="sxs-lookup"><span data-stu-id="9c173-125">Represents the type of sorting of this condition.</span></span> <span data-ttu-id="9c173-126">可能的值为: `Value`、 `CellColor`、 `FontColor`、 `Icon`。</span><span class="sxs-lookup"><span data-stu-id="9c173-126">The possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|
|<span data-ttu-id="9c173-127">图标</span><span class="sxs-lookup"><span data-stu-id="9c173-127">icon</span></span>|[<span data-ttu-id="9c173-128">WorkbookIcon</span><span class="sxs-lookup"><span data-stu-id="9c173-128">WorkbookIcon</span></span>](icon.md)|<span data-ttu-id="9c173-129">表示对单元格图标进行排序时，条件的目标图标。</span><span class="sxs-lookup"><span data-stu-id="9c173-129">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9c173-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9c173-130">JSON representation</span></span>

<span data-ttu-id="9c173-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9c173-131">Here is a JSON representation of the resource.</span></span>

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
