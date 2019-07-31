---
title: shiftItem 资源类型
description: ShiftItem 代表班次的一个版本。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: df012df0ec563a29f15e40d3fefbcd1535dc5211
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008341"
---
# <a name="shiftitem-resource-type"></a><span data-ttu-id="0abcc-103">shiftItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="0abcc-103">shiftItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0abcc-104">代表[班次](shift.md)的一个版本。</span><span class="sxs-lookup"><span data-stu-id="0abcc-104">Represents a version of a [shift](shift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0abcc-105">属性</span><span class="sxs-lookup"><span data-stu-id="0abcc-105">Properties</span></span>
| <span data-ttu-id="0abcc-106">属性</span><span class="sxs-lookup"><span data-stu-id="0abcc-106">Property</span></span>                         | <span data-ttu-id="0abcc-107">类型</span><span class="sxs-lookup"><span data-stu-id="0abcc-107">Type</span></span>                    | <span data-ttu-id="0abcc-108">说明</span><span class="sxs-lookup"><span data-stu-id="0abcc-108">Description</span></span>                                                                             |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="0abcc-109">注释</span><span class="sxs-lookup"><span data-stu-id="0abcc-109">notes</span></span>               | <span data-ttu-id="0abcc-110">string</span><span class="sxs-lookup"><span data-stu-id="0abcc-110">string</span></span>                  | <span data-ttu-id="0abcc-111">的备注`shiftItem`。</span><span class="sxs-lookup"><span data-stu-id="0abcc-111">The notes for the `shiftItem`.</span></span>      |
| <span data-ttu-id="0abcc-112">displayName</span><span class="sxs-lookup"><span data-stu-id="0abcc-112">displayName</span></span>               | <span data-ttu-id="0abcc-113">string</span><span class="sxs-lookup"><span data-stu-id="0abcc-113">string</span></span>                  | <span data-ttu-id="0abcc-114">的名称`shiftItem`。</span><span class="sxs-lookup"><span data-stu-id="0abcc-114">The name of the `shiftItem`.</span></span> |
| <span data-ttu-id="0abcc-115">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0abcc-115">startDateTime</span></span>               | <span data-ttu-id="0abcc-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0abcc-116">DateTimeOffset</span></span>                  | <span data-ttu-id="0abcc-117">的开始日期和时间`shiftItem`。</span><span class="sxs-lookup"><span data-stu-id="0abcc-117">The start date and time for the `shiftItem`.</span></span> <span data-ttu-id="0abcc-118">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="0abcc-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0abcc-119">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="0abcc-119">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="0abcc-120">必需。</span><span class="sxs-lookup"><span data-stu-id="0abcc-120">Required.</span></span> |
| <span data-ttu-id="0abcc-121">endDateTime</span><span class="sxs-lookup"><span data-stu-id="0abcc-121">endDateTime</span></span>               | <span data-ttu-id="0abcc-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0abcc-122">DateTimeOffset</span></span>                 | <span data-ttu-id="0abcc-123">的结束日期和时间`shiftItem`。</span><span class="sxs-lookup"><span data-stu-id="0abcc-123">The end date and time for the `shiftItem`.</span></span> <span data-ttu-id="0abcc-124">必需。</span><span class="sxs-lookup"><span data-stu-id="0abcc-124">Required.</span></span> <span data-ttu-id="0abcc-125">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="0abcc-125">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0abcc-126">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="0abcc-126">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="0abcc-127">theme</span><span class="sxs-lookup"><span data-stu-id="0abcc-127">theme</span></span> | <span data-ttu-id="0abcc-128">scheduleEntityTheme</span><span class="sxs-lookup"><span data-stu-id="0abcc-128">scheduleEntityTheme</span></span>   |  <span data-ttu-id="0abcc-129">支持的颜色: 白色;变为表示紫粉色黄色底纹darkBlue;darkGreen;darkPurple;darkPink;darkYellow.</span><span class="sxs-lookup"><span data-stu-id="0abcc-129">Supported colors: white; blue; green; purple; pink; yellow; gray; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span></span> |
| <span data-ttu-id="0abcc-130">activities</span><span class="sxs-lookup"><span data-stu-id="0abcc-130">activities</span></span>    | <span data-ttu-id="0abcc-131">[shiftActivity](shiftactivity.md)集合</span><span class="sxs-lookup"><span data-stu-id="0abcc-131">[shiftActivity](shiftactivity.md) collection</span></span>   | <span data-ttu-id="0abcc-132">班次的增量部分, 可包含员工在班次中的时间和地点的详细信息。</span><span class="sxs-lookup"><span data-stu-id="0abcc-132">An incremental part of a shift which can cover details of when and where an employee is during their shift.</span></span> <span data-ttu-id="0abcc-133">例如, 工作分配或计划工间休息或午餐。</span><span class="sxs-lookup"><span data-stu-id="0abcc-133">For example, an assignment or a scheduled break or lunch.</span></span> <span data-ttu-id="0abcc-134">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="0abcc-134">Required.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0abcc-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0abcc-135">JSON representation</span></span>

<span data-ttu-id="0abcc-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0abcc-136">Here is a JSON representation of the resource.</span></span>

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
