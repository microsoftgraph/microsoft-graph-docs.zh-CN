---
title: 'user: reminderView'
description: '返回指定开始时间和结束时间范围内的日历提醒列表。 '
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3346a54c67207df57cedc698510d55549dc3697c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050722"
---
# <a name="user-reminderview"></a><span data-ttu-id="58f6d-103">user: reminderView</span><span class="sxs-lookup"><span data-stu-id="58f6d-103">user: reminderView</span></span>

<span data-ttu-id="58f6d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58f6d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58f6d-105">返回指定开始时间和结束时间的用户日历中的事件提醒列表。</span><span class="sxs-lookup"><span data-stu-id="58f6d-105">Return a list of event reminders in a user calendar within the specified start and end times.</span></span> 

## <a name="permissions"></a><span data-ttu-id="58f6d-106">权限</span><span class="sxs-lookup"><span data-stu-id="58f6d-106">Permissions</span></span>
<span data-ttu-id="58f6d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="58f6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58f6d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="58f6d-109">Permission type</span></span>      | <span data-ttu-id="58f6d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="58f6d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58f6d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="58f6d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="58f6d-112">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="58f6d-112">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="58f6d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="58f6d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58f6d-114">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="58f6d-114">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="58f6d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="58f6d-115">Application</span></span> | <span data-ttu-id="58f6d-116">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="58f6d-116">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="58f6d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="58f6d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/reminderView(startDateTime=startDateTime-value,endDateTime=endDateTime-value)
```

## <a name="function-parameters"></a><span data-ttu-id="58f6d-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="58f6d-118">Function parameters</span></span>
<span data-ttu-id="58f6d-119">在请求 URL 中，提供以下包含值的函数参数。</span><span class="sxs-lookup"><span data-stu-id="58f6d-119">In the request URL, provide the following function parameters with values.</span></span>

| <span data-ttu-id="58f6d-120">参数</span><span class="sxs-lookup"><span data-stu-id="58f6d-120">Parameter</span></span>    | <span data-ttu-id="58f6d-121">类型</span><span class="sxs-lookup"><span data-stu-id="58f6d-121">Type</span></span>   |<span data-ttu-id="58f6d-122">说明</span><span class="sxs-lookup"><span data-stu-id="58f6d-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58f6d-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="58f6d-123">startDateTime</span></span>|<span data-ttu-id="58f6d-124">String</span><span class="sxs-lookup"><span data-stu-id="58f6d-124">String</span></span>|<span data-ttu-id="58f6d-p102">事件（已设置提醒）的开始日期和时间。该值用 ISO 8601 格式表示，例如，“2015-11-08T19:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="58f6d-p102">The start date and time of the event for which the reminder is set up. The value is represented in ISO 8601 format, for example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="58f6d-127">endDateTime</span><span class="sxs-lookup"><span data-stu-id="58f6d-127">endDateTime</span></span>|<span data-ttu-id="58f6d-128">String</span><span class="sxs-lookup"><span data-stu-id="58f6d-128">String</span></span>|<span data-ttu-id="58f6d-p103">事件（已设置提醒）的结束日期和时间。该值用 ISO 8601 格式表示，例如，“2015-11-08T20:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="58f6d-p103">The end date and time of the event for which the reminder is set up. The value is represented in ISO 8601 format, for example, "2015-11-08T20:00:00.0000000".</span></span>|

## <a name="request-headers"></a><span data-ttu-id="58f6d-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="58f6d-131">Request headers</span></span>
| <span data-ttu-id="58f6d-132">标头</span><span class="sxs-lookup"><span data-stu-id="58f6d-132">Header</span></span>       | <span data-ttu-id="58f6d-133">值</span><span class="sxs-lookup"><span data-stu-id="58f6d-133">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="58f6d-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="58f6d-134">Authorization</span></span>  | <span data-ttu-id="58f6d-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="58f6d-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="58f6d-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="58f6d-137">Content-Type</span></span>   | <span data-ttu-id="58f6d-138">application/json</span><span class="sxs-lookup"><span data-stu-id="58f6d-138">application/json</span></span> |
| <span data-ttu-id="58f6d-139">Prefer</span><span class="sxs-lookup"><span data-stu-id="58f6d-139">Prefer</span></span> | <span data-ttu-id="58f6d-p105">{Time-zone}。可选，如果缺省，则采用 UTC。</span><span class="sxs-lookup"><span data-stu-id="58f6d-p105">{Time-zone}. Optional, UTC assumed if absent.</span></span>|

## <a name="request-body"></a><span data-ttu-id="58f6d-142">请求正文</span><span class="sxs-lookup"><span data-stu-id="58f6d-142">Request body</span></span>
<span data-ttu-id="58f6d-143">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="58f6d-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58f6d-144">响应</span><span class="sxs-lookup"><span data-stu-id="58f6d-144">Response</span></span>

<span data-ttu-id="58f6d-145">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [reminder](../resources/reminder.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="58f6d-145">If successful, this method returns `200 OK` response code and [reminder](../resources/reminder.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58f6d-146">示例</span><span class="sxs-lookup"><span data-stu-id="58f6d-146">Example</span></span>
<span data-ttu-id="58f6d-147">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="58f6d-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="58f6d-148">请求</span><span class="sxs-lookup"><span data-stu-id="58f6d-148">Request</span></span>
<span data-ttu-id="58f6d-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="58f6d-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="58f6d-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="58f6d-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_reminderview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/reminderView(startDateTime='2017-06-05T10:00:00.0000000',endDateTime='2017-06-11T11:00:00.0000000')
```
# <a name="c"></a>[<span data-ttu-id="58f6d-151">C#</span><span class="sxs-lookup"><span data-stu-id="58f6d-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-reminderview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="58f6d-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="58f6d-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-reminderview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="58f6d-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="58f6d-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-reminderview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="58f6d-154">Java</span><span class="sxs-lookup"><span data-stu-id="58f6d-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-reminderview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="58f6d-155">响应</span><span class="sxs-lookup"><span data-stu-id="58f6d-155">Response</span></span>
<span data-ttu-id="58f6d-156">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="58f6d-156">Here is an example of the response.</span></span> <span data-ttu-id="58f6d-157">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="58f6d-157">Note: The response object shown here might be shortened for readability.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "user: reminderView",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


