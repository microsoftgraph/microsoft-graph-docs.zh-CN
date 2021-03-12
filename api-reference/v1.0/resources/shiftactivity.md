---
title: shiftActivity 资源类型
description: 表示班次中的活动。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 30552f0a5c856d0144fd231cda6b9e1aa825d97f
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721794"
---
# <a name="shiftactivity-resource-type"></a><span data-ttu-id="c249d-103">shiftActivity 资源类型</span><span class="sxs-lookup"><span data-stu-id="c249d-103">shiftActivity resource type</span></span>

<span data-ttu-id="c249d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c249d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c249d-105">表示班次中的 [活动](shift.md)。</span><span class="sxs-lookup"><span data-stu-id="c249d-105">Represents an activity in a [shift](shift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c249d-106">属性</span><span class="sxs-lookup"><span data-stu-id="c249d-106">Properties</span></span>
| <span data-ttu-id="c249d-107">属性</span><span class="sxs-lookup"><span data-stu-id="c249d-107">Property</span></span>                         | <span data-ttu-id="c249d-108">类型</span><span class="sxs-lookup"><span data-stu-id="c249d-108">Type</span></span>                    | <span data-ttu-id="c249d-109">说明</span><span class="sxs-lookup"><span data-stu-id="c249d-109">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="c249d-110">isPaid</span><span class="sxs-lookup"><span data-stu-id="c249d-110">isPaid</span></span>               | `bool`                  | <span data-ttu-id="c249d-111">指示 是否应该 `microsoft.graph.user` 在 活动期间为 活动付费 `shift` 。</span><span class="sxs-lookup"><span data-stu-id="c249d-111">Indicates whether the `microsoft.graph.user` should be paid for the activity during their `shift`.</span></span> <span data-ttu-id="c249d-112">必需。</span><span class="sxs-lookup"><span data-stu-id="c249d-112">Required.</span></span>    |
| <span data-ttu-id="c249d-113">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c249d-113">startDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="c249d-114">的开始日期和时间 `shiftActivity` 。</span><span class="sxs-lookup"><span data-stu-id="c249d-114">The start date and time for the `shiftActivity`.</span></span> <span data-ttu-id="c249d-115">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="c249d-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c249d-116">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="c249d-116">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="c249d-117">必需。</span><span class="sxs-lookup"><span data-stu-id="c249d-117">Required.</span></span> |
| <span data-ttu-id="c249d-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="c249d-118">endDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="c249d-119">的结束日期和时间 `shiftActivity` 。</span><span class="sxs-lookup"><span data-stu-id="c249d-119">The end date and time for the `shiftActivity`.</span></span> <span data-ttu-id="c249d-120">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="c249d-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c249d-121">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="c249d-121">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="c249d-122">必需。</span><span class="sxs-lookup"><span data-stu-id="c249d-122">Required.</span></span>    |
| <span data-ttu-id="c249d-123">code</span><span class="sxs-lookup"><span data-stu-id="c249d-123">code</span></span>               | `string`                  | <span data-ttu-id="c249d-124">客户定义的 `shiftActivity` 代码。</span><span class="sxs-lookup"><span data-stu-id="c249d-124">Customer defined code for the `shiftActivity`.</span></span> <span data-ttu-id="c249d-125">必需。</span><span class="sxs-lookup"><span data-stu-id="c249d-125">Required.</span></span>    |
| <span data-ttu-id="c249d-126">displayName</span><span class="sxs-lookup"><span data-stu-id="c249d-126">displayName</span></span>               | `string`                  | <span data-ttu-id="c249d-127">的名称 `shiftActivity` 。</span><span class="sxs-lookup"><span data-stu-id="c249d-127">The name of the `shiftActivity`.</span></span> <span data-ttu-id="c249d-128">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="c249d-128">Required.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="c249d-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c249d-129">JSON representation</span></span>

<span data-ttu-id="c249d-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c249d-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shiftActivity"
}-->
```json
{
  "isPaid": true,
  "startDateTime": "2019-03-11T15:00:00Z",
  "endDateTime": "2019-03-11T15:15:00Z",
  "code": "",
  "displayName": "Lunch"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "shiftActivity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

