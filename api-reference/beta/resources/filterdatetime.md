---
title: FilterDatetime 资源类型
description: 表示在筛选值时如何筛选日期。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 166ed04fc58933c805fdd388e14da683110d6729
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42498047"
---
# <a name="filterdatetime-resource-type"></a><span data-ttu-id="372a8-103">FilterDatetime 资源类型</span><span class="sxs-lookup"><span data-stu-id="372a8-103">FilterDatetime resource type</span></span>

<span data-ttu-id="372a8-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="372a8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="372a8-105">表示在筛选值时如何筛选日期。</span><span class="sxs-lookup"><span data-stu-id="372a8-105">Represents how to filter a date when filtering on values.</span></span>

## <a name="properties"></a><span data-ttu-id="372a8-106">属性</span><span class="sxs-lookup"><span data-stu-id="372a8-106">Properties</span></span>
| <span data-ttu-id="372a8-107">属性</span><span class="sxs-lookup"><span data-stu-id="372a8-107">Property</span></span>     | <span data-ttu-id="372a8-108">类型</span><span class="sxs-lookup"><span data-stu-id="372a8-108">Type</span></span>   |<span data-ttu-id="372a8-109">说明</span><span class="sxs-lookup"><span data-stu-id="372a8-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="372a8-110">date</span><span class="sxs-lookup"><span data-stu-id="372a8-110">date</span></span>|<span data-ttu-id="372a8-111">string</span><span class="sxs-lookup"><span data-stu-id="372a8-111">string</span></span>|<span data-ttu-id="372a8-112">用于筛选数据的采用 ISO8601 格式的日期。</span><span class="sxs-lookup"><span data-stu-id="372a8-112">The date in ISO8601 format used to filter data.</span></span>|
|<span data-ttu-id="372a8-113">specificity</span><span class="sxs-lookup"><span data-stu-id="372a8-113">specificity</span></span>|<span data-ttu-id="372a8-114">string</span><span class="sxs-lookup"><span data-stu-id="372a8-114">string</span></span>|<span data-ttu-id="372a8-p101">用于保留数据的日期的具体程度。例如，如果日期是 2005-04-02 并将特殊性设置为“月”，则筛选操作将保留包含 2009 年 4 月日期的所有行。可能的值是：`Year`、`Monday`、`Day`、`Hour`、`Minute`、`Second`。</span><span class="sxs-lookup"><span data-stu-id="372a8-p101">How specific the date should be used to keep data. For example, if the date is 2005-04-02 and the specifity is set to "month", the filter operation will keep all rows with a date in the month of april 2009. Possible values are: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="372a8-118">关系</span><span class="sxs-lookup"><span data-stu-id="372a8-118">Relationships</span></span>
<span data-ttu-id="372a8-119">无</span><span class="sxs-lookup"><span data-stu-id="372a8-119">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="372a8-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="372a8-120">JSON representation</span></span>

<span data-ttu-id="372a8-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="372a8-121">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterDateTime"
}-->

```json
{
  "date": "string",
  "specificity": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "FilterDatetime resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
