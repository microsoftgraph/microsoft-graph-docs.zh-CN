---
title: SortField 资源类型
description: 表示排序操作中的条件。
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: debc1f860e2e24306d6261444a29e126037aa3ae
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806742"
---
# <a name="sortfield-resource-type"></a><span data-ttu-id="e2cb8-103">SortField 资源类型</span><span class="sxs-lookup"><span data-stu-id="e2cb8-103">SortField resource type</span></span>

<span data-ttu-id="e2cb8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2cb8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e2cb8-105">表示排序操作中的条件。</span><span class="sxs-lookup"><span data-stu-id="e2cb8-105">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="e2cb8-106">属性</span><span class="sxs-lookup"><span data-stu-id="e2cb8-106">Properties</span></span>
| <span data-ttu-id="e2cb8-107">属性</span><span class="sxs-lookup"><span data-stu-id="e2cb8-107">Property</span></span>     | <span data-ttu-id="e2cb8-108">类型</span><span class="sxs-lookup"><span data-stu-id="e2cb8-108">Type</span></span>   |<span data-ttu-id="e2cb8-109">说明</span><span class="sxs-lookup"><span data-stu-id="e2cb8-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2cb8-110">ascending</span><span class="sxs-lookup"><span data-stu-id="e2cb8-110">ascending</span></span>|<span data-ttu-id="e2cb8-111">boolean</span><span class="sxs-lookup"><span data-stu-id="e2cb8-111">boolean</span></span>|<span data-ttu-id="e2cb8-112">表示是否以升序方式进行排序。</span><span class="sxs-lookup"><span data-stu-id="e2cb8-112">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="e2cb8-113">color</span><span class="sxs-lookup"><span data-stu-id="e2cb8-113">color</span></span>|<span data-ttu-id="e2cb8-114">string</span><span class="sxs-lookup"><span data-stu-id="e2cb8-114">string</span></span>|<span data-ttu-id="e2cb8-115">表示按字体或单元格颜色进行排序时，条件的目标颜色。</span><span class="sxs-lookup"><span data-stu-id="e2cb8-115">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="e2cb8-116">dataOption</span><span class="sxs-lookup"><span data-stu-id="e2cb8-116">dataOption</span></span>|<span data-ttu-id="e2cb8-117">string</span><span class="sxs-lookup"><span data-stu-id="e2cb8-117">string</span></span>|<span data-ttu-id="e2cb8-118">表示此字段的其他排序选项。</span><span class="sxs-lookup"><span data-stu-id="e2cb8-118">Represents additional sorting options for this field.</span></span> <span data-ttu-id="e2cb8-119">可能的值为： `Normal` 、 `TextAsNumber` 。</span><span class="sxs-lookup"><span data-stu-id="e2cb8-119">The possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="e2cb8-120">Key</span><span class="sxs-lookup"><span data-stu-id="e2cb8-120">key</span></span>|<span data-ttu-id="e2cb8-121">int</span><span class="sxs-lookup"><span data-stu-id="e2cb8-121">int</span></span>|<span data-ttu-id="e2cb8-p102">表示条件所在的列（或行，具体取决于排序方向）。表示与第一列（或行）的偏移量。</span><span class="sxs-lookup"><span data-stu-id="e2cb8-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="e2cb8-124">sortOn</span><span class="sxs-lookup"><span data-stu-id="e2cb8-124">sortOn</span></span>|<span data-ttu-id="e2cb8-125">string</span><span class="sxs-lookup"><span data-stu-id="e2cb8-125">string</span></span>|<span data-ttu-id="e2cb8-126">表示此条件的排序类型。</span><span class="sxs-lookup"><span data-stu-id="e2cb8-126">Represents the type of sorting of this condition.</span></span> <span data-ttu-id="e2cb8-127">可能的值包括 `Value`、`CellColor`、`FontColor`、`Icon`。</span><span class="sxs-lookup"><span data-stu-id="e2cb8-127">The possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|
|<span data-ttu-id="e2cb8-128">图标</span><span class="sxs-lookup"><span data-stu-id="e2cb8-128">icon</span></span>|[<span data-ttu-id="e2cb8-129">WorkbookIcon</span><span class="sxs-lookup"><span data-stu-id="e2cb8-129">WorkbookIcon</span></span>](icon.md)|<span data-ttu-id="e2cb8-130">表示对单元格图标进行排序时，条件的目标图标。</span><span class="sxs-lookup"><span data-stu-id="e2cb8-130">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e2cb8-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e2cb8-131">JSON representation</span></span>

<span data-ttu-id="e2cb8-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2cb8-132">Here is a JSON representation of the resource.</span></span>

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
