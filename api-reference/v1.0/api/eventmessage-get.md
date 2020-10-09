---
title: 获取 eventMessage
description: 在 **事件** 导航属性中展开参数，以在与会者的日历中获取关联的事件。
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: fbde80a9ccd1566df11be5f1c573abac7011a0da
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48403690"
---
# <a name="get-eventmessage"></a><span data-ttu-id="3cc18-103">获取 eventMessage</span><span class="sxs-lookup"><span data-stu-id="3cc18-103">Get eventMessage</span></span>

<span data-ttu-id="3cc18-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cc18-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3cc18-105">获取 [eventMessage](../resources/eventmessage.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3cc18-105">Get the properties and relationships of the [eventMessage](../resources/eventmessage.md) object.</span></span> <span data-ttu-id="3cc18-106">对 **event** 导航属性应用 $expand 参数，可以获取与会者日历中的相关 [event](../resources/event.md)。</span><span class="sxs-lookup"><span data-stu-id="3cc18-106">Apply the $expand parameter on the **event** navigation property to get the associated [event](../resources/event.md) in an attendee's calendar.</span></span>

<span data-ttu-id="3cc18-107">此操作暂返回纯 HTML 格式的事件邮件正文。</span><span class="sxs-lookup"><span data-stu-id="3cc18-107">Currently, this operation returns event message bodies in only HTML format.</span></span>

## <a name="permissions"></a><span data-ttu-id="3cc18-108">权限</span><span class="sxs-lookup"><span data-stu-id="3cc18-108">Permissions</span></span>
<span data-ttu-id="3cc18-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3cc18-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cc18-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3cc18-111">Permission type</span></span>      | <span data-ttu-id="3cc18-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3cc18-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3cc18-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3cc18-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3cc18-114">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3cc18-114">Mail.Read</span></span>    |
|<span data-ttu-id="3cc18-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3cc18-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3cc18-116">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3cc18-116">Mail.Read</span></span>    |
|<span data-ttu-id="3cc18-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3cc18-117">Application</span></span> | <span data-ttu-id="3cc18-118">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3cc18-118">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="3cc18-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3cc18-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}

GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3cc18-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3cc18-120">Optional query parameters</span></span>
<span data-ttu-id="3cc18-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3cc18-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3cc18-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="3cc18-122">Request headers</span></span>
| <span data-ttu-id="3cc18-123">名称</span><span class="sxs-lookup"><span data-stu-id="3cc18-123">Name</span></span>       | <span data-ttu-id="3cc18-124">类型</span><span class="sxs-lookup"><span data-stu-id="3cc18-124">Type</span></span> | <span data-ttu-id="3cc18-125">说明</span><span class="sxs-lookup"><span data-stu-id="3cc18-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3cc18-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="3cc18-126">Authorization</span></span>  | <span data-ttu-id="3cc18-127">string</span><span class="sxs-lookup"><span data-stu-id="3cc18-127">string</span></span>  | <span data-ttu-id="3cc18-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3cc18-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3cc18-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="3cc18-130">Request body</span></span>
<span data-ttu-id="3cc18-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3cc18-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3cc18-132">响应</span><span class="sxs-lookup"><span data-stu-id="3cc18-132">Response</span></span>

<span data-ttu-id="3cc18-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [eventMessage](../resources/eventmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3cc18-133">If successful, this method returns a `200 OK` response code and [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="3cc18-134">示例</span><span class="sxs-lookup"><span data-stu-id="3cc18-134">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="3cc18-135">示例 1</span><span class="sxs-lookup"><span data-stu-id="3cc18-135">Example 1</span></span>
#### <a name="request"></a><span data-ttu-id="3cc18-136">请求</span><span class="sxs-lookup"><span data-stu-id="3cc18-136">Request</span></span>

<span data-ttu-id="3cc18-137">第一个示例展示了如何根据事件邮件 ID 获取事件邮件的属性。</span><span class="sxs-lookup"><span data-stu-id="3cc18-137">The first example shows how to get the properties of an event message based on the event message ID.</span></span>

# <a name="http"></a>[<span data-ttu-id="3cc18-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="3cc18-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADYAAAImV_lAAA="],
  "name": "get_eventmessage"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADYAAAImV_lAAA=
```
# <a name="c"></a>[<span data-ttu-id="3cc18-139">C#</span><span class="sxs-lookup"><span data-stu-id="3cc18-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3cc18-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3cc18-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3cc18-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3cc18-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3cc18-142">Java</span><span class="sxs-lookup"><span data-stu-id="3cc18-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-eventmessage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="3cc18-143">响应</span><span class="sxs-lookup"><span data-stu-id="3cc18-143">Response</span></span>
<span data-ttu-id="3cc18-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3cc18-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8fd6e83b-3cc0-4bf0-8b26-950f4d7110f6')/messages/$entity",
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
    "meetingMessageType":"meetingRequest",
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

    ]
}
```

### <a name="example-2"></a><span data-ttu-id="3cc18-147">示例 2</span><span class="sxs-lookup"><span data-stu-id="3cc18-147">Example 2</span></span>
#### <a name="request"></a><span data-ttu-id="3cc18-148">请求</span><span class="sxs-lookup"><span data-stu-id="3cc18-148">Request</span></span>
<span data-ttu-id="3cc18-149">第二个示例展示了如何获取与事件消息关联的事件。</span><span class="sxs-lookup"><span data-stu-id="3cc18-149">The second example shows how to get the event associated with an event message.</span></span> <span data-ttu-id="3cc18-150">它使用事件消息 ID 获取事件消息，将事件消息显式强制转换为访问 **event** 导航属性，并应用 $expand 参数来获取事件属性。</span><span class="sxs-lookup"><span data-stu-id="3cc18-150">It uses the event message ID to get the event message, explicitly provides a cast on the event message to access its **event** navigation property, and apply an $expand parameter to get the properties of the event.</span></span>

# <a name="http"></a>[<span data-ttu-id="3cc18-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="3cc18-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADYAAAImV_jAAA="],
  "name": "get_event_based_on_eventmessage"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADYAAAImV_jAAA=?$expand=microsoft.graph.eventMessage/event
```
# <a name="c"></a>[<span data-ttu-id="3cc18-152">C#</span><span class="sxs-lookup"><span data-stu-id="3cc18-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-event-based-on-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3cc18-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3cc18-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-event-based-on-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3cc18-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3cc18-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-event-based-on-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3cc18-155">Java</span><span class="sxs-lookup"><span data-stu-id="3cc18-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-event-based-on-eventmessage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="3cc18-156">响应</span><span class="sxs-lookup"><span data-stu-id="3cc18-156">Response</span></span>
<span data-ttu-id="3cc18-157">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3cc18-157">Here is an example of the response.</span></span> <span data-ttu-id="3cc18-158">响应中返回关联事件的属性。</span><span class="sxs-lookup"><span data-stu-id="3cc18-158">The properties of the associated event are returned in the response.</span></span> <span data-ttu-id="3cc18-159">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3cc18-159">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3cc18-160">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3cc18-160">All of the properties will be returned from an actual call.</span></span>
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
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8fd6e83b-3cc0-4bf0-8b26-950f4d7110f6')/messages/$entity",
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
   "internetMessageId":"<MWHPR1301MB211042CF@MWHPR1301MB2110.namprd13.prod.outlook.com>",
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
   "meetingMessageType":"meetingRequest",
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
   "event@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8fd6e83b-3cc0-4bf0-8b26-950f4d7110f6')/messages('AAMkADYAAAImV_jAAA%3D')/microsoft.graph.eventMessage/event/$entity",
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
      "iCalUId":"040000008200E00074C5B7101A82E00800000000A2A6F3535D7FD3010000000000000000100000003D770E2E8974F44B9471BDB348097FE3",
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
         "displayName":"Mt. Hood"
      },
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
      }
   }
}
``` 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get eventMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->