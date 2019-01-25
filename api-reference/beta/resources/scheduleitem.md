---
title: scheduleItem 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: ed6b7441996cdf00b33be03f70afb888cc9bb251
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511350"
---
# <a name="scheduleitem-resource-type"></a><span data-ttu-id="765ac-104">scheduleItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="765ac-104">scheduleItem resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="765ac-105">介绍了在用户的默认日历上与实际事件对应的用户的可用性的项。</span><span class="sxs-lookup"><span data-stu-id="765ac-105">An item that describes the availability of a user corresponding to an actual event on the user's default calendar.</span></span> <span data-ttu-id="765ac-106">此项适用于资源以及。</span><span class="sxs-lookup"><span data-stu-id="765ac-106">This item applies to a resource as well.</span></span>

## <a name="properties"></a><span data-ttu-id="765ac-107">属性</span><span class="sxs-lookup"><span data-stu-id="765ac-107">Properties</span></span>
| <span data-ttu-id="765ac-108">属性</span><span class="sxs-lookup"><span data-stu-id="765ac-108">Property</span></span>     | <span data-ttu-id="765ac-109">类型</span><span class="sxs-lookup"><span data-stu-id="765ac-109">Type</span></span>   |<span data-ttu-id="765ac-110">说明</span><span class="sxs-lookup"><span data-stu-id="765ac-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="765ac-111">end</span><span class="sxs-lookup"><span data-stu-id="765ac-111">end</span></span> |[<span data-ttu-id="765ac-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="765ac-112">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="765ac-113">日期、 时间和结束对应的事件的时区。</span><span class="sxs-lookup"><span data-stu-id="765ac-113">The date, time, and time zone that the corresponding event ends.</span></span> |
|<span data-ttu-id="765ac-114">IsPrivate</span><span class="sxs-lookup"><span data-stu-id="765ac-114">isPrivate</span></span> |<span data-ttu-id="765ac-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="765ac-115">Boolean</span></span> |<span data-ttu-id="765ac-116">区分大小写的对应的事件。</span><span class="sxs-lookup"><span data-stu-id="765ac-116">The sensitivity of the corresponding event.</span></span> <span data-ttu-id="765ac-117">如果事件标记为`private`，则返回 false 否则为。</span><span class="sxs-lookup"><span data-stu-id="765ac-117">True if the event is marked `private`, false otherwise.</span></span> |
|<span data-ttu-id="765ac-118">location</span><span class="sxs-lookup"><span data-stu-id="765ac-118">location</span></span> |<span data-ttu-id="765ac-119">String</span><span class="sxs-lookup"><span data-stu-id="765ac-119">String</span></span> | <span data-ttu-id="765ac-120">相应的事件是保留或从参加的位置。</span><span class="sxs-lookup"><span data-stu-id="765ac-120">The location where the corresponding event is held or attended from.</span></span> <span data-ttu-id="765ac-121">可选。</span><span class="sxs-lookup"><span data-stu-id="765ac-121">Optional.</span></span>|
|<span data-ttu-id="765ac-122">start</span><span class="sxs-lookup"><span data-stu-id="765ac-122">start</span></span> |[<span data-ttu-id="765ac-123">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="765ac-123">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="765ac-124">日期、 时间和相应事件开始的时区。</span><span class="sxs-lookup"><span data-stu-id="765ac-124">The date, time, and time zone that the corresponding event starts.</span></span> |
|<span data-ttu-id="765ac-125">status</span><span class="sxs-lookup"><span data-stu-id="765ac-125">status</span></span> |<span data-ttu-id="765ac-126">String</span><span class="sxs-lookup"><span data-stu-id="765ac-126">String</span></span> | <span data-ttu-id="765ac-127">可用性的用户或资源的相应事件执行过程的状态。</span><span class="sxs-lookup"><span data-stu-id="765ac-127">The availability status of the user or resource during the corresponding event.</span></span> <span data-ttu-id="765ac-128">可能的值为： `free`， `tentative`， `busy`， `oof`， `workingElsewhere`， `unknown`。</span><span class="sxs-lookup"><span data-stu-id="765ac-128">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span> |
|<span data-ttu-id="765ac-129">subject</span><span class="sxs-lookup"><span data-stu-id="765ac-129">subject</span></span> |<span data-ttu-id="765ac-130">String</span><span class="sxs-lookup"><span data-stu-id="765ac-130">String</span></span> | <span data-ttu-id="765ac-131">相应的事件的主题行。</span><span class="sxs-lookup"><span data-stu-id="765ac-131">The corresponding event's subject line.</span></span> <span data-ttu-id="765ac-132">可选。</span><span class="sxs-lookup"><span data-stu-id="765ac-132">Optional.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="765ac-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="765ac-133">JSON representation</span></span>

<span data-ttu-id="765ac-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="765ac-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scheduleItem"
}-->

```json
{
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "isPrivate": true,
  "location": "String",
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "String",
  "subject": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "scheduleItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/scheduleitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
