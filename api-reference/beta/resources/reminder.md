---
title: 提醒资源类型
description: 用户日历中的事件提醒。
localization_priority: Normal
ms.openlocfilehash: 88d9cb4f30f60819a606b3b1f3573d16860d9a00
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521031"
---
# <a name="reminder-resource-type"></a><span data-ttu-id="258e7-103">提醒资源类型</span><span class="sxs-lookup"><span data-stu-id="258e7-103">reminder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="258e7-104">用户[日历](calendar.md)中的[事件](event.md)提醒。</span><span class="sxs-lookup"><span data-stu-id="258e7-104">A reminder for an [event](event.md) in a user [calendar](calendar.md).</span></span>

## <a name="properties"></a><span data-ttu-id="258e7-105">属性</span><span class="sxs-lookup"><span data-stu-id="258e7-105">Properties</span></span>
| <span data-ttu-id="258e7-106">属性</span><span class="sxs-lookup"><span data-stu-id="258e7-106">Property</span></span>     | <span data-ttu-id="258e7-107">类型</span><span class="sxs-lookup"><span data-stu-id="258e7-107">Type</span></span>   |<span data-ttu-id="258e7-108">说明</span><span class="sxs-lookup"><span data-stu-id="258e7-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="258e7-109">changeKey</span><span class="sxs-lookup"><span data-stu-id="258e7-109">changeKey</span></span>|<span data-ttu-id="258e7-110">String</span><span class="sxs-lookup"><span data-stu-id="258e7-110">String</span></span>|<span data-ttu-id="258e7-p101">标识提醒的版本。每次提醒更改时，**changeKey** 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。</span><span class="sxs-lookup"><span data-stu-id="258e7-p101">Identifies the version of the reminder. Every time the reminder is changed, **changeKey** changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="258e7-114">eventEndTime</span><span class="sxs-lookup"><span data-stu-id="258e7-114">eventEndTime</span></span>|[<span data-ttu-id="258e7-115">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="258e7-115">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="258e7-116">事件结束的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="258e7-116">The date, time and time zone that the event ends.</span></span>|
|<span data-ttu-id="258e7-117">eventId</span><span class="sxs-lookup"><span data-stu-id="258e7-117">eventId</span></span>|<span data-ttu-id="258e7-118">字符串</span><span class="sxs-lookup"><span data-stu-id="258e7-118">String</span></span>|<span data-ttu-id="258e7-p102">事件的唯一 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="258e7-p102">The unique ID of the event. Read only.</span></span>|
|<span data-ttu-id="258e7-121">eventLocation</span><span class="sxs-lookup"><span data-stu-id="258e7-121">eventLocation</span></span>|[<span data-ttu-id="258e7-122">位置</span><span class="sxs-lookup"><span data-stu-id="258e7-122">Location</span></span>](location.md)|<span data-ttu-id="258e7-123">事件的位置。</span><span class="sxs-lookup"><span data-stu-id="258e7-123">The location of the event.</span></span>|
|<span data-ttu-id="258e7-124">eventStartTime</span><span class="sxs-lookup"><span data-stu-id="258e7-124">eventStartTime</span></span>|[<span data-ttu-id="258e7-125">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="258e7-125">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="258e7-126">事件开始的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="258e7-126">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="258e7-127">eventSubject</span><span class="sxs-lookup"><span data-stu-id="258e7-127">eventSubject</span></span>|<span data-ttu-id="258e7-128">String</span><span class="sxs-lookup"><span data-stu-id="258e7-128">String</span></span>|<span data-ttu-id="258e7-129">事件的主题行文本。</span><span class="sxs-lookup"><span data-stu-id="258e7-129">The text of the event's subject line.</span></span>|
|<span data-ttu-id="258e7-130">eventWebLink</span><span class="sxs-lookup"><span data-stu-id="258e7-130">eventWebLink</span></span>|<span data-ttu-id="258e7-131">String</span><span class="sxs-lookup"><span data-stu-id="258e7-131">String</span></span>|<span data-ttu-id="258e7-132">要在 Web 上的 Outlook 中打开事件的 URL。</span><span class="sxs-lookup"><span data-stu-id="258e7-132">The URL to open the event in Outlook on the web.</span></span><br/><br/><span data-ttu-id="258e7-p103">如果你通过 Web 上的 Outlook 登录邮箱，该事件将在浏览器中打开。如果你尚未使用浏览器登录，系统将提示你登录。</span><span class="sxs-lookup"><span data-stu-id="258e7-p103">The event will open in the browser if you are logged in to your mailbox via Outlook on the web. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="258e7-135">可以从 iFrame 中访问此 URL。</span><span class="sxs-lookup"><span data-stu-id="258e7-135">This URL can be accessed from within an iFrame.</span></span>|
|<span data-ttu-id="258e7-136">reminderFireTime</span><span class="sxs-lookup"><span data-stu-id="258e7-136">reminderFireTime</span></span>|[<span data-ttu-id="258e7-137">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="258e7-137">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="258e7-138">设置提醒发生的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="258e7-138">The date, time, and time zone that the reminder is set to occur.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="258e7-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="258e7-139">JSON representation</span></span>

<span data-ttu-id="258e7-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="258e7-140">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/reminder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
