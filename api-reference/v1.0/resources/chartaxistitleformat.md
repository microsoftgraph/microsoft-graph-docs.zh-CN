---
title: ChartAxisTitleFormat 资源类型
description: 表示图表坐标轴标题格式。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 3ae74b7353a0b4198b42a04fdd420eb3447d4c11
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029846"
---
# <a name="chartaxistitleformat-resource-type"></a><span data-ttu-id="c05eb-103">ChartAxisTitleFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="c05eb-103">ChartAxisTitleFormat resource type</span></span>

<span data-ttu-id="c05eb-104">表示图表坐标轴标题格式。</span><span class="sxs-lookup"><span data-stu-id="c05eb-104">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="c05eb-105">方法</span><span class="sxs-lookup"><span data-stu-id="c05eb-105">Methods</span></span>
<span data-ttu-id="c05eb-106">无</span><span class="sxs-lookup"><span data-stu-id="c05eb-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="c05eb-107">属性</span><span class="sxs-lookup"><span data-stu-id="c05eb-107">Properties</span></span>
<span data-ttu-id="c05eb-108">无</span><span class="sxs-lookup"><span data-stu-id="c05eb-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="c05eb-109">关系</span><span class="sxs-lookup"><span data-stu-id="c05eb-109">Relationships</span></span>
| <span data-ttu-id="c05eb-110">关系</span><span class="sxs-lookup"><span data-stu-id="c05eb-110">Relationship</span></span> | <span data-ttu-id="c05eb-111">类型</span><span class="sxs-lookup"><span data-stu-id="c05eb-111">Type</span></span>   |<span data-ttu-id="c05eb-112">说明</span><span class="sxs-lookup"><span data-stu-id="c05eb-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c05eb-113">font</span><span class="sxs-lookup"><span data-stu-id="c05eb-113">font</span></span>|[<span data-ttu-id="c05eb-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="c05eb-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="c05eb-115">表示图表坐标轴标题对象的字体属性，例如字体名称、字体大小、颜色等。</span><span class="sxs-lookup"><span data-stu-id="c05eb-115">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object.</span></span> <span data-ttu-id="c05eb-116">只读。</span><span class="sxs-lookup"><span data-stu-id="c05eb-116">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c05eb-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c05eb-117">JSON representation</span></span>

<span data-ttu-id="c05eb-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c05eb-118">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxisTitleFormat"
}-->

```json
{
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisTitleFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
