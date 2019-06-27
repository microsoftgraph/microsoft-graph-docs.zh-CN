---
title: 获取 eventMessage
description: 在**事件**上展开 "参数
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 735dee1b67725c63fe8e95539630f4be2a33d043
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259078"
---
# <a name="get-eventmessage"></a><span data-ttu-id="43d0f-103">获取 eventMessage</span><span class="sxs-lookup"><span data-stu-id="43d0f-103">Get eventMessage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43d0f-104">获取 [eventMessage](../resources/eventmessage.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="43d0f-104">Get the properties and relationships of the [eventMessage](../resources/eventmessage.md) object.</span></span> <span data-ttu-id="43d0f-105">在事件`$expand`导航属性上\*\*\*\* 应用该参数, 以在与会者的日历中获取关联的[事件](../resources/event.md)。</span><span class="sxs-lookup"><span data-stu-id="43d0f-105">Apply the `$expand` parameter on the **event** navigation property to get the associated [event](../resources/event.md) in an attendee's calendar.</span></span>

### <a name="get-the-event-message-body-in-html-or-text-format"></a><span data-ttu-id="43d0f-106">获取 HTML 或文本格式的事件消息正文</span><span class="sxs-lookup"><span data-stu-id="43d0f-106">Get the event message body in HTML or text format</span></span>

<span data-ttu-id="43d0f-107">事件邮件正文可以是 HTML 格式或文本格式。</span><span class="sxs-lookup"><span data-stu-id="43d0f-107">Event message bodies can be in HTML or text format.</span></span>

<span data-ttu-id="43d0f-108">您`Prefer: outlook.body-content-type`可以使用标头指定`GET`在请求中的**body**和**uniqueBody**属性中返回的所需格式:</span><span class="sxs-lookup"><span data-stu-id="43d0f-108">You can use the `Prefer: outlook.body-content-type` header to specify the desired format returned in the **body** and **uniqueBody** properties in a `GET` request:</span></span>

- <span data-ttu-id="43d0f-109">指定`Prefer: outlook.body-content-type="text"`获取以文本格式返回的事件消息正文。</span><span class="sxs-lookup"><span data-stu-id="43d0f-109">Specify `Prefer: outlook.body-content-type="text"` to get a event message body returned in text format.</span></span>
- <span data-ttu-id="43d0f-110">指定`Prefer: outlook.body-content-type="html"`或直接跳过标头, 以返回 HTML 格式的事件消息正文。</span><span class="sxs-lookup"><span data-stu-id="43d0f-110">Specify `Prefer: outlook.body-content-type="html"`, or just skip the header, to return the event message body in HTML format.</span></span>

<span data-ttu-id="43d0f-111">如果指定任何一个标头, 则响应将包含相应`Preference-Applied`的标头作为确认:</span><span class="sxs-lookup"><span data-stu-id="43d0f-111">If you specify either header, the response will include the corresponding `Preference-Applied` header as confirmation:</span></span>

- <span data-ttu-id="43d0f-112">对于文本格式请求：`Preference-Applied: outlook.body-content-type="text"`</span><span class="sxs-lookup"><span data-stu-id="43d0f-112">For text format requests: `Preference-Applied: outlook.body-content-type="text"`</span></span>
- <span data-ttu-id="43d0f-113">对于 HTML 格式请求：`Preference-Applied: outlook.body-content-type="html"`</span><span class="sxs-lookup"><span data-stu-id="43d0f-113">For HTML format requests: `Preference-Applied: outlook.body-content-type="html"`</span></span>

## <a name="permissions"></a><span data-ttu-id="43d0f-114">权限</span><span class="sxs-lookup"><span data-stu-id="43d0f-114">Permissions</span></span>
<span data-ttu-id="43d0f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="43d0f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43d0f-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="43d0f-117">Permission type</span></span>      | <span data-ttu-id="43d0f-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="43d0f-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="43d0f-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="43d0f-119">Delegated (work or school account)</span></span> | <span data-ttu-id="43d0f-120">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="43d0f-120">Mail.Read</span></span>    |
|<span data-ttu-id="43d0f-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="43d0f-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43d0f-122">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="43d0f-122">Mail.Read</span></span>    |
|<span data-ttu-id="43d0f-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="43d0f-123">Application</span></span> | <span data-ttu-id="43d0f-124">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="43d0f-124">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="43d0f-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="43d0f-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}

GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="43d0f-126">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="43d0f-126">Optional query parameters</span></span>
<span data-ttu-id="43d0f-127">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="43d0f-127">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="43d0f-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="43d0f-128">Request headers</span></span>
| <span data-ttu-id="43d0f-129">名称</span><span class="sxs-lookup"><span data-stu-id="43d0f-129">Name</span></span>       | <span data-ttu-id="43d0f-130">类型</span><span class="sxs-lookup"><span data-stu-id="43d0f-130">Type</span></span> | <span data-ttu-id="43d0f-131">说明</span><span class="sxs-lookup"><span data-stu-id="43d0f-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="43d0f-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="43d0f-132">Authorization</span></span>  | <span data-ttu-id="43d0f-133">string</span><span class="sxs-lookup"><span data-stu-id="43d0f-133">string</span></span>  | <span data-ttu-id="43d0f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="43d0f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="43d0f-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="43d0f-136">Request body</span></span>
<span data-ttu-id="43d0f-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="43d0f-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43d0f-138">响应</span><span class="sxs-lookup"><span data-stu-id="43d0f-138">Response</span></span>

<span data-ttu-id="43d0f-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [eventMessage](../resources/eventmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="43d0f-139">If successful, this method returns a `200 OK` response code and [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="43d0f-140">示例</span><span class="sxs-lookup"><span data-stu-id="43d0f-140">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="43d0f-141">请求 1</span><span class="sxs-lookup"><span data-stu-id="43d0f-141">Request 1</span></span>
<span data-ttu-id="43d0f-142">第一个示例展示了如何根据事件邮件 ID 获取事件邮件的属性。</span><span class="sxs-lookup"><span data-stu-id="43d0f-142">The first example shows how to get the properties of an event message based on the event message ID.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_eventmessage"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages/AAMkADYAAAImV_lAAA=
```
##### <a name="response-1"></a><span data-ttu-id="43d0f-143">响应 1</span><span class="sxs-lookup"><span data-stu-id="43d0f-143">Response 1</span></span>
<span data-ttu-id="43d0f-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="43d0f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_eventmessage",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventMessageRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8fd6e83b-3cc0-4bf0-8b26-950f4d7110f6')/messages/$entity",
    "@odata.type":"#microsoft.graph.eventMessageRequest",
    "@odata.etag":"W/\"CwAAABYAAABXlB/SL0N4Q6g6o+jSYAEuAAAImkVD\"",
    "id":"AAMkADYAAAImV_lAAA=",
    "createdDateTime":"2017-12-27T21:58:36Z",
    "lastModifiedDateTime":"2017-12-27T23:26:38Z",
    "changeKey":"CwAAABYAAABXlB/SL0N4Q6g6o+jSYAEuAAAImkVD",
    "categories":[

    ],
    "receivedDateTime":"2017-12-27T21:58:36Z",
    "sentDateTime":"2017-12-27T21:58:36Z",
    "hasAttachments":false,
    "internetMessageId":"<MWHPR1301MB2110DCFC@MWHPR1301MB2110.namprd13.prod.outlook.com>",
    "subject":"Debrief from meetup",
    "bodyPreview":"Let's debrief after community meetup.",
    "importance":"normal",
    "parentFolderId":"AQMkADYAAAIBDAAAAA==",
    "conversationId":"AAQkADYCipTiRjXQORU=",
    "conversationIndex":"AdN/Xdgnql4N9FlrT0KKlOJGNdA5FQ==",
    "isDeliveryReceiptRequested":null,
    "isReadReceiptRequested":false,
    "isRead":false,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADYAAAImV%2BlAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "unsubscribeData":[

    ],
    "unsubscribeEnabled":false,
    "meetingMessageType":"meetingRequest",
    "type":"singleInstance",
    "isOutOfDate":false,
    "isAllDay":false,
    "isDelegated":false,
    "responseRequested":true,
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n<style type=\"text/css\" style=\"display:none\">\r\n<!--\r\np\r\n\t{margin-top:0;\r\n\tmargin-bottom:0}\r\n-->\r\n</style>\r\n</head>\r\n<body dir=\"ltr\">\r\n<div id=\"divtagdefaultwrapper\" dir=\"ltr\" style=\"font-size:12pt; color:#000000; font-family:Calibri,Helvetica,sans-serif\">\r\n<p style=\"margin-top:0; margin-bottom:0\">Let's debrief after community meetup.<br>\r\n</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
    },
    "sender":{
        "emailAddress":{
            "name":"Administrator",
            "address":"admin@contoso.onmicrosoft.com"
        }
    },
    "from":{
        "emailAddress":{
            "name":"Administrator",
            "address":"admin@contoso.onmicrosoft.com"
        }
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"Alex Wilber",
                "address":"AlexW@contoso.onmicrosoft.com"
            }
        }
    ],
    "ccRecipients":[

    ],
    "bccRecipients":[

    ],
    "replyTo":[

    ],
    "mentionsPreview":null,
    "flag":{
        "flagStatus":"notFlagged"
    },
    "startDateTime":{
        "dateTime":"2018-02-19T19:00:00.0000000",
        "timeZone":"UTC"
    },
    "endDateTime":{
        "dateTime":"2018-02-19T19:30:00.0000000",
        "timeZone":"UTC"
    },
    "location":{
        "displayName":"Mt. Hood",
        "locationType":"default",
        "uniqueIdType":"unknown"
    },
    "recurrence":null,
    "previousLocation":null,
    "previousStartDateTime":null,
    "previousEndDateTime":null
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="43d0f-147">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="43d0f-147">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="43d0f-148">C#</span><span class="sxs-lookup"><span data-stu-id="43d0f-148">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_eventmessage-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="43d0f-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="43d0f-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_eventmessage-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="43d0f-150">目标-C</span><span class="sxs-lookup"><span data-stu-id="43d0f-150">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_eventmessage-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


##### <a name="request-2"></a><span data-ttu-id="43d0f-151">请求 2</span><span class="sxs-lookup"><span data-stu-id="43d0f-151">Request 2</span></span>
<span data-ttu-id="43d0f-152">第二个示例展示了如何获取与事件消息关联的事件。</span><span class="sxs-lookup"><span data-stu-id="43d0f-152">The second example shows how to get the event associated with an event message.</span></span> <span data-ttu-id="43d0f-153">它使用事件消息 ID 获取事件消息，将事件消息显式强制转换为访问 **event** 导航属性，并应用 $expand 参数来获取事件属性。</span><span class="sxs-lookup"><span data-stu-id="43d0f-153">It uses the event message ID to get the event message, explicitly provides a cast on the event message to access its **event** navigation property, and apply an $expand parameter to get the properties of the event.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_event_based_on_eventmessage"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages/AAMkADYAAAImV_jAAA=/?$expand=microsoft.graph.eventMessage/event
```
##### <a name="response-2"></a><span data-ttu-id="43d0f-154">响应 2</span><span class="sxs-lookup"><span data-stu-id="43d0f-154">Response 2</span></span>
<span data-ttu-id="43d0f-155">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="43d0f-155">Here is an example of the response.</span></span> <span data-ttu-id="43d0f-156">响应中返回关联事件的属性。</span><span class="sxs-lookup"><span data-stu-id="43d0f-156">The properties of the associated event are returned in the response.</span></span>
<span data-ttu-id="43d0f-157">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="43d0f-157">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="43d0f-158">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="43d0f-158">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_event_based_on_eventmessage",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventMessageRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8fd6e83b-3cc0-4bf0-8b26-950f4d7110f6')/messages/$entity",
    "@odata.type":"#microsoft.graph.eventMessageRequest",
    "@odata.etag":"W/\"CwAAABYAAABXlB/SL0N4Q6g6o+jSYAEuAAAImkVF\"",
    "id":"AAMkADYAAAImV_jAAA=",
    "createdDateTime":"2017-12-27T21:54:55Z",
    "lastModifiedDateTime":"2017-12-27T23:26:38Z",
    "changeKey":"CwAAABYAAABXlB/SL0N4Q6g6o+jSYAEuAAAImkVF",
    "categories":[

    ],
    "receivedDateTime":"2017-12-27T21:54:55Z",
    "sentDateTime":"2017-12-27T21:54:54Z",
    "hasAttachments":false,
    "internetMessageId":"<MWHPR1301MB211042CFBF@MWHPR1301MB2110.namprd13.prod.outlook.com>",
    "subject":"Kick off planning",
    "bodyPreview":"Let's collect opinions from our teams and organize action items.",
    "importance":"normal",
    "parentFolderId":"AQMkADYAS4AAAIBDAAAAA==",
    "conversationId":"AAQkADYRuffB3wDlPn-ReFZarI60=",
    "conversationIndex":"AdN/XVP4JG598HfAOU+f9F4VlqsjrQ==",
    "isDeliveryReceiptRequested":null,
    "isReadReceiptRequested":false,
    "isRead":false,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADYAAAImV%2BjAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "unsubscribeData":[

    ],
    "unsubscribeEnabled":false,
    "meetingMessageType":"meetingRequest",
    "type":"singleInstance",
    "isOutOfDate":false,
    "isAllDay":false,
    "isDelegated":false,
    "responseRequested":true,
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n<style type=\"text/css\" style=\"display:none\">\r\n<!--\r\np\r\n\t{margin-top:0;\r\n\tmargin-bottom:0}\r\n-->\r\n</style>\r\n</head>\r\n<body dir=\"ltr\">\r\n<div id=\"divtagdefaultwrapper\" dir=\"ltr\" style=\"font-size:12pt; color:#000000; font-family:Calibri,Helvetica,sans-serif\">\r\n<p style=\"margin-top:0; margin-bottom:0\">Let's collect opinions from our teams and organize action items.<br>\r\n</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
    },
    "sender":{
        "emailAddress":{
            "name":"Administrator",
            "address":"admin@contoso.onmicrosoft.com"
        }
    },
    "from":{
        "emailAddress":{
            "name":"Administrator",
            "address":"admin@contoso.onmicrosoft.com"
        }
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"Alex Wilber",
                "address":"AlexW@contoso.onmicrosoft.com"
            }
        }
    ],
    "ccRecipients":[

    ],
    "bccRecipients":[

    ],
    "replyTo":[

    ],
    "mentionsPreview":null,
    "flag":{
        "flagStatus":"notFlagged"
    },
    "startDateTime":{
        "dateTime":"2018-02-02T22:00:00.0000000",
        "timeZone":"UTC"
    },
    "endDateTime":{
        "dateTime":"2018-02-02T23:00:00.0000000",
        "timeZone":"UTC"
    },
    "location":{
        "displayName":"Mt. Hood",
        "locationType":"default",
        "uniqueIdType":"unknown"
    },
    "recurrence":null,
    "previousLocation":null,
    "previousStartDateTime":null,
    "previousEndDateTime":null,
    "event@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8fd6e83b-3cc0-4bf0-8b26-950f4d7110f6')/messages('AAMkADYAAAImV_jAAA%3D')/microsoft.graph.eventMessage/event/$entity",
    "event":{
        "@odata.etag":"W/\"V5Qf0i9DeEOoOqPo0mABLgAACJpBWg==\"",
        "id":"AAMkADYAAAImVu6AAA=",
        "createdDateTime":"2017-12-27T21:54:55.2624551Z",
        "lastModifiedDateTime":"2017-12-27T22:19:16.6667889Z",
        "changeKey":"V5Qf0i9DeEOoOqPo0mABLgAACJpBWg==",
        "categories":[

        ],
        "originalStartTimeZone":"Pacific Standard Time",
        "originalEndTimeZone":"Pacific Standard Time",
        "uid":"040000008200E00074C5B7101A82E00800000000A2A6F3535D7FD3010000000000000000100000003D770E2E8974F44B9471BDB348097FE3",
        "reminderMinutesBeforeStart":15,
        "isReminderOn":true,
        "hasAttachments":false,
        "subject":"Kick off planning",
        "bodyPreview":"Let's collect opinions from our teams and organize action items.",
        "importance":"normal",
        "sensitivity":"normal",
        "isAllDay":false,
        "isCancelled":false,
        "isOrganizer":false,
        "responseRequested":true,
        "seriesMasterId":null,
        "showAs":"tentative",
        "type":"singleInstance",
        "webLink":"https://outlook.office365.com/owa/?itemid=AAMkADYAAAImVu6AAA%3D&exvsurl=1&path=/calendar/item",
        "onlineMeetingUrl":null,
        "responseStatus":{
            "response":"tentativelyAccepted",
            "time":"2017-12-27T22:19:12.6197462Z"
        },
        "body":{
            "contentType":"html",
            "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n<style type=\"text/css\" style=\"display:none\">\r\n<!--\r\np\r\n\t{margin-top:0;\r\n\tmargin-bottom:0}\r\n-->\r\n</style>\r\n</head>\r\n<body dir=\"ltr\">\r\n<div id=\"divtagdefaultwrapper\" dir=\"ltr\" style=\"font-size:12pt; color:#000000; font-family:Calibri,Helvetica,sans-serif\">\r\n<p style=\"margin-top:0; margin-bottom:0\">Let's collect opinions from our teams and organize action items.<br>\r\n</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
        },
        "start":{
            "dateTime":"2018-02-02T22:00:00.0000000",
            "timeZone":"UTC"
        },
        "end":{
            "dateTime":"2018-02-02T23:00:00.0000000",
            "timeZone":"UTC"
        },
        "location":{
            "displayName":"Mt. Hood",
            "locationType":"default",
            "uniqueId":"Mt. Hood",
            "uniqueIdType":"private"
        },
        "locations":[
            {
                "displayName":"Mt. Hood",
                "locationType":"default",
                "uniqueId":"Mt. Hood",
                "uniqueIdType":"private"
            }
        ],
        "recurrence":null,
        "attendees":[
            {
                "type":"required",
                "status":{
                    "response":"none",
                    "time":"0001-01-01T00:00:00Z"
                },
                "emailAddress":{
                    "name":"Administrator",
                    "address":"admin@contoso.onmicrosoft.com"
                }
            },
            {
                "type":"required",
                "status":{
                    "response":"tentativelyAccepted",
                    "time":"0001-01-01T00:00:00Z"
                },
                "emailAddress":{
                    "name":"Alex Wilber",
                    "address":"AlexW@contoso.onmicrosoft.com"
                }
            }
        ],
        "organizer":{
            "emailAddress":{
                "name":"Administrator",
                "address":"admin@contoso.onmicrosoft.com"
            }
        },
        "OnlineMeeting":null
    }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="43d0f-159">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="43d0f-159">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="43d0f-160">C#</span><span class="sxs-lookup"><span data-stu-id="43d0f-160">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_event_based_on_eventmessage-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="43d0f-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="43d0f-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_event_based_on_eventmessage-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="43d0f-162">目标-C</span><span class="sxs-lookup"><span data-stu-id="43d0f-162">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_event_based_on_eventmessage-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get eventMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/eventmessage-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/eventmessage-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/eventmessage-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/eventmessage-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/eventmessage-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
