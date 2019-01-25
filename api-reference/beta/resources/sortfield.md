---
title: SortField 资源类型
description: 表示排序操作中的条件。
localization_priority: Normal
ms.openlocfilehash: 52817df89ed130b6984ae3a76da775e0e000dee5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521633"
---
# <a name="sortfield-resource-type"></a><span data-ttu-id="db6e1-103">SortField 资源类型</span><span class="sxs-lookup"><span data-stu-id="db6e1-103">SortField resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db6e1-104">表示排序操作中的条件。</span><span class="sxs-lookup"><span data-stu-id="db6e1-104">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="db6e1-105">属性</span><span class="sxs-lookup"><span data-stu-id="db6e1-105">Properties</span></span>
| <span data-ttu-id="db6e1-106">属性</span><span class="sxs-lookup"><span data-stu-id="db6e1-106">Property</span></span>     | <span data-ttu-id="db6e1-107">类型</span><span class="sxs-lookup"><span data-stu-id="db6e1-107">Type</span></span>   |<span data-ttu-id="db6e1-108">说明</span><span class="sxs-lookup"><span data-stu-id="db6e1-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db6e1-109">ascending</span><span class="sxs-lookup"><span data-stu-id="db6e1-109">ascending</span></span>|<span data-ttu-id="db6e1-110">布尔</span><span class="sxs-lookup"><span data-stu-id="db6e1-110">boolean</span></span>|<span data-ttu-id="db6e1-111">表示是否以升序方式进行排序。</span><span class="sxs-lookup"><span data-stu-id="db6e1-111">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="db6e1-112">color</span><span class="sxs-lookup"><span data-stu-id="db6e1-112">color</span></span>|<span data-ttu-id="db6e1-113">string</span><span class="sxs-lookup"><span data-stu-id="db6e1-113">string</span></span>|<span data-ttu-id="db6e1-114">表示按字体或单元格颜色进行排序时，条件的目标颜色。</span><span class="sxs-lookup"><span data-stu-id="db6e1-114">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="db6e1-115">dataOption</span><span class="sxs-lookup"><span data-stu-id="db6e1-115">dataOption</span></span>|<span data-ttu-id="db6e1-116">string</span><span class="sxs-lookup"><span data-stu-id="db6e1-116">string</span></span>|<span data-ttu-id="db6e1-p101">表示此字段的其他排序选项。可能的值是：`Normal`、`TextAsNumber`。</span><span class="sxs-lookup"><span data-stu-id="db6e1-p101">Represents additional sorting options for this field. Possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="db6e1-119">Key</span><span class="sxs-lookup"><span data-stu-id="db6e1-119">key</span></span>|<span data-ttu-id="db6e1-120">int</span><span class="sxs-lookup"><span data-stu-id="db6e1-120">int</span></span>|<span data-ttu-id="db6e1-p102">表示条件所在的列（或行，具体取决于排序方向）。表示与第一列（或行）的偏移量。</span><span class="sxs-lookup"><span data-stu-id="db6e1-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="db6e1-123">sortOn</span><span class="sxs-lookup"><span data-stu-id="db6e1-123">sortOn</span></span>|<span data-ttu-id="db6e1-124">string</span><span class="sxs-lookup"><span data-stu-id="db6e1-124">string</span></span>|<span data-ttu-id="db6e1-p103">表示此条件的排序类型。可能的值是：`Value`、`CellColor`、`FontColor`、`Icon`。</span><span class="sxs-lookup"><span data-stu-id="db6e1-p103">Represents the type of sorting of this condition. Possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="db6e1-127">关系</span><span class="sxs-lookup"><span data-stu-id="db6e1-127">Relationships</span></span>
| <span data-ttu-id="db6e1-128">关系</span><span class="sxs-lookup"><span data-stu-id="db6e1-128">Relationship</span></span> | <span data-ttu-id="db6e1-129">类型</span><span class="sxs-lookup"><span data-stu-id="db6e1-129">Type</span></span>   |<span data-ttu-id="db6e1-130">说明</span><span class="sxs-lookup"><span data-stu-id="db6e1-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db6e1-131">icon</span><span class="sxs-lookup"><span data-stu-id="db6e1-131">icon</span></span>|[<span data-ttu-id="db6e1-132">Icon</span><span class="sxs-lookup"><span data-stu-id="db6e1-132">Icon</span></span>](icon.md)|<span data-ttu-id="db6e1-133">表示对单元格图标进行排序时，条件的目标图标。</span><span class="sxs-lookup"><span data-stu-id="db6e1-133">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="db6e1-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="db6e1-134">JSON representation</span></span>

<span data-ttu-id="db6e1-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="db6e1-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sortField"
}-->

```json
{
  "ascending": true,
  "color": "string",
  "dataOption": "string",
  "key": 1024,
  "sortOn": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "SortField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/sortfield.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
