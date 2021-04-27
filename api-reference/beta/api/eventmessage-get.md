---
title: 获取 eventMessage
description: 事件上的 expand' **参数**
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a321d0ca2332b3a76492f7a16c1201cb8f565ed5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042441"
---
# <a name="get-eventmessage"></a><span data-ttu-id="1a868-103">获取 eventMessage</span><span class="sxs-lookup"><span data-stu-id="1a868-103">Get eventMessage</span></span>

<span data-ttu-id="1a868-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a868-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a868-105">获取 [eventMessage](../resources/eventmessage.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1a868-105">Get the properties and relationships of the [eventMessage](../resources/eventmessage.md) object.</span></span> <span data-ttu-id="1a868-106">对 `$expand` 事件导航 **属性** 应用 参数，获取与会者日历中的关联 [](../resources/event.md)事件。</span><span class="sxs-lookup"><span data-stu-id="1a868-106">Apply the `$expand` parameter on the **event** navigation property to get the associated [event](../resources/event.md) in an attendee's calendar.</span></span>

### <a name="get-the-event-message-body-in-html-or-text-format"></a><span data-ttu-id="1a868-107">获取 HTML 或文本格式的事件邮件正文</span><span class="sxs-lookup"><span data-stu-id="1a868-107">Get the event message body in HTML or text format</span></span>

<span data-ttu-id="1a868-108">事件邮件正文可以是 HTML 格式或文本格式。</span><span class="sxs-lookup"><span data-stu-id="1a868-108">Event message bodies can be in HTML or text format.</span></span>

<span data-ttu-id="1a868-109">可以使用 标头指定在请求的 body 和 `Prefer: outlook.body-content-type` **uniqueBody** 属性中返回的所需 `GET` 格式：</span><span class="sxs-lookup"><span data-stu-id="1a868-109">You can use the `Prefer: outlook.body-content-type` header to specify the desired format returned in the **body** and **uniqueBody** properties in a `GET` request:</span></span>

- <span data-ttu-id="1a868-110">指定 `Prefer: outlook.body-content-type="text"` 获取以文本格式返回的事件邮件正文。</span><span class="sxs-lookup"><span data-stu-id="1a868-110">Specify `Prefer: outlook.body-content-type="text"` to get a event message body returned in text format.</span></span>
- <span data-ttu-id="1a868-111">指定 `Prefer: outlook.body-content-type="html"` 或直接跳过 标头，以 HTML 格式返回事件邮件正文。</span><span class="sxs-lookup"><span data-stu-id="1a868-111">Specify `Prefer: outlook.body-content-type="html"`, or just skip the header, to return the event message body in HTML format.</span></span>

<span data-ttu-id="1a868-112">如果指定任一标头，响应中将包含相应的 `Preference-Applied` 标头作为确认：</span><span class="sxs-lookup"><span data-stu-id="1a868-112">If you specify either header, the response will include the corresponding `Preference-Applied` header as confirmation:</span></span>

- <span data-ttu-id="1a868-113">对于文本格式请求：`Preference-Applied: outlook.body-content-type="text"`</span><span class="sxs-lookup"><span data-stu-id="1a868-113">For text format requests: `Preference-Applied: outlook.body-content-type="text"`</span></span>
- <span data-ttu-id="1a868-114">对于 HTML 格式请求：`Preference-Applied: outlook.body-content-type="html"`</span><span class="sxs-lookup"><span data-stu-id="1a868-114">For HTML format requests: `Preference-Applied: outlook.body-content-type="html"`</span></span>

## <a name="permissions"></a><span data-ttu-id="1a868-115">权限</span><span class="sxs-lookup"><span data-stu-id="1a868-115">Permissions</span></span>
<span data-ttu-id="1a868-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a868-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a868-118">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a868-118">Permission type</span></span>      | <span data-ttu-id="1a868-119">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1a868-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a868-120">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a868-120">Delegated (work or school account)</span></span> | <span data-ttu-id="1a868-121">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1a868-121">Mail.Read</span></span>    |
|<span data-ttu-id="1a868-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a868-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a868-123">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1a868-123">Mail.Read</span></span>    |
|<span data-ttu-id="1a868-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a868-124">Application</span></span> | <span data-ttu-id="1a868-125">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1a868-125">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a868-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a868-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}

GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1a868-127">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1a868-127">Optional query parameters</span></span>
<span data-ttu-id="1a868-128">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1a868-128">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1a868-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a868-129">Request headers</span></span>
| <span data-ttu-id="1a868-130">名称</span><span class="sxs-lookup"><span data-stu-id="1a868-130">Name</span></span>       | <span data-ttu-id="1a868-131">类型</span><span class="sxs-lookup"><span data-stu-id="1a868-131">Type</span></span> | <span data-ttu-id="1a868-132">说明</span><span class="sxs-lookup"><span data-stu-id="1a868-132">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1a868-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a868-133">Authorization</span></span>  | <span data-ttu-id="1a868-134">string</span><span class="sxs-lookup"><span data-stu-id="1a868-134">string</span></span>  | <span data-ttu-id="1a868-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1a868-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a868-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a868-137">Request body</span></span>
<span data-ttu-id="1a868-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1a868-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a868-139">响应</span><span class="sxs-lookup"><span data-stu-id="1a868-139">Response</span></span>

<span data-ttu-id="1a868-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [eventMessage](../resources/eventmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1a868-140">If successful, this method returns a `200 OK` response code and [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="1a868-141">示例</span><span class="sxs-lookup"><span data-stu-id="1a868-141">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="1a868-142">示例 1</span><span class="sxs-lookup"><span data-stu-id="1a868-142">Example 1</span></span>
#### <a name="request"></a><span data-ttu-id="1a868-143">请求</span><span class="sxs-lookup"><span data-stu-id="1a868-143">Request</span></span>
<span data-ttu-id="1a868-144">第一个示例展示了如何根据事件邮件 ID 获取事件邮件的属性。</span><span class="sxs-lookup"><span data-stu-id="1a868-144">The first example shows how to get the properties of an event message based on the event message ID.</span></span>

# <a name="http"></a>[<span data-ttu-id="1a868-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a868-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_eventmessage"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AAMkADYAAAImV_lAAA=
```
# <a name="c"></a>[<span data-ttu-id="1a868-146">C#</span><span class="sxs-lookup"><span data-stu-id="1a868-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1a868-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a868-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1a868-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a868-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1a868-149">Java</span><span class="sxs-lookup"><span data-stu-id="1a868-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-eventmessage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="1a868-150">响应</span><span class="sxs-lookup"><span data-stu-id="1a868-150">Response</span></span>
<span data-ttu-id="1a868-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1a868-151">Here is an example of the response.</span></span> <span data-ttu-id="1a868-152">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1a868-152">Note: The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2"></a><span data-ttu-id="1a868-153">示例 2</span><span class="sxs-lookup"><span data-stu-id="1a868-153">Example 2</span></span>
#### <a name="request"></a><span data-ttu-id="1a868-154">请求</span><span class="sxs-lookup"><span data-stu-id="1a868-154">Request</span></span>
<span data-ttu-id="1a868-155">第二个示例展示了如何获取与事件消息关联的事件。</span><span class="sxs-lookup"><span data-stu-id="1a868-155">The second example shows how to get the event associated with an event message.</span></span> <span data-ttu-id="1a868-156">它使用事件消息 ID 获取事件消息，将事件消息显式强制转换为访问 **event** 导航属性，并应用 $expand 参数来获取事件属性。</span><span class="sxs-lookup"><span data-stu-id="1a868-156">It uses the event message ID to get the event message, explicitly provides a cast on the event message to access its **event** navigation property, and apply an $expand parameter to get the properties of the event.</span></span>

# <a name="http"></a>[<span data-ttu-id="1a868-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a868-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_event_based_on_eventmessage"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AAMkADYAAAImV_jAAA=/?$expand=microsoft.graph.eventMessage/event
```
# <a name="c"></a>[<span data-ttu-id="1a868-158">C#</span><span class="sxs-lookup"><span data-stu-id="1a868-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-event-based-on-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1a868-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a868-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-event-based-on-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1a868-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a868-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-event-based-on-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1a868-161">Java</span><span class="sxs-lookup"><span data-stu-id="1a868-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-event-based-on-eventmessage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="1a868-162">响应</span><span class="sxs-lookup"><span data-stu-id="1a868-162">Response</span></span>
<span data-ttu-id="1a868-163">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1a868-163">Here is an example of the response.</span></span> <span data-ttu-id="1a868-164">响应中返回关联事件的属性。</span><span class="sxs-lookup"><span data-stu-id="1a868-164">The properties of the associated event are returned in the response.</span></span>
<span data-ttu-id="1a868-165">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1a868-165">Note: The response object shown here might be shortened for readability.</span></span>
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
  ]
}
-->
