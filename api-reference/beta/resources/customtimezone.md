---
title: customTimeZone 资源类型
description: 表示从标准时间到夏令时的切换不标准（反之亦然）的时区。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 40ab8318931f720780ef21ae6b1c455fc6125814
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507315"
---
# <a name="customtimezone-resource-type"></a><span data-ttu-id="f6967-103">customTimeZone 资源类型</span><span class="sxs-lookup"><span data-stu-id="f6967-103">customTimeZone resource type</span></span>

<span data-ttu-id="f6967-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f6967-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6967-105">表示从标准时间到夏令时的切换不标准（反之亦然）的时区。</span><span class="sxs-lookup"><span data-stu-id="f6967-105">Represents a time zone where the transition from standard to daylight saving time, or vice versa is not standard.</span></span>


## <a name="properties"></a><span data-ttu-id="f6967-106">属性</span><span class="sxs-lookup"><span data-stu-id="f6967-106">Properties</span></span>
| <span data-ttu-id="f6967-107">属性</span><span class="sxs-lookup"><span data-stu-id="f6967-107">Property</span></span>     | <span data-ttu-id="f6967-108">类型</span><span class="sxs-lookup"><span data-stu-id="f6967-108">Type</span></span>   |<span data-ttu-id="f6967-109">说明</span><span class="sxs-lookup"><span data-stu-id="f6967-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f6967-110">bias</span><span class="sxs-lookup"><span data-stu-id="f6967-110">bias</span></span> | <span data-ttu-id="f6967-111">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="f6967-111">Edm.Int32</span></span> | <span data-ttu-id="f6967-112">时区与协调世界时 (UTC) 的时间偏移量。</span><span class="sxs-lookup"><span data-stu-id="f6967-112">The time offset of the time zone from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="f6967-113">此值以分钟为单位。</span><span class="sxs-lookup"><span data-stu-id="f6967-113">This value is in minutes.</span></span><span data-ttu-id="f6967-114">早于 UTC 的时区为正偏移；晚于 UTC 的时区为负偏移。</span><span class="sxs-lookup"><span data-stu-id="f6967-114"> Time zones that are ahead of UTC have a positive offset; time zones that are behind UTC have a negative offset.</span></span>|
| <span data-ttu-id="f6967-115">daylightOffset</span><span class="sxs-lookup"><span data-stu-id="f6967-115">daylightOffset</span></span> | [<span data-ttu-id="f6967-116">daylightTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="f6967-116">daylightTimeZoneOffset</span></span>](daylighttimezoneoffset.md) | <span data-ttu-id="f6967-117">指定时区何时从标准时间切换到夏令时。</span><span class="sxs-lookup"><span data-stu-id="f6967-117">Specifies when the time zone switches from standard time to daylight saving time.</span></span> |
| <span data-ttu-id="f6967-118">name</span><span class="sxs-lookup"><span data-stu-id="f6967-118">name</span></span> | <span data-ttu-id="f6967-119">string</span><span class="sxs-lookup"><span data-stu-id="f6967-119">string</span></span> | <span data-ttu-id="f6967-120">自定义时区的名称。</span><span class="sxs-lookup"><span data-stu-id="f6967-120">The name of the custom time zone.</span></span> |
| <span data-ttu-id="f6967-121">standardOffset</span><span class="sxs-lookup"><span data-stu-id="f6967-121">standardOffset</span></span> | [<span data-ttu-id="f6967-122">standardTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="f6967-122">standardTimeZoneOffset</span></span>](standardtimezoneoffset.md) | <span data-ttu-id="f6967-123">指定时区何时从夏令时切换到标准时间。</span><span class="sxs-lookup"><span data-stu-id="f6967-123">Specifies when the time zone switches from daylight saving time to standard time.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="f6967-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f6967-124">JSON representation</span></span>

<span data-ttu-id="f6967-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f6967-125">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.customTimeZone"
}-->

```json
{
  "bias": "Int32",
  "daylightOffset": {"@odata.type": "microsoft.graph.daylightTimeZoneOffset"},
  "name": "string",
  "standardOffset": {"@odata.type": "microsoft.graph.standardTimeZoneOffset"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "customTimeZone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
