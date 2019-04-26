---
title: shiftActivity 资源类型
description: 代表班次中的活动。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 24946630e9bc3ae9ba418f5c322ab212c022d6d1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343083"
---
# <a name="shiftactivity-resource-type"></a><span data-ttu-id="535fa-103">shiftActivity 资源类型</span><span class="sxs-lookup"><span data-stu-id="535fa-103">shiftActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="535fa-104">代表[班次](shift.md)中的活动。</span><span class="sxs-lookup"><span data-stu-id="535fa-104">Represents an activity in a [shift](shift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="535fa-105">属性</span><span class="sxs-lookup"><span data-stu-id="535fa-105">Properties</span></span>
| <span data-ttu-id="535fa-106">属性</span><span class="sxs-lookup"><span data-stu-id="535fa-106">Property</span></span>                         | <span data-ttu-id="535fa-107">类型</span><span class="sxs-lookup"><span data-stu-id="535fa-107">Type</span></span>                    | <span data-ttu-id="535fa-108">说明</span><span class="sxs-lookup"><span data-stu-id="535fa-108">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="535fa-109">isPaid</span><span class="sxs-lookup"><span data-stu-id="535fa-109">isPaid</span></span>               | `bool`                  | <span data-ttu-id="535fa-110">指示是否`microsoft.graph.user`应在其`shift`期间向活动付款。</span><span class="sxs-lookup"><span data-stu-id="535fa-110">Indicates whether the `microsoft.graph.user` should be paid for the activity during their `shift`.</span></span> <span data-ttu-id="535fa-111">必需。</span><span class="sxs-lookup"><span data-stu-id="535fa-111">Required.</span></span>    |
| <span data-ttu-id="535fa-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="535fa-112">startDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="535fa-113">的开始日期和时间`shiftActivity`。</span><span class="sxs-lookup"><span data-stu-id="535fa-113">The start date and time for the `shiftActivity`.</span></span> <span data-ttu-id="535fa-114">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="535fa-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="535fa-115">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="535fa-115">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="535fa-116">必需。</span><span class="sxs-lookup"><span data-stu-id="535fa-116">Required.</span></span> |
| <span data-ttu-id="535fa-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="535fa-117">endDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="535fa-118">的结束日期和时间`shiftActivity`。</span><span class="sxs-lookup"><span data-stu-id="535fa-118">The end date and time for the `shiftActivity`.</span></span> <span data-ttu-id="535fa-119">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="535fa-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="535fa-120">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="535fa-120">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="535fa-121">必需。</span><span class="sxs-lookup"><span data-stu-id="535fa-121">Required.</span></span>    |
| <span data-ttu-id="535fa-122">code</span><span class="sxs-lookup"><span data-stu-id="535fa-122">code</span></span>               | `string`                  | <span data-ttu-id="535fa-123">的客户定义的代码`shiftActivity`。</span><span class="sxs-lookup"><span data-stu-id="535fa-123">Customer defined code for the `shiftActivity`.</span></span> <span data-ttu-id="535fa-124">必需。</span><span class="sxs-lookup"><span data-stu-id="535fa-124">Required.</span></span>    |
| <span data-ttu-id="535fa-125">displayName</span><span class="sxs-lookup"><span data-stu-id="535fa-125">displayName</span></span>               | `string`                  | <span data-ttu-id="535fa-126">的名称`shiftActivity`。</span><span class="sxs-lookup"><span data-stu-id="535fa-126">The name of the `shiftActivity`.</span></span> <span data-ttu-id="535fa-127">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="535fa-127">Required.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="535fa-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="535fa-128">JSON representation</span></span>

<span data-ttu-id="535fa-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="535fa-129">Here is a JSON representation of the resource.</span></span>

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
