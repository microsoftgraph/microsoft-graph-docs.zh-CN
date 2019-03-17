---
title: shiftItem 资源类型
description: shiftItem 代表班次的一个版本。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7ff829ca0f43124404b4b99b048c9919368b6009
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657705"
---
# <a name="shiftitem-resource-type"></a><span data-ttu-id="033fa-103">shiftItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="033fa-103">shiftItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="033fa-104">代表[班次](shift.md)的一个版本。</span><span class="sxs-lookup"><span data-stu-id="033fa-104">Represents a version of a [shift](shift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="033fa-105">属性</span><span class="sxs-lookup"><span data-stu-id="033fa-105">Properties</span></span>
| <span data-ttu-id="033fa-106">属性</span><span class="sxs-lookup"><span data-stu-id="033fa-106">Property</span></span>                         | <span data-ttu-id="033fa-107">类型</span><span class="sxs-lookup"><span data-stu-id="033fa-107">Type</span></span>                    | <span data-ttu-id="033fa-108">说明</span><span class="sxs-lookup"><span data-stu-id="033fa-108">Description</span></span>                                                                             |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="033fa-109">注释</span><span class="sxs-lookup"><span data-stu-id="033fa-109">notes</span></span>               | `string`                  | <span data-ttu-id="033fa-110">的备注`shiftItem`。</span><span class="sxs-lookup"><span data-stu-id="033fa-110">The notes for the `shiftItem`.</span></span>      |
| <span data-ttu-id="033fa-111">displayName</span><span class="sxs-lookup"><span data-stu-id="033fa-111">displayName</span></span>               | `string`                  | <span data-ttu-id="033fa-112">的名称`shiftItem`。</span><span class="sxs-lookup"><span data-stu-id="033fa-112">The name of the `shiftItem`.</span></span> |
| <span data-ttu-id="033fa-113">startDateTime</span><span class="sxs-lookup"><span data-stu-id="033fa-113">startDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="033fa-114">的开始日期和时间`shiftItem`。</span><span class="sxs-lookup"><span data-stu-id="033fa-114">The start date and time for the `shiftItem`.</span></span> <span data-ttu-id="033fa-115">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="033fa-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="033fa-116">例如, 2014 年1月1日午夜 UTC 将如下所示: "2014-01-01T00:00: 00Z"。</span><span class="sxs-lookup"><span data-stu-id="033fa-116">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="033fa-117">必需。</span><span class="sxs-lookup"><span data-stu-id="033fa-117">Required.</span></span> |
| <span data-ttu-id="033fa-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="033fa-118">endDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="033fa-119">的结束日期和时间`shiftItem`。</span><span class="sxs-lookup"><span data-stu-id="033fa-119">The end date and time for the `shiftItem`.</span></span> <span data-ttu-id="033fa-120">必需。</span><span class="sxs-lookup"><span data-stu-id="033fa-120">Required.</span></span> <span data-ttu-id="033fa-121">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="033fa-121">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="033fa-122">例如, 2014 年1月1日午夜 UTC 将如下所示: "2014-01-01T00:00: 00Z"。</span><span class="sxs-lookup"><span data-stu-id="033fa-122">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="033fa-123">theme</span><span class="sxs-lookup"><span data-stu-id="033fa-123">theme</span></span> | `enum`   |    |  |  | <span data-ttu-id="033fa-124">支持的颜色: 白色;变为表示紫粉色黄色底纹darkBlue;darkGreen;darkPurple;darkPink;darkYellow。</span><span class="sxs-lookup"><span data-stu-id="033fa-124">Supported colors: white; blue; green; purple; pink; yellow; gray; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span></span> |
| <span data-ttu-id="033fa-125">activities</span><span class="sxs-lookup"><span data-stu-id="033fa-125">activities</span></span>    | `collection([shiftActivity](shiftactivity.md))`    | <span data-ttu-id="033fa-126">班次的增量部分, 可包含员工在班次中的时间和地点的详细信息。</span><span class="sxs-lookup"><span data-stu-id="033fa-126">An incremental part of a shift which can cover details of when and where an employee is during their shift.</span></span> <span data-ttu-id="033fa-127">例如, 工作分配或计划工间休息或午餐。</span><span class="sxs-lookup"><span data-stu-id="033fa-127">For example, an assignment or a scheduled break or lunch.</span></span> <span data-ttu-id="033fa-128">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="033fa-128">Required.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="033fa-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="033fa-129">JSON representation</span></span>

<span data-ttu-id="033fa-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="033fa-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shiftItem"
}-->
```json
{
  "displayName": "Day shift",
  "notes": "Please do inventory as part of your shift.",
  "startDateTime": "2019-03-11T15:00:00Z",
  "endDateTime": "2019-03-12T00:00:00Z",
  "theme": "blue",
  "activities": [
    {
      "isPaid": true,
      "startDateTime": "2019-03-11T15:00:00Z",
      "endDateTime": "2019-03-11T15:15:00Z",
      "code": "",
      "displayName": "Lunch"
    }
  ]
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
  "suppressions": [
    "Error: /api-reference/beta/resources/shiftitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
