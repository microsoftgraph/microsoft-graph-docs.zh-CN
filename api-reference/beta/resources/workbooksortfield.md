---
title: workbookSortField 资源类型
description: 表示排序操作中的条件。
localization_priority: Normal
ms.openlocfilehash: 239c0e3b9f95108165ed32e7e22f94049e787432
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348625"
---
# <a name="workbooksortfield-resource-type"></a><span data-ttu-id="d1f6c-103">workbookSortField 资源类型</span><span class="sxs-lookup"><span data-stu-id="d1f6c-103">workbookSortField resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1f6c-104">表示排序操作中的条件。</span><span class="sxs-lookup"><span data-stu-id="d1f6c-104">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="d1f6c-105">属性</span><span class="sxs-lookup"><span data-stu-id="d1f6c-105">Properties</span></span>
| <span data-ttu-id="d1f6c-106">属性</span><span class="sxs-lookup"><span data-stu-id="d1f6c-106">Property</span></span>     | <span data-ttu-id="d1f6c-107">类型</span><span class="sxs-lookup"><span data-stu-id="d1f6c-107">Type</span></span>   |<span data-ttu-id="d1f6c-108">说明</span><span class="sxs-lookup"><span data-stu-id="d1f6c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1f6c-109">ascending</span><span class="sxs-lookup"><span data-stu-id="d1f6c-109">ascending</span></span>|<span data-ttu-id="d1f6c-110">boolean</span><span class="sxs-lookup"><span data-stu-id="d1f6c-110">boolean</span></span>|<span data-ttu-id="d1f6c-111">表示是否以升序方式进行排序。</span><span class="sxs-lookup"><span data-stu-id="d1f6c-111">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="d1f6c-112">color</span><span class="sxs-lookup"><span data-stu-id="d1f6c-112">color</span></span>|<span data-ttu-id="d1f6c-113">字符串</span><span class="sxs-lookup"><span data-stu-id="d1f6c-113">string</span></span>|<span data-ttu-id="d1f6c-114">表示按字体或单元格颜色进行排序时，条件的目标颜色。</span><span class="sxs-lookup"><span data-stu-id="d1f6c-114">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="d1f6c-115">dataOption</span><span class="sxs-lookup"><span data-stu-id="d1f6c-115">dataOption</span></span>|<span data-ttu-id="d1f6c-116">string</span><span class="sxs-lookup"><span data-stu-id="d1f6c-116">string</span></span>|<span data-ttu-id="d1f6c-p101">表示此字段的其他排序选项。可能的值是：`Normal`、`TextAsNumber`。</span><span class="sxs-lookup"><span data-stu-id="d1f6c-p101">Represents additional sorting options for this field. Possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="d1f6c-119">Key</span><span class="sxs-lookup"><span data-stu-id="d1f6c-119">key</span></span>|<span data-ttu-id="d1f6c-120">int</span><span class="sxs-lookup"><span data-stu-id="d1f6c-120">int</span></span>|<span data-ttu-id="d1f6c-p102">表示条件所在的列（或行，具体取决于排序方向）。表示与第一列（或行）的偏移量。</span><span class="sxs-lookup"><span data-stu-id="d1f6c-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="d1f6c-123">sortOn</span><span class="sxs-lookup"><span data-stu-id="d1f6c-123">sortOn</span></span>|<span data-ttu-id="d1f6c-124">string</span><span class="sxs-lookup"><span data-stu-id="d1f6c-124">string</span></span>|<span data-ttu-id="d1f6c-p103">表示此条件的排序类型。可能的值是：`Value`、`CellColor`、`FontColor`、`Icon`。</span><span class="sxs-lookup"><span data-stu-id="d1f6c-p103">Represents the type of sorting of this condition. Possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1f6c-127">关系</span><span class="sxs-lookup"><span data-stu-id="d1f6c-127">Relationships</span></span>
| <span data-ttu-id="d1f6c-128">关系</span><span class="sxs-lookup"><span data-stu-id="d1f6c-128">Relationship</span></span> | <span data-ttu-id="d1f6c-129">类型</span><span class="sxs-lookup"><span data-stu-id="d1f6c-129">Type</span></span>   |<span data-ttu-id="d1f6c-130">说明</span><span class="sxs-lookup"><span data-stu-id="d1f6c-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1f6c-131">icon</span><span class="sxs-lookup"><span data-stu-id="d1f6c-131">icon</span></span>|[<span data-ttu-id="d1f6c-132">workbookIcon</span><span class="sxs-lookup"><span data-stu-id="d1f6c-132">workbookIcon</span></span>](workbookicon.md)|<span data-ttu-id="d1f6c-133">表示对单元格图标进行排序时，条件的目标图标。</span><span class="sxs-lookup"><span data-stu-id="d1f6c-133">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d1f6c-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d1f6c-134">JSON representation</span></span>

<span data-ttu-id="d1f6c-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d1f6c-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookSortField"
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
  "suppressions": []
}
-->
