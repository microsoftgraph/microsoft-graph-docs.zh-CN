---
title: workbookSortField 资源类型
description: 表示排序操作中的条件。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: ruoyingl
ms.openlocfilehash: a245591755542a0a9bcfefb3f220511bd1521118
ms.sourcegitcommit: de175a11806f9e9ba3c916384e897aee1cc7f75c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/09/2021
ms.locfileid: "49790669"
---
# <a name="workbooksortfield-resource-type"></a><span data-ttu-id="efc4e-103">workbookSortField 资源类型</span><span class="sxs-lookup"><span data-stu-id="efc4e-103">workbookSortField resource type</span></span>

<span data-ttu-id="efc4e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efc4e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efc4e-105">表示排序操作中的条件。</span><span class="sxs-lookup"><span data-stu-id="efc4e-105">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="efc4e-106">属性</span><span class="sxs-lookup"><span data-stu-id="efc4e-106">Properties</span></span>
| <span data-ttu-id="efc4e-107">属性</span><span class="sxs-lookup"><span data-stu-id="efc4e-107">Property</span></span>     | <span data-ttu-id="efc4e-108">类型</span><span class="sxs-lookup"><span data-stu-id="efc4e-108">Type</span></span>   |<span data-ttu-id="efc4e-109">说明</span><span class="sxs-lookup"><span data-stu-id="efc4e-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="efc4e-110">ascending</span><span class="sxs-lookup"><span data-stu-id="efc4e-110">ascending</span></span>|<span data-ttu-id="efc4e-111">boolean</span><span class="sxs-lookup"><span data-stu-id="efc4e-111">boolean</span></span>|<span data-ttu-id="efc4e-112">表示是否以升序方式进行排序。</span><span class="sxs-lookup"><span data-stu-id="efc4e-112">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="efc4e-113">color</span><span class="sxs-lookup"><span data-stu-id="efc4e-113">color</span></span>|<span data-ttu-id="efc4e-114">string</span><span class="sxs-lookup"><span data-stu-id="efc4e-114">string</span></span>|<span data-ttu-id="efc4e-115">表示按字体或单元格颜色进行排序时，条件的目标颜色。</span><span class="sxs-lookup"><span data-stu-id="efc4e-115">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="efc4e-116">dataOption</span><span class="sxs-lookup"><span data-stu-id="efc4e-116">dataOption</span></span>|<span data-ttu-id="efc4e-117">string</span><span class="sxs-lookup"><span data-stu-id="efc4e-117">string</span></span>|<span data-ttu-id="efc4e-p101">表示此字段的其他排序选项。可能的值是：`Normal`、`TextAsNumber`。</span><span class="sxs-lookup"><span data-stu-id="efc4e-p101">Represents additional sorting options for this field. Possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="efc4e-120">图标</span><span class="sxs-lookup"><span data-stu-id="efc4e-120">icon</span></span>|[<span data-ttu-id="efc4e-121">workbookIcon</span><span class="sxs-lookup"><span data-stu-id="efc4e-121">workbookIcon</span></span>](workbookicon.md)|<span data-ttu-id="efc4e-122">表示对单元格图标进行排序时，条件的目标图标。</span><span class="sxs-lookup"><span data-stu-id="efc4e-122">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|
|<span data-ttu-id="efc4e-123">Key</span><span class="sxs-lookup"><span data-stu-id="efc4e-123">key</span></span>|<span data-ttu-id="efc4e-124">int</span><span class="sxs-lookup"><span data-stu-id="efc4e-124">int</span></span>|<span data-ttu-id="efc4e-p102">表示条件所在的列（或行，具体取决于排序方向）。表示与第一列（或行）的偏移量。</span><span class="sxs-lookup"><span data-stu-id="efc4e-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="efc4e-127">sortOn</span><span class="sxs-lookup"><span data-stu-id="efc4e-127">sortOn</span></span>|<span data-ttu-id="efc4e-128">string</span><span class="sxs-lookup"><span data-stu-id="efc4e-128">string</span></span>|<span data-ttu-id="efc4e-p103">表示此条件的排序类型。可能的值是：`Value`、`CellColor`、`FontColor`、`Icon`。</span><span class="sxs-lookup"><span data-stu-id="efc4e-p103">Represents the type of sorting of this condition. Possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="efc4e-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="efc4e-131">JSON representation</span></span>

<span data-ttu-id="efc4e-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="efc4e-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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


