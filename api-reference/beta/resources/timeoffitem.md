---
title: timeOffItem 资源类型
description: 表示 timeOff 的版本。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8fbe535fcbc63f94a50e65c62c694ffaac1a9aed
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786080"
---
# <a name="timeoffitem-resource-type"></a><span data-ttu-id="77324-103">timeOffItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="77324-103">timeOffItem resource type</span></span>

<span data-ttu-id="77324-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77324-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77324-105">表示 [timeOff 的版本](timeoff.md)。</span><span class="sxs-lookup"><span data-stu-id="77324-105">Represents a version of the [timeOff](timeoff.md).</span></span>

## <a name="properties"></a><span data-ttu-id="77324-106">属性</span><span class="sxs-lookup"><span data-stu-id="77324-106">Properties</span></span>
| <span data-ttu-id="77324-107">属性</span><span class="sxs-lookup"><span data-stu-id="77324-107">Property</span></span>                         | <span data-ttu-id="77324-108">类型</span><span class="sxs-lookup"><span data-stu-id="77324-108">Type</span></span>                    | <span data-ttu-id="77324-109">说明</span><span class="sxs-lookup"><span data-stu-id="77324-109">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="77324-110">timeOffReasonId</span><span class="sxs-lookup"><span data-stu-id="77324-110">timeOffReasonId</span></span>               | <span data-ttu-id="77324-111">string</span><span class="sxs-lookup"><span data-stu-id="77324-111">string</span></span>                  | <span data-ttu-id="77324-112">此时 `timeOffReason` **OffItem** 的 ID。</span><span class="sxs-lookup"><span data-stu-id="77324-112">ID of the `timeOffReason` for this **timeOffItem**.</span></span> <span data-ttu-id="77324-113">必填。</span><span class="sxs-lookup"><span data-stu-id="77324-113">Required.</span></span>     |
| <span data-ttu-id="77324-114">startDateTime</span><span class="sxs-lookup"><span data-stu-id="77324-114">startDateTime</span></span>               | <span data-ttu-id="77324-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77324-115">DateTimeOffset</span></span>                  | <span data-ttu-id="77324-116">**timeOffItem** 的开始日期和时间。</span><span class="sxs-lookup"><span data-stu-id="77324-116">The start date and time for the **timeOffItem**.</span></span> <span data-ttu-id="77324-117">必填。</span><span class="sxs-lookup"><span data-stu-id="77324-117">Required.</span></span> <span data-ttu-id="77324-118">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="77324-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="77324-119">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="77324-119">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="77324-120">endDateTime</span><span class="sxs-lookup"><span data-stu-id="77324-120">endDateTime</span></span>               | <span data-ttu-id="77324-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77324-121">DateTimeOffset</span></span>                  | <span data-ttu-id="77324-122">**timeOffItem 的结束日期和时间**。</span><span class="sxs-lookup"><span data-stu-id="77324-122">The end date and time for the **timeOffItem**.</span></span> <span data-ttu-id="77324-123">必填。</span><span class="sxs-lookup"><span data-stu-id="77324-123">Required.</span></span> <span data-ttu-id="77324-124">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="77324-124">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="77324-125">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="77324-125">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="77324-126">theme</span><span class="sxs-lookup"><span data-stu-id="77324-126">theme</span></span> | <span data-ttu-id="77324-127">scheduleEntityTheme</span><span class="sxs-lookup"><span data-stu-id="77324-127">scheduleEntityTheme</span></span>   | <span data-ttu-id="77324-128">支持的颜色：白色;blue;绿色;紫色;粉色;黄色;灰色;darkBlue;darkGreen;darkPurple;darkPink;darkYellow。</span><span class="sxs-lookup"><span data-stu-id="77324-128">Supported colors: white; blue; green; purple; pink; yellow; gray; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="77324-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="77324-129">JSON representation</span></span>

<span data-ttu-id="77324-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="77324-130">Here is a JSON representation of the resource.</span></span>

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
  "theme": {"@odata.type": "microsoft.graph.scheduleEntityTheme"}
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


