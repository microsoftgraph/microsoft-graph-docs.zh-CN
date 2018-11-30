---
title: customTimeZone 资源类型
description: 表示从标准时间到夏令时的切换不标准（反之亦然）的时区。
ms.openlocfilehash: 83375c96e4247cb0ddf2d17b1bede2c295f0b27f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041582"
---
# <a name="customtimezone-resource-type"></a><span data-ttu-id="fec38-103">customTimeZone 资源类型</span><span class="sxs-lookup"><span data-stu-id="fec38-103">customTimeZone resource type</span></span>

> <span data-ttu-id="fec38-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fec38-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fec38-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fec38-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fec38-106">表示从标准时间到夏令时的切换不标准（反之亦然）的时区。</span><span class="sxs-lookup"><span data-stu-id="fec38-106">Represents a time zone where the transition from standard to daylight saving time, or vice versa is not standard.</span></span>


## <a name="properties"></a><span data-ttu-id="fec38-107">属性</span><span class="sxs-lookup"><span data-stu-id="fec38-107">Properties</span></span>
| <span data-ttu-id="fec38-108">属性</span><span class="sxs-lookup"><span data-stu-id="fec38-108">Property</span></span>     | <span data-ttu-id="fec38-109">类型</span><span class="sxs-lookup"><span data-stu-id="fec38-109">Type</span></span>   |<span data-ttu-id="fec38-110">说明</span><span class="sxs-lookup"><span data-stu-id="fec38-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fec38-111">bias</span><span class="sxs-lookup"><span data-stu-id="fec38-111">bias</span></span> | <span data-ttu-id="fec38-112">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="fec38-112">Edm.Int32</span></span> | <span data-ttu-id="fec38-113">时区与协调世界时 (UTC) 的时间偏移量。</span><span class="sxs-lookup"><span data-stu-id="fec38-113">The time offset of the time zone from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="fec38-114">此值以分钟为单位。</span><span class="sxs-lookup"><span data-stu-id="fec38-114">This value is in minutes.</span></span><span data-ttu-id="fec38-115">早于 UTC 的时区为正偏移；晚于 UTC 的时区为负偏移。</span><span class="sxs-lookup"><span data-stu-id="fec38-115"> Time zones that are ahead of UTC have a positive offset; time zones that are behind UTC have a negative offset.</span></span>|
| <span data-ttu-id="fec38-116">daylightOffset</span><span class="sxs-lookup"><span data-stu-id="fec38-116">daylightOffset</span></span> | [<span data-ttu-id="fec38-117">daylightTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="fec38-117">daylightTimeZoneOffset</span></span>](daylighttimezoneoffset.md) | <span data-ttu-id="fec38-118">指定时区何时从标准时间切换到夏令时。</span><span class="sxs-lookup"><span data-stu-id="fec38-118">Specifies when the time zone switches from standard time to daylight saving time.</span></span> |
| <span data-ttu-id="fec38-119">name</span><span class="sxs-lookup"><span data-stu-id="fec38-119">name</span></span> | <span data-ttu-id="fec38-120">string</span><span class="sxs-lookup"><span data-stu-id="fec38-120">string</span></span> | <span data-ttu-id="fec38-121">自定义时区的名称。</span><span class="sxs-lookup"><span data-stu-id="fec38-121">The name of the custom time zone.</span></span> |
| <span data-ttu-id="fec38-122">standardOffset</span><span class="sxs-lookup"><span data-stu-id="fec38-122">standardOffset</span></span> | [<span data-ttu-id="fec38-123">standardTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="fec38-123">standardTimeZoneOffset</span></span>](standardtimezoneoffset.md) | <span data-ttu-id="fec38-124">指定时区何时从夏令时切换到标准时间。</span><span class="sxs-lookup"><span data-stu-id="fec38-124">Specifies when the time zone switches from daylight saving time to standard time.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="fec38-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fec38-125">JSON representation</span></span>

<span data-ttu-id="fec38-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fec38-126">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "customTimeZone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->