---
title: 'user: reminderView'
description: '返回指定开始时间和结束时间范围内的日历提醒列表。 '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 34c2f1a55b6dea1daff36c5ce98d1959fd78b301
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547737"
---
# <a name="user-reminderview"></a><span data-ttu-id="49f7e-103">user: reminderView</span><span class="sxs-lookup"><span data-stu-id="49f7e-103">user: reminderView</span></span>
<span data-ttu-id="49f7e-104">在指定的开始时间和结束时间内, 返回用户日历中的事件提醒列表。</span><span class="sxs-lookup"><span data-stu-id="49f7e-104">Return a list of event reminders in a user calendar within the specified start and end times.</span></span> 

## <a name="permissions"></a><span data-ttu-id="49f7e-105">权限</span><span class="sxs-lookup"><span data-stu-id="49f7e-105">Permissions</span></span>
<span data-ttu-id="49f7e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="49f7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49f7e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="49f7e-108">Permission type</span></span>      | <span data-ttu-id="49f7e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="49f7e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49f7e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="49f7e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="49f7e-111">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="49f7e-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="49f7e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="49f7e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49f7e-113">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="49f7e-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="49f7e-114">Application</span><span class="sxs-lookup"><span data-stu-id="49f7e-114">Application</span></span> | <span data-ttu-id="49f7e-115">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="49f7e-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="49f7e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="49f7e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/reminderView(startDateTime=startDateTime-value,endDateTime=endDateTime-value)
```

## <a name="function-parameters"></a><span data-ttu-id="49f7e-117">函数参数</span><span class="sxs-lookup"><span data-stu-id="49f7e-117">Function parameters</span></span>
<span data-ttu-id="49f7e-118">在请求 URL 中，提供以下包含值的函数参数。</span><span class="sxs-lookup"><span data-stu-id="49f7e-118">In the request URL, provide the following function parameters with values.</span></span>

| <span data-ttu-id="49f7e-119">参数</span><span class="sxs-lookup"><span data-stu-id="49f7e-119">Parameter</span></span>    | <span data-ttu-id="49f7e-120">类型</span><span class="sxs-lookup"><span data-stu-id="49f7e-120">Type</span></span>   |<span data-ttu-id="49f7e-121">说明</span><span class="sxs-lookup"><span data-stu-id="49f7e-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49f7e-122">startDateTime</span><span class="sxs-lookup"><span data-stu-id="49f7e-122">startDateTime</span></span>|<span data-ttu-id="49f7e-123">String</span><span class="sxs-lookup"><span data-stu-id="49f7e-123">String</span></span>|<span data-ttu-id="49f7e-p102">事件（已设置提醒）的开始日期和时间。该值用 ISO 8601 格式表示，例如，“2015-11-08T19:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="49f7e-p102">The start date and time of the event for which the reminder is set up. The value is represented in ISO 8601 format, for example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="49f7e-126">endDateTime</span><span class="sxs-lookup"><span data-stu-id="49f7e-126">endDateTime</span></span>|<span data-ttu-id="49f7e-127">String</span><span class="sxs-lookup"><span data-stu-id="49f7e-127">String</span></span>|<span data-ttu-id="49f7e-p103">事件（已设置提醒）的结束日期和时间。该值用 ISO 8601 格式表示，例如，“2015-11-08T20:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="49f7e-p103">The end date and time of the event for which the reminder is set up. The value is represented in ISO 8601 format, for example, "2015-11-08T20:00:00.0000000".</span></span>|

## <a name="request-headers"></a><span data-ttu-id="49f7e-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="49f7e-130">Request headers</span></span>
| <span data-ttu-id="49f7e-131">标头</span><span class="sxs-lookup"><span data-stu-id="49f7e-131">Header</span></span>       | <span data-ttu-id="49f7e-132">值</span><span class="sxs-lookup"><span data-stu-id="49f7e-132">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="49f7e-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="49f7e-133">Authorization</span></span>  | <span data-ttu-id="49f7e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="49f7e-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="49f7e-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="49f7e-136">Content-Type</span></span>   | <span data-ttu-id="49f7e-137">application/json</span><span class="sxs-lookup"><span data-stu-id="49f7e-137">application/json</span></span> |
| <span data-ttu-id="49f7e-138">Prefer</span><span class="sxs-lookup"><span data-stu-id="49f7e-138">Prefer</span></span> | <span data-ttu-id="49f7e-p105">{Time-zone}。可选，如果缺省，则采用 UTC。</span><span class="sxs-lookup"><span data-stu-id="49f7e-p105">{Time-zone}. Optional, UTC assumed if absent.</span></span>|

## <a name="request-body"></a><span data-ttu-id="49f7e-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="49f7e-141">Request body</span></span>
<span data-ttu-id="49f7e-142">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="49f7e-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49f7e-143">响应</span><span class="sxs-lookup"><span data-stu-id="49f7e-143">Response</span></span>

<span data-ttu-id="49f7e-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [reminder](../resources/reminder.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="49f7e-144">If successful, this method returns `200 OK` response code and [reminder](../resources/reminder.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49f7e-145">示例</span><span class="sxs-lookup"><span data-stu-id="49f7e-145">Example</span></span>
<span data-ttu-id="49f7e-146">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="49f7e-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="49f7e-147">请求</span><span class="sxs-lookup"><span data-stu-id="49f7e-147">Request</span></span>
<span data-ttu-id="49f7e-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="49f7e-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_reminderview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/reminderView(startDateTime='2017-06-05T10:00:00.0000000',endDateTime='2017-06-11T11:00:00.0000000')
```

##### <a name="response"></a><span data-ttu-id="49f7e-149">响应</span><span class="sxs-lookup"><span data-stu-id="49f7e-149">Response</span></span>
<span data-ttu-id="49f7e-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="49f7e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.reminder)",
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
