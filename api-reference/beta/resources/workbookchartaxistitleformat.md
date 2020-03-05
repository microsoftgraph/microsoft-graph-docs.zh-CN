---
title: workbookChartAxisTitleFormat 资源类型
description: 表示图表坐标轴标题格式。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: a676bb28ccce19c7f4293e9fc082a59ec0cfdbb7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519356"
---
# <a name="workbookchartaxistitleformat-resource-type"></a><span data-ttu-id="d608c-103">workbookChartAxisTitleFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="d608c-103">workbookChartAxisTitleFormat resource type</span></span>

<span data-ttu-id="d608c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d608c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d608c-105">表示图表坐标轴标题格式。</span><span class="sxs-lookup"><span data-stu-id="d608c-105">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="d608c-106">方法</span><span class="sxs-lookup"><span data-stu-id="d608c-106">Methods</span></span>
<span data-ttu-id="d608c-107">无</span><span class="sxs-lookup"><span data-stu-id="d608c-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="d608c-108">属性</span><span class="sxs-lookup"><span data-stu-id="d608c-108">Properties</span></span>
<span data-ttu-id="d608c-109">无</span><span class="sxs-lookup"><span data-stu-id="d608c-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="d608c-110">关系</span><span class="sxs-lookup"><span data-stu-id="d608c-110">Relationships</span></span>
| <span data-ttu-id="d608c-111">关系</span><span class="sxs-lookup"><span data-stu-id="d608c-111">Relationship</span></span> | <span data-ttu-id="d608c-112">类型</span><span class="sxs-lookup"><span data-stu-id="d608c-112">Type</span></span>   |<span data-ttu-id="d608c-113">说明</span><span class="sxs-lookup"><span data-stu-id="d608c-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d608c-114">font</span><span class="sxs-lookup"><span data-stu-id="d608c-114">font</span></span>|[<span data-ttu-id="d608c-115">workbookChartFont</span><span class="sxs-lookup"><span data-stu-id="d608c-115">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="d608c-116">表示图表坐标轴标题对象的字体属性，例如字体名称、字体大小、颜色等。</span><span class="sxs-lookup"><span data-stu-id="d608c-116">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object.</span></span> <span data-ttu-id="d608c-117">只读。</span><span class="sxs-lookup"><span data-stu-id="d608c-117">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d608c-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d608c-118">JSON representation</span></span>

<span data-ttu-id="d608c-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d608c-119">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "font"
    ],
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
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxisTitleFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
