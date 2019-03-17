---
title: timeOffItem 资源类型
description: 表示 timeOff 的版本。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c83a8725a0048a622ed88ec8265be76c30e46cc0
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657852"
---
# <a name="timeoffitem-resource-type"></a><span data-ttu-id="a5f31-103">timeOffItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="a5f31-103">timeOffItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5f31-104">表示[timeOff](timeoff.md)的版本。</span><span class="sxs-lookup"><span data-stu-id="a5f31-104">Represents a version of the [timeOff](timeoff.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a5f31-105">属性</span><span class="sxs-lookup"><span data-stu-id="a5f31-105">Properties</span></span>
| <span data-ttu-id="a5f31-106">属性</span><span class="sxs-lookup"><span data-stu-id="a5f31-106">Property</span></span>                         | <span data-ttu-id="a5f31-107">类型</span><span class="sxs-lookup"><span data-stu-id="a5f31-107">Type</span></span>                    | <span data-ttu-id="a5f31-108">说明</span><span class="sxs-lookup"><span data-stu-id="a5f31-108">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="a5f31-109">timeOffReasonId</span><span class="sxs-lookup"><span data-stu-id="a5f31-109">timeOffReasonId</span></span>               | `string`                  | <span data-ttu-id="a5f31-110">`timeOffReason`此`timeOffItem`的的 ID。</span><span class="sxs-lookup"><span data-stu-id="a5f31-110">ID of the `timeOffReason` for this `timeOffItem`.</span></span> <span data-ttu-id="a5f31-111">必需。</span><span class="sxs-lookup"><span data-stu-id="a5f31-111">Required.</span></span>     |
| <span data-ttu-id="a5f31-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a5f31-112">startDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="a5f31-113">的开始日期和时间`timeOffItem`。</span><span class="sxs-lookup"><span data-stu-id="a5f31-113">The start date and time for the `timeOffItem`.</span></span> <span data-ttu-id="a5f31-114">必需。</span><span class="sxs-lookup"><span data-stu-id="a5f31-114">Required.</span></span> <span data-ttu-id="a5f31-115">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="a5f31-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a5f31-116">例如, 2014 年1月1日午夜 UTC 将如下所示: "2014-01-01T00:00: 00Z"。</span><span class="sxs-lookup"><span data-stu-id="a5f31-116">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="a5f31-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="a5f31-117">endDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="a5f31-118">的结束日期和时间`timeOffItem`。</span><span class="sxs-lookup"><span data-stu-id="a5f31-118">The end date and time for the `timeOffItem`.</span></span> <span data-ttu-id="a5f31-119">必需。</span><span class="sxs-lookup"><span data-stu-id="a5f31-119">Required.</span></span> <span data-ttu-id="a5f31-120">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="a5f31-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a5f31-121">例如, 2014 年1月1日午夜 UTC 将如下所示: "2014-01-01T00:00: 00Z"。</span><span class="sxs-lookup"><span data-stu-id="a5f31-121">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="a5f31-122">theme</span><span class="sxs-lookup"><span data-stu-id="a5f31-122">theme</span></span> | `enum`   | <span data-ttu-id="a5f31-123">支持的颜色: 白色;变为表示紫粉色黄色底纹darkBlue;darkGreen;darkPurple;darkPink;darkYellow。</span><span class="sxs-lookup"><span data-stu-id="a5f31-123">Supported colors: white; blue; green; purple; pink; yellow; gray; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a5f31-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a5f31-124">JSON representation</span></span>

<span data-ttu-id="a5f31-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a5f31-125">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOffItem"
}-->
```json
{
  "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
  "startDateTime": "2019-03-11T07:00:00Z",
  "endDateTime": "2019-03-12T07:00:00Z",
  "theme": "pink"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/timeoffitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
