---
title: List messages
description: '获取登录用户的邮箱（包括“已删除邮件”和“待筛选邮件”文件夹）中的邮件。 '
localization_priority: Normal
ms.openlocfilehash: cc361c3f6a4f41d96eb058fdd5f1fd8ac1d015a1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894598"
---
# <a name="list-messages"></a><span data-ttu-id="2d2aa-103">List messages</span><span class="sxs-lookup"><span data-stu-id="2d2aa-103">List messages</span></span>

> <span data-ttu-id="2d2aa-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2d2aa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2d2aa-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2d2aa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2d2aa-106">获取登录用户的邮箱（包括“已删除邮件”和“待筛选邮件”文件夹）中的邮件。</span><span class="sxs-lookup"><span data-stu-id="2d2aa-106">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span> 

<span data-ttu-id="2d2aa-107">具体而言，您可以对邮件筛选和获取仅包含[提及](../resources/mention.md)的登录用户的那些。</span><span class="sxs-lookup"><span data-stu-id="2d2aa-107">In particular, you can filter on the messages and get only those that include a [mention](../resources/mention.md) of the signed-in user.</span></span>

<span data-ttu-id="2d2aa-108">请注意，默认情况下，`GET /me/messages`操作不会返回**提到**属性。</span><span class="sxs-lookup"><span data-stu-id="2d2aa-108">Note that by default, the `GET /me/messages` operation does not return the **mentions** property.</span></span> <span data-ttu-id="2d2aa-109">使用`$expand`查询参数[找到一条消息中的每个提及的详细信息](../api/message-get.md#request-2)。</span><span class="sxs-lookup"><span data-stu-id="2d2aa-109">Use the `$expand` query parameter to [find details of each mention in a message](../api/message-get.md#request-2).</span></span>

<span data-ttu-id="2d2aa-110">有两种应用程序，另一个用户的邮件文件夹中收到消息的情况：</span><span class="sxs-lookup"><span data-stu-id="2d2aa-110">There are two scenarios where an app can get messages in another user's mail folder:</span></span>

* <span data-ttu-id="2d2aa-111">如果应用程序具有应用程序权限，或，</span><span class="sxs-lookup"><span data-stu-id="2d2aa-111">If the app has application permissions, or,</span></span>
* <span data-ttu-id="2d2aa-112">如果应用程序具有相应从一个用户委派[权限](#permissions)，并另一个用户具有与该用户，共享邮件文件夹，或具有委派的访问赋予该用户。</span><span class="sxs-lookup"><span data-stu-id="2d2aa-112">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="2d2aa-113">请参阅[详细信息和示例](/graph/outlook-share-messages-folders)。</span><span class="sxs-lookup"><span data-stu-id="2d2aa-113">See [details and an example](/graph/outlook-share-messages-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="2d2aa-114">权限</span><span class="sxs-lookup"><span data-stu-id="2d2aa-114">Permissions</span></span>
<span data-ttu-id="2d2aa-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2d2aa-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d2aa-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="2d2aa-117">Permission type</span></span>      | <span data-ttu-id="2d2aa-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2d2aa-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d2aa-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2d2aa-119">Delegated (work or school account)</span></span> | <span data-ttu-id="2d2aa-120">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d2aa-120">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2d2aa-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2d2aa-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d2aa-122">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d2aa-122">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2d2aa-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="2d2aa-123">Application</span></span> | <span data-ttu-id="2d2aa-124">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d2aa-124">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d2aa-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2d2aa-125">HTTP request</span></span>

<span data-ttu-id="2d2aa-126">若要获取用户邮箱中的所有邮件，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="2d2aa-126">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="2d2aa-127">若要获取用户邮箱中特定文件夹中的邮件，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="2d2aa-127">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

<span data-ttu-id="2d2aa-128">若要获取包括**提及**的用户的用户的邮箱中的所有邮件：</span><span class="sxs-lookup"><span data-stu-id="2d2aa-128">To get all the messages in the user's mailbox that include a **mention** of the user:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=mentionsPreview/isMentioned eq true
GET /users/{id | userPrincipalName}/messages?$filter=mentionsPreview/isMentioned eq true
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2d2aa-129">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2d2aa-129">Optional query parameters</span></span>
<span data-ttu-id="2d2aa-130">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2d2aa-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="2d2aa-131">您可以使用`$filter`查询**mentionsPreview**属性来获取这些消息是否有提及登录用户的参数。</span><span class="sxs-lookup"><span data-stu-id="2d2aa-131">You can use the `$filter` query parameter on the **mentionsPreview** property to get those messages that mention the signed-in user.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2d2aa-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="2d2aa-132">Request headers</span></span>
| <span data-ttu-id="2d2aa-133">名称</span><span class="sxs-lookup"><span data-stu-id="2d2aa-133">Name</span></span>       | <span data-ttu-id="2d2aa-134">类型</span><span class="sxs-lookup"><span data-stu-id="2d2aa-134">Type</span></span> | <span data-ttu-id="2d2aa-135">说明</span><span class="sxs-lookup"><span data-stu-id="2d2aa-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2d2aa-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d2aa-136">Authorization</span></span>  | <span data-ttu-id="2d2aa-137">string</span><span class="sxs-lookup"><span data-stu-id="2d2aa-137">string</span></span>  | <span data-ttu-id="2d2aa-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2d2aa-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2d2aa-140">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="2d2aa-140">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="2d2aa-141">string</span><span class="sxs-lookup"><span data-stu-id="2d2aa-141">string</span></span> | <span data-ttu-id="2d2aa-142">要返回的 **body** 和 **uniqueBody** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="2d2aa-142">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="2d2aa-143">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="2d2aa-143">Values can be "text" or "html".</span></span> <span data-ttu-id="2d2aa-144">如果未指定此头，采用 HTML 格式返回 **body** 和 **uniqueBody** 属性。</span><span class="sxs-lookup"><span data-stu-id="2d2aa-144">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="2d2aa-145">可选。</span><span class="sxs-lookup"><span data-stu-id="2d2aa-145">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2d2aa-146">请求正文</span><span class="sxs-lookup"><span data-stu-id="2d2aa-146">Request body</span></span>
<span data-ttu-id="2d2aa-147">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2d2aa-147">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d2aa-148">响应</span><span class="sxs-lookup"><span data-stu-id="2d2aa-148">Response</span></span>

<span data-ttu-id="2d2aa-149">如果成功，此方法返回`200 OK`响应代码和响应正文中的[消息](../resources/message.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="2d2aa-149">If successful, this method returns a `200 OK` response code and collection of [message](../resources/message.md) objects in the response body.</span></span>

<span data-ttu-id="2d2aa-150">此请求的默认页面大小为 10 封邮件。</span><span class="sxs-lookup"><span data-stu-id="2d2aa-150">The default page size for this request is 10 messages.</span></span> 

## <a name="example"></a><span data-ttu-id="2d2aa-151">示例</span><span class="sxs-lookup"><span data-stu-id="2d2aa-151">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="2d2aa-152">请求 1</span><span class="sxs-lookup"><span data-stu-id="2d2aa-152">Request 1</span></span>
<span data-ttu-id="2d2aa-153">第一个示例获取已登录的用户邮箱中的顶部的 10 条消息。</span><span class="sxs-lookup"><span data-stu-id="2d2aa-153">The first example gets the top 10 messages in the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages
```
##### <a name="response-1"></a><span data-ttu-id="2d2aa-154">响应 1</span><span class="sxs-lookup"><span data-stu-id="2d2aa-154">Response 1</span></span>
<span data-ttu-id="2d2aa-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2d2aa-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 317

{
  "value": [
    {
      "receivedDateTime": "2016-10-19T10:37:00Z",
      "sentDateTime": "2016-10-19T10:37:00Z",
      "hasAttachments": true,
      "subject": "subject-value",
      "body": {
        "contentType": "",
        "content": "content-value"
      },
      "bodyPreview": "bodyPreview-value"
    }
  ]
}
```


##### <a name="request-2"></a><span data-ttu-id="2d2aa-158">请求 2</span><span class="sxs-lookup"><span data-stu-id="2d2aa-158">Request 2</span></span>
<span data-ttu-id="2d2aa-159">下一个示例为那些提及用户筛选器已登录的用户邮箱中的所有邮件。</span><span class="sxs-lookup"><span data-stu-id="2d2aa-159">The next example filters all messages in the signed-in user's mailbox for those that mention the user.</span></span> <span data-ttu-id="2d2aa-160">它使用`$select`的响应中返回的属性的每条消息子集。</span><span class="sxs-lookup"><span data-stu-id="2d2aa-160">It uses `$select` to return a subset of the properties of each message in the response.</span></span> 

<span data-ttu-id="2d2aa-161">此示例还包含 URL 的查询参数字符串中的空格字符编码。</span><span class="sxs-lookup"><span data-stu-id="2d2aa-161">The example also incorporates URL encoding for the space characters in the query parameter string.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages_with_mentions"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=MentionsPreview/IsMentioned%20eq%20true&$select=Subject,Sender,ReceivedDateTime,MentionsPreview
```
##### <a name="response-2"></a><span data-ttu-id="2d2aa-162">响应 2</span><span class="sxs-lookup"><span data-stu-id="2d2aa-162">Response 2</span></span>
<span data-ttu-id="2d2aa-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2d2aa-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 987

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/messages(subject,sender,receivedDateTime,mentionsPreview)",
  "value":[
    {
      "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAgVZAAAA')",
      "@odata.etag":"W/\"CQAAABYAAAAPFhK2FclcRbABBJhCde8iAAAAAATI\"",
      "id":"AQMkADJmMTUAAAgVZAAAA",
      "receivedDateTime":"2016-07-21T07:40:21Z",
      "subject":"Re: Start planning soon",
      "sender":{
        "emailAddress":{
          "name":"Randi Welch",
          "address":"randiw@contoso.onmicrosoft.com"
        }
      },
      "mentionsPreview":{
        "isMentioned":true
      }
    },
    {
      "@odata.id":"https://graph.microsoft.com/beta/Users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/Messages('AQMkADJmMTUAAAjwVAAAA')",
      "@odata.etag":"W/\"CQAAABYAAAAPFhK2FclcRbABBJhCde8iAAAAAEGj\"",
      "id":"AQMkADJmMTUAAAjwVAAAA",
      "receivedDateTime":"2016-07-21T07:40:20Z",
      "subject":"Re: Start planning soon",
      "sender":{
        "emailAddress":{
          "name":"Randi Welch",
          "address":"randiw@contoso.onmicrosoft.com"
        }
      },
      "mentionsPreview":{
        "isMentioned":true
      }
    }
  ]
}
```

##### <a name="request-3"></a><span data-ttu-id="2d2aa-166">请求 3</span><span class="sxs-lookup"><span data-stu-id="2d2aa-166">Request 3</span></span>
<span data-ttu-id="2d2aa-167">第三个示例演示如何使用`Prefer: outlook.body-content-type="text"`标头以获取每封邮件的**正文**和**uniqueBody**属性以文本格式。</span><span class="sxs-lookup"><span data-stu-id="2d2aa-167">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** properties of each message in text format.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages_in_text"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```
##### <a name="response-3"></a><span data-ttu-id="2d2aa-168">响应 3</span><span class="sxs-lookup"><span data-stu-id="2d2aa-168">Response 3</span></span>
<span data-ttu-id="2d2aa-169">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2d2aa-169">Here is an example of the response.</span></span> 

<!--
Note: The response includes a `Preference-Applied: outlook.body-content-type` header to acknowledge the `Prefer: outlook.body-content-type` request header.
-->

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2704

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/messages(subject,body,bodyPreview,uniqueBody)",
    "value":[
        {
            "@odata.type":"#microsoft.graph.eventMessageRequest",
            "@odata.etag":"W/\"CwAAABYAAABmWdbhEgBXTophjCWt81m9AAAoZYj5\"",
            "id":"AAMkAGIAAAoZCfIAAA=",
            "subject":"Orientation ",
            "bodyPreview":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.",
            "body":{
                "contentType":"text",
                "content":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.\r\n"
            },
            "uniqueBody":{
                "contentType":"text",
                "content":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.\r\n"
            }
        },
        {
            "@odata.etag":"W/\"CQAAABYAAABmWdbhEgBXTophjCWt81m9AAAoZYj4\"",
            "id":"AAMkAGIAAAoZCfHAAA=",
            "subject":"Welcome to our group!",
            "bodyPreview":"Welcome to our group, Dana! Hope you will enjoy working with us !\r\n\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\n\r\nTh",
            "body":{
                "contentType":"text",
                "content":"Welcome to our group, Dana! Hope you will enjoy working with us [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] !\r\n\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\n\r\nThanks!\r\n\r\n"
            },
            "uniqueBody":{
                "contentType":"text",
                "content":"Welcome to our group, Dana! Hope you will enjoy working with us [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] !\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\nThanks!\r\n"
            }
        },
        {
            "@odata.etag":"W/\"CQAAABYAAABmWdbhEgBXTophjCWt81m9AAAAAAjr\"",
            "id":"AQMkAGIAAAIJTQAAAA==",
            "subject":"Welcome aboard!",
            "bodyPreview":"Welcome to the Support group!",
            "body":{
                "contentType":"text",
                "content":"Welcome to the Support group!\r\n"
            },
            "uniqueBody":{
                "contentType":"text",
                "content":"Welcome to the Support group!\r\n"
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
