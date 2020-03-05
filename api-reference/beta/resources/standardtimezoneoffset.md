---
title: standardTimeZoneOffset 资源类型
description: 指定时区何时从夏令时切换到标准时间。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: a547329bc6f82ec76d0efc44d7a9e1ffb7700389
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520329"
---
# <a name="standardtimezoneoffset-resource-type"></a><span data-ttu-id="94315-103">standardTimeZoneOffset 资源类型</span><span class="sxs-lookup"><span data-stu-id="94315-103">standardTimeZoneOffset resource type</span></span>

<span data-ttu-id="94315-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="94315-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94315-105">指定时区何时从夏令时切换到标准时间。</span><span class="sxs-lookup"><span data-stu-id="94315-105">Specifies when a time zone switches from daylight saving time to standard time.</span></span>

<span data-ttu-id="94315-106">例如，如果为一个时区指定了以下属性：</span><span class="sxs-lookup"><span data-stu-id="94315-106">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="94315-107">**dayOccurrence** 为 3</span><span class="sxs-lookup"><span data-stu-id="94315-107">**dayOccurrence** is 3</span></span>
- <span data-ttu-id="94315-108">**dayOfWeek** 为“Sunday”</span><span class="sxs-lookup"><span data-stu-id="94315-108">**dayOfWeek** is "Sunday"</span></span>
- <span data-ttu-id="94315-109">**month** 为 10</span><span class="sxs-lookup"><span data-stu-id="94315-109">**month** is 10</span></span>
- <span data-ttu-id="94315-110">**time** 为 02:00:00 _ **year** 为 0，这意味着从夏令时切换到标准时间出现在每年十月第三个星期日的早上 2 点。</span><span class="sxs-lookup"><span data-stu-id="94315-110">**time** is 02:00:00 _ **year** is 0 That means the transition from daylight saving time to standard occurs at 2 AM on the third Sunday of October, every year.</span></span>

## <a name="properties"></a><span data-ttu-id="94315-111">属性</span><span class="sxs-lookup"><span data-stu-id="94315-111">Properties</span></span>
| <span data-ttu-id="94315-112">属性</span><span class="sxs-lookup"><span data-stu-id="94315-112">Property</span></span>     | <span data-ttu-id="94315-113">类型</span><span class="sxs-lookup"><span data-stu-id="94315-113">Type</span></span>   |<span data-ttu-id="94315-114">说明</span><span class="sxs-lookup"><span data-stu-id="94315-114">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="94315-115">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="94315-115">dayOccurrence</span></span> | <span data-ttu-id="94315-116">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="94315-116">Edm.Int32</span></span> | <span data-ttu-id="94315-117">表示从夏令时到标准时间的切换在一周的具体某天出现的次数。</span><span class="sxs-lookup"><span data-stu-id="94315-117">Represents the nth occurrence of the day of week that the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="94315-118">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="94315-118">dayOfWeek</span></span> | <span data-ttu-id="94315-119">string</span><span class="sxs-lookup"><span data-stu-id="94315-119">string</span></span> | <span data-ttu-id="94315-120">表示从夏令时切换为标准时间时一周的具体某日。</span><span class="sxs-lookup"><span data-stu-id="94315-120">Represents the day of the week when the transition from daylight saving time to standard time.</span></span> |
| <span data-ttu-id="94315-121">month</span><span class="sxs-lookup"><span data-stu-id="94315-121">month</span></span> | <span data-ttu-id="94315-122">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="94315-122">Edm.Int32</span></span> | <span data-ttu-id="94315-123">表示从夏令时到标准时间的切换出现时一年的具体月份。</span><span class="sxs-lookup"><span data-stu-id="94315-123">Represents the month of the year when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="94315-124">time</span><span class="sxs-lookup"><span data-stu-id="94315-124">time</span></span> | <span data-ttu-id="94315-125">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="94315-125">Edm.TimeOfDay</span></span> | <span data-ttu-id="94315-126">表示从夏令时到标准时间的切换出现时某日的具体时间。</span><span class="sxs-lookup"><span data-stu-id="94315-126">Represents the time of day when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="94315-127">year</span><span class="sxs-lookup"><span data-stu-id="94315-127">year</span></span> | <span data-ttu-id="94315-128">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="94315-128">Edm.Int32</span></span> | <span data-ttu-id="94315-129">表示从夏令时到标准时间的变更出现时的年度频率。</span><span class="sxs-lookup"><span data-stu-id="94315-129">Represents how frequently in terms of years the change from daylight saving time to standard time occurs.</span></span> <span data-ttu-id="94315-130">例如，值为 0 意味着每年。</span><span class="sxs-lookup"><span data-stu-id="94315-130">For example, a value of 0 means every year.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="94315-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="94315-131">JSON representation</span></span>

<span data-ttu-id="94315-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94315-132">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
