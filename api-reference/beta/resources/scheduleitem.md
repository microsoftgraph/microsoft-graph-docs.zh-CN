---
title: scheduleItem 资源类型
description: 一个项目, 该项目描述与用户的默认日历上的实际事件相对应的用户的可用性。 此项也适用于资源。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-teams
author: ''
ms.openlocfilehash: f2901412dcf1d52d8b117afa214da159b4553a8a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008640"
---
# <a name="scheduleitem-resource-type"></a><span data-ttu-id="15d06-104">scheduleItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="15d06-104">scheduleItem resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="15d06-105">一个项目, 该项目描述与用户的默认日历上的实际事件相对应的用户的可用性。</span><span class="sxs-lookup"><span data-stu-id="15d06-105">An item that describes the availability of a user corresponding to an actual event on the user's default calendar.</span></span> <span data-ttu-id="15d06-106">此项也适用于资源 (会议室或设备)。</span><span class="sxs-lookup"><span data-stu-id="15d06-106">This item applies to a resource (room or equipment) as well.</span></span>

## <a name="properties"></a><span data-ttu-id="15d06-107">属性</span><span class="sxs-lookup"><span data-stu-id="15d06-107">Properties</span></span>
| <span data-ttu-id="15d06-108">属性</span><span class="sxs-lookup"><span data-stu-id="15d06-108">Property</span></span>     | <span data-ttu-id="15d06-109">类型</span><span class="sxs-lookup"><span data-stu-id="15d06-109">Type</span></span>   |<span data-ttu-id="15d06-110">说明</span><span class="sxs-lookup"><span data-stu-id="15d06-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="15d06-111">end</span><span class="sxs-lookup"><span data-stu-id="15d06-111">end</span></span> |[<span data-ttu-id="15d06-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="15d06-112">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="15d06-113">相应事件结束时的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="15d06-113">The date, time, and time zone that the corresponding event ends.</span></span> |
|<span data-ttu-id="15d06-114">isPrivate</span><span class="sxs-lookup"><span data-stu-id="15d06-114">isPrivate</span></span> |<span data-ttu-id="15d06-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="15d06-115">Boolean</span></span> |<span data-ttu-id="15d06-116">相应事件的敏感度。</span><span class="sxs-lookup"><span data-stu-id="15d06-116">The sensitivity of the corresponding event.</span></span> <span data-ttu-id="15d06-117">如果已标记`private`事件, 则为 True, 否则为 false。</span><span class="sxs-lookup"><span data-stu-id="15d06-117">True if the event is marked `private`, false otherwise.</span></span> <span data-ttu-id="15d06-118">可选。</span><span class="sxs-lookup"><span data-stu-id="15d06-118">Optional.</span></span> |
|<span data-ttu-id="15d06-119">location</span><span class="sxs-lookup"><span data-stu-id="15d06-119">location</span></span> |<span data-ttu-id="15d06-120">String</span><span class="sxs-lookup"><span data-stu-id="15d06-120">String</span></span> | <span data-ttu-id="15d06-121">保留或参与的相应事件的位置。</span><span class="sxs-lookup"><span data-stu-id="15d06-121">The location where the corresponding event is held or attended from.</span></span> <span data-ttu-id="15d06-122">可选。</span><span class="sxs-lookup"><span data-stu-id="15d06-122">Optional.</span></span>|
|<span data-ttu-id="15d06-123">start</span><span class="sxs-lookup"><span data-stu-id="15d06-123">start</span></span> |[<span data-ttu-id="15d06-124">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="15d06-124">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="15d06-125">相应事件的开始日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="15d06-125">The date, time, and time zone that the corresponding event starts.</span></span> |
|<span data-ttu-id="15d06-126">status</span><span class="sxs-lookup"><span data-stu-id="15d06-126">status</span></span> |<span data-ttu-id="15d06-127">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="15d06-127">freeBusyStatus</span></span> | <span data-ttu-id="15d06-128">相应事件期间用户或资源的可用性状态。</span><span class="sxs-lookup"><span data-stu-id="15d06-128">The availability status of the user or resource during the corresponding event.</span></span> <span data-ttu-id="15d06-129">可能的值包括 `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="15d06-129">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span> |
|<span data-ttu-id="15d06-130">subject</span><span class="sxs-lookup"><span data-stu-id="15d06-130">subject</span></span> |<span data-ttu-id="15d06-131">String</span><span class="sxs-lookup"><span data-stu-id="15d06-131">String</span></span> | <span data-ttu-id="15d06-132">相应事件的主题行。</span><span class="sxs-lookup"><span data-stu-id="15d06-132">The corresponding event's subject line.</span></span> <span data-ttu-id="15d06-133">可选。</span><span class="sxs-lookup"><span data-stu-id="15d06-133">Optional.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="15d06-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="15d06-134">JSON representation</span></span>

<span data-ttu-id="15d06-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="15d06-135">The following is a JSON representation of the resource.</span></span>

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
