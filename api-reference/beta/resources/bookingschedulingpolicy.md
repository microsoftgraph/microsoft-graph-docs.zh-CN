---
title: bookingSchedulingPolicy 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 3dee3314818d46c4131526dc92565eb4f8ca6ea2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543730"
---
# <a name="bookingschedulingpolicy-resource-type"></a><span data-ttu-id="7b50b-104">bookingSchedulingPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="7b50b-104">bookingSchedulingPolicy resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="7b50b-105">表示一组策略, 这些策略确定应如何在 Microsoft 预定日历中创建约会。</span><span class="sxs-lookup"><span data-stu-id="7b50b-105">Represents the set of policies that determine how appointments should be created in a Microsoft Bookings calendar.</span></span>

## <a name="properties"></a><span data-ttu-id="7b50b-106">属性</span><span class="sxs-lookup"><span data-stu-id="7b50b-106">Properties</span></span>
| <span data-ttu-id="7b50b-107">属性</span><span class="sxs-lookup"><span data-stu-id="7b50b-107">Property</span></span>     | <span data-ttu-id="7b50b-108">类型</span><span class="sxs-lookup"><span data-stu-id="7b50b-108">Type</span></span>   |<span data-ttu-id="7b50b-109">说明</span><span class="sxs-lookup"><span data-stu-id="7b50b-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b50b-110">allowStaffSelection</span><span class="sxs-lookup"><span data-stu-id="7b50b-110">allowStaffSelection</span></span>|<span data-ttu-id="7b50b-111">布尔值</span><span class="sxs-lookup"><span data-stu-id="7b50b-111">Boolean</span></span>|<span data-ttu-id="7b50b-112">如此如果允许客户选择预订的特定人员。</span><span class="sxs-lookup"><span data-stu-id="7b50b-112">True if to allow customers to choose a specific person for the booking.</span></span>|
|<span data-ttu-id="7b50b-113">maximumAdvance</span><span class="sxs-lookup"><span data-stu-id="7b50b-113">maximumAdvance</span></span>|<span data-ttu-id="7b50b-114">持续时间</span><span class="sxs-lookup"><span data-stu-id="7b50b-114">Duration</span></span>|<span data-ttu-id="7b50b-115">可以提前进行预订的最大天数。</span><span class="sxs-lookup"><span data-stu-id="7b50b-115">Maximum number of days in advance that a booking can be made.</span></span> <span data-ttu-id="7b50b-116">它遵循[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式。</span><span class="sxs-lookup"><span data-stu-id="7b50b-116">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="7b50b-117">minimumLeadTime</span><span class="sxs-lookup"><span data-stu-id="7b50b-117">minimumLeadTime</span></span>|<span data-ttu-id="7b50b-118">持续时间</span><span class="sxs-lookup"><span data-stu-id="7b50b-118">Duration</span></span>|<span data-ttu-id="7b50b-119">在必须进行预订和取消的前的最小时间量。</span><span class="sxs-lookup"><span data-stu-id="7b50b-119">The minimum amount of time before which bookings and cancellations must be made.</span></span> <span data-ttu-id="7b50b-120">它遵循[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式。</span><span class="sxs-lookup"><span data-stu-id="7b50b-120">It follows the [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|
|<span data-ttu-id="7b50b-121">sendConfirmationsToOwner</span><span class="sxs-lookup"><span data-stu-id="7b50b-121">sendConfirmationsToOwner</span></span>|<span data-ttu-id="7b50b-122">布尔值</span><span class="sxs-lookup"><span data-stu-id="7b50b-122">Boolean</span></span>| <span data-ttu-id="7b50b-123">真要在创建或更改预订时通过电子邮件通知商业。</span><span class="sxs-lookup"><span data-stu-id="7b50b-123">True to notify the business via email when a booking is created or changed.</span></span> <span data-ttu-id="7b50b-124">使用在企业的**bookingBusiness**实体的**email**属性中指定的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="7b50b-124">Use the email address specified in the **email** property of the **bookingBusiness** entity for the business.</span></span> |
|<span data-ttu-id="7b50b-125">timeSlotInterval</span><span class="sxs-lookup"><span data-stu-id="7b50b-125">timeSlotInterval</span></span>|<span data-ttu-id="7b50b-126">持续时间</span><span class="sxs-lookup"><span data-stu-id="7b50b-126">Duration</span></span>|<span data-ttu-id="7b50b-127">每个时间段的持续时间, 以[ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html)格式表示。</span><span class="sxs-lookup"><span data-stu-id="7b50b-127">Duration of each time slot, denoted in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7b50b-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7b50b-128">JSON representation</span></span>

<span data-ttu-id="7b50b-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7b50b-129">The following is a JSON representation of the resource.</span></span>

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
