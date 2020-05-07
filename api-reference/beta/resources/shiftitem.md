---
title: shiftItem 资源类型
description: ShiftItem 代表班次的一个版本。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5b86f232d5d5c6c41c2eab873e992b2b9902c976
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154337"
---
# <a name="shiftitem-resource-type"></a><span data-ttu-id="10392-103">shiftItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="10392-103">shiftItem resource type</span></span>

<span data-ttu-id="10392-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10392-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10392-105">代表[班次](shift.md)的一个版本。</span><span class="sxs-lookup"><span data-stu-id="10392-105">Represents a version of a [shift](shift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="10392-106">属性</span><span class="sxs-lookup"><span data-stu-id="10392-106">Properties</span></span>
| <span data-ttu-id="10392-107">属性</span><span class="sxs-lookup"><span data-stu-id="10392-107">Property</span></span>                         | <span data-ttu-id="10392-108">类型</span><span class="sxs-lookup"><span data-stu-id="10392-108">Type</span></span>                    | <span data-ttu-id="10392-109">Description</span><span class="sxs-lookup"><span data-stu-id="10392-109">Description</span></span>                                                                             |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="10392-110">注释</span><span class="sxs-lookup"><span data-stu-id="10392-110">notes</span></span>               | <span data-ttu-id="10392-111">string</span><span class="sxs-lookup"><span data-stu-id="10392-111">string</span></span>                  | <span data-ttu-id="10392-112">的 shift 说明`shiftItem`。</span><span class="sxs-lookup"><span data-stu-id="10392-112">The shift notes for the `shiftItem`.</span></span>      |
| <span data-ttu-id="10392-113">displayName</span><span class="sxs-lookup"><span data-stu-id="10392-113">displayName</span></span>               | <span data-ttu-id="10392-114">string</span><span class="sxs-lookup"><span data-stu-id="10392-114">string</span></span>                  | <span data-ttu-id="10392-115">的 shift 标签`shiftItem`。</span><span class="sxs-lookup"><span data-stu-id="10392-115">The shift label of the `shiftItem`.</span></span> |
| <span data-ttu-id="10392-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="10392-116">startDateTime</span></span>               | <span data-ttu-id="10392-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10392-117">DateTimeOffset</span></span>                  | <span data-ttu-id="10392-118">的开始日期和时间`shiftItem`。</span><span class="sxs-lookup"><span data-stu-id="10392-118">The start date and time for the `shiftItem`.</span></span> <span data-ttu-id="10392-119">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="10392-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="10392-120">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="10392-120">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="10392-121">必需。</span><span class="sxs-lookup"><span data-stu-id="10392-121">Required.</span></span> |
| <span data-ttu-id="10392-122">endDateTime</span><span class="sxs-lookup"><span data-stu-id="10392-122">endDateTime</span></span>               | <span data-ttu-id="10392-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10392-123">DateTimeOffset</span></span>                 | <span data-ttu-id="10392-124">的结束日期和时间`shiftItem`。</span><span class="sxs-lookup"><span data-stu-id="10392-124">The end date and time for the `shiftItem`.</span></span> <span data-ttu-id="10392-125">必需。</span><span class="sxs-lookup"><span data-stu-id="10392-125">Required.</span></span> <span data-ttu-id="10392-126">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="10392-126">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="10392-127">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="10392-127">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="10392-128">theme</span><span class="sxs-lookup"><span data-stu-id="10392-128">theme</span></span> | <span data-ttu-id="10392-129">scheduleEntityTheme</span><span class="sxs-lookup"><span data-stu-id="10392-129">scheduleEntityTheme</span></span>   |  <span data-ttu-id="10392-130">支持的颜色：白色;变为表示紫粉色黄色底纹darkBlue;darkGreen;darkPurple;darkPink;darkYellow.</span><span class="sxs-lookup"><span data-stu-id="10392-130">Supported colors: white; blue; green; purple; pink; yellow; gray; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span></span> |
| <span data-ttu-id="10392-131">activities</span><span class="sxs-lookup"><span data-stu-id="10392-131">activities</span></span>    | <span data-ttu-id="10392-132">[shiftActivity](shiftactivity.md)集合</span><span class="sxs-lookup"><span data-stu-id="10392-132">[shiftActivity](shiftactivity.md) collection</span></span>   | <span data-ttu-id="10392-133">班次的增量部分，可包含员工在班次中的时间和地点的详细信息。</span><span class="sxs-lookup"><span data-stu-id="10392-133">An incremental part of a shift which can cover details of when and where an employee is during their shift.</span></span> <span data-ttu-id="10392-134">例如，工作分配或计划工间休息或午餐。</span><span class="sxs-lookup"><span data-stu-id="10392-134">For example, an assignment or a scheduled break or lunch.</span></span> <span data-ttu-id="10392-135">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="10392-135">Required.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="10392-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="10392-136">JSON representation</span></span>

<span data-ttu-id="10392-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10392-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shiftItem"
}-->
```json
{
  "displayName": "String",
  "notes": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "theme": "String",
  "activities": [{"@odata.type": "microsoft.graph.shiftActivity"}]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "shiftItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
