---
title: timeOffItem 资源类型
description: 表示 timeOff 的版本。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 91d97c2b9da09ece24adf7b00d3eb7b54fc0fe24
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154954"
---
# <a name="timeoffitem-resource-type"></a><span data-ttu-id="9e789-103">timeOffItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="9e789-103">timeOffItem resource type</span></span>

<span data-ttu-id="9e789-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e789-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9e789-105">表示[timeOff](timeoff.md)的版本。</span><span class="sxs-lookup"><span data-stu-id="9e789-105">Represents a version of the [timeOff](timeoff.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9e789-106">属性</span><span class="sxs-lookup"><span data-stu-id="9e789-106">Properties</span></span>
| <span data-ttu-id="9e789-107">属性</span><span class="sxs-lookup"><span data-stu-id="9e789-107">Property</span></span>                         | <span data-ttu-id="9e789-108">类型</span><span class="sxs-lookup"><span data-stu-id="9e789-108">Type</span></span>                    | <span data-ttu-id="9e789-109">Description</span><span class="sxs-lookup"><span data-stu-id="9e789-109">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="9e789-110">timeOffReasonId</span><span class="sxs-lookup"><span data-stu-id="9e789-110">timeOffReasonId</span></span>               | <span data-ttu-id="9e789-111">string</span><span class="sxs-lookup"><span data-stu-id="9e789-111">string</span></span>                  | <span data-ttu-id="9e789-112">`timeOffReason`此`timeOffItem`的的 ID。</span><span class="sxs-lookup"><span data-stu-id="9e789-112">ID of the `timeOffReason` for this `timeOffItem`.</span></span> <span data-ttu-id="9e789-113">必需。</span><span class="sxs-lookup"><span data-stu-id="9e789-113">Required.</span></span>     |
| <span data-ttu-id="9e789-114">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9e789-114">startDateTime</span></span>               | <span data-ttu-id="9e789-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e789-115">DateTimeOffset</span></span>                  | <span data-ttu-id="9e789-116">的开始日期和时间`timeOffItem`。</span><span class="sxs-lookup"><span data-stu-id="9e789-116">The start date and time for the `timeOffItem`.</span></span> <span data-ttu-id="9e789-117">必需。</span><span class="sxs-lookup"><span data-stu-id="9e789-117">Required.</span></span> <span data-ttu-id="9e789-118">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="9e789-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9e789-119">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="9e789-119">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="9e789-120">endDateTime</span><span class="sxs-lookup"><span data-stu-id="9e789-120">endDateTime</span></span>               | <span data-ttu-id="9e789-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e789-121">DateTimeOffset</span></span>                  | <span data-ttu-id="9e789-122">的结束日期和时间`timeOffItem`。</span><span class="sxs-lookup"><span data-stu-id="9e789-122">The end date and time for the `timeOffItem`.</span></span> <span data-ttu-id="9e789-123">必需。</span><span class="sxs-lookup"><span data-stu-id="9e789-123">Required.</span></span> <span data-ttu-id="9e789-124">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="9e789-124">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9e789-125">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="9e789-125">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="9e789-126">theme</span><span class="sxs-lookup"><span data-stu-id="9e789-126">theme</span></span> | <span data-ttu-id="9e789-127">scheduleEntityTheme</span><span class="sxs-lookup"><span data-stu-id="9e789-127">scheduleEntityTheme</span></span>   | <span data-ttu-id="9e789-128">支持的颜色：白色;变为表示紫粉色黄色底纹darkBlue;darkGreen;darkPurple;darkPink;darkYellow.</span><span class="sxs-lookup"><span data-stu-id="9e789-128">Supported colors: white; blue; green; purple; pink; yellow; gray; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9e789-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9e789-129">JSON representation</span></span>

<span data-ttu-id="9e789-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e789-130">Here is a JSON representation of the resource.</span></span>

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
