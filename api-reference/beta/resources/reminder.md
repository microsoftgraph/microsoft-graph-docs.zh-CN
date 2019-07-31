---
title: 提醒资源类型
description: 用户日历中的事件提醒。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4b2a0e86a87420bb59f35371ec957e004e2fa9fe
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965437"
---
# <a name="reminder-resource-type"></a><span data-ttu-id="d849a-103">提醒资源类型</span><span class="sxs-lookup"><span data-stu-id="d849a-103">reminder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d849a-104">用户[日历](calendar.md)中的[事件](event.md)提醒。</span><span class="sxs-lookup"><span data-stu-id="d849a-104">A reminder for an [event](event.md) in a user [calendar](calendar.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d849a-105">属性</span><span class="sxs-lookup"><span data-stu-id="d849a-105">Properties</span></span>
| <span data-ttu-id="d849a-106">属性</span><span class="sxs-lookup"><span data-stu-id="d849a-106">Property</span></span>     | <span data-ttu-id="d849a-107">类型</span><span class="sxs-lookup"><span data-stu-id="d849a-107">Type</span></span>   |<span data-ttu-id="d849a-108">说明</span><span class="sxs-lookup"><span data-stu-id="d849a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d849a-109">changeKey</span><span class="sxs-lookup"><span data-stu-id="d849a-109">changeKey</span></span>|<span data-ttu-id="d849a-110">String</span><span class="sxs-lookup"><span data-stu-id="d849a-110">String</span></span>|<span data-ttu-id="d849a-p101">标识提醒的版本。每次提醒更改时，**changeKey** 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。</span><span class="sxs-lookup"><span data-stu-id="d849a-p101">Identifies the version of the reminder. Every time the reminder is changed, **changeKey** changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="d849a-114">eventEndTime</span><span class="sxs-lookup"><span data-stu-id="d849a-114">eventEndTime</span></span>|[<span data-ttu-id="d849a-115">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="d849a-115">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="d849a-116">事件结束的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="d849a-116">The date, time and time zone that the event ends.</span></span>|
|<span data-ttu-id="d849a-117">eventId</span><span class="sxs-lookup"><span data-stu-id="d849a-117">eventId</span></span>|<span data-ttu-id="d849a-118">字符串</span><span class="sxs-lookup"><span data-stu-id="d849a-118">String</span></span>|<span data-ttu-id="d849a-p102">事件的唯一 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="d849a-p102">The unique ID of the event. Read only.</span></span>|
|<span data-ttu-id="d849a-121">eventLocation</span><span class="sxs-lookup"><span data-stu-id="d849a-121">eventLocation</span></span>|[<span data-ttu-id="d849a-122">位置</span><span class="sxs-lookup"><span data-stu-id="d849a-122">Location</span></span>](location.md)|<span data-ttu-id="d849a-123">事件的位置。</span><span class="sxs-lookup"><span data-stu-id="d849a-123">The location of the event.</span></span>|
|<span data-ttu-id="d849a-124">eventStartTime</span><span class="sxs-lookup"><span data-stu-id="d849a-124">eventStartTime</span></span>|[<span data-ttu-id="d849a-125">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="d849a-125">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="d849a-126">事件开始的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="d849a-126">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="d849a-127">eventSubject</span><span class="sxs-lookup"><span data-stu-id="d849a-127">eventSubject</span></span>|<span data-ttu-id="d849a-128">String</span><span class="sxs-lookup"><span data-stu-id="d849a-128">String</span></span>|<span data-ttu-id="d849a-129">事件的主题行文本。</span><span class="sxs-lookup"><span data-stu-id="d849a-129">The text of the event's subject line.</span></span>|
|<span data-ttu-id="d849a-130">eventWebLink</span><span class="sxs-lookup"><span data-stu-id="d849a-130">eventWebLink</span></span>|<span data-ttu-id="d849a-131">String</span><span class="sxs-lookup"><span data-stu-id="d849a-131">String</span></span>|<span data-ttu-id="d849a-132">要在 Web 上的 Outlook 中打开事件的 URL。</span><span class="sxs-lookup"><span data-stu-id="d849a-132">The URL to open the event in Outlook on the web.</span></span><br/><br/><span data-ttu-id="d849a-p103">如果你通过 Web 上的 Outlook 登录邮箱，该事件将在浏览器中打开。如果你尚未使用浏览器登录，系统将提示你登录。</span><span class="sxs-lookup"><span data-stu-id="d849a-p103">The event will open in the browser if you are logged in to your mailbox via Outlook on the web. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="d849a-135">可以从 iFrame 中访问此 URL。</span><span class="sxs-lookup"><span data-stu-id="d849a-135">This URL can be accessed from within an iFrame.</span></span>|
|<span data-ttu-id="d849a-136">reminderFireTime</span><span class="sxs-lookup"><span data-stu-id="d849a-136">reminderFireTime</span></span>|[<span data-ttu-id="d849a-137">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="d849a-137">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="d849a-138">设置提醒发生的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="d849a-138">The date, time, and time zone that the reminder is set to occur.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d849a-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d849a-139">JSON representation</span></span>

<span data-ttu-id="d849a-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d849a-140">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "reminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
