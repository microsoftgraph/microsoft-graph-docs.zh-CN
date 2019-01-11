---
title: 获取邮件
description: 检索的属性和 message 对象的关系。
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 5c83d0e9a59a69ebf0e20cfa0f883301b827c84f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852386"
---
# <a name="get-message"></a><span data-ttu-id="5dd0b-103">获取邮件</span><span class="sxs-lookup"><span data-stu-id="5dd0b-103">Get message</span></span>

> <span data-ttu-id="5dd0b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5dd0b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5dd0b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5dd0b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5dd0b-106">检索的属性和[message](../resources/message.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="5dd0b-106">Retrieve the properties and relationships of the [message](../resources/message.md) object.</span></span>

<span data-ttu-id="5dd0b-107">例如，您可以收到一条消息，展开邮件中所有[提及](../resources/mention.md)的实例。</span><span class="sxs-lookup"><span data-stu-id="5dd0b-107">For example, you can get a message and expand all the [mention](../resources/mention.md) instances in the message.</span></span>

<span data-ttu-id="5dd0b-108">有两种方案，其中应用程序可以在另一个用户的邮件文件夹中收到一条消息：</span><span class="sxs-lookup"><span data-stu-id="5dd0b-108">There are two scenarios where an app can get a message in another user's mail folder:</span></span>

* <span data-ttu-id="5dd0b-109">如果应用程序具有应用程序权限，或，</span><span class="sxs-lookup"><span data-stu-id="5dd0b-109">If the app has application permissions, or,</span></span>
* <span data-ttu-id="5dd0b-110">如果应用程序具有相应从一个用户委派[权限](#permissions)，并另一个用户具有与该用户，共享邮件文件夹，或具有委派的访问赋予该用户。</span><span class="sxs-lookup"><span data-stu-id="5dd0b-110">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="5dd0b-111">请参阅[详细信息和示例](/graph/outlook-share-messages-folders)。</span><span class="sxs-lookup"><span data-stu-id="5dd0b-111">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

<span data-ttu-id="5dd0b-112">由于**邮件**资源支持[扩展](/graph/extensibility-overview)，因此也可使用 `GET` 操作获取**邮件**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="5dd0b-112">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>


## <a name="permissions"></a><span data-ttu-id="5dd0b-113">权限</span><span class="sxs-lookup"><span data-stu-id="5dd0b-113">Permissions</span></span>
<span data-ttu-id="5dd0b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5dd0b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5dd0b-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="5dd0b-116">Permission type</span></span>      | <span data-ttu-id="5dd0b-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5dd0b-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5dd0b-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5dd0b-118">Delegated (work or school account)</span></span> | <span data-ttu-id="5dd0b-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5dd0b-119">Mail.Read</span></span>    |
|<span data-ttu-id="5dd0b-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5dd0b-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5dd0b-121">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5dd0b-121">Mail.Read</span></span>    |
|<span data-ttu-id="5dd0b-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="5dd0b-122">Application</span></span> | <span data-ttu-id="5dd0b-123">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5dd0b-123">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="5dd0b-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5dd0b-124">HTTP request</span></span>

<span data-ttu-id="5dd0b-125">若要获取指定的消息：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5dd0b-125">To get the specified message: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="5dd0b-126">收到一条消息，并展开邮件中的所有提及：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5dd0b-126">To get a message and expand all mentions in the message: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages/{id}?$expand=mentions
GET /users/{id | userPrincipalName}/messages/{id}?$expand=mentions
GET /me/mailFolders/{id}/messages/{id}?$expand=mentions
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}?$expand=mentions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5dd0b-127">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5dd0b-127">Optional query parameters</span></span>
<span data-ttu-id="5dd0b-128">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5dd0b-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="5dd0b-129">您可以使用`$expand`上的**提到**导航属性获取邮件中包含的每个[提及](../resources/mention.md)的详细信息的消息的查询参数扩展。</span><span class="sxs-lookup"><span data-stu-id="5dd0b-129">You can use the `$expand` query parameter on the **mentions** navigation property to get a message with the details of each [mention](../resources/mention.md) in the message expanded.</span></span>



## <a name="request-headers"></a><span data-ttu-id="5dd0b-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="5dd0b-130">Request headers</span></span>
| <span data-ttu-id="5dd0b-131">名称</span><span class="sxs-lookup"><span data-stu-id="5dd0b-131">Name</span></span>       | <span data-ttu-id="5dd0b-132">类型</span><span class="sxs-lookup"><span data-stu-id="5dd0b-132">Type</span></span> | <span data-ttu-id="5dd0b-133">说明</span><span class="sxs-lookup"><span data-stu-id="5dd0b-133">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5dd0b-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="5dd0b-134">Authorization</span></span>  | <span data-ttu-id="5dd0b-135">string</span><span class="sxs-lookup"><span data-stu-id="5dd0b-135">string</span></span>  | <span data-ttu-id="5dd0b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5dd0b-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5dd0b-138">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="5dd0b-138">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="5dd0b-139">string</span><span class="sxs-lookup"><span data-stu-id="5dd0b-139">string</span></span> | <span data-ttu-id="5dd0b-140">要返回的 **body** 和 **uniqueBody** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="5dd0b-140">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="5dd0b-141">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="5dd0b-141">Values can be "text" or "html".</span></span> <span data-ttu-id="5dd0b-142">如果指定此 `Preference-Applied` 头，返回 `Prefer` 头作为证明。</span><span class="sxs-lookup"><span data-stu-id="5dd0b-142">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="5dd0b-143">如果未指定此头，采用 HTML 格式返回 **body** 和 **uniqueBody** 属性。</span><span class="sxs-lookup"><span data-stu-id="5dd0b-143">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="5dd0b-144">可选。</span><span class="sxs-lookup"><span data-stu-id="5dd0b-144">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5dd0b-145">请求正文</span><span class="sxs-lookup"><span data-stu-id="5dd0b-145">Request body</span></span>
<span data-ttu-id="5dd0b-146">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5dd0b-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5dd0b-147">响应</span><span class="sxs-lookup"><span data-stu-id="5dd0b-147">Response</span></span>

<span data-ttu-id="5dd0b-148">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5dd0b-148">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5dd0b-149">示例</span><span class="sxs-lookup"><span data-stu-id="5dd0b-149">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="5dd0b-150">请求 1</span><span class="sxs-lookup"><span data-stu-id="5dd0b-150">Request 1</span></span>
<span data-ttu-id="5dd0b-151">第一个示例获取指定的消息。</span><span class="sxs-lookup"><span data-stu-id="5dd0b-151">The first example gets the specified message.</span></span> <span data-ttu-id="5dd0b-152">它不指定任何标头，以指示要返回的正文的所需的格式。</span><span class="sxs-lookup"><span data-stu-id="5dd0b-152">It does not specify any header to indicate the desired format of the body to be returned.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages('AAMkAGI1AAAoZCfHAAA=')
```
##### <a name="response-1"></a><span data-ttu-id="5dd0b-153">响应 1</span><span class="sxs-lookup"><span data-stu-id="5dd0b-153">Response 1</span></span>
<span data-ttu-id="5dd0b-154">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5dd0b-154">Here is an example of the response.</span></span> <span data-ttu-id="5dd0b-155">**正文**和**uniqueBody**属性中的默认 HTML 格式返回。</span><span class="sxs-lookup"><span data-stu-id="5dd0b-155">The **body** and **uniqueBody** properties are returned in the default HTML format.</span></span>
<span data-ttu-id="5dd0b-156">注意： 为了简单起见截断如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5dd0b-156">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="5dd0b-157">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5dd0b-157">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 523

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/messages/$entity",
    "@odata.etag":"W/\"CQAAABYAAABmWdbhEgBXTophjCWt81m9AAAoZYj4\"",
    "id":"AAMkAGI1AAAoZCfHAAA=",
    "subject":"Welcome to our group!",
    "bodyPreview":"Welcome to our group, Dana! Hope you will enjoy working with us !\r\n",
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head></head><body><p>Welcome to our group, Dana! Hope you will enjoy working with us </p></body></html>\r\n"
    },
    "uniqueBody":{
        "contentType":"html",
        "content":"<html>\r\n<head></head><body><p>Welcome to our group, Dana! Hope you will enjoy working with us </p></body></html>\r\n"
    }
}
```

##### <a name="request-2"></a><span data-ttu-id="5dd0b-158">请求 2</span><span class="sxs-lookup"><span data-stu-id="5dd0b-158">Request 2</span></span>
<span data-ttu-id="5dd0b-159">在下一个示例中，已登录的用户是 Dana Swope。</span><span class="sxs-lookup"><span data-stu-id="5dd0b-159">In the next example, the signed-in user is Dana Swope.</span></span> <span data-ttu-id="5dd0b-160">该示例演示 Dana 的邮箱中获取指定的消息中的所有提及的详细信息。</span><span class="sxs-lookup"><span data-stu-id="5dd0b-160">The example shows getting the details of all the mentions in the specified message in Dana's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AQMkADJmMTUAAAgVZAAAA"],
  "name": "get_mentions_in_message"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages/('AQMkADJmMTUAAAgVZAAAA')?$expand=mentions
```
##### <a name="response-2"></a><span data-ttu-id="5dd0b-161">响应 2</span><span class="sxs-lookup"><span data-stu-id="5dd0b-161">Response 2</span></span>
<span data-ttu-id="5dd0b-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5dd0b-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2248

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/messages/$entity",
  "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAgVZAAAA')",
  "@odata.etag":"W/\"CQAAABYAAAAPFhK2FclcRbABBJhCde8iAAAAAATI\"",
  "id":"AQMkADJmMTUAAAgVZAAAA",
  "subject":"Start planning soon",
  "body":{
    "contentType":"HTML",
    "content":"<html><head></head><body><p><a href=\"mailto:danas@contoso.onmicrosoft.com\">@Dana Swope</a>,<a href=\"mailto:randiw@contoso.onmicrosoft.com\">@Randi Welch</a>, forgot to mention, I will be away&nbsp;this weekend. I can start on Monday though.</p></body></html>"
  },
  "bodyPreview":"@Dana Swope<mailto:danas@contoso.onmicrosoft.com>, @Randi Welch, forgot to mention, I will be away this weekend. I can start on Monday though.",
  "sender":{
    "emailAddress":{
      "name":"Samantha Booth",
      "address":"samanthab@contoso.onmicrosoft.com"
    }
  },
  "from":{
    "emailAddress":{
      "name":"Samantha Booth",
      "address":"samanthab@contoso.onmicrosoft.com"
    }
  },
  "toRecipients":[
    {
      "emailAddress":{
        "name":"Dana Swope",
        "address":"danas@contoso.onmicrosoft.com"
      }
    },
    {
      "emailAddress":{
        "name":"Randi Welch",
        "address":"randiw@contoso.onmicrosoft.com"
      }
    }
  ],
  "ccRecipients":[
  ],
  "bccRecipients":[
  ],
  "mentionsPreview":{
    "isMentioned":true
  },
  "mentions@odata.context":"https://graph.microsoft.com/beta/$metadata#me/messages('AQMkADJmMTUAAAgVZAAAA')/mentions",
  "mentions":[
    {
      "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAgVZAAAA')/mentions('138f4c0a-1130-4776-b780-bf79d73abb3f')",
      "id":"138f4c0a-1130-4776-b780-bf79d73abb3f",
      "mentioned":{
        "name":"Dana Swope",
        "address":"danas@contoso.onmicrosoft.com"
      },
      "mentionText":null,
      "clientReference":null,
      "createdBy":{
        "name":"Samantha Booth",
        "address":"samanthab@contoso.onmicrosoft.com"
      },
      "createdDateTime":"2016-07-21T07:40:20.152Z",
      "serverCreatedDateTime":"2016-07-21T07:40:20.152Z",
      "deepLink":null,
      "application":null
    },
    {
      "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAgVZAAAA')/mentions('7b94df1a-0086-482a-b0da-e62fae12f983')",
      "id":"7b94df1a-0086-482a-b0da-e62fae12f983",
      "mentioned":{
        "name":"Randi Welch",
        "address":"randiw@contoso.onmicrosoft.com"
      },
      "mentionText":null,
      "clientReference":null,
      "createdBy":{
        "name":"Samantha Booth",
        "address":"samanthab@contoso.onmicrosoft.com"
      },
      "createdDateTime":"2016-07-21T07:40:20.158Z",
      "serverCreatedDateTime":"2016-07-21T07:40:20.158Z",
      "deepLink":null,
      "application":null
    }
  ]
}
```


##### <a name="request-3"></a><span data-ttu-id="5dd0b-165">请求 3</span><span class="sxs-lookup"><span data-stu-id="5dd0b-165">Request 3</span></span>

<span data-ttu-id="5dd0b-166">第三个示例演示如何使用`Prefer: outlook.body-content-type="text"`标头以获取的**正文**和**uniqueBody**指定的消息的文本格式。</span><span class="sxs-lookup"><span data-stu-id="5dd0b-166">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** of the specified message in text format.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message_in_text"
}-->

```http
GET https://graph.microsoft.com/beta/me/messages('AAMkAGI1AAAoZCfHAAA=')?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```

##### <a name="response-3"></a><span data-ttu-id="5dd0b-167">响应 3</span><span class="sxs-lookup"><span data-stu-id="5dd0b-167">Response 3</span></span>

<span data-ttu-id="5dd0b-168">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5dd0b-168">Here is an example of the response.</span></span> <span data-ttu-id="5dd0b-169">注意： 该响应包括`Preference-Applied: outlook.body-content-type`标头以确认`Prefer: outlook.body-content-type`请求标头。</span><span class="sxs-lookup"><span data-stu-id="5dd0b-169">Note: The response includes a `Preference-Applied: outlook.body-content-type` header to acknowledge the `Prefer: outlook.body-content-type` request header.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.body-content-type="text"
Content-length: 1550

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/messages(subject,body,bodyPreview,uniqueBody)/$entity",
    "@odata.etag":"W/\"CQAAABYAAABmWdbhEgBXTophjCWt81m9AAAoZYj4\"",
    "id":"AAMkAGI1AAAoZCfHAAA=",
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
}
```

##### <a name="request-4"></a><span data-ttu-id="5dd0b-170">请求 4</span><span class="sxs-lookup"><span data-stu-id="5dd0b-170">Request 4</span></span>

<span data-ttu-id="5dd0b-171">第四个示例演示如何获取特定邮件的 Internet 邮件标头。</span><span class="sxs-lookup"><span data-stu-id="5dd0b-171">The fourth example shows how to get the Internet message headers of a specific message.</span></span>  

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEz"],
  "name": "get_message_internet_headers"
}-->

```http
GET https://graph.microsoft.com/beta/me/messages('AAMkAGVmMDEz')?$select=internetMessageHeaders
```

##### <a name="response-4"></a><span data-ttu-id="5dd0b-172">响应 4</span><span class="sxs-lookup"><span data-stu-id="5dd0b-172">Response 4</span></span>

<span data-ttu-id="5dd0b-173">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5dd0b-173">Here is an example of the response.</span></span> <span data-ttu-id="5dd0b-174">注意： 响应对象中的 Internet 邮件头数减少了为简便起见。</span><span class="sxs-lookup"><span data-stu-id="5dd0b-174">Note: The number of Internet message headers in the response object has been reduced for brevity.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('48d31887-5fad-4d73-a9f5-3c356e68a038')/messages(internetMessageHeaders)/$entity",
  "@odata.type":"#microsoft.graph.eventMessageRequest",
  "@odata.etag":"W/\"CwAAABYAAAAiIsqMbYjsT5e/T7KzowPTAAAa/qUB\"",
  "id":"AAMkAGVmMDEz",
  "internetMessageHeaders":[
    {
      "name":"Content-Type",
      "value":"application/ms-tnef"
    },
    {
      "name":"Content-Transfer-Encoding",
      "value":"binary"
    },
    {
      "name":"Subject",
      "value":"Cloud and Mobile Working Group"
    },
    {
      "name":"x-custom-header-group-name",
      "value":"Washington"
    },
    {
      "name":"x-custom-header-group-id",
      "value":"WA001"
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="5dd0b-175">另请参阅</span><span class="sxs-lookup"><span data-stu-id="5dd0b-175">See also</span></span>

- [<span data-ttu-id="5dd0b-176">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="5dd0b-176">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="5dd0b-177">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="5dd0b-177">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="5dd0b-178">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="5dd0b-178">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
