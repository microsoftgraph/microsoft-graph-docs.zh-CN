---
title: bookingSchedulingPolicy 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 039d76b00787c9bf2e4f0bee4eb927a7628a9e76
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914635"
---
# <a name="bookingschedulingpolicy-resource-type"></a><span data-ttu-id="ea984-104">bookingSchedulingPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="ea984-104">bookingSchedulingPolicy resource type</span></span>

 > <span data-ttu-id="ea984-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ea984-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ea984-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ea984-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="ea984-107">代表确定应如何在 Microsoft 预订日历中创建约会的策略的组。</span><span class="sxs-lookup"><span data-stu-id="ea984-107">Represents the set of policies that determine how appointments should be created in a Microsoft Bookings calendar.</span></span>

## <a name="properties"></a><span data-ttu-id="ea984-108">属性</span><span class="sxs-lookup"><span data-stu-id="ea984-108">Properties</span></span>
| <span data-ttu-id="ea984-109">属性</span><span class="sxs-lookup"><span data-stu-id="ea984-109">Property</span></span>     | <span data-ttu-id="ea984-110">类型</span><span class="sxs-lookup"><span data-stu-id="ea984-110">Type</span></span>   |<span data-ttu-id="ea984-111">Description</span><span class="sxs-lookup"><span data-stu-id="ea984-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea984-112">allowStaffSelection</span><span class="sxs-lookup"><span data-stu-id="ea984-112">allowStaffSelection</span></span>|<span data-ttu-id="ea984-113">布尔</span><span class="sxs-lookup"><span data-stu-id="ea984-113">Boolean</span></span>|<span data-ttu-id="ea984-114">True 如果以使客户能够选择特定预定的人员。</span><span class="sxs-lookup"><span data-stu-id="ea984-114">True if to allow customers to choose a specific person for the booking.</span></span>|
|<span data-ttu-id="ea984-115">maximumAdvance</span><span class="sxs-lookup"><span data-stu-id="ea984-115">maximumAdvance</span></span>|<span data-ttu-id="ea984-116">Duration</span><span class="sxs-lookup"><span data-stu-id="ea984-116">Duration</span></span>|<span data-ttu-id="ea984-117">最大天数提前所能进行预订。</span><span class="sxs-lookup"><span data-stu-id="ea984-117">Maximum number of days in advance that a booking can be made.</span></span> <span data-ttu-id="ea984-118">遵循[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式。</span><span class="sxs-lookup"><span data-stu-id="ea984-118">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="ea984-119">minimumLeadTime</span><span class="sxs-lookup"><span data-stu-id="ea984-119">minimumLeadTime</span></span>|<span data-ttu-id="ea984-120">Duration</span><span class="sxs-lookup"><span data-stu-id="ea984-120">Duration</span></span>|<span data-ttu-id="ea984-121">最小在其前面预订和取消通知必须进行的时间量。</span><span class="sxs-lookup"><span data-stu-id="ea984-121">The minimum amount of time before which bookings and cancellations must be made.</span></span> <span data-ttu-id="ea984-122">遵循[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式。</span><span class="sxs-lookup"><span data-stu-id="ea984-122">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="ea984-123">sendConfirmationsToOwner</span><span class="sxs-lookup"><span data-stu-id="ea984-123">sendConfirmationsToOwner</span></span>|<span data-ttu-id="ea984-124">布尔</span><span class="sxs-lookup"><span data-stu-id="ea984-124">Boolean</span></span>| <span data-ttu-id="ea984-125">预定会创建或更改时通知通过电子邮件的业务，则为 true。</span><span class="sxs-lookup"><span data-stu-id="ea984-125">True to notify the business via email when a booking is created or changed.</span></span> <span data-ttu-id="ea984-126">使用业务**bookingBusiness**实体的**email**属性中指定的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="ea984-126">Use the email address specified in the **email** property of the **bookingBusiness** entity for the business.</span></span> |
|<span data-ttu-id="ea984-127">timeSlotInterval</span><span class="sxs-lookup"><span data-stu-id="ea984-127">timeSlotInterval</span></span>|<span data-ttu-id="ea984-128">Duration</span><span class="sxs-lookup"><span data-stu-id="ea984-128">Duration</span></span>|<span data-ttu-id="ea984-129">[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式中每个时间段的持续时间。</span><span class="sxs-lookup"><span data-stu-id="ea984-129">Duration of each time slot, denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ea984-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ea984-130">JSON representation</span></span>

<span data-ttu-id="ea984-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ea984-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingSchedulingPolicy"
}-->

```json
{
  "allowStaffSelection": true,
  "maximumAdvance": "String (timestamp)",
  "minimumLeadTime": "String (timestamp)",
  "sendConfirmationsToOwner": true,
  "timeSlotInterval": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingSchedulingPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
