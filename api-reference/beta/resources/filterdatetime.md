---
title: FilterDatetime 资源类型
description: 表示在筛选值时如何筛选日期。
localization_priority: Normal
ms.openlocfilehash: 24929695ff65173933b91fd82ac3e82de1f04da0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871307"
---
# <a name="filterdatetime-resource-type"></a><span data-ttu-id="9f765-103">FilterDatetime 资源类型</span><span class="sxs-lookup"><span data-stu-id="9f765-103">FilterDatetime resource type</span></span>

> <span data-ttu-id="9f765-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9f765-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f765-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9f765-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9f765-106">表示在筛选值时如何筛选日期。</span><span class="sxs-lookup"><span data-stu-id="9f765-106">Represents how to filter a date when filtering on values.</span></span>

## <a name="properties"></a><span data-ttu-id="9f765-107">属性</span><span class="sxs-lookup"><span data-stu-id="9f765-107">Properties</span></span>
| <span data-ttu-id="9f765-108">属性</span><span class="sxs-lookup"><span data-stu-id="9f765-108">Property</span></span>     | <span data-ttu-id="9f765-109">类型</span><span class="sxs-lookup"><span data-stu-id="9f765-109">Type</span></span>   |<span data-ttu-id="9f765-110">说明</span><span class="sxs-lookup"><span data-stu-id="9f765-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f765-111">date</span><span class="sxs-lookup"><span data-stu-id="9f765-111">date</span></span>|<span data-ttu-id="9f765-112">string</span><span class="sxs-lookup"><span data-stu-id="9f765-112">string</span></span>|<span data-ttu-id="9f765-113">用于筛选数据的采用 ISO8601 格式的日期。</span><span class="sxs-lookup"><span data-stu-id="9f765-113">The date in ISO8601 format used to filter data.</span></span>|
|<span data-ttu-id="9f765-114">specificity</span><span class="sxs-lookup"><span data-stu-id="9f765-114">specificity</span></span>|<span data-ttu-id="9f765-115">string</span><span class="sxs-lookup"><span data-stu-id="9f765-115">string</span></span>|<span data-ttu-id="9f765-p102">用于保留数据的日期的具体程度。例如，如果日期是 2005-04-02 并将特殊性设置为“月”，则筛选操作将保留包含 2009 年 4 月日期的所有行。可能的值是：`Year`、`Monday`、`Day`、`Hour`、`Minute`、`Second`。</span><span class="sxs-lookup"><span data-stu-id="9f765-p102">How specific the date should be used to keep data. For example, if the date is 2005-04-02 and the specifity is set to "month", the filter operation will keep all rows with a date in the month of april 2009. Possible values are: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f765-119">Relationships</span><span class="sxs-lookup"><span data-stu-id="9f765-119">Relationships</span></span>
<span data-ttu-id="9f765-120">无</span><span class="sxs-lookup"><span data-stu-id="9f765-120">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9f765-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9f765-121">JSON representation</span></span>

<span data-ttu-id="9f765-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9f765-122">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "FilterDatetime resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
