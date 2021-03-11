---
title: shiftItem 资源类型
description: shiftItem 表示班次的版本。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3998176fbd001e1136a107dd3aa53ff8442fe8f3
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721115"
---
# <a name="shiftitem-resource-type"></a><span data-ttu-id="75629-103">shiftItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="75629-103">shiftItem resource type</span></span>

<span data-ttu-id="75629-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75629-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75629-105">表示一个版本的 [班次](shift.md)。</span><span class="sxs-lookup"><span data-stu-id="75629-105">Represents a version of a [shift](shift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="75629-106">属性</span><span class="sxs-lookup"><span data-stu-id="75629-106">Properties</span></span>
| <span data-ttu-id="75629-107">属性</span><span class="sxs-lookup"><span data-stu-id="75629-107">Property</span></span>                         | <span data-ttu-id="75629-108">类型</span><span class="sxs-lookup"><span data-stu-id="75629-108">Type</span></span>                    | <span data-ttu-id="75629-109">说明</span><span class="sxs-lookup"><span data-stu-id="75629-109">Description</span></span>                                                                             |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="75629-110">notes</span><span class="sxs-lookup"><span data-stu-id="75629-110">notes</span></span>               | <span data-ttu-id="75629-111">string</span><span class="sxs-lookup"><span data-stu-id="75629-111">string</span></span>                  | <span data-ttu-id="75629-112">的班次注释 `shiftItem` 。</span><span class="sxs-lookup"><span data-stu-id="75629-112">The shift notes for the `shiftItem`.</span></span>      |
| <span data-ttu-id="75629-113">displayName</span><span class="sxs-lookup"><span data-stu-id="75629-113">displayName</span></span>               | <span data-ttu-id="75629-114">string</span><span class="sxs-lookup"><span data-stu-id="75629-114">string</span></span>                  | <span data-ttu-id="75629-115">的班次标签 `shiftItem` 。</span><span class="sxs-lookup"><span data-stu-id="75629-115">The shift label of the `shiftItem`.</span></span> |
| <span data-ttu-id="75629-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="75629-116">startDateTime</span></span>               | <span data-ttu-id="75629-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75629-117">DateTimeOffset</span></span>                  | <span data-ttu-id="75629-118">的开始日期和时间 `shiftItem` 。</span><span class="sxs-lookup"><span data-stu-id="75629-118">The start date and time for the `shiftItem`.</span></span> <span data-ttu-id="75629-119">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="75629-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="75629-120">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="75629-120">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="75629-121">必需。</span><span class="sxs-lookup"><span data-stu-id="75629-121">Required.</span></span> |
| <span data-ttu-id="75629-122">endDateTime</span><span class="sxs-lookup"><span data-stu-id="75629-122">endDateTime</span></span>               | <span data-ttu-id="75629-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75629-123">DateTimeOffset</span></span>                 | <span data-ttu-id="75629-124">的结束日期和时间 `shiftItem` 。</span><span class="sxs-lookup"><span data-stu-id="75629-124">The end date and time for the `shiftItem`.</span></span> <span data-ttu-id="75629-125">必需。</span><span class="sxs-lookup"><span data-stu-id="75629-125">Required.</span></span> <span data-ttu-id="75629-126">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="75629-126">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="75629-127">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="75629-127">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="75629-128">theme</span><span class="sxs-lookup"><span data-stu-id="75629-128">theme</span></span> | <span data-ttu-id="75629-129">scheduleEntityTheme</span><span class="sxs-lookup"><span data-stu-id="75629-129">scheduleEntityTheme</span></span>   |  <span data-ttu-id="75629-130">支持的颜色：白色;蓝色;绿色;紫色;粉红色;黄色;灰色;darkBlue;darkGreen;darkPurple;darkPink;darkYellow。</span><span class="sxs-lookup"><span data-stu-id="75629-130">Supported colors: white; blue; green; purple; pink; yellow; gray; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span></span> |
| <span data-ttu-id="75629-131">activities</span><span class="sxs-lookup"><span data-stu-id="75629-131">activities</span></span>    | <span data-ttu-id="75629-132">[shiftActivity](shiftactivity.md) 集合</span><span class="sxs-lookup"><span data-stu-id="75629-132">[shiftActivity](shiftactivity.md) collection</span></span>   | <span data-ttu-id="75629-133">班次的增量部分，可涵盖员工在轮班期间在何时何地工作的详细信息。</span><span class="sxs-lookup"><span data-stu-id="75629-133">An incremental part of a shift which can cover details of when and where an employee is during their shift.</span></span> <span data-ttu-id="75629-134">例如，工作分配或安排的休息或午餐。</span><span class="sxs-lookup"><span data-stu-id="75629-134">For example, an assignment or a scheduled break or lunch.</span></span> <span data-ttu-id="75629-135">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="75629-135">Required.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="75629-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="75629-136">JSON representation</span></span>

<span data-ttu-id="75629-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="75629-137">Here is a JSON representation of the resource.</span></span>

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


