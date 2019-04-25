---
title: bookingWorkTimeSlot 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: a193843617d5acc7e18d8a06993a1629b80762be
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543708"
---
# <a name="bookingworktimeslot-resource-type"></a><span data-ttu-id="57abe-104">bookingWorkTimeSlot 资源类型</span><span class="sxs-lookup"><span data-stu-id="57abe-104">bookingWorkTimeSlot resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="57abe-105">工作的开始和结束时间。</span><span class="sxs-lookup"><span data-stu-id="57abe-105">The start and end times for work.</span></span>


## <a name="properties"></a><span data-ttu-id="57abe-106">属性</span><span class="sxs-lookup"><span data-stu-id="57abe-106">Properties</span></span>
| <span data-ttu-id="57abe-107">属性</span><span class="sxs-lookup"><span data-stu-id="57abe-107">Property</span></span>     | <span data-ttu-id="57abe-108">类型</span><span class="sxs-lookup"><span data-stu-id="57abe-108">Type</span></span>   |<span data-ttu-id="57abe-109">说明</span><span class="sxs-lookup"><span data-stu-id="57abe-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="57abe-110">end</span><span class="sxs-lookup"><span data-stu-id="57abe-110">end</span></span>|<span data-ttu-id="57abe-111">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="57abe-111">TimeOfDay</span></span>|<span data-ttu-id="57abe-112">一天中开始工作的时间。</span><span class="sxs-lookup"><span data-stu-id="57abe-112">The time of the day that work starts.</span></span> <span data-ttu-id="57abe-113">例如, 08:00: 00.0000000。</span><span class="sxs-lookup"><span data-stu-id="57abe-113">For example, 08:00:00.0000000.</span></span>|
|<span data-ttu-id="57abe-114">start</span><span class="sxs-lookup"><span data-stu-id="57abe-114">start</span></span>|<span data-ttu-id="57abe-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="57abe-115">TimeOfDay</span></span>|<span data-ttu-id="57abe-116">一天中停止工作的时间。</span><span class="sxs-lookup"><span data-stu-id="57abe-116">The time of the day that work stops.</span></span> <span data-ttu-id="57abe-117">例如, 17:00: 00.0000000。</span><span class="sxs-lookup"><span data-stu-id="57abe-117">For example, 17:00:00.0000000.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="57abe-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="57abe-118">JSON representation</span></span>

<span data-ttu-id="57abe-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="57abe-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingWorkTimeSlot"
}-->

```json
{
  "end": "String (timestamp)",
  "start": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingWorkTimeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingworktimeslot.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
