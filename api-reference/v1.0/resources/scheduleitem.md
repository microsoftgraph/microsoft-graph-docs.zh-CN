---
title: scheduleItem 资源类型
description: 一个项目，该项目描述与用户的默认日历上的实际事件相对应的用户的可用性。 此项也适用于资源 (会议室或设备) 。
localization_priority: Normal
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: cad5cfa500d3ae6e68bb1db06688e13e8e0d43e6
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811243"
---
# <a name="scheduleitem-resource-type"></a><span data-ttu-id="dfaad-104">scheduleItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="dfaad-104">scheduleItem resource type</span></span>

<span data-ttu-id="dfaad-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfaad-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dfaad-106">一个项目，该项目描述与用户的默认日历上的实际事件相对应的用户的可用性。</span><span class="sxs-lookup"><span data-stu-id="dfaad-106">An item that describes the availability of a user corresponding to an actual event on the user's default calendar.</span></span> <span data-ttu-id="dfaad-107">此项也适用于资源 (会议室或设备) 。</span><span class="sxs-lookup"><span data-stu-id="dfaad-107">This item applies to a resource (room or equipment) as well.</span></span>

## <a name="properties"></a><span data-ttu-id="dfaad-108">属性</span><span class="sxs-lookup"><span data-stu-id="dfaad-108">Properties</span></span>
| <span data-ttu-id="dfaad-109">属性</span><span class="sxs-lookup"><span data-stu-id="dfaad-109">Property</span></span>     | <span data-ttu-id="dfaad-110">类型</span><span class="sxs-lookup"><span data-stu-id="dfaad-110">Type</span></span>   |<span data-ttu-id="dfaad-111">说明</span><span class="sxs-lookup"><span data-stu-id="dfaad-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dfaad-112">end</span><span class="sxs-lookup"><span data-stu-id="dfaad-112">end</span></span> |[<span data-ttu-id="dfaad-113">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="dfaad-113">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="dfaad-114">相应事件结束时的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="dfaad-114">The date, time, and time zone that the corresponding event ends.</span></span> |
|<span data-ttu-id="dfaad-115">isPrivate</span><span class="sxs-lookup"><span data-stu-id="dfaad-115">isPrivate</span></span> |<span data-ttu-id="dfaad-116">布尔值</span><span class="sxs-lookup"><span data-stu-id="dfaad-116">Boolean</span></span> |<span data-ttu-id="dfaad-117">相应事件的敏感度。</span><span class="sxs-lookup"><span data-stu-id="dfaad-117">The sensitivity of the corresponding event.</span></span> <span data-ttu-id="dfaad-118">如果已标记事件，则为 True `private` ，否则为 false。</span><span class="sxs-lookup"><span data-stu-id="dfaad-118">True if the event is marked `private`, false otherwise.</span></span> <span data-ttu-id="dfaad-119">可选。</span><span class="sxs-lookup"><span data-stu-id="dfaad-119">Optional.</span></span>|
|<span data-ttu-id="dfaad-120">位置</span><span class="sxs-lookup"><span data-stu-id="dfaad-120">location</span></span> |<span data-ttu-id="dfaad-121">String</span><span class="sxs-lookup"><span data-stu-id="dfaad-121">String</span></span> | <span data-ttu-id="dfaad-122">保留或参与的相应事件的位置。</span><span class="sxs-lookup"><span data-stu-id="dfaad-122">The location where the corresponding event is held or attended from.</span></span> <span data-ttu-id="dfaad-123">可选。</span><span class="sxs-lookup"><span data-stu-id="dfaad-123">Optional.</span></span>|
|<span data-ttu-id="dfaad-124">start</span><span class="sxs-lookup"><span data-stu-id="dfaad-124">start</span></span> |[<span data-ttu-id="dfaad-125">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="dfaad-125">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="dfaad-126">相应事件的开始日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="dfaad-126">The date, time, and time zone that the corresponding event starts.</span></span> |
|<span data-ttu-id="dfaad-127">status</span><span class="sxs-lookup"><span data-stu-id="dfaad-127">status</span></span> |<span data-ttu-id="dfaad-128">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="dfaad-128">freeBusyStatus</span></span> | <span data-ttu-id="dfaad-129">相应事件期间用户或资源的可用性状态。</span><span class="sxs-lookup"><span data-stu-id="dfaad-129">The availability status of the user or resource during the corresponding event.</span></span> <span data-ttu-id="dfaad-130">可能的值包括 `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="dfaad-130">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span> |
|<span data-ttu-id="dfaad-131">subject</span><span class="sxs-lookup"><span data-stu-id="dfaad-131">subject</span></span> |<span data-ttu-id="dfaad-132">String</span><span class="sxs-lookup"><span data-stu-id="dfaad-132">String</span></span> | <span data-ttu-id="dfaad-133">相应事件的主题行。</span><span class="sxs-lookup"><span data-stu-id="dfaad-133">The corresponding event's subject line.</span></span> <span data-ttu-id="dfaad-134">可选。</span><span class="sxs-lookup"><span data-stu-id="dfaad-134">Optional.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="dfaad-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dfaad-135">JSON representation</span></span>

<span data-ttu-id="dfaad-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dfaad-136">The following is a JSON representation of the resource.</span></span>

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
