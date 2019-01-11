---
title: 提醒资源类型
description: 用户日历中的事件提醒。
localization_priority: Normal
ms.openlocfilehash: a78c7f82ea0a7db9da45a60de98bb3b1311aaeeb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819962"
---
# <a name="reminder-resource-type"></a><span data-ttu-id="69ffd-103">提醒资源类型</span><span class="sxs-lookup"><span data-stu-id="69ffd-103">reminder resource type</span></span>

> <span data-ttu-id="69ffd-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="69ffd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="69ffd-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="69ffd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="69ffd-106">用户[日历](calendar.md)中的[事件](event.md)提醒。</span><span class="sxs-lookup"><span data-stu-id="69ffd-106">A reminder for an [event](event.md) in a user [calendar](calendar.md).</span></span>

## <a name="properties"></a><span data-ttu-id="69ffd-107">属性</span><span class="sxs-lookup"><span data-stu-id="69ffd-107">Properties</span></span>
| <span data-ttu-id="69ffd-108">属性</span><span class="sxs-lookup"><span data-stu-id="69ffd-108">Property</span></span>     | <span data-ttu-id="69ffd-109">类型</span><span class="sxs-lookup"><span data-stu-id="69ffd-109">Type</span></span>   |<span data-ttu-id="69ffd-110">说明</span><span class="sxs-lookup"><span data-stu-id="69ffd-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69ffd-111">changeKey</span><span class="sxs-lookup"><span data-stu-id="69ffd-111">changeKey</span></span>|<span data-ttu-id="69ffd-112">String</span><span class="sxs-lookup"><span data-stu-id="69ffd-112">String</span></span>|<span data-ttu-id="69ffd-p102">标识提醒的版本。每次提醒更改时，**changeKey** 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。</span><span class="sxs-lookup"><span data-stu-id="69ffd-p102">Identifies the version of the reminder. Every time the reminder is changed, **changeKey** changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="69ffd-116">eventEndTime</span><span class="sxs-lookup"><span data-stu-id="69ffd-116">eventEndTime</span></span>|[<span data-ttu-id="69ffd-117">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="69ffd-117">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="69ffd-118">事件结束的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="69ffd-118">The date, time and time zone that the event ends.</span></span>|
|<span data-ttu-id="69ffd-119">eventId</span><span class="sxs-lookup"><span data-stu-id="69ffd-119">eventId</span></span>|<span data-ttu-id="69ffd-120">字符串</span><span class="sxs-lookup"><span data-stu-id="69ffd-120">String</span></span>|<span data-ttu-id="69ffd-p103">事件的唯一 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="69ffd-p103">The unique ID of the event. Read only.</span></span>|
|<span data-ttu-id="69ffd-123">eventLocation</span><span class="sxs-lookup"><span data-stu-id="69ffd-123">eventLocation</span></span>|[<span data-ttu-id="69ffd-124">位置</span><span class="sxs-lookup"><span data-stu-id="69ffd-124">Location</span></span>](location.md)|<span data-ttu-id="69ffd-125">事件的位置。</span><span class="sxs-lookup"><span data-stu-id="69ffd-125">The location of the event.</span></span>|
|<span data-ttu-id="69ffd-126">eventStartTime</span><span class="sxs-lookup"><span data-stu-id="69ffd-126">eventStartTime</span></span>|[<span data-ttu-id="69ffd-127">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="69ffd-127">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="69ffd-128">事件开始的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="69ffd-128">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="69ffd-129">eventSubject</span><span class="sxs-lookup"><span data-stu-id="69ffd-129">eventSubject</span></span>|<span data-ttu-id="69ffd-130">String</span><span class="sxs-lookup"><span data-stu-id="69ffd-130">String</span></span>|<span data-ttu-id="69ffd-131">事件的主题行文本。</span><span class="sxs-lookup"><span data-stu-id="69ffd-131">The text of the event's subject line.</span></span>|
|<span data-ttu-id="69ffd-132">eventWebLink</span><span class="sxs-lookup"><span data-stu-id="69ffd-132">eventWebLink</span></span>|<span data-ttu-id="69ffd-133">String</span><span class="sxs-lookup"><span data-stu-id="69ffd-133">String</span></span>|<span data-ttu-id="69ffd-134">要在 Web 上的 Outlook 中打开事件的 URL。</span><span class="sxs-lookup"><span data-stu-id="69ffd-134">The URL to open the event in Outlook on the web.</span></span><br/><br/><span data-ttu-id="69ffd-p104">如果你通过 Web 上的 Outlook 登录邮箱，该事件将在浏览器中打开。如果你尚未使用浏览器登录，系统将提示你登录。</span><span class="sxs-lookup"><span data-stu-id="69ffd-p104">The event will open in the browser if you are logged in to your mailbox via Outlook on the web. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="69ffd-137">可以从 iFrame 中访问此 URL。</span><span class="sxs-lookup"><span data-stu-id="69ffd-137">This URL can be accessed from within an iFrame.</span></span>|
|<span data-ttu-id="69ffd-138">reminderFireTime</span><span class="sxs-lookup"><span data-stu-id="69ffd-138">reminderFireTime</span></span>|[<span data-ttu-id="69ffd-139">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="69ffd-139">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="69ffd-140">设置提醒发生的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="69ffd-140">The date, time, and time zone that the reminder is set to occur.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="69ffd-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="69ffd-141">JSON representation</span></span>

<span data-ttu-id="69ffd-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69ffd-142">Here is a JSON representation of the resource</span></span>

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
