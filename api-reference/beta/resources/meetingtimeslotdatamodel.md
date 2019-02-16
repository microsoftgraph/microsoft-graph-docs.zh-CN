---
title: meetingTimeSlotDataModel 资源类型
description: 时间段。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: acbd08da5e15dd733c63c0141db5b58cee896666
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057342"
---
# <a name="meetingtimeslotdatamodel-resource-type"></a><span data-ttu-id="b41c8-103">meetingTimeSlotDataModel 资源类型</span><span class="sxs-lookup"><span data-stu-id="b41c8-103">meetingTimeSlotDataModel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b41c8-104">表示会议的时间段。</span><span class="sxs-lookup"><span data-stu-id="b41c8-104">Represents a time slot for a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b41c8-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b41c8-105">JSON representation</span></span>

<span data-ttu-id="b41c8-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b41c8-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeSlotDataModel"
}-->

```json
{
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```
## <a name="properties"></a><span data-ttu-id="b41c8-107">属性</span><span class="sxs-lookup"><span data-stu-id="b41c8-107">Properties</span></span>
| <span data-ttu-id="b41c8-108">属性</span><span class="sxs-lookup"><span data-stu-id="b41c8-108">Property</span></span>     | <span data-ttu-id="b41c8-109">类型</span><span class="sxs-lookup"><span data-stu-id="b41c8-109">Type</span></span>   |<span data-ttu-id="b41c8-110">说明</span><span class="sxs-lookup"><span data-stu-id="b41c8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b41c8-111">end</span><span class="sxs-lookup"><span data-stu-id="b41c8-111">end</span></span>|[<span data-ttu-id="b41c8-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="b41c8-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="b41c8-113">时间段开始的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="b41c8-113">The date, time, and time zone that a period begins.</span></span> |
|<span data-ttu-id="b41c8-114">start</span><span class="sxs-lookup"><span data-stu-id="b41c8-114">start</span></span>|[<span data-ttu-id="b41c8-115">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="b41c8-115">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="b41c8-116">时间段结束的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="b41c8-116">The date, time, and time zone that a period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingTimeSlotDataModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/meetingtimeslotdatamodel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->