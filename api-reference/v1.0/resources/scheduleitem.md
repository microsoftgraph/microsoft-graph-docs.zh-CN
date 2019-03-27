---
title: scheduleItem 资源类型
description: 一个项目, 该项目描述与用户的默认日历上的实际事件相对应的用户的可用性。 此项也适用于资源 (会议室或设备)。
localization_priority: Normal
ms.openlocfilehash: 8a30dcb4394a963e35047fab00391f0cc7eb7715
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/27/2019
ms.locfileid: "30926587"
---
# <a name="scheduleitem-resource-type"></a><span data-ttu-id="b8283-104">scheduleItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="b8283-104">scheduleItem resource type</span></span>

<span data-ttu-id="b8283-105">一个项目, 该项目描述与用户的默认日历上的实际事件相对应的用户的可用性。</span><span class="sxs-lookup"><span data-stu-id="b8283-105">An item that describes the availability of a user corresponding to an actual event on the user's default calendar.</span></span> <span data-ttu-id="b8283-106">此项也适用于资源 (会议室或设备)。</span><span class="sxs-lookup"><span data-stu-id="b8283-106">This item applies to a resource (room or equipment) as well.</span></span>

## <a name="properties"></a><span data-ttu-id="b8283-107">属性</span><span class="sxs-lookup"><span data-stu-id="b8283-107">Properties</span></span>
| <span data-ttu-id="b8283-108">属性</span><span class="sxs-lookup"><span data-stu-id="b8283-108">Property</span></span>     | <span data-ttu-id="b8283-109">类型</span><span class="sxs-lookup"><span data-stu-id="b8283-109">Type</span></span>   |<span data-ttu-id="b8283-110">说明</span><span class="sxs-lookup"><span data-stu-id="b8283-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8283-111">end</span><span class="sxs-lookup"><span data-stu-id="b8283-111">end</span></span> |[<span data-ttu-id="b8283-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="b8283-112">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="b8283-113">相应事件结束时的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="b8283-113">The date, time, and time zone that the corresponding event ends.</span></span> |
|<span data-ttu-id="b8283-114">isPrivate</span><span class="sxs-lookup"><span data-stu-id="b8283-114">isPrivate</span></span> |<span data-ttu-id="b8283-115">布尔</span><span class="sxs-lookup"><span data-stu-id="b8283-115">Boolean</span></span> |<span data-ttu-id="b8283-116">相应事件的敏感度。</span><span class="sxs-lookup"><span data-stu-id="b8283-116">The sensitivity of the corresponding event.</span></span> <span data-ttu-id="b8283-117">如果已标记`private`事件, 则为 True, 否则为 false。</span><span class="sxs-lookup"><span data-stu-id="b8283-117">True if the event is marked `private`, false otherwise.</span></span> <span data-ttu-id="b8283-118">可选。</span><span class="sxs-lookup"><span data-stu-id="b8283-118">Optional.</span></span>|
|<span data-ttu-id="b8283-119">location</span><span class="sxs-lookup"><span data-stu-id="b8283-119">location</span></span> |<span data-ttu-id="b8283-120">字符串</span><span class="sxs-lookup"><span data-stu-id="b8283-120">String</span></span> | <span data-ttu-id="b8283-121">保留或参与的相应事件的位置。</span><span class="sxs-lookup"><span data-stu-id="b8283-121">The location where the corresponding event is held or attended from.</span></span> <span data-ttu-id="b8283-122">可选。</span><span class="sxs-lookup"><span data-stu-id="b8283-122">Optional.</span></span>|
|<span data-ttu-id="b8283-123">start</span><span class="sxs-lookup"><span data-stu-id="b8283-123">start</span></span> |[<span data-ttu-id="b8283-124">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="b8283-124">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="b8283-125">相应事件的开始日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="b8283-125">The date, time, and time zone that the corresponding event starts.</span></span> |
|<span data-ttu-id="b8283-126">status</span><span class="sxs-lookup"><span data-stu-id="b8283-126">status</span></span> |<span data-ttu-id="b8283-127">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="b8283-127">freeBusyStatus</span></span> | <span data-ttu-id="b8283-128">相应事件期间用户或资源的可用性状态。</span><span class="sxs-lookup"><span data-stu-id="b8283-128">The availability status of the user or resource during the corresponding event.</span></span> <span data-ttu-id="b8283-129">可能的值为: `free`、 `tentative`、 `busy` `oof`、、 `workingElsewhere`、 `unknown`。</span><span class="sxs-lookup"><span data-stu-id="b8283-129">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span> |
|<span data-ttu-id="b8283-130">subject</span><span class="sxs-lookup"><span data-stu-id="b8283-130">subject</span></span> |<span data-ttu-id="b8283-131">String</span><span class="sxs-lookup"><span data-stu-id="b8283-131">String</span></span> | <span data-ttu-id="b8283-132">相应事件的主题行。</span><span class="sxs-lookup"><span data-stu-id="b8283-132">The corresponding event's subject line.</span></span> <span data-ttu-id="b8283-133">可选。</span><span class="sxs-lookup"><span data-stu-id="b8283-133">Optional.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="b8283-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b8283-134">JSON representation</span></span>

<span data-ttu-id="b8283-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8283-135">The following is a JSON representation of the resource.</span></span>

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
  "tocPath": ""
}
-->
