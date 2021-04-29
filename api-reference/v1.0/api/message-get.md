---
title: 获取邮件
description: 检索邮件对象的属性和关系。
author: abheek-das
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: faef3fd45e331012b642624361c9fc03e35d9a97
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52035377"
---
# <a name="get-message"></a><span data-ttu-id="70150-103">获取邮件</span><span class="sxs-lookup"><span data-stu-id="70150-103">Get message</span></span>

<span data-ttu-id="70150-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70150-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="70150-105">检索[邮件](../resources/message.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="70150-105">Retrieve the properties and relationships of a [message](../resources/message.md) object.</span></span>

<span data-ttu-id="70150-106">可使用 `$value` 参数来[获取邮件的 MIME 内容](/graph/outlook-get-mime-message)。</span><span class="sxs-lookup"><span data-stu-id="70150-106">You can use the `$value` parameter to [get the MIME content of a message](/graph/outlook-get-mime-message).</span></span> <span data-ttu-id="70150-107">另请参阅下面的 [示例](#example-4-get-mime-content)。</span><span class="sxs-lookup"><span data-stu-id="70150-107">See also an [example](#example-4-get-mime-content) below.</span></span>

<span data-ttu-id="70150-108">在以下两种情况下，应用可以获取其他用户的邮件文件夹中的邮件：</span><span class="sxs-lookup"><span data-stu-id="70150-108">There are two scenarios where an app can get a message in another user's mail folder:</span></span>

* <span data-ttu-id="70150-109">如果该应用具有应用程序权限，或者</span><span class="sxs-lookup"><span data-stu-id="70150-109">If the app has application permissions, or,</span></span>
* <span data-ttu-id="70150-110">如果应用具有来自某个用户的相应委派[权限](#permissions)，而另一个用户与该用户共享了邮件文件夹，或者已为该用户授予委派的访问权限。</span><span class="sxs-lookup"><span data-stu-id="70150-110">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="70150-111">请参阅[详细信息和示例](/graph/outlook-share-messages-folders)。</span><span class="sxs-lookup"><span data-stu-id="70150-111">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

<span data-ttu-id="70150-112">由于 **邮件** 资源支持 [扩展](/graph/extensibility-overview)，因此也可使用 `GET` 操作获取 **邮件** 实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="70150-112">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>


## <a name="permissions"></a><span data-ttu-id="70150-113">权限</span><span class="sxs-lookup"><span data-stu-id="70150-113">Permissions</span></span>
<span data-ttu-id="70150-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="70150-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70150-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="70150-116">Permission type</span></span>      | <span data-ttu-id="70150-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="70150-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70150-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="70150-118">Delegated (work or school account)</span></span> | <span data-ttu-id="70150-119">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="70150-119">Mail.ReadBasic, Mail.Read</span></span>    |
|<span data-ttu-id="70150-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="70150-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70150-121">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="70150-121">Mail.ReadBasic, Mail.Read</span></span>    |
|<span data-ttu-id="70150-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="70150-122">Application</span></span> | <span data-ttu-id="70150-123">Mail.ReadBasic.All、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="70150-123">Mail.ReadBasic.All, Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="70150-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="70150-124">HTTP request</span></span>

<span data-ttu-id="70150-125">要获取指定的邮件：</span><span class="sxs-lookup"><span data-stu-id="70150-125">To get the specified message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="70150-126">要获取指定邮件的 MIME 内容：</span><span class="sxs-lookup"><span data-stu-id="70150-126">To get the MIME content of the specified message:</span></span>
<!-- { "blockType": "ignored" } --> 
```http 
GET /me/messages/{id}/$value 
GET /users/{id | userPrincipalName}/messages/{id}/$value 
GET /me/mailFolders/{id}/messages/{id}/$value 
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/$value 
```

## <a name="optional-query-parameters"></a><span data-ttu-id="70150-127">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="70150-127">Optional query parameters</span></span>
<span data-ttu-id="70150-128">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="70150-128">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="70150-129">使用 `$value` 参数获取邮件的 MIME 内容。</span><span class="sxs-lookup"><span data-stu-id="70150-129">Use the `$value` parameter to get the MIME content of a message.</span></span>
## <a name="request-headers"></a><span data-ttu-id="70150-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="70150-130">Request headers</span></span>
| <span data-ttu-id="70150-131">名称</span><span class="sxs-lookup"><span data-stu-id="70150-131">Name</span></span>       | <span data-ttu-id="70150-132">类型</span><span class="sxs-lookup"><span data-stu-id="70150-132">Type</span></span> | <span data-ttu-id="70150-133">说明</span><span class="sxs-lookup"><span data-stu-id="70150-133">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="70150-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="70150-134">Authorization</span></span>  | <span data-ttu-id="70150-135">string</span><span class="sxs-lookup"><span data-stu-id="70150-135">string</span></span>  | <span data-ttu-id="70150-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="70150-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="70150-138">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="70150-138">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="70150-139">string</span><span class="sxs-lookup"><span data-stu-id="70150-139">string</span></span> | <span data-ttu-id="70150-140">要返回的 **body** 和 **uniqueBody** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="70150-140">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="70150-141">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="70150-141">Values can be "text" or "html".</span></span> <span data-ttu-id="70150-142">如果指定此 `Preference-Applied` 头，返回 `Prefer` 头作为证明。</span><span class="sxs-lookup"><span data-stu-id="70150-142">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="70150-143">如果未指定此头，采用 HTML 格式返回 **body** 和 **uniqueBody** 属性。</span><span class="sxs-lookup"><span data-stu-id="70150-143">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="70150-144">可选。</span><span class="sxs-lookup"><span data-stu-id="70150-144">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="70150-145">请求正文</span><span class="sxs-lookup"><span data-stu-id="70150-145">Request body</span></span>
<span data-ttu-id="70150-146">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="70150-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70150-147">响应</span><span class="sxs-lookup"><span data-stu-id="70150-147">Response</span></span>

<span data-ttu-id="70150-148">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="70150-148">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>

<span data-ttu-id="70150-149">如果指定 `$value` 参数，则返回 MIME 格式的邮件内容，而不是 **邮件** 资源。</span><span class="sxs-lookup"><span data-stu-id="70150-149">Specifying the `$value` parameter returns the message content in MIME format, and not a **message** resource.</span></span>


## <a name="examples"></a><span data-ttu-id="70150-150">示例</span><span class="sxs-lookup"><span data-stu-id="70150-150">Examples</span></span>
### <a name="example-1-get-a-specific-message"></a><span data-ttu-id="70150-151">示例1：获取特定邮件</span><span class="sxs-lookup"><span data-stu-id="70150-151">Example 1: Get a specific message</span></span>
#### <a name="request"></a><span data-ttu-id="70150-152">请求</span><span class="sxs-lookup"><span data-stu-id="70150-152">Request</span></span>
<span data-ttu-id="70150-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="70150-153">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="70150-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="70150-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhMGAAA="],
  "name": "get_message"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhMGAAA=
```
# <a name="c"></a>[<span data-ttu-id="70150-155">C#</span><span class="sxs-lookup"><span data-stu-id="70150-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="70150-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70150-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="70150-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70150-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="70150-158">Java</span><span class="sxs-lookup"><span data-stu-id="70150-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="70150-159">响应</span><span class="sxs-lookup"><span data-stu-id="70150-159">Response</span></span>
<span data-ttu-id="70150-160">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="70150-160">Here is an example of the response.</span></span> <span data-ttu-id="70150-161">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="70150-161">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_message",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('7f180cbb-a5ae-457c-b7e8-6f5b42ba33e7')/messages/$entity",
    "@odata.etag":"W/\"CQAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAnjjuZ\"",
    "id":"AAMkADhMGAAA=",
    "createdDateTime":"2018-09-09T03:15:05Z",
    "lastModifiedDateTime":"2018-09-09T03:15:08Z",
    "changeKey":"CQAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAnjjuZ",
    "categories":[

    ],
    "receivedDateTime":"2018-09-09T03:15:08Z",
    "sentDateTime":"2018-09-09T03:15:06Z",
    "hasAttachments":false,
    "internetMessageId":"<MWHPR6E1BE060@MWHPR1120.namprd22.prod.outlook.com>",
    "subject":"9/9/2018: concert",
    "bodyPreview":"The group represents Nevada.",
    "importance":"normal",
    "parentFolderId":"AAMkADcbAAAAAAEJAAA=",
    "conversationId":"AAQkADOUpag6yWs=",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":true,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADMGAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nThe group represents Nevada.\r\n</body>\r\n</html>\r\n"
    },
    "sender":{
        "emailAddress":{
            "name":"Adele Vance",
            "address":"adelev@contoso.OnMicrosoft.com"
        }
    },
    "from":{
        "emailAddress":{
            "name":"Adele Vance",
            "address":"adelev@contoso.OnMicrosoft.com"
        }
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"Alex Wilber",
                "address":"AlexW@contoso.OnMicrosoft.com"
            }
        }
    ],
    "ccRecipients":[

    ],
    "bccRecipients":[

    ],
    "replyTo":[

    ],
    "flag":{
        "flagStatus":"notFlagged"
    }
}
```

### <a name="example-2-get-internet-message-headers"></a><span data-ttu-id="70150-162">示例 2：获取 Internet 邮件头</span><span class="sxs-lookup"><span data-stu-id="70150-162">Example 2: Get Internet message headers</span></span>
#### <a name="request"></a><span data-ttu-id="70150-163">请求</span><span class="sxs-lookup"><span data-stu-id="70150-163">Request</span></span>
<span data-ttu-id="70150-164">下一个示例使用 `$select` 查询参数获取邮件的 Internet 邮件标头。</span><span class="sxs-lookup"><span data-stu-id="70150-164">The next example uses a `$select` query parameter to get the Internet message headers of a message.</span></span> 

# <a name="http"></a>[<span data-ttu-id="70150-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="70150-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAAW-VPeAAA="],
  "name": "get_message_headers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhAAAW-VPeAAA=/?$select=internetMessageHeaders
```
# <a name="c"></a>[<span data-ttu-id="70150-166">C#</span><span class="sxs-lookup"><span data-stu-id="70150-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="70150-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70150-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="70150-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70150-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="70150-169">Java</span><span class="sxs-lookup"><span data-stu-id="70150-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-headers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="70150-170">响应</span><span class="sxs-lookup"><span data-stu-id="70150-170">Response</span></span>
<span data-ttu-id="70150-p107">下面是一个响应示例。注意：为简洁起见，会将响应对象中的一组邮件头截断。将从实际调用中返回所有头。</span><span class="sxs-lookup"><span data-stu-id="70150-p107">Here is an example of the response. Note: The set of message headers in the response object is truncated for brevity. All of the headers will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_message_headers",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('7f180cbb-a5ae-457c-b7e8-6f5b42ba33e7')/messages(internetMessageHeaders)/$entity",
    "@odata.etag":"W/\"FwAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAW/0tB\"",
    "id":"AAMkADhAAAW-VPeAAA=",
    "internetMessageHeaders":[
        {
            "name":"MIME-Version",
            "value":"1.0"
        },
        {
            "name":"Content-Type",
            "value":"multipart/report"
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

### <a name="example-3-get-message-body-in-text-format"></a><span data-ttu-id="70150-174">示例 3：以文本格式获取邮件正文</span><span class="sxs-lookup"><span data-stu-id="70150-174">Example 3: Get message body in text format</span></span>
#### <a name="request"></a><span data-ttu-id="70150-175">请求</span><span class="sxs-lookup"><span data-stu-id="70150-175">Request</span></span>

<span data-ttu-id="70150-176">第三个示例介绍如何使用 `Prefer: outlook.body-content-type="text"` 标头获取采用文本格式的指定消息的 **body** 和 **uniqueBody**。</span><span class="sxs-lookup"><span data-stu-id="70150-176">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** of the specified message in text format.</span></span>


# <a name="http"></a>[<span data-ttu-id="70150-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="70150-177">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message_in_text"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGI1AAAoZCfHAAA=/?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```
# <a name="c"></a>[<span data-ttu-id="70150-178">C#</span><span class="sxs-lookup"><span data-stu-id="70150-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="70150-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70150-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="70150-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70150-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="70150-181">Java</span><span class="sxs-lookup"><span data-stu-id="70150-181">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-in-text-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="70150-182">响应</span><span class="sxs-lookup"><span data-stu-id="70150-182">Response</span></span>

<span data-ttu-id="70150-183">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="70150-183">Here is an example of the response.</span></span> <span data-ttu-id="70150-184">注意：响应包含用于确认 `Prefer: outlook.body-content-type` 请求标头的 `Preference-Applied: outlook.body-content-type` 标头。</span><span class="sxs-lookup"><span data-stu-id="70150-184">Note: The response includes a `Preference-Applied: outlook.body-content-type` header to acknowledge the `Prefer: outlook.body-content-type` request header.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/messages(subject,body,bodyPreview,uniqueBody)/$entity",
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

### <a name="example-4-get-mime-content"></a><span data-ttu-id="70150-185">示例 4：获取 MIME 内容</span><span class="sxs-lookup"><span data-stu-id="70150-185">Example 4: Get MIME content</span></span>
#### <a name="request"></a><span data-ttu-id="70150-186">请求</span><span class="sxs-lookup"><span data-stu-id="70150-186">Request</span></span>
<span data-ttu-id="70150-187">第 4 个示例获取已登录用户的邮箱中邮件的 MIME 内容。</span><span class="sxs-lookup"><span data-stu-id="70150-187">The fourth example gets the MIME content of a message in the signed-in user's mailbox.</span></span>


# <a name="http"></a>[<span data-ttu-id="70150-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="70150-188">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_message_in_mime",
  "sampleKeys": ["4aade2547798441eab5188a7a2436bc1"]
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/4aade2547798441eab5188a7a2436bc1/$value
```
# <a name="c"></a>[<span data-ttu-id="70150-189">C#</span><span class="sxs-lookup"><span data-stu-id="70150-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-in-mime-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="70150-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70150-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-in-mime-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="70150-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70150-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-in-mime-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="70150-192">Java</span><span class="sxs-lookup"><span data-stu-id="70150-192">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-in-mime-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="70150-193">响应</span><span class="sxs-lookup"><span data-stu-id="70150-193">Response</span></span>
<span data-ttu-id="70150-194">以下是答复。</span><span class="sxs-lookup"><span data-stu-id="70150-194">The following is the response.</span></span> <span data-ttu-id="70150-195">MIME 内容以 `MIME-Version` 标头开头。</span><span class="sxs-lookup"><span data-stu-id="70150-195">The MIME content begins with the `MIME-Version` header.</span></span> 

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


## <a name="see-also"></a><span data-ttu-id="70150-196">另请参阅</span><span class="sxs-lookup"><span data-stu-id="70150-196">See also</span></span>

- [<span data-ttu-id="70150-197">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="70150-197">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="70150-198">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="70150-198">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
