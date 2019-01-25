---
title: bookingSchedulingPolicy 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 3dee3314818d46c4131526dc92565eb4f8ca6ea2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523447"
---
# <a name="bookingschedulingpolicy-resource-type"></a><span data-ttu-id="1e06e-104">bookingSchedulingPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="1e06e-104">bookingSchedulingPolicy resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="1e06e-105">代表确定应如何在 Microsoft 预订日历中创建约会的策略的组。</span><span class="sxs-lookup"><span data-stu-id="1e06e-105">Represents the set of policies that determine how appointments should be created in a Microsoft Bookings calendar.</span></span>

## <a name="properties"></a><span data-ttu-id="1e06e-106">属性</span><span class="sxs-lookup"><span data-stu-id="1e06e-106">Properties</span></span>
| <span data-ttu-id="1e06e-107">属性</span><span class="sxs-lookup"><span data-stu-id="1e06e-107">Property</span></span>     | <span data-ttu-id="1e06e-108">类型</span><span class="sxs-lookup"><span data-stu-id="1e06e-108">Type</span></span>   |<span data-ttu-id="1e06e-109">说明</span><span class="sxs-lookup"><span data-stu-id="1e06e-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e06e-110">allowStaffSelection</span><span class="sxs-lookup"><span data-stu-id="1e06e-110">allowStaffSelection</span></span>|<span data-ttu-id="1e06e-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e06e-111">Boolean</span></span>|<span data-ttu-id="1e06e-112">True 如果以使客户能够选择特定预定的人员。</span><span class="sxs-lookup"><span data-stu-id="1e06e-112">True if to allow customers to choose a specific person for the booking.</span></span>|
|<span data-ttu-id="1e06e-113">maximumAdvance</span><span class="sxs-lookup"><span data-stu-id="1e06e-113">maximumAdvance</span></span>|<span data-ttu-id="1e06e-114">持续时间</span><span class="sxs-lookup"><span data-stu-id="1e06e-114">Duration</span></span>|<span data-ttu-id="1e06e-115">最大天数提前所能进行预订。</span><span class="sxs-lookup"><span data-stu-id="1e06e-115">Maximum number of days in advance that a booking can be made.</span></span> <span data-ttu-id="1e06e-116">遵循[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式。</span><span class="sxs-lookup"><span data-stu-id="1e06e-116">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="1e06e-117">minimumLeadTime</span><span class="sxs-lookup"><span data-stu-id="1e06e-117">minimumLeadTime</span></span>|<span data-ttu-id="1e06e-118">持续时间</span><span class="sxs-lookup"><span data-stu-id="1e06e-118">Duration</span></span>|<span data-ttu-id="1e06e-119">最小在其前面预订和取消通知必须进行的时间量。</span><span class="sxs-lookup"><span data-stu-id="1e06e-119">The minimum amount of time before which bookings and cancellations must be made.</span></span> <span data-ttu-id="1e06e-120">遵循[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式。</span><span class="sxs-lookup"><span data-stu-id="1e06e-120">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="1e06e-121">sendConfirmationsToOwner</span><span class="sxs-lookup"><span data-stu-id="1e06e-121">sendConfirmationsToOwner</span></span>|<span data-ttu-id="1e06e-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e06e-122">Boolean</span></span>| <span data-ttu-id="1e06e-123">预定会创建或更改时通知通过电子邮件的业务，则为 true。</span><span class="sxs-lookup"><span data-stu-id="1e06e-123">True to notify the business via email when a booking is created or changed.</span></span> <span data-ttu-id="1e06e-124">使用业务**bookingBusiness**实体的**email**属性中指定的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="1e06e-124">Use the email address specified in the **email** property of the **bookingBusiness** entity for the business.</span></span> |
|<span data-ttu-id="1e06e-125">timeSlotInterval</span><span class="sxs-lookup"><span data-stu-id="1e06e-125">timeSlotInterval</span></span>|<span data-ttu-id="1e06e-126">持续时间</span><span class="sxs-lookup"><span data-stu-id="1e06e-126">Duration</span></span>|<span data-ttu-id="1e06e-127">[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式中每个时间段的持续时间。</span><span class="sxs-lookup"><span data-stu-id="1e06e-127">Duration of each time slot, denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1e06e-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1e06e-128">JSON representation</span></span>

<span data-ttu-id="1e06e-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1e06e-129">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingschedulingpolicy.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
