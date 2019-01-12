---
title: bookingWorkTimeSlot 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 33dd856d678d2cf1ba9da2a747c0bd46f2fd4932
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968482"
---
# <a name="bookingworktimeslot-resource-type"></a><span data-ttu-id="37f98-104">bookingWorkTimeSlot 资源类型</span><span class="sxs-lookup"><span data-stu-id="37f98-104">bookingWorkTimeSlot resource type</span></span>

 > <span data-ttu-id="37f98-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="37f98-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="37f98-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="37f98-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="37f98-107">用于开始和结束时间。</span><span class="sxs-lookup"><span data-stu-id="37f98-107">The start and end times for work.</span></span>


## <a name="properties"></a><span data-ttu-id="37f98-108">属性</span><span class="sxs-lookup"><span data-stu-id="37f98-108">Properties</span></span>
| <span data-ttu-id="37f98-109">属性</span><span class="sxs-lookup"><span data-stu-id="37f98-109">Property</span></span>     | <span data-ttu-id="37f98-110">类型</span><span class="sxs-lookup"><span data-stu-id="37f98-110">Type</span></span>   |<span data-ttu-id="37f98-111">说明</span><span class="sxs-lookup"><span data-stu-id="37f98-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37f98-112">end</span><span class="sxs-lookup"><span data-stu-id="37f98-112">end</span></span>|<span data-ttu-id="37f98-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="37f98-113">TimeOfDay</span></span>|<span data-ttu-id="37f98-114">工作开始的时间。</span><span class="sxs-lookup"><span data-stu-id="37f98-114">The time of the day that work starts.</span></span> <span data-ttu-id="37f98-115">例如，08:00:00.0000000。</span><span class="sxs-lookup"><span data-stu-id="37f98-115">For example, 08:00:00.0000000.</span></span>|
|<span data-ttu-id="37f98-116">start</span><span class="sxs-lookup"><span data-stu-id="37f98-116">start</span></span>|<span data-ttu-id="37f98-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="37f98-117">TimeOfDay</span></span>|<span data-ttu-id="37f98-118">工作停止的时间。</span><span class="sxs-lookup"><span data-stu-id="37f98-118">The time of the day that work stops.</span></span> <span data-ttu-id="37f98-119">例如，17:00:00.0000000。</span><span class="sxs-lookup"><span data-stu-id="37f98-119">For example, 17:00:00.0000000.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="37f98-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="37f98-120">JSON representation</span></span>

<span data-ttu-id="37f98-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="37f98-121">The following is a JSON representation of the resource.</span></span>

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
