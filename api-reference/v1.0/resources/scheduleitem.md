---
title: scheduleItem 资源类型
description: 一个项目，该项目描述与用户的默认日历上的实际事件相对应的用户的可用性。 此项也适用于资源（会议室或设备）。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 4136b71dfb273525e8793521d50545ee5b1873cb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533794"
---
# <a name="scheduleitem-resource-type"></a><span data-ttu-id="5abf8-104">scheduleItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="5abf8-104">scheduleItem resource type</span></span>

<span data-ttu-id="5abf8-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5abf8-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5abf8-106">一个项目，该项目描述与用户的默认日历上的实际事件相对应的用户的可用性。</span><span class="sxs-lookup"><span data-stu-id="5abf8-106">An item that describes the availability of a user corresponding to an actual event on the user's default calendar.</span></span> <span data-ttu-id="5abf8-107">此项也适用于资源（会议室或设备）。</span><span class="sxs-lookup"><span data-stu-id="5abf8-107">This item applies to a resource (room or equipment) as well.</span></span>

## <a name="properties"></a><span data-ttu-id="5abf8-108">属性</span><span class="sxs-lookup"><span data-stu-id="5abf8-108">Properties</span></span>
| <span data-ttu-id="5abf8-109">属性</span><span class="sxs-lookup"><span data-stu-id="5abf8-109">Property</span></span>     | <span data-ttu-id="5abf8-110">类型</span><span class="sxs-lookup"><span data-stu-id="5abf8-110">Type</span></span>   |<span data-ttu-id="5abf8-111">说明</span><span class="sxs-lookup"><span data-stu-id="5abf8-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5abf8-112">end</span><span class="sxs-lookup"><span data-stu-id="5abf8-112">end</span></span> |[<span data-ttu-id="5abf8-113">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="5abf8-113">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="5abf8-114">相应事件结束时的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="5abf8-114">The date, time, and time zone that the corresponding event ends.</span></span> |
|<span data-ttu-id="5abf8-115">isPrivate</span><span class="sxs-lookup"><span data-stu-id="5abf8-115">isPrivate</span></span> |<span data-ttu-id="5abf8-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="5abf8-116">Boolean</span></span> |<span data-ttu-id="5abf8-117">相应事件的敏感度。</span><span class="sxs-lookup"><span data-stu-id="5abf8-117">The sensitivity of the corresponding event.</span></span> <span data-ttu-id="5abf8-118">如果已标记`private`事件，则为 True，否则为 false。</span><span class="sxs-lookup"><span data-stu-id="5abf8-118">True if the event is marked `private`, false otherwise.</span></span> <span data-ttu-id="5abf8-119">可选。</span><span class="sxs-lookup"><span data-stu-id="5abf8-119">Optional.</span></span>|
|<span data-ttu-id="5abf8-120">位置</span><span class="sxs-lookup"><span data-stu-id="5abf8-120">location</span></span> |<span data-ttu-id="5abf8-121">字符串</span><span class="sxs-lookup"><span data-stu-id="5abf8-121">String</span></span> | <span data-ttu-id="5abf8-122">保留或参与的相应事件的位置。</span><span class="sxs-lookup"><span data-stu-id="5abf8-122">The location where the corresponding event is held or attended from.</span></span> <span data-ttu-id="5abf8-123">可选。</span><span class="sxs-lookup"><span data-stu-id="5abf8-123">Optional.</span></span>|
|<span data-ttu-id="5abf8-124">start</span><span class="sxs-lookup"><span data-stu-id="5abf8-124">start</span></span> |[<span data-ttu-id="5abf8-125">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="5abf8-125">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="5abf8-126">相应事件的开始日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="5abf8-126">The date, time, and time zone that the corresponding event starts.</span></span> |
|<span data-ttu-id="5abf8-127">状态</span><span class="sxs-lookup"><span data-stu-id="5abf8-127">status</span></span> |<span data-ttu-id="5abf8-128">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="5abf8-128">freeBusyStatus</span></span> | <span data-ttu-id="5abf8-129">相应事件期间用户或资源的可用性状态。</span><span class="sxs-lookup"><span data-stu-id="5abf8-129">The availability status of the user or resource during the corresponding event.</span></span> <span data-ttu-id="5abf8-130">可能的值包括 `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="5abf8-130">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span> |
|<span data-ttu-id="5abf8-131">subject</span><span class="sxs-lookup"><span data-stu-id="5abf8-131">subject</span></span> |<span data-ttu-id="5abf8-132">String</span><span class="sxs-lookup"><span data-stu-id="5abf8-132">String</span></span> | <span data-ttu-id="5abf8-133">相应事件的主题行。</span><span class="sxs-lookup"><span data-stu-id="5abf8-133">The corresponding event's subject line.</span></span> <span data-ttu-id="5abf8-134">可选。</span><span class="sxs-lookup"><span data-stu-id="5abf8-134">Optional.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="5abf8-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5abf8-135">JSON representation</span></span>

<span data-ttu-id="5abf8-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5abf8-136">The following is a JSON representation of the resource.</span></span>

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
