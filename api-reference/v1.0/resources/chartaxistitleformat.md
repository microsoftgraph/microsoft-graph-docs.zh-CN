---
title: ChartAxisTitleFormat 资源类型
description: 表示图表坐标轴标题格式。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 26d305d8bd4a0059123f77bd86cbbf5fd01dcea7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569079"
---
# <a name="chartaxistitleformat-resource-type"></a><span data-ttu-id="7737d-103">ChartAxisTitleFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="7737d-103">ChartAxisTitleFormat resource type</span></span>

<span data-ttu-id="7737d-104">表示图表坐标轴标题格式。</span><span class="sxs-lookup"><span data-stu-id="7737d-104">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="7737d-105">方法</span><span class="sxs-lookup"><span data-stu-id="7737d-105">Methods</span></span>
<span data-ttu-id="7737d-106">无</span><span class="sxs-lookup"><span data-stu-id="7737d-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="7737d-107">属性</span><span class="sxs-lookup"><span data-stu-id="7737d-107">Properties</span></span>
<span data-ttu-id="7737d-108">无</span><span class="sxs-lookup"><span data-stu-id="7737d-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="7737d-109">关系</span><span class="sxs-lookup"><span data-stu-id="7737d-109">Relationships</span></span>
| <span data-ttu-id="7737d-110">关系</span><span class="sxs-lookup"><span data-stu-id="7737d-110">Relationship</span></span> | <span data-ttu-id="7737d-111">类型</span><span class="sxs-lookup"><span data-stu-id="7737d-111">Type</span></span>   |<span data-ttu-id="7737d-112">说明</span><span class="sxs-lookup"><span data-stu-id="7737d-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7737d-113">font</span><span class="sxs-lookup"><span data-stu-id="7737d-113">font</span></span>|[<span data-ttu-id="7737d-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="7737d-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="7737d-115">表示图表坐标轴标题对象的字体属性，例如字体名称、字体大小、颜色等。</span><span class="sxs-lookup"><span data-stu-id="7737d-115">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object.</span></span> <span data-ttu-id="7737d-116">只读。</span><span class="sxs-lookup"><span data-stu-id="7737d-116">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7737d-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7737d-117">JSON representation</span></span>

<span data-ttu-id="7737d-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7737d-118">Here is a JSON representation of the resource.</span></span>

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
