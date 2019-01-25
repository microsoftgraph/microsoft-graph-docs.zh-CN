---
title: standardTimeZoneOffset 资源类型
description: 指定时区何时从夏令时切换到标准时间。
localization_priority: Normal
ms.openlocfilehash: cc3de9a0977caf6c222291fdff2b4e0f96a9d9e5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514479"
---
# <a name="standardtimezoneoffset-resource-type"></a><span data-ttu-id="0b503-103">standardTimeZoneOffset 资源类型</span><span class="sxs-lookup"><span data-stu-id="0b503-103">standardTimeZoneOffset resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b503-104">指定时区何时从夏令时切换到标准时间。</span><span class="sxs-lookup"><span data-stu-id="0b503-104">Specifies when a time zone switches from daylight saving time to standard time.</span></span>

<span data-ttu-id="0b503-105">例如，如果为一个时区指定了以下属性：</span><span class="sxs-lookup"><span data-stu-id="0b503-105">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="0b503-106">**dayOccurrence** 为 3</span><span class="sxs-lookup"><span data-stu-id="0b503-106">**dayOccurrence** is 3</span></span>
- <span data-ttu-id="0b503-107">**dayOfWeek** 为“Sunday”</span><span class="sxs-lookup"><span data-stu-id="0b503-107">**dayOfWeek** is "Sunday"</span></span>
- <span data-ttu-id="0b503-108">**month** 为 10</span><span class="sxs-lookup"><span data-stu-id="0b503-108">**month** is 10</span></span>
- <span data-ttu-id="0b503-109">**time** 为 02:00:00 _ **year** 为 0，这意味着从夏令时切换到标准时间出现在每年十月第三个星期日的早上 2 点。</span><span class="sxs-lookup"><span data-stu-id="0b503-109">**time** is 02:00:00 _ **year** is 0 That means the transition from daylight saving time to standard occurs at 2 AM on the third Sunday of October, every year.</span></span>

## <a name="properties"></a><span data-ttu-id="0b503-110">属性</span><span class="sxs-lookup"><span data-stu-id="0b503-110">Properties</span></span>
| <span data-ttu-id="0b503-111">属性</span><span class="sxs-lookup"><span data-stu-id="0b503-111">Property</span></span>     | <span data-ttu-id="0b503-112">类型</span><span class="sxs-lookup"><span data-stu-id="0b503-112">Type</span></span>   |<span data-ttu-id="0b503-113">说明</span><span class="sxs-lookup"><span data-stu-id="0b503-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0b503-114">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="0b503-114">dayOccurrence</span></span> | <span data-ttu-id="0b503-115">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="0b503-115">Edm.Int32</span></span> | <span data-ttu-id="0b503-116">表示从夏令时到标准时间的切换在一周的具体某天出现的次数。</span><span class="sxs-lookup"><span data-stu-id="0b503-116">Represents the nth occurrence of the day of week that the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="0b503-117">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="0b503-117">dayOfWeek</span></span> | <span data-ttu-id="0b503-118">string</span><span class="sxs-lookup"><span data-stu-id="0b503-118">string</span></span> | <span data-ttu-id="0b503-119">表示从夏令时切换为标准时间时一周的具体某日。</span><span class="sxs-lookup"><span data-stu-id="0b503-119">Represents the day of the week when the transition from daylight saving time to standard time.</span></span> |
| <span data-ttu-id="0b503-120">month</span><span class="sxs-lookup"><span data-stu-id="0b503-120">month</span></span> | <span data-ttu-id="0b503-121">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="0b503-121">Edm.Int32</span></span> | <span data-ttu-id="0b503-122">表示从夏令时到标准时间的切换出现时一年的具体月份。</span><span class="sxs-lookup"><span data-stu-id="0b503-122">Represents the month of the year when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="0b503-123">time</span><span class="sxs-lookup"><span data-stu-id="0b503-123">time</span></span> | <span data-ttu-id="0b503-124">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="0b503-124">Edm.TimeOfDay</span></span> | <span data-ttu-id="0b503-125">表示从夏令时到标准时间的切换出现时某日的具体时间。</span><span class="sxs-lookup"><span data-stu-id="0b503-125">Represents the time of day when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="0b503-126">year</span><span class="sxs-lookup"><span data-stu-id="0b503-126">year</span></span> | <span data-ttu-id="0b503-127">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="0b503-127">Edm.Int32</span></span> | <span data-ttu-id="0b503-128">表示从夏令时到标准时间的变更出现时的年度频率。</span><span class="sxs-lookup"><span data-stu-id="0b503-128">Represents how frequently in terms of years the change from daylight saving time to standard time occurs.</span></span> <span data-ttu-id="0b503-129">例如，值为 0 意味着每年。</span><span class="sxs-lookup"><span data-stu-id="0b503-129">For example, a value of 0 means every year.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="0b503-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0b503-130">JSON representation</span></span>

<span data-ttu-id="0b503-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b503-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.standardTimeZoneOffset"
}-->

```json
{
  "dayOccurrence": "Int32",
  "dayOfWeek": "string",
  "month": "Int32",
  "time": "TimeOfDay",
  "year": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "standardTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/standardtimezoneoffset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
