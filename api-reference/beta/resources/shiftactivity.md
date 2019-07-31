---
title: shiftActivity 资源类型
description: 代表班次中的活动。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 8acfb16235c90cf6067ad5fd6c5d8e82ae239f8d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965073"
---
# <a name="shiftactivity-resource-type"></a><span data-ttu-id="b9a8e-103">shiftActivity 资源类型</span><span class="sxs-lookup"><span data-stu-id="b9a8e-103">shiftActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9a8e-104">代表[班次](shift.md)中的活动。</span><span class="sxs-lookup"><span data-stu-id="b9a8e-104">Represents an activity in a [shift](shift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b9a8e-105">属性</span><span class="sxs-lookup"><span data-stu-id="b9a8e-105">Properties</span></span>
| <span data-ttu-id="b9a8e-106">属性</span><span class="sxs-lookup"><span data-stu-id="b9a8e-106">Property</span></span>                         | <span data-ttu-id="b9a8e-107">类型</span><span class="sxs-lookup"><span data-stu-id="b9a8e-107">Type</span></span>                    | <span data-ttu-id="b9a8e-108">说明</span><span class="sxs-lookup"><span data-stu-id="b9a8e-108">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="b9a8e-109">isPaid</span><span class="sxs-lookup"><span data-stu-id="b9a8e-109">isPaid</span></span>               | `bool`                  | <span data-ttu-id="b9a8e-110">指示是否`microsoft.graph.user`应在其`shift`期间向活动付款。</span><span class="sxs-lookup"><span data-stu-id="b9a8e-110">Indicates whether the `microsoft.graph.user` should be paid for the activity during their `shift`.</span></span> <span data-ttu-id="b9a8e-111">必需。</span><span class="sxs-lookup"><span data-stu-id="b9a8e-111">Required.</span></span>    |
| <span data-ttu-id="b9a8e-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b9a8e-112">startDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="b9a8e-113">的开始日期和时间`shiftActivity`。</span><span class="sxs-lookup"><span data-stu-id="b9a8e-113">The start date and time for the `shiftActivity`.</span></span> <span data-ttu-id="b9a8e-114">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="b9a8e-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b9a8e-115">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="b9a8e-115">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="b9a8e-116">必需。</span><span class="sxs-lookup"><span data-stu-id="b9a8e-116">Required.</span></span> |
| <span data-ttu-id="b9a8e-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="b9a8e-117">endDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="b9a8e-118">的结束日期和时间`shiftActivity`。</span><span class="sxs-lookup"><span data-stu-id="b9a8e-118">The end date and time for the `shiftActivity`.</span></span> <span data-ttu-id="b9a8e-119">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="b9a8e-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b9a8e-120">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="b9a8e-120">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="b9a8e-121">必需。</span><span class="sxs-lookup"><span data-stu-id="b9a8e-121">Required.</span></span>    |
| <span data-ttu-id="b9a8e-122">code</span><span class="sxs-lookup"><span data-stu-id="b9a8e-122">code</span></span>               | `string`                  | <span data-ttu-id="b9a8e-123">的客户定义的代码`shiftActivity`。</span><span class="sxs-lookup"><span data-stu-id="b9a8e-123">Customer defined code for the `shiftActivity`.</span></span> <span data-ttu-id="b9a8e-124">必需。</span><span class="sxs-lookup"><span data-stu-id="b9a8e-124">Required.</span></span>    |
| <span data-ttu-id="b9a8e-125">displayName</span><span class="sxs-lookup"><span data-stu-id="b9a8e-125">displayName</span></span>               | `string`                  | <span data-ttu-id="b9a8e-126">的名称`shiftActivity`。</span><span class="sxs-lookup"><span data-stu-id="b9a8e-126">The name of the `shiftActivity`.</span></span> <span data-ttu-id="b9a8e-127">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="b9a8e-127">Required.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="b9a8e-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b9a8e-128">JSON representation</span></span>

<span data-ttu-id="b9a8e-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b9a8e-129">Here is a JSON representation of the resource.</span></span>

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
