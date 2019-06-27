---
title: 获取邮件
description: 检索 message 对象的属性和关系。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 85d31fa1758eb54347fa96bcb0ee0ea3791ad47c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266540"
---
# <a name="get-message"></a><span data-ttu-id="7330c-103">获取邮件</span><span class="sxs-lookup"><span data-stu-id="7330c-103">Get message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7330c-104">检索[message](../resources/message.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7330c-104">Retrieve the properties and relationships of the [message](../resources/message.md) object.</span></span>

<span data-ttu-id="7330c-105">例如, 您可以收到一条消息, 并在邮件中展开所有[提及](../resources/mention.md)的实例。</span><span class="sxs-lookup"><span data-stu-id="7330c-105">For example, you can get a message and expand all the [mention](../resources/mention.md) instances in the message.</span></span>

<span data-ttu-id="7330c-106">您可以使用`$value`参数来[获取邮件的 MIME 内容](/graph/outlook-get-mime-message)。</span><span class="sxs-lookup"><span data-stu-id="7330c-106">You can use the `$value` parameter to [get the MIME content of a message](/graph/outlook-get-mime-message).</span></span>

<span data-ttu-id="7330c-107">在以下两种情况下，应用可以获取其他用户的邮件文件夹中的邮件：</span><span class="sxs-lookup"><span data-stu-id="7330c-107">There are two scenarios where an app can get a message in another user's mail folder:</span></span>

* <span data-ttu-id="7330c-108">如果该应用具有应用程序权限，或者</span><span class="sxs-lookup"><span data-stu-id="7330c-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="7330c-109">如果应用具有来自某个用户的相应委派[权限](#permissions)，而另一个用户与该用户共享了邮件文件夹，或者已为该用户授予委派的访问权限。</span><span class="sxs-lookup"><span data-stu-id="7330c-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="7330c-110">请参阅[详细信息和示例](/graph/outlook-share-messages-folders)。</span><span class="sxs-lookup"><span data-stu-id="7330c-110">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

<span data-ttu-id="7330c-111">由于**邮件**资源支持[扩展](/graph/extensibility-overview)，因此也可使用 `GET` 操作获取**邮件**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="7330c-111">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>


## <a name="permissions"></a><span data-ttu-id="7330c-112">权限</span><span class="sxs-lookup"><span data-stu-id="7330c-112">Permissions</span></span>
<span data-ttu-id="7330c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7330c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7330c-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="7330c-115">Permission type</span></span>      | <span data-ttu-id="7330c-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7330c-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7330c-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7330c-117">Delegated (work or school account)</span></span> | <span data-ttu-id="7330c-118">User.readbasic.all、Mail. Read</span><span class="sxs-lookup"><span data-stu-id="7330c-118">Mail.ReadBasic, Mail.Read</span></span>    |
|<span data-ttu-id="7330c-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7330c-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7330c-120">User.readbasic.all、Mail. Read</span><span class="sxs-lookup"><span data-stu-id="7330c-120">Mail.ReadBasic, Mail.Read</span></span>    |
|<span data-ttu-id="7330c-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="7330c-121">Application</span></span> | <span data-ttu-id="7330c-122">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="7330c-122">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="7330c-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7330c-123">HTTP request</span></span>

<span data-ttu-id="7330c-124">若要获取指定的邮件:</span><span class="sxs-lookup"><span data-stu-id="7330c-124">To get the specified message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="7330c-125">若要获取指定邮件的 MIME 内容, 请执行以下操作:</span><span class="sxs-lookup"><span data-stu-id="7330c-125">To get the MIME content of the specified message:</span></span>
<!-- { "blockType": "ignored" } --> 
```http 
GET /me/messages/{id}/$value 
GET /users/{id | userPrincipalName}/messages/{id}/$value 
GET /me/mailFolders/{id}/messages/{id}/$value 
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/$value 
```

<span data-ttu-id="7330c-126">若要获取邮件并展开邮件中的所有提及内容, 请执行以下操作:</span><span class="sxs-lookup"><span data-stu-id="7330c-126">To get a message and expand all mentions in the message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=mentions
GET /users/{id | userPrincipalName}/messages/{id}?$expand=mentions
GET /me/mailFolders/{id}/messages/{id}?$expand=mentions
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}?$expand=mentions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7330c-127">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7330c-127">Optional query parameters</span></span>
<span data-ttu-id="7330c-128">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7330c-128">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="7330c-129">使用`$value`参数获取邮件的 MIME 内容。</span><span class="sxs-lookup"><span data-stu-id="7330c-129">Use the `$value` parameter to get the MIME content of a message.</span></span>

<span data-ttu-id="7330c-130">使用 " `$expand` **提及**" 导航属性上的查询参数, 可以获取消息, 其中包含已展开邮件中每个[提及](../resources/mention.md)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="7330c-130">Use the `$expand` query parameter on the **mentions** navigation property to get a message with the details of each [mention](../resources/mention.md) in the message expanded.</span></span>



## <a name="request-headers"></a><span data-ttu-id="7330c-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="7330c-131">Request headers</span></span>
| <span data-ttu-id="7330c-132">名称</span><span class="sxs-lookup"><span data-stu-id="7330c-132">Name</span></span>       | <span data-ttu-id="7330c-133">类型</span><span class="sxs-lookup"><span data-stu-id="7330c-133">Type</span></span> | <span data-ttu-id="7330c-134">说明</span><span class="sxs-lookup"><span data-stu-id="7330c-134">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7330c-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="7330c-135">Authorization</span></span>  | <span data-ttu-id="7330c-136">string</span><span class="sxs-lookup"><span data-stu-id="7330c-136">string</span></span>  | <span data-ttu-id="7330c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7330c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7330c-139">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="7330c-139">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="7330c-140">string</span><span class="sxs-lookup"><span data-stu-id="7330c-140">string</span></span> | <span data-ttu-id="7330c-141">要返回的 **body** 和 **uniqueBody** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="7330c-141">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="7330c-142">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="7330c-142">Values can be "text" or "html".</span></span> <span data-ttu-id="7330c-143">如果指定此 `Preference-Applied` 头，返回 `Prefer` 头作为证明。</span><span class="sxs-lookup"><span data-stu-id="7330c-143">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="7330c-144">如果未指定此头，采用 HTML 格式返回 **body** 和 **uniqueBody** 属性。</span><span class="sxs-lookup"><span data-stu-id="7330c-144">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="7330c-145">可选。</span><span class="sxs-lookup"><span data-stu-id="7330c-145">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7330c-146">请求正文</span><span class="sxs-lookup"><span data-stu-id="7330c-146">Request body</span></span>
<span data-ttu-id="7330c-147">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7330c-147">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7330c-148">响应</span><span class="sxs-lookup"><span data-stu-id="7330c-148">Response</span></span>

<span data-ttu-id="7330c-149">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7330c-149">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7330c-150">示例</span><span class="sxs-lookup"><span data-stu-id="7330c-150">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="7330c-151">请求 1</span><span class="sxs-lookup"><span data-stu-id="7330c-151">Request 1</span></span>
<span data-ttu-id="7330c-152">第一个示例获取指定的邮件。</span><span class="sxs-lookup"><span data-stu-id="7330c-152">The first example gets the specified message.</span></span> <span data-ttu-id="7330c-153">它不指定任何标头以指示要返回的正文的所需格式。</span><span class="sxs-lookup"><span data-stu-id="7330c-153">It does not specify any header to indicate the desired format of the body to be returned.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages/AAMkAGI1AAAoZCfHAAA=
```
##### <a name="response-1"></a><span data-ttu-id="7330c-154">响应 1</span><span class="sxs-lookup"><span data-stu-id="7330c-154">Response 1</span></span>
<span data-ttu-id="7330c-155">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7330c-155">Here is an example of the response.</span></span> <span data-ttu-id="7330c-156">**Body**和**uniqueBody**属性以默认的 HTML 格式返回。</span><span class="sxs-lookup"><span data-stu-id="7330c-156">The **body** and **uniqueBody** properties are returned in the default HTML format.</span></span>
<span data-ttu-id="7330c-157">注意: 为简洁起见, 此处显示的响应对象将被截断。</span><span class="sxs-lookup"><span data-stu-id="7330c-157">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="7330c-158">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7330c-158">All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="7330c-159">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="7330c-159">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7330c-160">C#</span><span class="sxs-lookup"><span data-stu-id="7330c-160">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_message-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7330c-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="7330c-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_message-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7330c-162">目标-C</span><span class="sxs-lookup"><span data-stu-id="7330c-162">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_message-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-2"></a><span data-ttu-id="7330c-163">请求 2</span><span class="sxs-lookup"><span data-stu-id="7330c-163">Request 2</span></span>
<span data-ttu-id="7330c-164">在下一个示例中, 登录用户是 Dana Swope。</span><span class="sxs-lookup"><span data-stu-id="7330c-164">In the next example, the signed-in user is Dana Swope.</span></span> <span data-ttu-id="7330c-165">此示例显示了如何获取 Dana 的邮箱中指定邮件中所有提及内容的详细信息。</span><span class="sxs-lookup"><span data-stu-id="7330c-165">The example shows getting the details of all the mentions in the specified message in Dana's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AQMkADJmMTUAAAgVZAAAA"],
  "name": "get_mentions_in_message"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages/AQMkADJmMTUAAAgVZAAAA/?$expand=mentions
```
##### <a name="response-2"></a><span data-ttu-id="7330c-166">响应 2</span><span class="sxs-lookup"><span data-stu-id="7330c-166">Response 2</span></span>
<span data-ttu-id="7330c-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7330c-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="7330c-170">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="7330c-170">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7330c-171">C#</span><span class="sxs-lookup"><span data-stu-id="7330c-171">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_mentions_in_message-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7330c-172">Javascript</span><span class="sxs-lookup"><span data-stu-id="7330c-172">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_mentions_in_message-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7330c-173">目标-C</span><span class="sxs-lookup"><span data-stu-id="7330c-173">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_mentions_in_message-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


##### <a name="request-3"></a><span data-ttu-id="7330c-174">请求 3</span><span class="sxs-lookup"><span data-stu-id="7330c-174">Request 3</span></span>

<span data-ttu-id="7330c-175">第三个示例演示如何使用`Prefer: outlook.body-content-type="text"`标头以文本格式获取指定邮件的**正文**和**uniqueBody** 。</span><span class="sxs-lookup"><span data-stu-id="7330c-175">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** of the specified message in text format.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message_in_text"
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkAGI1AAAoZCfHAAA=/?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```

##### <a name="response-3"></a><span data-ttu-id="7330c-176">响应 3</span><span class="sxs-lookup"><span data-stu-id="7330c-176">Response 3</span></span>

<span data-ttu-id="7330c-177">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7330c-177">Here is an example of the response.</span></span> <span data-ttu-id="7330c-178">注意: 响应包括用于确认`Preference-Applied: outlook.body-content-type` `Prefer: outlook.body-content-type`请求标头的标头。</span><span class="sxs-lookup"><span data-stu-id="7330c-178">Note: The response includes a `Preference-Applied: outlook.body-content-type` header to acknowledge the `Prefer: outlook.body-content-type` request header.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="7330c-179">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="7330c-179">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7330c-180">C#</span><span class="sxs-lookup"><span data-stu-id="7330c-180">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_message_in_text-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7330c-181">Javascript</span><span class="sxs-lookup"><span data-stu-id="7330c-181">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_message_in_text-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7330c-182">目标-C</span><span class="sxs-lookup"><span data-stu-id="7330c-182">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_message_in_text-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-4"></a><span data-ttu-id="7330c-183">请求 4</span><span class="sxs-lookup"><span data-stu-id="7330c-183">Request 4</span></span>

<span data-ttu-id="7330c-184">第四个示例演示如何获取特定邮件的 Internet 邮件头。</span><span class="sxs-lookup"><span data-stu-id="7330c-184">The fourth example shows how to get the Internet message headers of a specific message.</span></span>  

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEz"],
  "name": "get_message_internet_headers"
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkAGVmMDEz/?$select=internetMessageHeaders
```

##### <a name="response-4"></a><span data-ttu-id="7330c-185">响应 4</span><span class="sxs-lookup"><span data-stu-id="7330c-185">Response 4</span></span>

<span data-ttu-id="7330c-186">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7330c-186">Here is an example of the response.</span></span> <span data-ttu-id="7330c-187">注意: 响应对象中的 Internet 邮件头数已降低为简洁起见。</span><span class="sxs-lookup"><span data-stu-id="7330c-187">Note: The number of Internet message headers in the response object has been reduced for brevity.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="7330c-188">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="7330c-188">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7330c-189">C#</span><span class="sxs-lookup"><span data-stu-id="7330c-189">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_message_internet_headers-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7330c-190">Javascript</span><span class="sxs-lookup"><span data-stu-id="7330c-190">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_message_internet_headers-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7330c-191">目标-C</span><span class="sxs-lookup"><span data-stu-id="7330c-191">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_message_internet_headers-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="7330c-192">另请参阅</span><span class="sxs-lookup"><span data-stu-id="7330c-192">See also</span></span>

- [<span data-ttu-id="7330c-193">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="7330c-193">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="7330c-194">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="7330c-194">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="7330c-195">使用架构扩展向组添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="7330c-195">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/message-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/message-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/message-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/message-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/message-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/message-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/message-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/message-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: get_message_internet_headers/internetMessageHeaders/member/value:\r\n       Expected type String but actual was Binary. Property: value, actual value: 'binary'"
  ]
}
-->
