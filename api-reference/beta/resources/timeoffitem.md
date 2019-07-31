---
title: timeOffItem 资源类型
description: 表示 timeOff 的版本。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 6b240f587e20e2da178f9afa3e8d712cf2ae114d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964303"
---
# <a name="timeoffitem-resource-type"></a><span data-ttu-id="3a5f8-103">timeOffItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="3a5f8-103">timeOffItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a5f8-104">表示[timeOff](timeoff.md)的版本。</span><span class="sxs-lookup"><span data-stu-id="3a5f8-104">Represents a version of the [timeOff](timeoff.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3a5f8-105">属性</span><span class="sxs-lookup"><span data-stu-id="3a5f8-105">Properties</span></span>
| <span data-ttu-id="3a5f8-106">属性</span><span class="sxs-lookup"><span data-stu-id="3a5f8-106">Property</span></span>                         | <span data-ttu-id="3a5f8-107">类型</span><span class="sxs-lookup"><span data-stu-id="3a5f8-107">Type</span></span>                    | <span data-ttu-id="3a5f8-108">说明</span><span class="sxs-lookup"><span data-stu-id="3a5f8-108">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="3a5f8-109">timeOffReasonId</span><span class="sxs-lookup"><span data-stu-id="3a5f8-109">timeOffReasonId</span></span>               | <span data-ttu-id="3a5f8-110">string</span><span class="sxs-lookup"><span data-stu-id="3a5f8-110">string</span></span>                  | <span data-ttu-id="3a5f8-111">`timeOffReason`此`timeOffItem`的的 ID。</span><span class="sxs-lookup"><span data-stu-id="3a5f8-111">ID of the `timeOffReason` for this `timeOffItem`.</span></span> <span data-ttu-id="3a5f8-112">必需。</span><span class="sxs-lookup"><span data-stu-id="3a5f8-112">Required.</span></span>     |
| <span data-ttu-id="3a5f8-113">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3a5f8-113">startDateTime</span></span>               | <span data-ttu-id="3a5f8-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a5f8-114">DateTimeOffset</span></span>                  | <span data-ttu-id="3a5f8-115">的开始日期和时间`timeOffItem`。</span><span class="sxs-lookup"><span data-stu-id="3a5f8-115">The start date and time for the `timeOffItem`.</span></span> <span data-ttu-id="3a5f8-116">必需。</span><span class="sxs-lookup"><span data-stu-id="3a5f8-116">Required.</span></span> <span data-ttu-id="3a5f8-117">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="3a5f8-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3a5f8-118">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="3a5f8-118">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="3a5f8-119">endDateTime</span><span class="sxs-lookup"><span data-stu-id="3a5f8-119">endDateTime</span></span>               | <span data-ttu-id="3a5f8-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a5f8-120">DateTimeOffset</span></span>                  | <span data-ttu-id="3a5f8-121">的结束日期和时间`timeOffItem`。</span><span class="sxs-lookup"><span data-stu-id="3a5f8-121">The end date and time for the `timeOffItem`.</span></span> <span data-ttu-id="3a5f8-122">必需。</span><span class="sxs-lookup"><span data-stu-id="3a5f8-122">Required.</span></span> <span data-ttu-id="3a5f8-123">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="3a5f8-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3a5f8-124">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="3a5f8-124">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="3a5f8-125">theme</span><span class="sxs-lookup"><span data-stu-id="3a5f8-125">theme</span></span> | <span data-ttu-id="3a5f8-126">scheduleEntityTheme</span><span class="sxs-lookup"><span data-stu-id="3a5f8-126">scheduleEntityTheme</span></span>   | <span data-ttu-id="3a5f8-127">支持的颜色: 白色;变为表示紫粉色黄色底纹darkBlue;darkGreen;darkPurple;darkPink;darkYellow.</span><span class="sxs-lookup"><span data-stu-id="3a5f8-127">Supported colors: white; blue; green; purple; pink; yellow; gray; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3a5f8-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3a5f8-128">JSON representation</span></span>

<span data-ttu-id="3a5f8-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3a5f8-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOffItem"
}-->
```json
{
  "timeOffReasonId": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "theme": "pink"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeOffItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
