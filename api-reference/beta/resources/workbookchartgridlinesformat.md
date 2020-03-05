---
title: workbookChartGridlinesFormat 资源类型
description: 封装图表网格线的格式属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: bdd676f1271c0fdfd0273d3a5064c46127b73fd3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519314"
---
# <a name="workbookchartgridlinesformat-resource-type"></a><span data-ttu-id="9e166-103">workbookChartGridlinesFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="9e166-103">workbookChartGridlinesFormat resource type</span></span>

<span data-ttu-id="9e166-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="9e166-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e166-105">封装图表网格线的格式属性。</span><span class="sxs-lookup"><span data-stu-id="9e166-105">Encapsulates the format properties for chart gridlines.</span></span>

## <a name="methods"></a><span data-ttu-id="9e166-106">方法</span><span class="sxs-lookup"><span data-stu-id="9e166-106">Methods</span></span>
<span data-ttu-id="9e166-107">无</span><span class="sxs-lookup"><span data-stu-id="9e166-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="9e166-108">属性</span><span class="sxs-lookup"><span data-stu-id="9e166-108">Properties</span></span>
<span data-ttu-id="9e166-109">无</span><span class="sxs-lookup"><span data-stu-id="9e166-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="9e166-110">关系</span><span class="sxs-lookup"><span data-stu-id="9e166-110">Relationships</span></span>
| <span data-ttu-id="9e166-111">关系</span><span class="sxs-lookup"><span data-stu-id="9e166-111">Relationship</span></span> | <span data-ttu-id="9e166-112">类型</span><span class="sxs-lookup"><span data-stu-id="9e166-112">Type</span></span>   |<span data-ttu-id="9e166-113">说明</span><span class="sxs-lookup"><span data-stu-id="9e166-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e166-114">line</span><span class="sxs-lookup"><span data-stu-id="9e166-114">line</span></span>|[<span data-ttu-id="9e166-115">workbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="9e166-115">workbookChartLineFormat</span></span>](workbookchartlineformat.md)|<span data-ttu-id="9e166-116">表示图表线条格式。</span><span class="sxs-lookup"><span data-stu-id="9e166-116">Represents chart line formatting.</span></span> <span data-ttu-id="9e166-117">只读。</span><span class="sxs-lookup"><span data-stu-id="9e166-117">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="9e166-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9e166-118">JSON representation</span></span>

<span data-ttu-id="9e166-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e166-119">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "line"
    ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartGridlinesFormat"
}-->

```json
{
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartGridlinesFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
