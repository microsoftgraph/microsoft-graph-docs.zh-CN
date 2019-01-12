---
title: 'user: reminderView'
description: '返回指定开始时间和结束时间范围内的日历提醒列表。 '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3fb0283aaae4f814f06b59a8a6ad6183cc18fec1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918208"
---
# <a name="user-reminderview"></a><span data-ttu-id="2b26d-103">user: reminderView</span><span class="sxs-lookup"><span data-stu-id="2b26d-103">user: reminderView</span></span>

> <span data-ttu-id="2b26d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2b26d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b26d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2b26d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2b26d-106">返回一组事件提醒中用户日历中指定的开始和结束时间。</span><span class="sxs-lookup"><span data-stu-id="2b26d-106">Return a list of event reminders in a user calendar within the specified start and end times.</span></span> 

## <a name="permissions"></a><span data-ttu-id="2b26d-107">权限</span><span class="sxs-lookup"><span data-stu-id="2b26d-107">Permissions</span></span>
<span data-ttu-id="2b26d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2b26d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b26d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2b26d-110">Permission type</span></span>      | <span data-ttu-id="2b26d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2b26d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b26d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2b26d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2b26d-113">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b26d-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="2b26d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2b26d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b26d-115">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b26d-115">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="2b26d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2b26d-116">Application</span></span> | <span data-ttu-id="2b26d-117">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b26d-117">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b26d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2b26d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/reminderView(startDateTime=startDateTime-value,endDateTime=endDateTime-value)
```

## <a name="function-parameters"></a><span data-ttu-id="2b26d-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="2b26d-119">Function parameters</span></span>
<span data-ttu-id="2b26d-120">在请求 URL 中，提供以下包含值的函数参数。</span><span class="sxs-lookup"><span data-stu-id="2b26d-120">In the request URL, provide the following function parameters with values.</span></span>

| <span data-ttu-id="2b26d-121">参数</span><span class="sxs-lookup"><span data-stu-id="2b26d-121">Parameter</span></span>    | <span data-ttu-id="2b26d-122">类型</span><span class="sxs-lookup"><span data-stu-id="2b26d-122">Type</span></span>   |<span data-ttu-id="2b26d-123">说明</span><span class="sxs-lookup"><span data-stu-id="2b26d-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b26d-124">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2b26d-124">startDateTime</span></span>|<span data-ttu-id="2b26d-125">字符串</span><span class="sxs-lookup"><span data-stu-id="2b26d-125">String</span></span>|<span data-ttu-id="2b26d-p103">事件（已设置提醒）的开始日期和时间。该值用 ISO 8601 格式表示，例如，“2015-11-08T19:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="2b26d-p103">The start date and time of the event for which the reminder is set up. The value is represented in ISO 8601 format, for example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="2b26d-128">endDateTime</span><span class="sxs-lookup"><span data-stu-id="2b26d-128">endDateTime</span></span>|<span data-ttu-id="2b26d-129">字符串</span><span class="sxs-lookup"><span data-stu-id="2b26d-129">String</span></span>|<span data-ttu-id="2b26d-p104">事件（已设置提醒）的结束日期和时间。该值用 ISO 8601 格式表示，例如，“2015-11-08T20:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="2b26d-p104">The end date and time of the event for which the reminder is set up. The value is represented in ISO 8601 format, for example, "2015-11-08T20:00:00.0000000".</span></span>|

## <a name="request-headers"></a><span data-ttu-id="2b26d-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="2b26d-132">Request headers</span></span>
| <span data-ttu-id="2b26d-133">标头</span><span class="sxs-lookup"><span data-stu-id="2b26d-133">Header</span></span>       | <span data-ttu-id="2b26d-134">值</span><span class="sxs-lookup"><span data-stu-id="2b26d-134">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="2b26d-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b26d-135">Authorization</span></span>  | <span data-ttu-id="2b26d-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2b26d-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2b26d-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2b26d-138">Content-Type</span></span>   | <span data-ttu-id="2b26d-139">application/json</span><span class="sxs-lookup"><span data-stu-id="2b26d-139">application/json</span></span> |
| <span data-ttu-id="2b26d-140">Prefer</span><span class="sxs-lookup"><span data-stu-id="2b26d-140">Prefer</span></span> | <span data-ttu-id="2b26d-p106">{Time-zone}。可选，如果缺省，则采用 UTC。</span><span class="sxs-lookup"><span data-stu-id="2b26d-p106">{Time-zone}. Optional, UTC assumed if absent.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b26d-143">请求正文</span><span class="sxs-lookup"><span data-stu-id="2b26d-143">Request body</span></span>
<span data-ttu-id="2b26d-144">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2b26d-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b26d-145">响应</span><span class="sxs-lookup"><span data-stu-id="2b26d-145">Response</span></span>

<span data-ttu-id="2b26d-146">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [reminder](../resources/reminder.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="2b26d-146">If successful, this method returns `200 OK` response code and [reminder](../resources/reminder.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b26d-147">示例</span><span class="sxs-lookup"><span data-stu-id="2b26d-147">Example</span></span>
<span data-ttu-id="2b26d-148">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="2b26d-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2b26d-149">请求</span><span class="sxs-lookup"><span data-stu-id="2b26d-149">Request</span></span>
<span data-ttu-id="2b26d-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2b26d-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_reminderview"
}-->
```http
GET https://graph.microsoft.com/beta/me/reminderView(startDateTime='2017-06-05T10:00:00.0000000',endDateTime='2017-06-11T11:00:00.0000000')
```

##### <a name="response"></a><span data-ttu-id="2b26d-151">响应</span><span class="sxs-lookup"><span data-stu-id="2b26d-151">Response</span></span>
<span data-ttu-id="2b26d-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2b26d-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.reminder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 673

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.reminder)",
    "value": [
        {
            "eventId": "AAMkADNsvAAA=",
            "changeKey": "SuFHwDRP1EeXJUopWbSLlgAAmBvk2g==",
            "eventSubject": "Plan summer company picnic",
            "eventWebLink": "https://outlook.office365.com/owa/?itemid=AAMkADNsvAAA%3D&exvsurl=1&path=/calendar/item",
            "eventStartTime": {
                "dateTime": "2017-06-09T18:00:00.0000000",
                "timeZone": "UTC"
            },
            "eventEndTime": {
                "dateTime": "2017-06-09T19:00:00.0000000",
                "timeZone": "UTC"
            },
            "eventLocation": {
                "displayName": "Conf Room 3"
            },
            "reminderFireTime": {
                "dateTime": "2017-06-09T17:45:00.0000000",
                "timeZone": "UTC"
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: reminderView",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
