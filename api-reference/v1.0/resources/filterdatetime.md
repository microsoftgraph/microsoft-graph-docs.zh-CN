---
title: FilterDatetime 资源类型
description: 表示在筛选值时如何筛选日期。
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: bd8d7c01b94306245708df8290a44ffb936ac4d6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018289"
---
# <a name="filterdatetime-resource-type"></a><span data-ttu-id="a6b91-103">FilterDatetime 资源类型</span><span class="sxs-lookup"><span data-stu-id="a6b91-103">FilterDatetime resource type</span></span>

<span data-ttu-id="a6b91-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6b91-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a6b91-105">表示在筛选值时如何筛选日期。</span><span class="sxs-lookup"><span data-stu-id="a6b91-105">Represents how to filter a date when filtering on values.</span></span>

## <a name="properties"></a><span data-ttu-id="a6b91-106">属性</span><span class="sxs-lookup"><span data-stu-id="a6b91-106">Properties</span></span>
| <span data-ttu-id="a6b91-107">属性</span><span class="sxs-lookup"><span data-stu-id="a6b91-107">Property</span></span>     | <span data-ttu-id="a6b91-108">类型</span><span class="sxs-lookup"><span data-stu-id="a6b91-108">Type</span></span>   |<span data-ttu-id="a6b91-109">说明</span><span class="sxs-lookup"><span data-stu-id="a6b91-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6b91-110">date</span><span class="sxs-lookup"><span data-stu-id="a6b91-110">date</span></span>|<span data-ttu-id="a6b91-111">string</span><span class="sxs-lookup"><span data-stu-id="a6b91-111">string</span></span>|<span data-ttu-id="a6b91-112">用于筛选数据的采用 ISO8601 格式的日期。</span><span class="sxs-lookup"><span data-stu-id="a6b91-112">The date in ISO8601 format used to filter data.</span></span>|
|<span data-ttu-id="a6b91-113">specificity</span><span class="sxs-lookup"><span data-stu-id="a6b91-113">specificity</span></span>|<span data-ttu-id="a6b91-114">string</span><span class="sxs-lookup"><span data-stu-id="a6b91-114">string</span></span>|<span data-ttu-id="a6b91-115">用于保留数据的日期的具体程度。</span><span class="sxs-lookup"><span data-stu-id="a6b91-115">How specific the date should be used to keep data.</span></span> <span data-ttu-id="a6b91-116">例如，如果日期是 2005-04-02 并且将特殊性设置为“月”，则筛选操作将保留包含 2009 年 4 月日期的所有行。</span><span class="sxs-lookup"><span data-stu-id="a6b91-116">For example, if the date is 2005-04-02 and the specifity is set to "month", the filter operation will keep all rows with a date in the month of april 2009.</span></span> <span data-ttu-id="a6b91-117">可能的值包括 `Year`、`Monday`、`Day`、`Hour`、`Minute`、`Second`。</span><span class="sxs-lookup"><span data-stu-id="a6b91-117">The possible values are: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6b91-118">关系</span><span class="sxs-lookup"><span data-stu-id="a6b91-118">Relationships</span></span>
<span data-ttu-id="a6b91-119">无</span><span class="sxs-lookup"><span data-stu-id="a6b91-119">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a6b91-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a6b91-120">JSON representation</span></span>

<span data-ttu-id="a6b91-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a6b91-121">Here is a JSON representation of the resource.</span></span>

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

