---
title: 提醒资源类型
description: 用户日历中的事件提醒。
localization_priority: Normal
ms.openlocfilehash: 88d9cb4f30f60819a606b3b1f3573d16860d9a00
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563125"
---
# <a name="reminder-resource-type"></a><span data-ttu-id="3d34e-103">提醒资源类型</span><span class="sxs-lookup"><span data-stu-id="3d34e-103">reminder resource type</span></span>

<span data-ttu-id="3d34e-104">用户[日历](calendar.md)中的[事件](event.md)提醒。</span><span class="sxs-lookup"><span data-stu-id="3d34e-104">A reminder for an [event](event.md) in a user [calendar](calendar.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3d34e-105">属性</span><span class="sxs-lookup"><span data-stu-id="3d34e-105">Properties</span></span>
| <span data-ttu-id="3d34e-106">属性</span><span class="sxs-lookup"><span data-stu-id="3d34e-106">Property</span></span>     | <span data-ttu-id="3d34e-107">类型</span><span class="sxs-lookup"><span data-stu-id="3d34e-107">Type</span></span>   |<span data-ttu-id="3d34e-108">说明</span><span class="sxs-lookup"><span data-stu-id="3d34e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3d34e-109">changeKey</span><span class="sxs-lookup"><span data-stu-id="3d34e-109">changeKey</span></span>|<span data-ttu-id="3d34e-110">String</span><span class="sxs-lookup"><span data-stu-id="3d34e-110">String</span></span>|<span data-ttu-id="3d34e-p101">标识提醒的版本。每次提醒更改时，**changeKey** 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。</span><span class="sxs-lookup"><span data-stu-id="3d34e-p101">Identifies the version of the reminder. Every time the reminder is changed, **changeKey** changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="3d34e-114">eventEndTime</span><span class="sxs-lookup"><span data-stu-id="3d34e-114">eventEndTime</span></span>|[<span data-ttu-id="3d34e-115">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="3d34e-115">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="3d34e-116">事件结束的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="3d34e-116">The date, time and time zone that the event ends.</span></span>|
|<span data-ttu-id="3d34e-117">eventId</span><span class="sxs-lookup"><span data-stu-id="3d34e-117">eventId</span></span>|<span data-ttu-id="3d34e-118">字符串</span><span class="sxs-lookup"><span data-stu-id="3d34e-118">String</span></span>|<span data-ttu-id="3d34e-p102">事件的唯一 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="3d34e-p102">The unique ID of the event. Read only.</span></span>|
|<span data-ttu-id="3d34e-121">eventLocation</span><span class="sxs-lookup"><span data-stu-id="3d34e-121">eventLocation</span></span>|[<span data-ttu-id="3d34e-122">位置</span><span class="sxs-lookup"><span data-stu-id="3d34e-122">Location</span></span>](location.md)|<span data-ttu-id="3d34e-123">事件的位置。</span><span class="sxs-lookup"><span data-stu-id="3d34e-123">The location of the event.</span></span>|
|<span data-ttu-id="3d34e-124">eventStartTime</span><span class="sxs-lookup"><span data-stu-id="3d34e-124">eventStartTime</span></span>|[<span data-ttu-id="3d34e-125">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="3d34e-125">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="3d34e-126">事件开始的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="3d34e-126">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="3d34e-127">eventSubject</span><span class="sxs-lookup"><span data-stu-id="3d34e-127">eventSubject</span></span>|<span data-ttu-id="3d34e-128">String</span><span class="sxs-lookup"><span data-stu-id="3d34e-128">String</span></span>|<span data-ttu-id="3d34e-129">事件的主题行文本。</span><span class="sxs-lookup"><span data-stu-id="3d34e-129">The text of the event's subject line.</span></span>|
|<span data-ttu-id="3d34e-130">eventWebLink</span><span class="sxs-lookup"><span data-stu-id="3d34e-130">eventWebLink</span></span>|<span data-ttu-id="3d34e-131">String</span><span class="sxs-lookup"><span data-stu-id="3d34e-131">String</span></span>|<span data-ttu-id="3d34e-132">要在 Web 上的 Outlook 中打开事件的 URL。</span><span class="sxs-lookup"><span data-stu-id="3d34e-132">The URL to open the event in Outlook on the web.</span></span><br/><br/><span data-ttu-id="3d34e-p103">如果你通过 Web 上的 Outlook 登录邮箱，该事件将在浏览器中打开。如果你尚未使用浏览器登录，系统将提示你登录。</span><span class="sxs-lookup"><span data-stu-id="3d34e-p103">The event will open in the browser if you are logged in to your mailbox via Outlook on the web. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="3d34e-135">可以从 iFrame 中访问此 URL。</span><span class="sxs-lookup"><span data-stu-id="3d34e-135">This URL can be accessed from within an iFrame.</span></span>|
|<span data-ttu-id="3d34e-136">reminderFireTime</span><span class="sxs-lookup"><span data-stu-id="3d34e-136">reminderFireTime</span></span>|[<span data-ttu-id="3d34e-137">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="3d34e-137">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="3d34e-138">设置提醒发生的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="3d34e-138">The date, time, and time zone that the reminder is set to occur.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3d34e-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3d34e-139">JSON representation</span></span>

<span data-ttu-id="3d34e-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3d34e-140">Here is a JSON representation of the resource</span></span>

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
