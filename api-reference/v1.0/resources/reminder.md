---
title: 提醒资源类型
description: 用户日历中的事件提醒。
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 4e5343299e424d299328ec531ed7c3a52fbc4be2
ms.sourcegitcommit: 60ced1be6ed8dd2d23263090a1cfbc16689bb043
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/28/2020
ms.locfileid: "48782968"
---
# <a name="reminder-resource-type"></a><span data-ttu-id="48665-103">提醒资源类型</span><span class="sxs-lookup"><span data-stu-id="48665-103">reminder resource type</span></span>

<span data-ttu-id="48665-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48665-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="48665-105">用户[日历](calendar.md)中的[事件](event.md)提醒。</span><span class="sxs-lookup"><span data-stu-id="48665-105">A reminder for an [event](event.md) in a user [calendar](calendar.md).</span></span>

## <a name="properties"></a><span data-ttu-id="48665-106">属性</span><span class="sxs-lookup"><span data-stu-id="48665-106">Properties</span></span>
| <span data-ttu-id="48665-107">属性</span><span class="sxs-lookup"><span data-stu-id="48665-107">Property</span></span>     | <span data-ttu-id="48665-108">类型</span><span class="sxs-lookup"><span data-stu-id="48665-108">Type</span></span>   |<span data-ttu-id="48665-109">说明</span><span class="sxs-lookup"><span data-stu-id="48665-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48665-110">changeKey</span><span class="sxs-lookup"><span data-stu-id="48665-110">changeKey</span></span>|<span data-ttu-id="48665-111">String</span><span class="sxs-lookup"><span data-stu-id="48665-111">String</span></span>|<span data-ttu-id="48665-p101">标识提醒的版本。每次提醒更改时， **changeKey** 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。</span><span class="sxs-lookup"><span data-stu-id="48665-p101">Identifies the version of the reminder. Every time the reminder is changed, **changeKey** changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="48665-115">eventEndTime</span><span class="sxs-lookup"><span data-stu-id="48665-115">eventEndTime</span></span>|[<span data-ttu-id="48665-116">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="48665-116">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="48665-117">事件结束的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="48665-117">The date, time and time zone that the event ends.</span></span>|
|<span data-ttu-id="48665-118">eventId</span><span class="sxs-lookup"><span data-stu-id="48665-118">eventId</span></span>|<span data-ttu-id="48665-119">String</span><span class="sxs-lookup"><span data-stu-id="48665-119">String</span></span>|<span data-ttu-id="48665-p102">事件的唯一 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="48665-p102">The unique ID of the event. Read only.</span></span>|
|<span data-ttu-id="48665-122">eventLocation</span><span class="sxs-lookup"><span data-stu-id="48665-122">eventLocation</span></span>|[<span data-ttu-id="48665-123">位置</span><span class="sxs-lookup"><span data-stu-id="48665-123">Location</span></span>](location.md)|<span data-ttu-id="48665-124">事件的位置。</span><span class="sxs-lookup"><span data-stu-id="48665-124">The location of the event.</span></span>|
|<span data-ttu-id="48665-125">eventStartTime</span><span class="sxs-lookup"><span data-stu-id="48665-125">eventStartTime</span></span>|[<span data-ttu-id="48665-126">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="48665-126">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="48665-127">事件开始的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="48665-127">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="48665-128">eventSubject</span><span class="sxs-lookup"><span data-stu-id="48665-128">eventSubject</span></span>|<span data-ttu-id="48665-129">String</span><span class="sxs-lookup"><span data-stu-id="48665-129">String</span></span>|<span data-ttu-id="48665-130">事件的主题行文本。</span><span class="sxs-lookup"><span data-stu-id="48665-130">The text of the event's subject line.</span></span>|
|<span data-ttu-id="48665-131">eventWebLink</span><span class="sxs-lookup"><span data-stu-id="48665-131">eventWebLink</span></span>|<span data-ttu-id="48665-132">String</span><span class="sxs-lookup"><span data-stu-id="48665-132">String</span></span>|<span data-ttu-id="48665-133">要在 Web 上的 Outlook 中打开事件的 URL。</span><span class="sxs-lookup"><span data-stu-id="48665-133">The URL to open the event in Outlook on the web.</span></span><br/><br/><span data-ttu-id="48665-p103">如果你通过 Web 上的 Outlook 登录邮箱，该事件将在浏览器中打开。如果你尚未使用浏览器登录，系统将提示你登录。</span><span class="sxs-lookup"><span data-stu-id="48665-p103">The event will open in the browser if you are logged in to your mailbox via Outlook on the web. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="48665-136">无法从 iFrame 中访问此 URL。</span><span class="sxs-lookup"><span data-stu-id="48665-136">This URL cannot be accessed from within an iFrame.</span></span>|
|<span data-ttu-id="48665-137">reminderFireTime</span><span class="sxs-lookup"><span data-stu-id="48665-137">reminderFireTime</span></span>|[<span data-ttu-id="48665-138">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="48665-138">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="48665-139">设置提醒发生的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="48665-139">The date, time, and time zone that the reminder is set to occur.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="48665-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="48665-140">JSON representation</span></span>

<span data-ttu-id="48665-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="48665-141">Here is a JSON representation of the resource</span></span>

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

