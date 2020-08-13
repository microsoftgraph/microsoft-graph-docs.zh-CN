---
title: timeConstraint 资源类型
description: 根据指定的活动和打开时间段的性质，将会议时间建议限制在一周的特定时间和几天。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 205737e5dee56da9a91bd290a3393487d3a5b7eb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519741"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="c2fb9-103">timeConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="c2fb9-103">timeConstraint resource type</span></span>

<span data-ttu-id="c2fb9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2fb9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2fb9-105">根据指定的活动和打开时间段的性质，将会议时间建议限制在一周的特定时间和几天。</span><span class="sxs-lookup"><span data-stu-id="c2fb9-105">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>


## <a name="json-representation"></a><span data-ttu-id="c2fb9-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c2fb9-106">JSON representation</span></span>
<span data-ttu-id="c2fb9-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c2fb9-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeConstraint"
}-->

```json
{
  "activityDomain": "String",
  "timeslots": [{"@odata.type": "microsoft.graph.timeSlot"}]
}
```

## <a name="properties"></a><span data-ttu-id="c2fb9-108">属性</span><span class="sxs-lookup"><span data-stu-id="c2fb9-108">Properties</span></span>
| <span data-ttu-id="c2fb9-109">属性</span><span class="sxs-lookup"><span data-stu-id="c2fb9-109">Property</span></span>     | <span data-ttu-id="c2fb9-110">类型</span><span class="sxs-lookup"><span data-stu-id="c2fb9-110">Type</span></span>   |<span data-ttu-id="c2fb9-111">说明</span><span class="sxs-lookup"><span data-stu-id="c2fb9-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2fb9-112">activityDomain</span><span class="sxs-lookup"><span data-stu-id="c2fb9-112">activityDomain</span></span>|<span data-ttu-id="c2fb9-113">activityDomain</span><span class="sxs-lookup"><span data-stu-id="c2fb9-113">activityDomain</span></span>|<span data-ttu-id="c2fb9-114">（可选）会议性质。</span><span class="sxs-lookup"><span data-stu-id="c2fb9-114">The nature of the activity, optional.</span></span> <span data-ttu-id="c2fb9-115">可能的值包括： `work` 、 `personal` 、 `unrestricted` 或 `unknown` 。</span><span class="sxs-lookup"><span data-stu-id="c2fb9-115">Possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="c2fb9-116">timeslots</span><span class="sxs-lookup"><span data-stu-id="c2fb9-116">timeslots</span></span>|<span data-ttu-id="c2fb9-117">[timeSlot](timeslot.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c2fb9-117">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="c2fb9-118">一组时间段。</span><span class="sxs-lookup"><span data-stu-id="c2fb9-118">An array of time periods.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
