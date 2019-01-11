---
title: FilterDatetime 资源类型
description: 表示在筛选值时如何筛选日期。
localization_priority: Normal
ms.openlocfilehash: 26d42b45a2e9b9cdd279f33330a877a64ea1c8d0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840360"
---
# <a name="filterdatetime-resource-type"></a><span data-ttu-id="47d81-103">FilterDatetime 资源类型</span><span class="sxs-lookup"><span data-stu-id="47d81-103">FilterDatetime resource type</span></span>

<span data-ttu-id="47d81-104">表示在筛选值时如何筛选日期。</span><span class="sxs-lookup"><span data-stu-id="47d81-104">Represents how to filter a date when filtering on values.</span></span>

## <a name="properties"></a><span data-ttu-id="47d81-105">属性</span><span class="sxs-lookup"><span data-stu-id="47d81-105">Properties</span></span>
| <span data-ttu-id="47d81-106">属性</span><span class="sxs-lookup"><span data-stu-id="47d81-106">Property</span></span>     | <span data-ttu-id="47d81-107">类型</span><span class="sxs-lookup"><span data-stu-id="47d81-107">Type</span></span>   |<span data-ttu-id="47d81-108">说明</span><span class="sxs-lookup"><span data-stu-id="47d81-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47d81-109">date</span><span class="sxs-lookup"><span data-stu-id="47d81-109">date</span></span>|<span data-ttu-id="47d81-110">string</span><span class="sxs-lookup"><span data-stu-id="47d81-110">string</span></span>|<span data-ttu-id="47d81-111">用于筛选数据的采用 ISO8601 格式的日期。</span><span class="sxs-lookup"><span data-stu-id="47d81-111">The date in ISO8601 format used to filter data.</span></span>|
|<span data-ttu-id="47d81-112">specificity</span><span class="sxs-lookup"><span data-stu-id="47d81-112">specificity</span></span>|<span data-ttu-id="47d81-113">string</span><span class="sxs-lookup"><span data-stu-id="47d81-113">string</span></span>|<span data-ttu-id="47d81-114">如何特定日期应该用于保留数据。</span><span class="sxs-lookup"><span data-stu-id="47d81-114">How specific the date should be used to keep data.</span></span> <span data-ttu-id="47d81-115">例如，如果日期是 2005年-04-02 并且 specifity 设置为"月"，则筛选器操作将在举行的 2009 年 4 月保留具有日期的所有行。</span><span class="sxs-lookup"><span data-stu-id="47d81-115">For example, if the date is 2005-04-02 and the specifity is set to "month", the filter operation will keep all rows with a date in the month of april 2009.</span></span> <span data-ttu-id="47d81-116">可能的值为： `Year`， `Monday`， `Day`， `Hour`， `Minute`， `Second`。</span><span class="sxs-lookup"><span data-stu-id="47d81-116">The possible values are: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="47d81-117">Relationships</span><span class="sxs-lookup"><span data-stu-id="47d81-117">Relationships</span></span>
<span data-ttu-id="47d81-118">无</span><span class="sxs-lookup"><span data-stu-id="47d81-118">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="47d81-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="47d81-119">JSON representation</span></span>

<span data-ttu-id="47d81-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="47d81-120">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilterDateTime"
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
