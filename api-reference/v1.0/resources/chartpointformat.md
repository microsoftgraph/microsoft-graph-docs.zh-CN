---
title: ChartPointFormat 资源类型
description: 表示图表点的格式化对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: c71b7158b7ba3cef208fb6bf983d077c9474e77c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533103"
---
# <a name="chartpointformat-resource-type"></a><span data-ttu-id="41aa0-103">ChartPointFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="41aa0-103">ChartPointFormat resource type</span></span>

<span data-ttu-id="41aa0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41aa0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="41aa0-105">表示图表点的格式化对象。</span><span class="sxs-lookup"><span data-stu-id="41aa0-105">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="41aa0-106">Methods</span><span class="sxs-lookup"><span data-stu-id="41aa0-106">Methods</span></span>
<span data-ttu-id="41aa0-107">无</span><span class="sxs-lookup"><span data-stu-id="41aa0-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="41aa0-108">属性</span><span class="sxs-lookup"><span data-stu-id="41aa0-108">Properties</span></span>
<span data-ttu-id="41aa0-109">无</span><span class="sxs-lookup"><span data-stu-id="41aa0-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="41aa0-110">关系</span><span class="sxs-lookup"><span data-stu-id="41aa0-110">Relationships</span></span>
| <span data-ttu-id="41aa0-111">关系</span><span class="sxs-lookup"><span data-stu-id="41aa0-111">Relationship</span></span> | <span data-ttu-id="41aa0-112">类型</span><span class="sxs-lookup"><span data-stu-id="41aa0-112">Type</span></span>   |<span data-ttu-id="41aa0-113">说明</span><span class="sxs-lookup"><span data-stu-id="41aa0-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41aa0-114">fill</span><span class="sxs-lookup"><span data-stu-id="41aa0-114">fill</span></span>|[<span data-ttu-id="41aa0-115">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="41aa0-115">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="41aa0-116">表示图表的填充格式，包括背景格式信息。</span><span class="sxs-lookup"><span data-stu-id="41aa0-116">Represents the fill format of a chart, which includes background formating information.</span></span> <span data-ttu-id="41aa0-117">只读。</span><span class="sxs-lookup"><span data-stu-id="41aa0-117">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="41aa0-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="41aa0-118">JSON representation</span></span>

<span data-ttu-id="41aa0-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="41aa0-119">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPointFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPointFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
