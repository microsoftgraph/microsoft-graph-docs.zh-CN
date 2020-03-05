---
title: bookingSchedulingPolicy 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: edc456aaa03cc54bd7b385bc97d37eb657ea53b2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507906"
---
# <a name="bookingschedulingpolicy-resource-type"></a><span data-ttu-id="621e8-104">bookingSchedulingPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="621e8-104">bookingSchedulingPolicy resource type</span></span>

<span data-ttu-id="621e8-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="621e8-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="621e8-106">表示一组策略，这些策略确定应如何在 Microsoft 预定日历中创建约会。</span><span class="sxs-lookup"><span data-stu-id="621e8-106">Represents the set of policies that determine how appointments should be created in a Microsoft Bookings calendar.</span></span>

## <a name="properties"></a><span data-ttu-id="621e8-107">属性</span><span class="sxs-lookup"><span data-stu-id="621e8-107">Properties</span></span>
| <span data-ttu-id="621e8-108">属性</span><span class="sxs-lookup"><span data-stu-id="621e8-108">Property</span></span>     | <span data-ttu-id="621e8-109">类型</span><span class="sxs-lookup"><span data-stu-id="621e8-109">Type</span></span>   |<span data-ttu-id="621e8-110">说明</span><span class="sxs-lookup"><span data-stu-id="621e8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="621e8-111">allowStaffSelection</span><span class="sxs-lookup"><span data-stu-id="621e8-111">allowStaffSelection</span></span>|<span data-ttu-id="621e8-112">布尔</span><span class="sxs-lookup"><span data-stu-id="621e8-112">Boolean</span></span>|<span data-ttu-id="621e8-113">如此如果允许客户选择预订的特定人员。</span><span class="sxs-lookup"><span data-stu-id="621e8-113">True if to allow customers to choose a specific person for the booking.</span></span>|
|<span data-ttu-id="621e8-114">maximumAdvance</span><span class="sxs-lookup"><span data-stu-id="621e8-114">maximumAdvance</span></span>|<span data-ttu-id="621e8-115">持续时间</span><span class="sxs-lookup"><span data-stu-id="621e8-115">Duration</span></span>|<span data-ttu-id="621e8-116">可以提前进行预订的最大天数。</span><span class="sxs-lookup"><span data-stu-id="621e8-116">Maximum number of days in advance that a booking can be made.</span></span> <span data-ttu-id="621e8-117">它遵循[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式。</span><span class="sxs-lookup"><span data-stu-id="621e8-117">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="621e8-118">minimumLeadTime</span><span class="sxs-lookup"><span data-stu-id="621e8-118">minimumLeadTime</span></span>|<span data-ttu-id="621e8-119">持续时间</span><span class="sxs-lookup"><span data-stu-id="621e8-119">Duration</span></span>|<span data-ttu-id="621e8-120">在必须进行预订和取消的前的最小时间量。</span><span class="sxs-lookup"><span data-stu-id="621e8-120">The minimum amount of time before which bookings and cancellations must be made.</span></span> <span data-ttu-id="621e8-121">它遵循[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式。</span><span class="sxs-lookup"><span data-stu-id="621e8-121">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="621e8-122">sendConfirmationsToOwner</span><span class="sxs-lookup"><span data-stu-id="621e8-122">sendConfirmationsToOwner</span></span>|<span data-ttu-id="621e8-123">布尔</span><span class="sxs-lookup"><span data-stu-id="621e8-123">Boolean</span></span>| <span data-ttu-id="621e8-124">真要在创建或更改预订时通过电子邮件通知商业。</span><span class="sxs-lookup"><span data-stu-id="621e8-124">True to notify the business via email when a booking is created or changed.</span></span> <span data-ttu-id="621e8-125">使用在企业的**bookingBusiness**实体的**email**属性中指定的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="621e8-125">Use the email address specified in the **email** property of the **bookingBusiness** entity for the business.</span></span> |
|<span data-ttu-id="621e8-126">timeSlotInterval</span><span class="sxs-lookup"><span data-stu-id="621e8-126">timeSlotInterval</span></span>|<span data-ttu-id="621e8-127">持续时间</span><span class="sxs-lookup"><span data-stu-id="621e8-127">Duration</span></span>|<span data-ttu-id="621e8-128">每个时间段的持续时间，以[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式表示。</span><span class="sxs-lookup"><span data-stu-id="621e8-128">Duration of each time slot, denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="621e8-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="621e8-129">JSON representation</span></span>

<span data-ttu-id="621e8-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="621e8-130">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "bookingSchedulingPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
