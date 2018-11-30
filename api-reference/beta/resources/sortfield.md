---
title: SortField 资源类型
description: 表示排序操作中的条件。
ms.openlocfilehash: bb5915e9d9637912b97c0425819acd15a6ed40ca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047233"
---
# <a name="sortfield-resource-type"></a><span data-ttu-id="247c5-103">SortField 资源类型</span><span class="sxs-lookup"><span data-stu-id="247c5-103">SortField resource type</span></span>

> <span data-ttu-id="247c5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="247c5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="247c5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="247c5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="247c5-106">表示排序操作中的条件。</span><span class="sxs-lookup"><span data-stu-id="247c5-106">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="247c5-107">属性</span><span class="sxs-lookup"><span data-stu-id="247c5-107">Properties</span></span>
| <span data-ttu-id="247c5-108">属性</span><span class="sxs-lookup"><span data-stu-id="247c5-108">Property</span></span>     | <span data-ttu-id="247c5-109">类型</span><span class="sxs-lookup"><span data-stu-id="247c5-109">Type</span></span>   |<span data-ttu-id="247c5-110">说明</span><span class="sxs-lookup"><span data-stu-id="247c5-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="247c5-111">ascending</span><span class="sxs-lookup"><span data-stu-id="247c5-111">ascending</span></span>|<span data-ttu-id="247c5-112">boolean</span><span class="sxs-lookup"><span data-stu-id="247c5-112">boolean</span></span>|<span data-ttu-id="247c5-113">表示是否以升序方式进行排序。</span><span class="sxs-lookup"><span data-stu-id="247c5-113">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="247c5-114">color</span><span class="sxs-lookup"><span data-stu-id="247c5-114">color</span></span>|<span data-ttu-id="247c5-115">string</span><span class="sxs-lookup"><span data-stu-id="247c5-115">string</span></span>|<span data-ttu-id="247c5-116">表示按字体或单元格颜色进行排序时，条件的目标颜色。</span><span class="sxs-lookup"><span data-stu-id="247c5-116">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="247c5-117">dataOption</span><span class="sxs-lookup"><span data-stu-id="247c5-117">dataOption</span></span>|<span data-ttu-id="247c5-118">string</span><span class="sxs-lookup"><span data-stu-id="247c5-118">string</span></span>|<span data-ttu-id="247c5-p102">表示此字段的其他排序选项。可能的值是：`Normal`、`TextAsNumber`。</span><span class="sxs-lookup"><span data-stu-id="247c5-p102">Represents additional sorting options for this field. Possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="247c5-121">Key</span><span class="sxs-lookup"><span data-stu-id="247c5-121">key</span></span>|<span data-ttu-id="247c5-122">整数</span><span class="sxs-lookup"><span data-stu-id="247c5-122">int</span></span>|<span data-ttu-id="247c5-p103">表示条件所在的列（或行，具体取决于排序方向）。表示与第一列（或行）的偏移量。</span><span class="sxs-lookup"><span data-stu-id="247c5-p103">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="247c5-125">sortOn</span><span class="sxs-lookup"><span data-stu-id="247c5-125">sortOn</span></span>|<span data-ttu-id="247c5-126">string</span><span class="sxs-lookup"><span data-stu-id="247c5-126">string</span></span>|<span data-ttu-id="247c5-p104">表示此条件的排序类型。可能的值是：`Value`、`CellColor`、`FontColor`、`Icon`。</span><span class="sxs-lookup"><span data-stu-id="247c5-p104">Represents the type of sorting of this condition. Possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="247c5-129">Relationships</span><span class="sxs-lookup"><span data-stu-id="247c5-129">Relationships</span></span>
| <span data-ttu-id="247c5-130">关系</span><span class="sxs-lookup"><span data-stu-id="247c5-130">Relationship</span></span> | <span data-ttu-id="247c5-131">类型</span><span class="sxs-lookup"><span data-stu-id="247c5-131">Type</span></span>   |<span data-ttu-id="247c5-132">说明</span><span class="sxs-lookup"><span data-stu-id="247c5-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="247c5-133">icon</span><span class="sxs-lookup"><span data-stu-id="247c5-133">icon</span></span>|[<span data-ttu-id="247c5-134">Icon</span><span class="sxs-lookup"><span data-stu-id="247c5-134">Icon</span></span>](icon.md)|<span data-ttu-id="247c5-135">表示对单元格图标进行排序时，条件的目标图标。</span><span class="sxs-lookup"><span data-stu-id="247c5-135">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="247c5-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="247c5-136">JSON representation</span></span>

<span data-ttu-id="247c5-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="247c5-137">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "SortField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->