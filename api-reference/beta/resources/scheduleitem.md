---
title: scheduleItem 资源类型
description: 一个项目, 该项目描述与用户的默认日历上的实际事件相对应的用户的可用性。 此项也适用于资源。
localization_priority: Normal
ms.openlocfilehash: d8b0d7bc18c00ca8bda3ef91b2ec8c629c980a97
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343456"
---
# <a name="scheduleitem-resource-type"></a><span data-ttu-id="b21e7-104">scheduleItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="b21e7-104">scheduleItem resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="b21e7-105">一个项目, 该项目描述与用户的默认日历上的实际事件相对应的用户的可用性。</span><span class="sxs-lookup"><span data-stu-id="b21e7-105">An item that describes the availability of a user corresponding to an actual event on the user's default calendar.</span></span> <span data-ttu-id="b21e7-106">此项也适用于资源 (会议室或设备)。</span><span class="sxs-lookup"><span data-stu-id="b21e7-106">This item applies to a resource (room or equipment) as well.</span></span>

## <a name="properties"></a><span data-ttu-id="b21e7-107">属性</span><span class="sxs-lookup"><span data-stu-id="b21e7-107">Properties</span></span>
| <span data-ttu-id="b21e7-108">属性</span><span class="sxs-lookup"><span data-stu-id="b21e7-108">Property</span></span>     | <span data-ttu-id="b21e7-109">类型</span><span class="sxs-lookup"><span data-stu-id="b21e7-109">Type</span></span>   |<span data-ttu-id="b21e7-110">说明</span><span class="sxs-lookup"><span data-stu-id="b21e7-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b21e7-111">end</span><span class="sxs-lookup"><span data-stu-id="b21e7-111">end</span></span> |[<span data-ttu-id="b21e7-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="b21e7-112">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="b21e7-113">相应事件结束时的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="b21e7-113">The date, time, and time zone that the corresponding event ends.</span></span> |
|<span data-ttu-id="b21e7-114">isPrivate</span><span class="sxs-lookup"><span data-stu-id="b21e7-114">isPrivate</span></span> |<span data-ttu-id="b21e7-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="b21e7-115">Boolean</span></span> |<span data-ttu-id="b21e7-116">相应事件的敏感度。</span><span class="sxs-lookup"><span data-stu-id="b21e7-116">The sensitivity of the corresponding event.</span></span> <span data-ttu-id="b21e7-117">如果已标记`private`事件, 则为 True, 否则为 false。</span><span class="sxs-lookup"><span data-stu-id="b21e7-117">True if the event is marked `private`, false otherwise.</span></span> <span data-ttu-id="b21e7-118">可选。</span><span class="sxs-lookup"><span data-stu-id="b21e7-118">Optional.</span></span> |
|<span data-ttu-id="b21e7-119">location</span><span class="sxs-lookup"><span data-stu-id="b21e7-119">location</span></span> |<span data-ttu-id="b21e7-120">String</span><span class="sxs-lookup"><span data-stu-id="b21e7-120">String</span></span> | <span data-ttu-id="b21e7-121">保留或参与的相应事件的位置。</span><span class="sxs-lookup"><span data-stu-id="b21e7-121">The location where the corresponding event is held or attended from.</span></span> <span data-ttu-id="b21e7-122">可选。</span><span class="sxs-lookup"><span data-stu-id="b21e7-122">Optional.</span></span>|
|<span data-ttu-id="b21e7-123">start</span><span class="sxs-lookup"><span data-stu-id="b21e7-123">start</span></span> |[<span data-ttu-id="b21e7-124">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="b21e7-124">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="b21e7-125">相应事件的开始日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="b21e7-125">The date, time, and time zone that the corresponding event starts.</span></span> |
|<span data-ttu-id="b21e7-126">status</span><span class="sxs-lookup"><span data-stu-id="b21e7-126">status</span></span> |<span data-ttu-id="b21e7-127">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="b21e7-127">freeBusyStatus</span></span> | <span data-ttu-id="b21e7-128">相应事件期间用户或资源的可用性状态。</span><span class="sxs-lookup"><span data-stu-id="b21e7-128">The availability status of the user or resource during the corresponding event.</span></span> <span data-ttu-id="b21e7-129">可能的值为: `free`、 `tentative`、 `busy` `oof`、、 `workingElsewhere`、 `unknown`。</span><span class="sxs-lookup"><span data-stu-id="b21e7-129">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span> |
|<span data-ttu-id="b21e7-130">subject</span><span class="sxs-lookup"><span data-stu-id="b21e7-130">subject</span></span> |<span data-ttu-id="b21e7-131">String</span><span class="sxs-lookup"><span data-stu-id="b21e7-131">String</span></span> | <span data-ttu-id="b21e7-132">相应事件的主题行。</span><span class="sxs-lookup"><span data-stu-id="b21e7-132">The corresponding event's subject line.</span></span> <span data-ttu-id="b21e7-133">可选。</span><span class="sxs-lookup"><span data-stu-id="b21e7-133">Optional.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="b21e7-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b21e7-134">JSON representation</span></span>

<span data-ttu-id="b21e7-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b21e7-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "isPrivate",
    "location",
    "subject"
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
  "suppressions": []
}
-->
