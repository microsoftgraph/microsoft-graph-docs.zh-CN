---
title: 获取邮件
description: 检索 message 对象的属性和关系。
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a727179016a5352a55d0923dfcd5ac5834f73d84
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050155"
---
# <a name="get-message"></a><span data-ttu-id="77c80-103">获取邮件</span><span class="sxs-lookup"><span data-stu-id="77c80-103">Get message</span></span>

<span data-ttu-id="77c80-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77c80-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77c80-105">检索 message 对象的属性 [和](../resources/message.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="77c80-105">Retrieve the properties and relationships of the [message](../resources/message.md) object.</span></span>

<span data-ttu-id="77c80-106">例如，您可以获取一条消息，并展开 [邮件中提及](../resources/mention.md) 的所有实例。</span><span class="sxs-lookup"><span data-stu-id="77c80-106">For instance, you can get a message and expand all the [mention](../resources/mention.md) instances in the message.</span></span> <span data-ttu-id="77c80-107">请参阅以下[示例](#example-2-get-all-mentions-in-a-specific-message)。</span><span class="sxs-lookup"><span data-stu-id="77c80-107">See an [example](#example-2-get-all-mentions-in-a-specific-message) below.</span></span>

<span data-ttu-id="77c80-108">可使用 `$value` 参数来[获取邮件的 MIME 内容](/graph/outlook-get-mime-message)。</span><span class="sxs-lookup"><span data-stu-id="77c80-108">You can use the `$value` parameter to [get the MIME content of a message](/graph/outlook-get-mime-message).</span></span> <span data-ttu-id="77c80-109">另请参阅下面的 [示例](#example-5-get-mime-content)。</span><span class="sxs-lookup"><span data-stu-id="77c80-109">See also an [example](#example-5-get-mime-content) below.</span></span>

<span data-ttu-id="77c80-110">在以下两种情况下，应用可以获取其他用户的邮件文件夹中的邮件：</span><span class="sxs-lookup"><span data-stu-id="77c80-110">There are two scenarios where an app can get a message in another user's mail folder:</span></span>

* <span data-ttu-id="77c80-111">如果该应用具有应用程序权限，或者</span><span class="sxs-lookup"><span data-stu-id="77c80-111">If the app has application permissions, or,</span></span>
* <span data-ttu-id="77c80-112">如果应用具有来自某个用户的相应委派[权限](#permissions)，而另一个用户与该用户共享了邮件文件夹，或者已为该用户授予委派的访问权限。</span><span class="sxs-lookup"><span data-stu-id="77c80-112">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="77c80-113">请参阅[详细信息和示例](/graph/outlook-share-messages-folders)。</span><span class="sxs-lookup"><span data-stu-id="77c80-113">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

<span data-ttu-id="77c80-114">由于 **邮件** 资源支持 [扩展](/graph/extensibility-overview)，因此也可使用 `GET` 操作获取 **邮件** 实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="77c80-114">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>


## <a name="permissions"></a><span data-ttu-id="77c80-115">权限</span><span class="sxs-lookup"><span data-stu-id="77c80-115">Permissions</span></span>
<span data-ttu-id="77c80-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="77c80-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77c80-118">权限类型</span><span class="sxs-lookup"><span data-stu-id="77c80-118">Permission type</span></span>      | <span data-ttu-id="77c80-119">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="77c80-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77c80-120">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="77c80-120">Delegated (work or school account)</span></span> | <span data-ttu-id="77c80-121">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="77c80-121">Mail.ReadBasic, Mail.Read</span></span>    |
|<span data-ttu-id="77c80-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="77c80-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77c80-123">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="77c80-123">Mail.ReadBasic, Mail.Read</span></span>    |
|<span data-ttu-id="77c80-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="77c80-124">Application</span></span> | <span data-ttu-id="77c80-125">Mail.ReadBasic.All、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="77c80-125">Mail.ReadBasic.All, Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="77c80-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="77c80-126">HTTP request</span></span>

<span data-ttu-id="77c80-127">要获取指定的邮件：</span><span class="sxs-lookup"><span data-stu-id="77c80-127">To get the specified message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="77c80-128">要获取指定邮件的 MIME 内容：</span><span class="sxs-lookup"><span data-stu-id="77c80-128">To get the MIME content of the specified message:</span></span>
<!-- { "blockType": "ignored" } --> 
```http 
GET /me/messages/{id}/$value 
GET /users/{id | userPrincipalName}/messages/{id}/$value 
GET /me/mailFolders/{id}/messages/{id}/$value 
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/$value 
```

<span data-ttu-id="77c80-129">若要获取邮件并展开邮件中提及的所有内容，</span><span class="sxs-lookup"><span data-stu-id="77c80-129">To get a message and expand all mentions in the message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=mentions
GET /users/{id | userPrincipalName}/messages/{id}?$expand=mentions
GET /me/mailFolders/{id}/messages/{id}?$expand=mentions
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}?$expand=mentions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="77c80-130">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="77c80-130">Optional query parameters</span></span>
<span data-ttu-id="77c80-131">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="77c80-131">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="77c80-132">使用 `$value` 参数获取邮件的 MIME 内容。</span><span class="sxs-lookup"><span data-stu-id="77c80-132">Use the `$value` parameter to get the MIME content of a message.</span></span>

<span data-ttu-id="77c80-133">使用 mentions 导航属性上的 query 参数可获取一封邮件，其中展开邮件中 `$expand` [每个提及](../resources/mention.md)的详细信息。 </span><span class="sxs-lookup"><span data-stu-id="77c80-133">Use the `$expand` query parameter on the **mentions** navigation property to get a message with the details of each [mention](../resources/mention.md) in the message expanded.</span></span>



## <a name="request-headers"></a><span data-ttu-id="77c80-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="77c80-134">Request headers</span></span>
| <span data-ttu-id="77c80-135">名称</span><span class="sxs-lookup"><span data-stu-id="77c80-135">Name</span></span>       | <span data-ttu-id="77c80-136">类型</span><span class="sxs-lookup"><span data-stu-id="77c80-136">Type</span></span> | <span data-ttu-id="77c80-137">说明</span><span class="sxs-lookup"><span data-stu-id="77c80-137">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="77c80-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="77c80-138">Authorization</span></span>  | <span data-ttu-id="77c80-139">string</span><span class="sxs-lookup"><span data-stu-id="77c80-139">string</span></span>  | <span data-ttu-id="77c80-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="77c80-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="77c80-142">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="77c80-142">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="77c80-143">string</span><span class="sxs-lookup"><span data-stu-id="77c80-143">string</span></span> | <span data-ttu-id="77c80-144">要返回的 **body** 和 **uniqueBody** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="77c80-144">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="77c80-145">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="77c80-145">Values can be "text" or "html".</span></span> <span data-ttu-id="77c80-146">如果指定此 `Preference-Applied` 头，返回 `Prefer` 头作为证明。</span><span class="sxs-lookup"><span data-stu-id="77c80-146">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="77c80-147">如果未指定此头，采用 HTML 格式返回 **body** 和 **uniqueBody** 属性。</span><span class="sxs-lookup"><span data-stu-id="77c80-147">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="77c80-148">可选。</span><span class="sxs-lookup"><span data-stu-id="77c80-148">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="77c80-149">请求正文</span><span class="sxs-lookup"><span data-stu-id="77c80-149">Request body</span></span>
<span data-ttu-id="77c80-150">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="77c80-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77c80-151">响应</span><span class="sxs-lookup"><span data-stu-id="77c80-151">Response</span></span>

<span data-ttu-id="77c80-152">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="77c80-152">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>

<span data-ttu-id="77c80-153">如果指定 `$value` 参数，则返回 MIME 格式的邮件内容，而不是 **邮件** 资源。</span><span class="sxs-lookup"><span data-stu-id="77c80-153">Specifying the `$value` parameter returns the message content in MIME format, and not a **message** resource.</span></span>

## <a name="examples"></a><span data-ttu-id="77c80-154">示例</span><span class="sxs-lookup"><span data-stu-id="77c80-154">Examples</span></span>
### <a name="example-1-get-a-specific-message"></a><span data-ttu-id="77c80-155">示例1：获取特定邮件</span><span class="sxs-lookup"><span data-stu-id="77c80-155">Example 1: Get a specific message</span></span>
#### <a name="request"></a><span data-ttu-id="77c80-156">请求</span><span class="sxs-lookup"><span data-stu-id="77c80-156">Request</span></span>
<span data-ttu-id="77c80-157">第一个示例获取指定的邮件。</span><span class="sxs-lookup"><span data-stu-id="77c80-157">The first example gets the specified message.</span></span> <span data-ttu-id="77c80-158">它不指定任何标头来指示要返回的正文的所需格式。</span><span class="sxs-lookup"><span data-stu-id="77c80-158">It does not specify any header to indicate the desired format of the body to be returned.</span></span>

# <a name="http"></a>[<span data-ttu-id="77c80-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="77c80-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AAMkAGI1AAAoZCfHAAA=
```
# <a name="c"></a>[<span data-ttu-id="77c80-160">C#</span><span class="sxs-lookup"><span data-stu-id="77c80-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="77c80-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77c80-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="77c80-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="77c80-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="77c80-163">Java</span><span class="sxs-lookup"><span data-stu-id="77c80-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="77c80-164">响应</span><span class="sxs-lookup"><span data-stu-id="77c80-164">Response</span></span>
<span data-ttu-id="77c80-165">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="77c80-165">Here is an example of the response.</span></span> <span data-ttu-id="77c80-166">body **和** **uniqueBody** 属性以默认 HTML 格式返回。</span><span class="sxs-lookup"><span data-stu-id="77c80-166">The **body** and **uniqueBody** properties are returned in the default HTML format.</span></span>
<span data-ttu-id="77c80-167">注意：为简洁起见，将截断此处所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="77c80-167">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="77c80-168">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="77c80-168">All of the properties will be returned from an actual call.</span></span>
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


### <a name="example-2-get-all-mentions-in-a-specific-message"></a><span data-ttu-id="77c80-169">示例 2：获取特定邮件的所有提及</span><span class="sxs-lookup"><span data-stu-id="77c80-169">Example 2: Get all mentions in a specific message</span></span>
#### <a name="request"></a><span data-ttu-id="77c80-170">请求</span><span class="sxs-lookup"><span data-stu-id="77c80-170">Request</span></span>
<span data-ttu-id="77c80-171">下一个示例中，登录用户是 Dana Swope。</span><span class="sxs-lookup"><span data-stu-id="77c80-171">In the next example, the signed-in user is Dana Swope.</span></span> <span data-ttu-id="77c80-172">该示例显示获取 Dana 邮箱中指定邮件中所有提及的详细信息。</span><span class="sxs-lookup"><span data-stu-id="77c80-172">The example shows getting the details of all the mentions in the specified message in Dana's mailbox.</span></span>

# <a name="http"></a>[<span data-ttu-id="77c80-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="77c80-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AQMkADJmMTUAAAgVZAAAA"],
  "name": "get_mentions_in_message"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AQMkADJmMTUAAAgVZAAAA/?$expand=mentions
```
# <a name="c"></a>[<span data-ttu-id="77c80-174">C#</span><span class="sxs-lookup"><span data-stu-id="77c80-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mentions-in-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="77c80-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77c80-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mentions-in-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="77c80-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="77c80-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mentions-in-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="77c80-177">Java</span><span class="sxs-lookup"><span data-stu-id="77c80-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mentions-in-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="77c80-178">响应</span><span class="sxs-lookup"><span data-stu-id="77c80-178">Response</span></span>
<span data-ttu-id="77c80-179">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="77c80-179">Here is an example of the response.</span></span> <span data-ttu-id="77c80-180">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="77c80-180">Note: The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-3-get-message-body-in-text-format"></a><span data-ttu-id="77c80-181">示例 3：以文本格式获取邮件正文</span><span class="sxs-lookup"><span data-stu-id="77c80-181">Example 3: Get message body in text format</span></span>
#### <a name="request"></a><span data-ttu-id="77c80-182">请求</span><span class="sxs-lookup"><span data-stu-id="77c80-182">Request</span></span>

<span data-ttu-id="77c80-183">第三个示例介绍如何使用 `Prefer: outlook.body-content-type="text"` 标头获取采用文本格式的指定消息的 **body** 和 **uniqueBody**。</span><span class="sxs-lookup"><span data-stu-id="77c80-183">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** of the specified message in text format.</span></span>


# <a name="http"></a>[<span data-ttu-id="77c80-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="77c80-184">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message_in_text"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AAMkAGI1AAAoZCfHAAA=/?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```
# <a name="c"></a>[<span data-ttu-id="77c80-185">C#</span><span class="sxs-lookup"><span data-stu-id="77c80-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="77c80-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77c80-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="77c80-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="77c80-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="77c80-188">Java</span><span class="sxs-lookup"><span data-stu-id="77c80-188">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-in-text-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="77c80-189">响应</span><span class="sxs-lookup"><span data-stu-id="77c80-189">Response</span></span>

<span data-ttu-id="77c80-190">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="77c80-190">Here is an example of the response.</span></span> <span data-ttu-id="77c80-191">注意：响应包含用于确认 `Prefer: outlook.body-content-type` 请求标头的 `Preference-Applied: outlook.body-content-type` 标头。</span><span class="sxs-lookup"><span data-stu-id="77c80-191">Note: The response includes a `Preference-Applied: outlook.body-content-type` header to acknowledge the `Prefer: outlook.body-content-type` request header.</span></span>
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
### <a name="example-4-get-internet-message-headers"></a><span data-ttu-id="77c80-192">示例 4：获取 Internet 邮件头</span><span class="sxs-lookup"><span data-stu-id="77c80-192">Example 4: Get Internet message headers</span></span>
#### <a name="request"></a><span data-ttu-id="77c80-193">请求</span><span class="sxs-lookup"><span data-stu-id="77c80-193">Request</span></span>

<span data-ttu-id="77c80-194">第四个示例演示如何获取特定邮件的 Internet 邮件头。</span><span class="sxs-lookup"><span data-stu-id="77c80-194">The fourth example shows how to get the Internet message headers of a specific message.</span></span>  


# <a name="http"></a>[<span data-ttu-id="77c80-195">HTTP</span><span class="sxs-lookup"><span data-stu-id="77c80-195">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEz"],
  "name": "get_message_internet_headers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AAMkAGVmMDEz/?$select=internetMessageHeaders
```
# <a name="c"></a>[<span data-ttu-id="77c80-196">C#</span><span class="sxs-lookup"><span data-stu-id="77c80-196">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-internet-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="77c80-197">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77c80-197">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-internet-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="77c80-198">Objective-C</span><span class="sxs-lookup"><span data-stu-id="77c80-198">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-internet-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="77c80-199">Java</span><span class="sxs-lookup"><span data-stu-id="77c80-199">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-internet-headers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="77c80-200">响应</span><span class="sxs-lookup"><span data-stu-id="77c80-200">Response</span></span>

<span data-ttu-id="77c80-201">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="77c80-201">Here is an example of the response.</span></span> <span data-ttu-id="77c80-202">注意：为简洁起见，响应对象中的 Internet 邮件头数量已减少。</span><span class="sxs-lookup"><span data-stu-id="77c80-202">Note: The number of Internet message headers in the response object has been reduced for brevity.</span></span>

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


### <a name="example-5-get-mime-content"></a><span data-ttu-id="77c80-203">示例 5：获取 MIME 内容</span><span class="sxs-lookup"><span data-stu-id="77c80-203">Example 5: Get MIME content</span></span>
#### <a name="request"></a><span data-ttu-id="77c80-204">请求</span><span class="sxs-lookup"><span data-stu-id="77c80-204">Request</span></span>
<span data-ttu-id="77c80-205">第五个示例获取已登录用户邮箱中邮件的 MIME 内容。</span><span class="sxs-lookup"><span data-stu-id="77c80-205">The fifth example gets the MIME content of a message in the signed-in user's mailbox.</span></span>


# <a name="http"></a>[<span data-ttu-id="77c80-206">HTTP</span><span class="sxs-lookup"><span data-stu-id="77c80-206">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_message_in_mime",
  "sampleKeys": ["4aade2547798441eab5188a7a2436bc1"]
} -->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/4aade2547798441eab5188a7a2436bc1/$value
```
# <a name="c"></a>[<span data-ttu-id="77c80-207">C#</span><span class="sxs-lookup"><span data-stu-id="77c80-207">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-in-mime-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="77c80-208">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77c80-208">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-in-mime-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="77c80-209">Objective-C</span><span class="sxs-lookup"><span data-stu-id="77c80-209">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-in-mime-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="77c80-210">Java</span><span class="sxs-lookup"><span data-stu-id="77c80-210">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-in-mime-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="77c80-211">响应</span><span class="sxs-lookup"><span data-stu-id="77c80-211">Response</span></span>
<span data-ttu-id="77c80-212">以下是答复。</span><span class="sxs-lookup"><span data-stu-id="77c80-212">The following is the response.</span></span> <span data-ttu-id="77c80-213">MIME 内容以 `MIME-Version` 标头开头。</span><span class="sxs-lookup"><span data-stu-id="77c80-213">The MIME content begins with the `MIME-Version` header.</span></span> 
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


## <a name="see-also"></a><span data-ttu-id="77c80-214">另请参阅</span><span class="sxs-lookup"><span data-stu-id="77c80-214">See also</span></span>

- [<span data-ttu-id="77c80-215">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="77c80-215">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="77c80-216">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="77c80-216">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="77c80-217">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="77c80-217">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

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


