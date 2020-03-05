---
title: workbookChartPointFormat 资源类型
description: 表示图表点的格式化对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 9e947fa02624f2c24ea6433dc2e62eb0da218308
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519279"
---
# <a name="workbookchartpointformat-resource-type"></a><span data-ttu-id="50d4d-103">workbookChartPointFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="50d4d-103">workbookChartPointFormat resource type</span></span>

<span data-ttu-id="50d4d-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="50d4d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50d4d-105">表示图表点的格式化对象。</span><span class="sxs-lookup"><span data-stu-id="50d4d-105">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="50d4d-106">方法</span><span class="sxs-lookup"><span data-stu-id="50d4d-106">Methods</span></span>
<span data-ttu-id="50d4d-107">无</span><span class="sxs-lookup"><span data-stu-id="50d4d-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="50d4d-108">属性</span><span class="sxs-lookup"><span data-stu-id="50d4d-108">Properties</span></span>
<span data-ttu-id="50d4d-109">无</span><span class="sxs-lookup"><span data-stu-id="50d4d-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="50d4d-110">关系</span><span class="sxs-lookup"><span data-stu-id="50d4d-110">Relationships</span></span>
| <span data-ttu-id="50d4d-111">关系</span><span class="sxs-lookup"><span data-stu-id="50d4d-111">Relationship</span></span> | <span data-ttu-id="50d4d-112">类型</span><span class="sxs-lookup"><span data-stu-id="50d4d-112">Type</span></span>   |<span data-ttu-id="50d4d-113">说明</span><span class="sxs-lookup"><span data-stu-id="50d4d-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50d4d-114">fill</span><span class="sxs-lookup"><span data-stu-id="50d4d-114">fill</span></span>|[<span data-ttu-id="50d4d-115">workbookChartFill</span><span class="sxs-lookup"><span data-stu-id="50d4d-115">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="50d4d-116">表示图表的填充格式，包括背景格式信息。</span><span class="sxs-lookup"><span data-stu-id="50d4d-116">Represents the fill format of a chart, which includes background formating information.</span></span> <span data-ttu-id="50d4d-117">只读。</span><span class="sxs-lookup"><span data-stu-id="50d4d-117">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="50d4d-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="50d4d-118">JSON representation</span></span>

<span data-ttu-id="50d4d-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50d4d-119">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "fill"
    ],
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
<!--
{
  "type": "#page.annotation",
  "description": "ChartPointFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
