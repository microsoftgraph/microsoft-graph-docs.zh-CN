---
title: shiftActivity 资源类型
description: 表示班次中的活动。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: de42cb7722e7d24ba105880790fa2071c4714091
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721122"
---
# <a name="shiftactivity-resource-type"></a><span data-ttu-id="06a91-103">shiftActivity 资源类型</span><span class="sxs-lookup"><span data-stu-id="06a91-103">shiftActivity resource type</span></span>

<span data-ttu-id="06a91-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06a91-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06a91-105">表示班次 [中的活动](shift.md)。</span><span class="sxs-lookup"><span data-stu-id="06a91-105">Represents an activity in a [shift](shift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="06a91-106">属性</span><span class="sxs-lookup"><span data-stu-id="06a91-106">Properties</span></span>
| <span data-ttu-id="06a91-107">属性</span><span class="sxs-lookup"><span data-stu-id="06a91-107">Property</span></span>                         | <span data-ttu-id="06a91-108">类型</span><span class="sxs-lookup"><span data-stu-id="06a91-108">Type</span></span>                    | <span data-ttu-id="06a91-109">说明</span><span class="sxs-lookup"><span data-stu-id="06a91-109">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="06a91-110">isPaid</span><span class="sxs-lookup"><span data-stu-id="06a91-110">isPaid</span></span>               | `bool`                  | <span data-ttu-id="06a91-111">指示是否应该 `microsoft.graph.user` 在活动期间为活动支付该费用 `shift` 。</span><span class="sxs-lookup"><span data-stu-id="06a91-111">Indicates whether the `microsoft.graph.user` should be paid for the activity during their `shift`.</span></span> <span data-ttu-id="06a91-112">必需。</span><span class="sxs-lookup"><span data-stu-id="06a91-112">Required.</span></span>    |
| <span data-ttu-id="06a91-113">startDateTime</span><span class="sxs-lookup"><span data-stu-id="06a91-113">startDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="06a91-114">的开始日期和时间 `shiftActivity` 。</span><span class="sxs-lookup"><span data-stu-id="06a91-114">The start date and time for the `shiftActivity`.</span></span> <span data-ttu-id="06a91-115">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="06a91-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="06a91-116">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="06a91-116">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="06a91-117">必需。</span><span class="sxs-lookup"><span data-stu-id="06a91-117">Required.</span></span> |
| <span data-ttu-id="06a91-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="06a91-118">endDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="06a91-119">的结束日期和时间 `shiftActivity` 。</span><span class="sxs-lookup"><span data-stu-id="06a91-119">The end date and time for the `shiftActivity`.</span></span> <span data-ttu-id="06a91-120">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="06a91-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="06a91-121">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="06a91-121">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="06a91-122">必需。</span><span class="sxs-lookup"><span data-stu-id="06a91-122">Required.</span></span>    |
| <span data-ttu-id="06a91-123">code</span><span class="sxs-lookup"><span data-stu-id="06a91-123">code</span></span>               | `string`                  | <span data-ttu-id="06a91-124">客户定义的 `shiftActivity` 代码。</span><span class="sxs-lookup"><span data-stu-id="06a91-124">Customer defined code for the `shiftActivity`.</span></span> <span data-ttu-id="06a91-125">必需。</span><span class="sxs-lookup"><span data-stu-id="06a91-125">Required.</span></span>    |
| <span data-ttu-id="06a91-126">displayName</span><span class="sxs-lookup"><span data-stu-id="06a91-126">displayName</span></span>               | `string`                  | <span data-ttu-id="06a91-127">`shiftActivity`的名称。</span><span class="sxs-lookup"><span data-stu-id="06a91-127">The name of the `shiftActivity`.</span></span> <span data-ttu-id="06a91-128">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="06a91-128">Required.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="06a91-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="06a91-129">JSON representation</span></span>

<span data-ttu-id="06a91-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06a91-130">Here is a JSON representation of the resource.</span></span>

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


