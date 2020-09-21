---
title: 提醒资源类型
description: 用户日历中的事件提醒。
localization_priority: Normal
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1cb61064b05668193947043998749e6306d3d606
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002952"
---
# <a name="reminder-resource-type"></a><span data-ttu-id="8fb61-103">提醒资源类型</span><span class="sxs-lookup"><span data-stu-id="8fb61-103">reminder resource type</span></span>

<span data-ttu-id="8fb61-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8fb61-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8fb61-105">用户[日历](calendar.md)中的[事件](event.md)提醒。</span><span class="sxs-lookup"><span data-stu-id="8fb61-105">A reminder for an [event](event.md) in a user [calendar](calendar.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8fb61-106">属性</span><span class="sxs-lookup"><span data-stu-id="8fb61-106">Properties</span></span>
| <span data-ttu-id="8fb61-107">属性</span><span class="sxs-lookup"><span data-stu-id="8fb61-107">Property</span></span>     | <span data-ttu-id="8fb61-108">类型</span><span class="sxs-lookup"><span data-stu-id="8fb61-108">Type</span></span>   |<span data-ttu-id="8fb61-109">说明</span><span class="sxs-lookup"><span data-stu-id="8fb61-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8fb61-110">changeKey</span><span class="sxs-lookup"><span data-stu-id="8fb61-110">changeKey</span></span>|<span data-ttu-id="8fb61-111">String</span><span class="sxs-lookup"><span data-stu-id="8fb61-111">String</span></span>|<span data-ttu-id="8fb61-p101">标识提醒的版本。每次提醒更改时，**changeKey** 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。</span><span class="sxs-lookup"><span data-stu-id="8fb61-p101">Identifies the version of the reminder. Every time the reminder is changed, **changeKey** changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="8fb61-115">eventEndTime</span><span class="sxs-lookup"><span data-stu-id="8fb61-115">eventEndTime</span></span>|[<span data-ttu-id="8fb61-116">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="8fb61-116">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="8fb61-117">事件结束的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="8fb61-117">The date, time and time zone that the event ends.</span></span>|
|<span data-ttu-id="8fb61-118">eventId</span><span class="sxs-lookup"><span data-stu-id="8fb61-118">eventId</span></span>|<span data-ttu-id="8fb61-119">String</span><span class="sxs-lookup"><span data-stu-id="8fb61-119">String</span></span>|<span data-ttu-id="8fb61-p102">事件的唯一 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="8fb61-p102">The unique ID of the event. Read only.</span></span>|
|<span data-ttu-id="8fb61-122">eventLocation</span><span class="sxs-lookup"><span data-stu-id="8fb61-122">eventLocation</span></span>|[<span data-ttu-id="8fb61-123">位置</span><span class="sxs-lookup"><span data-stu-id="8fb61-123">Location</span></span>](location.md)|<span data-ttu-id="8fb61-124">事件的位置。</span><span class="sxs-lookup"><span data-stu-id="8fb61-124">The location of the event.</span></span>|
|<span data-ttu-id="8fb61-125">eventStartTime</span><span class="sxs-lookup"><span data-stu-id="8fb61-125">eventStartTime</span></span>|[<span data-ttu-id="8fb61-126">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="8fb61-126">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="8fb61-127">事件开始的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="8fb61-127">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="8fb61-128">eventSubject</span><span class="sxs-lookup"><span data-stu-id="8fb61-128">eventSubject</span></span>|<span data-ttu-id="8fb61-129">String</span><span class="sxs-lookup"><span data-stu-id="8fb61-129">String</span></span>|<span data-ttu-id="8fb61-130">事件的主题行文本。</span><span class="sxs-lookup"><span data-stu-id="8fb61-130">The text of the event's subject line.</span></span>|
|<span data-ttu-id="8fb61-131">eventWebLink</span><span class="sxs-lookup"><span data-stu-id="8fb61-131">eventWebLink</span></span>|<span data-ttu-id="8fb61-132">String</span><span class="sxs-lookup"><span data-stu-id="8fb61-132">String</span></span>|<span data-ttu-id="8fb61-133">要在 Web 上的 Outlook 中打开事件的 URL。</span><span class="sxs-lookup"><span data-stu-id="8fb61-133">The URL to open the event in Outlook on the web.</span></span><br/><br/><span data-ttu-id="8fb61-p103">如果你通过 Web 上的 Outlook 登录邮箱，该事件将在浏览器中打开。如果你尚未使用浏览器登录，系统将提示你登录。</span><span class="sxs-lookup"><span data-stu-id="8fb61-p103">The event will open in the browser if you are logged in to your mailbox via Outlook on the web. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="8fb61-136">可以从 iFrame 中访问此 URL。</span><span class="sxs-lookup"><span data-stu-id="8fb61-136">This URL can be accessed from within an iFrame.</span></span>|
|<span data-ttu-id="8fb61-137">reminderFireTime</span><span class="sxs-lookup"><span data-stu-id="8fb61-137">reminderFireTime</span></span>|[<span data-ttu-id="8fb61-138">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="8fb61-138">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="8fb61-139">设置提醒发生的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="8fb61-139">The date, time, and time zone that the reminder is set to occur.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8fb61-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8fb61-140">JSON representation</span></span>

<span data-ttu-id="8fb61-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8fb61-141">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reminder"
}-->

```json
{
  "changeKey": "string",
  "eventEndTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "eventId": "string",
  "eventLocation": {"@odata.type": "microsoft.graph.location"},
  "eventStartTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "eventSubject": "string",
  "eventWebLink": "string",
  "reminderFireTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

