---
title: timeSlot 资源类型
description: 时间段。
localization_priority: Normal
ms.openlocfilehash: 9a2469447bbf0fbb059b41f9bf2b546c341f9190
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517762"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="cfcb8-103">timeSlot 资源类型</span><span class="sxs-lookup"><span data-stu-id="cfcb8-103">timeSlot resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfcb8-104">时间段。</span><span class="sxs-lookup"><span data-stu-id="cfcb8-104">A time period.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cfcb8-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cfcb8-105">JSON representation</span></span>

<span data-ttu-id="cfcb8-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cfcb8-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeSlot"
}-->

```json
{
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```
## <a name="properties"></a><span data-ttu-id="cfcb8-107">属性</span><span class="sxs-lookup"><span data-stu-id="cfcb8-107">Properties</span></span>
| <span data-ttu-id="cfcb8-108">属性</span><span class="sxs-lookup"><span data-stu-id="cfcb8-108">Property</span></span>     | <span data-ttu-id="cfcb8-109">类型</span><span class="sxs-lookup"><span data-stu-id="cfcb8-109">Type</span></span>   |<span data-ttu-id="cfcb8-110">说明</span><span class="sxs-lookup"><span data-stu-id="cfcb8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cfcb8-111">end</span><span class="sxs-lookup"><span data-stu-id="cfcb8-111">end</span></span>|[<span data-ttu-id="cfcb8-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="cfcb8-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="cfcb8-113">时间段的开始时间。</span><span class="sxs-lookup"><span data-stu-id="cfcb8-113">The time a period begins.</span></span>|
|<span data-ttu-id="cfcb8-114">start</span><span class="sxs-lookup"><span data-stu-id="cfcb8-114">start</span></span>|[<span data-ttu-id="cfcb8-115">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="cfcb8-115">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="cfcb8-116">时间段的结束时间。</span><span class="sxs-lookup"><span data-stu-id="cfcb8-116">The time the period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timeslot.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
