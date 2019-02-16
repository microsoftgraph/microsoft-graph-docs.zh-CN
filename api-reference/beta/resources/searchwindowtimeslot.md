---
title: searchWindowTimeSlot 资源类型
description: 时间段。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 393e6a87f35f4ea6da5e7c4a4ccf37f52d90a8de
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057348"
---
# <a name="searchwindowtimeslot-resource-type"></a><span data-ttu-id="c8751-103">searchWindowTimeSlot 资源类型</span><span class="sxs-lookup"><span data-stu-id="c8751-103">searchWindowTimeSlot resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8751-104">要在其中进行搜索的时间段。</span><span class="sxs-lookup"><span data-stu-id="c8751-104">A time period to search within.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8751-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c8751-105">JSON representation</span></span>

<span data-ttu-id="c8751-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c8751-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchWindowTimeSlot"
}-->

```json
{
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```
## <a name="properties"></a><span data-ttu-id="c8751-107">属性</span><span class="sxs-lookup"><span data-stu-id="c8751-107">Properties</span></span>
| <span data-ttu-id="c8751-108">属性</span><span class="sxs-lookup"><span data-stu-id="c8751-108">Property</span></span>     | <span data-ttu-id="c8751-109">类型</span><span class="sxs-lookup"><span data-stu-id="c8751-109">Type</span></span>   |<span data-ttu-id="c8751-110">说明</span><span class="sxs-lookup"><span data-stu-id="c8751-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c8751-111">end</span><span class="sxs-lookup"><span data-stu-id="c8751-111">end</span></span>|[<span data-ttu-id="c8751-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="c8751-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="c8751-113">时间段开始的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="c8751-113">The date, time, and time zone that a period begins.</span></span> |
|<span data-ttu-id="c8751-114">start</span><span class="sxs-lookup"><span data-stu-id="c8751-114">start</span></span>|[<span data-ttu-id="c8751-115">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="c8751-115">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="c8751-116">时间段结束的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="c8751-116">The date, time, and time zone that a period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "searchWindowTimeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/searchwindowtimeslot.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->