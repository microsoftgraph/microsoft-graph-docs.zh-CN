---
title: scheduleItem 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
ms.openlocfilehash: a7a31f47cde92549a72299b22a40b10c6f7845c6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046870"
---
# <a name="scheduleitem-resource-type"></a><span data-ttu-id="49cca-104">scheduleItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="49cca-104">scheduleItem resource type</span></span>

 > <span data-ttu-id="49cca-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="49cca-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="49cca-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="49cca-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="49cca-107">介绍了在用户的默认日历上与实际事件对应的用户的可用性的项。</span><span class="sxs-lookup"><span data-stu-id="49cca-107">An item that describes the availability of a user corresponding to an actual event on the user's default calendar.</span></span> <span data-ttu-id="49cca-108">此项适用于资源以及。</span><span class="sxs-lookup"><span data-stu-id="49cca-108">This item applies to a resource as well.</span></span>

## <a name="properties"></a><span data-ttu-id="49cca-109">属性</span><span class="sxs-lookup"><span data-stu-id="49cca-109">Properties</span></span>
| <span data-ttu-id="49cca-110">属性</span><span class="sxs-lookup"><span data-stu-id="49cca-110">Property</span></span>     | <span data-ttu-id="49cca-111">类型</span><span class="sxs-lookup"><span data-stu-id="49cca-111">Type</span></span>   |<span data-ttu-id="49cca-112">说明</span><span class="sxs-lookup"><span data-stu-id="49cca-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49cca-113">end</span><span class="sxs-lookup"><span data-stu-id="49cca-113">end</span></span> |[<span data-ttu-id="49cca-114">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="49cca-114">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="49cca-115">日期、 时间和结束对应的事件的时区。</span><span class="sxs-lookup"><span data-stu-id="49cca-115">The date, time, and time zone that the corresponding event ends.</span></span> |
|<span data-ttu-id="49cca-116">isPrivate</span><span class="sxs-lookup"><span data-stu-id="49cca-116">isPrivate</span></span> |<span data-ttu-id="49cca-117">布尔</span><span class="sxs-lookup"><span data-stu-id="49cca-117">Boolean</span></span> |<span data-ttu-id="49cca-118">区分大小写的对应的事件。</span><span class="sxs-lookup"><span data-stu-id="49cca-118">The sensitivity of the corresponding event.</span></span> <span data-ttu-id="49cca-119">如果事件标记为`private`，则返回 false 否则为。</span><span class="sxs-lookup"><span data-stu-id="49cca-119">True if the event is marked `private`, false otherwise.</span></span> |
|<span data-ttu-id="49cca-120">location</span><span class="sxs-lookup"><span data-stu-id="49cca-120">location</span></span> |<span data-ttu-id="49cca-121">字符串</span><span class="sxs-lookup"><span data-stu-id="49cca-121">String</span></span> | <span data-ttu-id="49cca-122">相应的事件是保留或从参加的位置。</span><span class="sxs-lookup"><span data-stu-id="49cca-122">The location where the corresponding event is held or attended from.</span></span> <span data-ttu-id="49cca-123">可选。</span><span class="sxs-lookup"><span data-stu-id="49cca-123">Optional.</span></span>|
|<span data-ttu-id="49cca-124">start</span><span class="sxs-lookup"><span data-stu-id="49cca-124">start</span></span> |[<span data-ttu-id="49cca-125">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="49cca-125">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="49cca-126">日期、 时间和相应事件开始的时区。</span><span class="sxs-lookup"><span data-stu-id="49cca-126">The date, time, and time zone that the corresponding event starts.</span></span> |
|<span data-ttu-id="49cca-127">状态</span><span class="sxs-lookup"><span data-stu-id="49cca-127">status</span></span> |<span data-ttu-id="49cca-128">字符串</span><span class="sxs-lookup"><span data-stu-id="49cca-128">String</span></span> | <span data-ttu-id="49cca-129">可用性的用户或资源的相应事件执行过程的状态。</span><span class="sxs-lookup"><span data-stu-id="49cca-129">The availability status of the user or resource during the corresponding event.</span></span> <span data-ttu-id="49cca-130">可能的值为： `free`， `tentative`， `busy`， `oof`， `workingElsewhere`， `unknown`。</span><span class="sxs-lookup"><span data-stu-id="49cca-130">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span> |
|<span data-ttu-id="49cca-131">subject</span><span class="sxs-lookup"><span data-stu-id="49cca-131">subject</span></span> |<span data-ttu-id="49cca-132">字符串</span><span class="sxs-lookup"><span data-stu-id="49cca-132">String</span></span> | <span data-ttu-id="49cca-133">相应的事件的主题行。</span><span class="sxs-lookup"><span data-stu-id="49cca-133">The corresponding event's subject line.</span></span> <span data-ttu-id="49cca-134">可选。</span><span class="sxs-lookup"><span data-stu-id="49cca-134">Optional.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="49cca-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="49cca-135">JSON representation</span></span>

<span data-ttu-id="49cca-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="49cca-136">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "scheduleItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->