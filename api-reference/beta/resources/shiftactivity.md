---
title: shiftActivity 资源类型
description: 代表班次中的活动。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d03cf481ec0360aa6ef7c4ab544189b420b2081b
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154344"
---
# <a name="shiftactivity-resource-type"></a><span data-ttu-id="87852-103">shiftActivity 资源类型</span><span class="sxs-lookup"><span data-stu-id="87852-103">shiftActivity resource type</span></span>

<span data-ttu-id="87852-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87852-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87852-105">代表[班次](shift.md)中的活动。</span><span class="sxs-lookup"><span data-stu-id="87852-105">Represents an activity in a [shift](shift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="87852-106">属性</span><span class="sxs-lookup"><span data-stu-id="87852-106">Properties</span></span>
| <span data-ttu-id="87852-107">属性</span><span class="sxs-lookup"><span data-stu-id="87852-107">Property</span></span>                         | <span data-ttu-id="87852-108">类型</span><span class="sxs-lookup"><span data-stu-id="87852-108">Type</span></span>                    | <span data-ttu-id="87852-109">Description</span><span class="sxs-lookup"><span data-stu-id="87852-109">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="87852-110">isPaid</span><span class="sxs-lookup"><span data-stu-id="87852-110">isPaid</span></span>               | `bool`                  | <span data-ttu-id="87852-111">指示是否`microsoft.graph.user`应在其`shift`期间向活动付款。</span><span class="sxs-lookup"><span data-stu-id="87852-111">Indicates whether the `microsoft.graph.user` should be paid for the activity during their `shift`.</span></span> <span data-ttu-id="87852-112">必需。</span><span class="sxs-lookup"><span data-stu-id="87852-112">Required.</span></span>    |
| <span data-ttu-id="87852-113">startDateTime</span><span class="sxs-lookup"><span data-stu-id="87852-113">startDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="87852-114">的开始日期和时间`shiftActivity`。</span><span class="sxs-lookup"><span data-stu-id="87852-114">The start date and time for the `shiftActivity`.</span></span> <span data-ttu-id="87852-115">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="87852-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="87852-116">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="87852-116">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="87852-117">必需。</span><span class="sxs-lookup"><span data-stu-id="87852-117">Required.</span></span> |
| <span data-ttu-id="87852-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="87852-118">endDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="87852-119">的结束日期和时间`shiftActivity`。</span><span class="sxs-lookup"><span data-stu-id="87852-119">The end date and time for the `shiftActivity`.</span></span> <span data-ttu-id="87852-120">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="87852-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="87852-121">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="87852-121">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="87852-122">必需。</span><span class="sxs-lookup"><span data-stu-id="87852-122">Required.</span></span>    |
| <span data-ttu-id="87852-123">code</span><span class="sxs-lookup"><span data-stu-id="87852-123">code</span></span>               | `string`                  | <span data-ttu-id="87852-124">的客户定义的代码`shiftActivity`。</span><span class="sxs-lookup"><span data-stu-id="87852-124">Customer defined code for the `shiftActivity`.</span></span> <span data-ttu-id="87852-125">必需。</span><span class="sxs-lookup"><span data-stu-id="87852-125">Required.</span></span>    |
| <span data-ttu-id="87852-126">displayName</span><span class="sxs-lookup"><span data-stu-id="87852-126">displayName</span></span>               | `string`                  | <span data-ttu-id="87852-127">的名称`shiftActivity`。</span><span class="sxs-lookup"><span data-stu-id="87852-127">The name of the `shiftActivity`.</span></span> <span data-ttu-id="87852-128">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="87852-128">Required.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="87852-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="87852-129">JSON representation</span></span>

<span data-ttu-id="87852-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="87852-130">Here is a JSON representation of the resource.</span></span>

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
