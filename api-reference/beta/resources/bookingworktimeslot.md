---
title: bookingWorkTimeSlot 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: 69a802e4addd3c0cb821a630707a62724ea984a2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839555"
---
# <a name="bookingworktimeslot-resource-type"></a><span data-ttu-id="e0430-104">bookingWorkTimeSlot 资源类型</span><span class="sxs-lookup"><span data-stu-id="e0430-104">bookingWorkTimeSlot resource type</span></span>

 > <span data-ttu-id="e0430-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e0430-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e0430-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e0430-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="e0430-107">用于开始和结束时间。</span><span class="sxs-lookup"><span data-stu-id="e0430-107">The start and end times for work.</span></span>


## <a name="properties"></a><span data-ttu-id="e0430-108">属性</span><span class="sxs-lookup"><span data-stu-id="e0430-108">Properties</span></span>
| <span data-ttu-id="e0430-109">属性</span><span class="sxs-lookup"><span data-stu-id="e0430-109">Property</span></span>     | <span data-ttu-id="e0430-110">类型</span><span class="sxs-lookup"><span data-stu-id="e0430-110">Type</span></span>   |<span data-ttu-id="e0430-111">说明</span><span class="sxs-lookup"><span data-stu-id="e0430-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0430-112">end</span><span class="sxs-lookup"><span data-stu-id="e0430-112">end</span></span>|<span data-ttu-id="e0430-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="e0430-113">TimeOfDay</span></span>|<span data-ttu-id="e0430-114">工作开始的时间。</span><span class="sxs-lookup"><span data-stu-id="e0430-114">The time of the day that work starts.</span></span> <span data-ttu-id="e0430-115">例如，08:00:00.0000000。</span><span class="sxs-lookup"><span data-stu-id="e0430-115">For example, 08:00:00.0000000.</span></span>|
|<span data-ttu-id="e0430-116">start</span><span class="sxs-lookup"><span data-stu-id="e0430-116">start</span></span>|<span data-ttu-id="e0430-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="e0430-117">TimeOfDay</span></span>|<span data-ttu-id="e0430-118">工作停止的时间。</span><span class="sxs-lookup"><span data-stu-id="e0430-118">The time of the day that work stops.</span></span> <span data-ttu-id="e0430-119">例如，17:00:00.0000000。</span><span class="sxs-lookup"><span data-stu-id="e0430-119">For example, 17:00:00.0000000.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e0430-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e0430-120">JSON representation</span></span>

<span data-ttu-id="e0430-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0430-121">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "bookingWorkTimeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
