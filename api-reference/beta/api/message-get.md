---
title: 获取邮件
description: 检索 message 对象的属性和关系。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9d0676f1d9558e92fe5d033c44a48bcfad140b0f
ms.sourcegitcommit: 844c6d552a8a60fcda5ef65148570a32fd1004bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/17/2020
ms.locfileid: "41216768"
---
# <a name="get-message"></a><span data-ttu-id="97a5a-103">获取邮件</span><span class="sxs-lookup"><span data-stu-id="97a5a-103">Get message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97a5a-104">检索[message](../resources/message.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="97a5a-104">Retrieve the properties and relationships of the [message](../resources/message.md) object.</span></span>

<span data-ttu-id="97a5a-105">例如，您可以收到一条消息，并在邮件中展开所有[提及](../resources/mention.md)的实例。</span><span class="sxs-lookup"><span data-stu-id="97a5a-105">For example, you can get a message and expand all the [mention](../resources/mention.md) instances in the message.</span></span>

<span data-ttu-id="97a5a-106">可使用 `$value` 参数来[获取邮件的 MIME 内容](/graph/outlook-get-mime-message)。</span><span class="sxs-lookup"><span data-stu-id="97a5a-106">You can use the `$value` parameter to [get the MIME content of a message](/graph/outlook-get-mime-message).</span></span>

<span data-ttu-id="97a5a-107">在以下两种情况下，应用可以获取其他用户的邮件文件夹中的邮件：</span><span class="sxs-lookup"><span data-stu-id="97a5a-107">There are two scenarios where an app can get a message in another user's mail folder:</span></span>

* <span data-ttu-id="97a5a-108">如果该应用具有应用程序权限，或者</span><span class="sxs-lookup"><span data-stu-id="97a5a-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="97a5a-109">如果应用具有来自某个用户的相应委派[权限](#permissions)，而另一个用户与该用户共享了邮件文件夹，或者已为该用户授予委派的访问权限。</span><span class="sxs-lookup"><span data-stu-id="97a5a-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="97a5a-110">请参阅[详细信息和示例](/graph/outlook-share-messages-folders)。</span><span class="sxs-lookup"><span data-stu-id="97a5a-110">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

<span data-ttu-id="97a5a-111">由于**邮件**资源支持[扩展](/graph/extensibility-overview)，因此也可使用 `GET` 操作获取**邮件**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="97a5a-111">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>


## <a name="permissions"></a><span data-ttu-id="97a5a-112">权限</span><span class="sxs-lookup"><span data-stu-id="97a5a-112">Permissions</span></span>
<span data-ttu-id="97a5a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="97a5a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97a5a-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="97a5a-115">Permission type</span></span>      | <span data-ttu-id="97a5a-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="97a5a-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97a5a-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="97a5a-117">Delegated (work or school account)</span></span> | <span data-ttu-id="97a5a-118">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="97a5a-118">Mail.ReadBasic, Mail.Read</span></span>    |
|<span data-ttu-id="97a5a-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="97a5a-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97a5a-120">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="97a5a-120">Mail.ReadBasic, Mail.Read</span></span>    |
|<span data-ttu-id="97a5a-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="97a5a-121">Application</span></span> | <span data-ttu-id="97a5a-122">Mail.ReadBasic.All、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="97a5a-122">Mail.ReadBasic.All, Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="97a5a-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="97a5a-123">HTTP request</span></span>

<span data-ttu-id="97a5a-124">要获取指定的邮件：</span><span class="sxs-lookup"><span data-stu-id="97a5a-124">To get the specified message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="97a5a-125">要获取指定邮件的 MIME 内容：</span><span class="sxs-lookup"><span data-stu-id="97a5a-125">To get the MIME content of the specified message:</span></span>
<!-- { "blockType": "ignored" } --> 
```http 
GET /me/messages/{id}/$value 
GET /users/{id | userPrincipalName}/messages/{id}/$value 
GET /me/mailFolders/{id}/messages/{id}/$value 
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/$value 
```

<span data-ttu-id="97a5a-126">若要获取邮件并展开邮件中的所有提及内容，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="97a5a-126">To get a message and expand all mentions in the message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=mentions
GET /users/{id | userPrincipalName}/messages/{id}?$expand=mentions
GET /me/mailFolders/{id}/messages/{id}?$expand=mentions
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}?$expand=mentions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="97a5a-127">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="97a5a-127">Optional query parameters</span></span>
<span data-ttu-id="97a5a-128">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="97a5a-128">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="97a5a-129">使用 `$value` 参数获取邮件的 MIME 内容。</span><span class="sxs-lookup"><span data-stu-id="97a5a-129">Use the `$value` parameter to get the MIME content of a message.</span></span>

<span data-ttu-id="97a5a-130">使用 " `$expand` **提及**" 导航属性上的查询参数，可以获取消息，其中包含已展开邮件中每个[提及](../resources/mention.md)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="97a5a-130">Use the `$expand` query parameter on the **mentions** navigation property to get a message with the details of each [mention](../resources/mention.md) in the message expanded.</span></span>



## <a name="request-headers"></a><span data-ttu-id="97a5a-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="97a5a-131">Request headers</span></span>
| <span data-ttu-id="97a5a-132">名称</span><span class="sxs-lookup"><span data-stu-id="97a5a-132">Name</span></span>       | <span data-ttu-id="97a5a-133">类型</span><span class="sxs-lookup"><span data-stu-id="97a5a-133">Type</span></span> | <span data-ttu-id="97a5a-134">说明</span><span class="sxs-lookup"><span data-stu-id="97a5a-134">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="97a5a-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="97a5a-135">Authorization</span></span>  | <span data-ttu-id="97a5a-136">string</span><span class="sxs-lookup"><span data-stu-id="97a5a-136">string</span></span>  | <span data-ttu-id="97a5a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="97a5a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="97a5a-139">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="97a5a-139">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="97a5a-140">string</span><span class="sxs-lookup"><span data-stu-id="97a5a-140">string</span></span> | <span data-ttu-id="97a5a-141">要返回的 **body** 和 **uniqueBody** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="97a5a-141">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="97a5a-142">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="97a5a-142">Values can be "text" or "html".</span></span> <span data-ttu-id="97a5a-143">如果指定此 `Preference-Applied` 头，返回 `Prefer` 头作为证明。</span><span class="sxs-lookup"><span data-stu-id="97a5a-143">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="97a5a-144">如果未指定此头，采用 HTML 格式返回 **body** 和 **uniqueBody** 属性。</span><span class="sxs-lookup"><span data-stu-id="97a5a-144">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="97a5a-145">可选。</span><span class="sxs-lookup"><span data-stu-id="97a5a-145">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="97a5a-146">请求正文</span><span class="sxs-lookup"><span data-stu-id="97a5a-146">Request body</span></span>
<span data-ttu-id="97a5a-147">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="97a5a-147">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97a5a-148">响应</span><span class="sxs-lookup"><span data-stu-id="97a5a-148">Response</span></span>

<span data-ttu-id="97a5a-149">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="97a5a-149">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>

<span data-ttu-id="97a5a-150">如果指定 `$value` 参数，则返回 MIME 格式的邮件内容，而不是**邮件**资源。</span><span class="sxs-lookup"><span data-stu-id="97a5a-150">Specifying the `$value` parameter returns the message content in MIME format, and not a **message** resource.</span></span>

## <a name="examples"></a><span data-ttu-id="97a5a-151">示例</span><span class="sxs-lookup"><span data-stu-id="97a5a-151">Examples</span></span>
### <a name="example-1"></a><span data-ttu-id="97a5a-152">示例 1</span><span class="sxs-lookup"><span data-stu-id="97a5a-152">Example 1</span></span>
#### <a name="request"></a><span data-ttu-id="97a5a-153">请求</span><span class="sxs-lookup"><span data-stu-id="97a5a-153">Request</span></span>
<span data-ttu-id="97a5a-154">第一个示例获取指定的邮件。</span><span class="sxs-lookup"><span data-stu-id="97a5a-154">The first example gets the specified message.</span></span> <span data-ttu-id="97a5a-155">它不指定任何标头以指示要返回的正文的所需格式。</span><span class="sxs-lookup"><span data-stu-id="97a5a-155">It does not specify any header to indicate the desired format of the body to be returned.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="97a5a-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="97a5a-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AAMkAGI1AAAoZCfHAAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="97a5a-157">C#</span><span class="sxs-lookup"><span data-stu-id="97a5a-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="97a5a-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="97a5a-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="97a5a-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="97a5a-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="97a5a-160">响应</span><span class="sxs-lookup"><span data-stu-id="97a5a-160">Response</span></span>
<span data-ttu-id="97a5a-161">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="97a5a-161">Here is an example of the response.</span></span> <span data-ttu-id="97a5a-162">**Body**和**uniqueBody**属性以默认的 HTML 格式返回。</span><span class="sxs-lookup"><span data-stu-id="97a5a-162">The **body** and **uniqueBody** properties are returned in the default HTML format.</span></span>
<span data-ttu-id="97a5a-163">注意：为简洁起见，此处显示的响应对象将被截断。</span><span class="sxs-lookup"><span data-stu-id="97a5a-163">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="97a5a-164">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="97a5a-164">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_message",
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


### <a name="example-2"></a><span data-ttu-id="97a5a-165">示例 2</span><span class="sxs-lookup"><span data-stu-id="97a5a-165">Example 2</span></span>
#### <a name="request"></a><span data-ttu-id="97a5a-166">请求</span><span class="sxs-lookup"><span data-stu-id="97a5a-166">Request</span></span>
<span data-ttu-id="97a5a-167">在下一个示例中，登录用户是 Dana Swope。</span><span class="sxs-lookup"><span data-stu-id="97a5a-167">In the next example, the signed-in user is Dana Swope.</span></span> <span data-ttu-id="97a5a-168">此示例显示了如何获取 Dana 的邮箱中指定邮件中所有提及内容的详细信息。</span><span class="sxs-lookup"><span data-stu-id="97a5a-168">The example shows getting the details of all the mentions in the specified message in Dana's mailbox.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="97a5a-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="97a5a-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AQMkADJmMTUAAAgVZAAAA"],
  "name": "get_mentions_in_message"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AQMkADJmMTUAAAgVZAAAA/?$expand=mentions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="97a5a-170">C#</span><span class="sxs-lookup"><span data-stu-id="97a5a-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mentions-in-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="97a5a-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="97a5a-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mentions-in-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="97a5a-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="97a5a-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mentions-in-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="97a5a-173">响应</span><span class="sxs-lookup"><span data-stu-id="97a5a-173">Response</span></span>
<span data-ttu-id="97a5a-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="97a5a-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_mentions_in_message",
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

### <a name="example-3"></a><span data-ttu-id="97a5a-177">示例 3</span><span class="sxs-lookup"><span data-stu-id="97a5a-177">Example 3</span></span>
#### <a name="request"></a><span data-ttu-id="97a5a-178">请求</span><span class="sxs-lookup"><span data-stu-id="97a5a-178">Request</span></span>

<span data-ttu-id="97a5a-179">第三个示例介绍如何使用 `Prefer: outlook.body-content-type="text"` 标头获取采用文本格式的指定消息的 **body** 和 **uniqueBody**。</span><span class="sxs-lookup"><span data-stu-id="97a5a-179">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** of the specified message in text format.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="97a5a-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="97a5a-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message_in_text"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AAMkAGI1AAAoZCfHAAA=/?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="97a5a-181">C#</span><span class="sxs-lookup"><span data-stu-id="97a5a-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="97a5a-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="97a5a-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="97a5a-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="97a5a-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="97a5a-184">响应</span><span class="sxs-lookup"><span data-stu-id="97a5a-184">Response</span></span>

<span data-ttu-id="97a5a-185">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="97a5a-185">Here is an example of the response.</span></span> <span data-ttu-id="97a5a-186">注意：响应包含用于确认 `Prefer: outlook.body-content-type` 请求标头的 `Preference-Applied: outlook.body-content-type` 标头。</span><span class="sxs-lookup"><span data-stu-id="97a5a-186">Note: The response includes a `Preference-Applied: outlook.body-content-type` header to acknowledge the `Prefer: outlook.body-content-type` request header.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_message_in_text",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.body-content-type="text"

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
### <a name="example-4"></a><span data-ttu-id="97a5a-187">示例 4</span><span class="sxs-lookup"><span data-stu-id="97a5a-187">Example 4</span></span>
#### <a name="request"></a><span data-ttu-id="97a5a-188">请求</span><span class="sxs-lookup"><span data-stu-id="97a5a-188">Request</span></span>

<span data-ttu-id="97a5a-189">第四个示例演示如何获取特定邮件的 Internet 邮件头。</span><span class="sxs-lookup"><span data-stu-id="97a5a-189">The fourth example shows how to get the Internet message headers of a specific message.</span></span>  


# <a name="httptabhttp"></a>[<span data-ttu-id="97a5a-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="97a5a-190">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEz"],
  "name": "get_message_internet_headers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AAMkAGVmMDEz/?$select=internetMessageHeaders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="97a5a-191">C#</span><span class="sxs-lookup"><span data-stu-id="97a5a-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-internet-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="97a5a-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="97a5a-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-internet-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="97a5a-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="97a5a-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-internet-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="97a5a-194">响应</span><span class="sxs-lookup"><span data-stu-id="97a5a-194">Response</span></span>

<span data-ttu-id="97a5a-195">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="97a5a-195">Here is an example of the response.</span></span> <span data-ttu-id="97a5a-196">注意：响应对象中的 Internet 邮件头数已降低为简洁起见。</span><span class="sxs-lookup"><span data-stu-id="97a5a-196">Note: The number of Internet message headers in the response object has been reduced for brevity.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_message_internet_headers",
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


### <a name="example-5"></a><span data-ttu-id="97a5a-197">示例 5</span><span class="sxs-lookup"><span data-stu-id="97a5a-197">Example 5</span></span>
#### <a name="request"></a><span data-ttu-id="97a5a-198">请求</span><span class="sxs-lookup"><span data-stu-id="97a5a-198">Request</span></span>
<span data-ttu-id="97a5a-199">第五个示例获取已登录用户的邮箱中的邮件的 MIME 内容。</span><span class="sxs-lookup"><span data-stu-id="97a5a-199">The fifth example gets the MIME content of a message in the signed-in user's mailbox.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_message_in_mime",
  "sampleKeys": ["4aade2547798441eab5188a7a2436bc1"]
} -->
```http
GET https://graph.microsoft.com/beta/me/messages/4aade2547798441eab5188a7a2436bc1/$value
```

#### <a name="response"></a><span data-ttu-id="97a5a-200">响应</span><span class="sxs-lookup"><span data-stu-id="97a5a-200">Response</span></span>
<span data-ttu-id="97a5a-201">以下是答复。</span><span class="sxs-lookup"><span data-stu-id="97a5a-201">The following is the response.</span></span> <span data-ttu-id="97a5a-202">MIME 内容以 `MIME-Version` 标头开头。</span><span class="sxs-lookup"><span data-stu-id="97a5a-202">The MIME content begins with the `MIME-Version` header.</span></span> 
<!-- {
  "blockType": "response",
  "name": "get_message_in_mime",
  "truncated": true,
  "@odata.type": "string"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

Received: from contoso.com (10.194.241.197) by 
contoso.com (10.194.241.197) with Microsoft 
SMTP Server (version=TLS1_2, 
cipher=TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384_P256) id 15.1.1374.0 via Mailbox 
Transport; Mon, 4 Sep 2017 03:00:08 -0700 
Received: from contoso.com (10.194.241.197) by 
contoso.com (10.194.241.197) with Microsoft 
SMTP Server (version=TLS1_2, 
cipher=TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384_P256) id 15.1.1374.0; Mon, 4 Sep 
2017 03:00:07 -0700 
Received: from contoso.com 
(fe80::5bf:5059:4ca0:5017) by contoso.com 
(fe80::5bf:5059:4ca0:5017%12) with mapi id 15.01.1374.000; Mon, 4 Sep 2017 
03:00:01 -0700 
From: Administrator <admin@contoso.com> 
To: Administrator <admin@contoso.com> 
Subject: This email has attachment. 
Thread-Topic: This email has attachment. 
Thread-Index: AQHTJWSHSywMzSz8o0OJud48nG50GQ== 
Date: Mon, 4 Sep 2017 10:00:00 +0000 
Message-ID: 
                <4aade2547798441eab5188a7a2436bc1@contoso.com> 
Accept-Language: en-US 
Content-Language: en-US 
X-MS-Exchange-Organization-AuthAs: Internal 
X-MS-Exchange-Organization-AuthMechanism: 04 
X-MS-Exchange-Organization-AuthSource: 
                contoso.com 
X-MS-Has-Attach: yes 
X-MS-Exchange-Organization-Network-Message-Id: 
                0ffdb402-ec03-42c8-5d32-08d4f37bb517 
X-MS-Exchange-Organization-SCL: -1 
X-MS-TNEF-Correlator: 
X-MS-Exchange-Organization-RecordReviewCfmType: 0 

MIME-Version: 1.0 
Content-Type: multipart/mixed; 
                boundary="_004_4aade2547798441eab5188a7a2436bc1contoso_" 
 
--_004_4aade2547798441eab5188a7a2436bc1contoso_ 
Content-Type: multipart/alternative; 
                boundary="_000_4aade2547798441eab5188a7a2436bc1contoso_" 
 
--_000_4aade2547798441eab5188a7a2436bc1contoso_ 
Content-Type: text/plain; charset="iso-8859-1" 
Content-Transfer-Encoding: quoted-printable 
 
The attachment is an email. 
 
--_000_4aade2547798441eab5188a7a2436bc1contoso_ 
Content-Type: text/html; charset="iso-8859-1" 
Content-Transfer-Encoding: quoted-printable 
 
<html> 
<head> 
<meta http-equiv=3D"Content-Type" content=3D"text/html; charset=3Diso-8859-= 
1"> 
<style type=3D"text/css" style=3D"display:none;"><!-- P {margin-top:0;margi= 
n-bottom:0;} --></style> 
</head> 
<body dir=3D"ltr"> 
<div id=3D"divtagdefaultwrapper" style=3D"font-size:12pt;color:#000000;font= 
-family:Calibri,Helvetica,sans-serif;" dir=3D"ltr"> 
<p>The attachment is an email.</p> 
</div> 
</body> 
</html> 
 
--_000_4aade2547798441eab5188a7a2436bc1contoso_-- 
 
--_004_4aade2547798441eab5188a7a2436bc1contoso_ 
Content-Type: application/octet-stream; name="Attachment email.eml" 
Content-Description: Attachment email.eml 
Content-Disposition: attachment; filename="Attachment email.eml"; size=408; 
                creation-date="Mon, 04 Sep 2017 09:59:43 GMT"; 
                modification-date="Mon, 04 Sep 2017 09:59:43 GMT" 
Content-Transfer-Encoding: base64 
 
RnJvbToJQWRtaW5pc3RyYXRvciA8YWRtaW5AdGVuYW50LUVYSEItMTQ3MS5jb20+DQpTZW50OglN 
b25kYXksIFNlcHRlbWJlciA0LCAyMDE3IDM6MjYgUE0NClRvOglTcml2YXJkaGFuIEhlYmJhcg0K 
U3ViamVjdDoJQXR0YWNobWVudCBlbWFpbA0KDQpJIHdpbGwgYXR0YWNoIHRoaXMgZW1haWwgdG8g 
YW5vdGhlciBtYWlsLg0K 
 
--_004_4aade2547798441eab5188a7a2436bc1contoso_-- 
```


## <a name="see-also"></a><span data-ttu-id="97a5a-203">另请参阅</span><span class="sxs-lookup"><span data-stu-id="97a5a-203">See also</span></span>

- [<span data-ttu-id="97a5a-204">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="97a5a-204">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="97a5a-205">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="97a5a-205">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="97a5a-206">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="97a5a-206">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

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
    "Error: get_message_internet_headers/internetMessageHeaders/member/value:\r\n       Expected type String but actual was Binary. Property: value, actual value: 'binary'"
  ]
}
-->
