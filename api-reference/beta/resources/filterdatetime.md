---
title: FilterDatetime 资源类型
description: 表示在筛选值时如何筛选日期。
localization_priority: Normal
ms.openlocfilehash: ad4341e13eadc911377ec7b9859d6a31305fadf8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506439"
---
# <a name="filterdatetime-resource-type"></a><span data-ttu-id="3dc77-103">FilterDatetime 资源类型</span><span class="sxs-lookup"><span data-stu-id="3dc77-103">FilterDatetime resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3dc77-104">表示在筛选值时如何筛选日期。</span><span class="sxs-lookup"><span data-stu-id="3dc77-104">Represents how to filter a date when filtering on values.</span></span>

## <a name="properties"></a><span data-ttu-id="3dc77-105">属性</span><span class="sxs-lookup"><span data-stu-id="3dc77-105">Properties</span></span>
| <span data-ttu-id="3dc77-106">属性</span><span class="sxs-lookup"><span data-stu-id="3dc77-106">Property</span></span>     | <span data-ttu-id="3dc77-107">类型</span><span class="sxs-lookup"><span data-stu-id="3dc77-107">Type</span></span>   |<span data-ttu-id="3dc77-108">说明</span><span class="sxs-lookup"><span data-stu-id="3dc77-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3dc77-109">date</span><span class="sxs-lookup"><span data-stu-id="3dc77-109">date</span></span>|<span data-ttu-id="3dc77-110">字符串</span><span class="sxs-lookup"><span data-stu-id="3dc77-110">string</span></span>|<span data-ttu-id="3dc77-111">用于筛选数据的采用 ISO8601 格式的日期。</span><span class="sxs-lookup"><span data-stu-id="3dc77-111">The date in ISO8601 format used to filter data.</span></span>|
|<span data-ttu-id="3dc77-112">specificity</span><span class="sxs-lookup"><span data-stu-id="3dc77-112">specificity</span></span>|<span data-ttu-id="3dc77-113">string</span><span class="sxs-lookup"><span data-stu-id="3dc77-113">string</span></span>|<span data-ttu-id="3dc77-p101">用于保留数据的日期的具体程度。例如，如果日期是 2005-04-02 并将特殊性设置为“月”，则筛选操作将保留包含 2009 年 4 月日期的所有行。可能的值是：`Year`、`Monday`、`Day`、`Hour`、`Minute`、`Second`。</span><span class="sxs-lookup"><span data-stu-id="3dc77-p101">How specific the date should be used to keep data. For example, if the date is 2005-04-02 and the specifity is set to "month", the filter operation will keep all rows with a date in the month of april 2009. Possible values are: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3dc77-117">关系</span><span class="sxs-lookup"><span data-stu-id="3dc77-117">Relationships</span></span>
<span data-ttu-id="3dc77-118">无</span><span class="sxs-lookup"><span data-stu-id="3dc77-118">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3dc77-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3dc77-119">JSON representation</span></span>

<span data-ttu-id="3dc77-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3dc77-120">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/filterdatetime.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
