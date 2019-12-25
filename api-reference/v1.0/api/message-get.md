---
title: 获取邮件
description: 检索邮件对象的属性和关系。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ab57e15b88cef2ba1749c19a1b00d3521136f274
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865564"
---
# <a name="get-message"></a><span data-ttu-id="7a4e3-103">获取邮件</span><span class="sxs-lookup"><span data-stu-id="7a4e3-103">Get message</span></span>

<span data-ttu-id="7a4e3-104">检索[邮件](../resources/message.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7a4e3-104">Retrieve the properties and relationships of a [message](../resources/message.md) object.</span></span>

<span data-ttu-id="7a4e3-105">可使用 `$value` 参数来[获取邮件的 MIME 内容](/graph/outlook-get-mime-message)。</span><span class="sxs-lookup"><span data-stu-id="7a4e3-105">You can use the `$value` parameter to [get the MIME content of a message](/graph/outlook-get-mime-message).</span></span>

<span data-ttu-id="7a4e3-106">在以下两种情况下，应用可以获取其他用户的邮件文件夹中的邮件：</span><span class="sxs-lookup"><span data-stu-id="7a4e3-106">There are two scenarios where an app can get a message in another user's mail folder:</span></span>

* <span data-ttu-id="7a4e3-107">如果该应用具有应用程序权限，或者</span><span class="sxs-lookup"><span data-stu-id="7a4e3-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="7a4e3-108">如果应用具有来自某个用户的相应委派[权限](#permissions)，而另一个用户与该用户共享了邮件文件夹，或者已为该用户授予委派的访问权限。</span><span class="sxs-lookup"><span data-stu-id="7a4e3-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="7a4e3-109">请参阅[详细信息和示例](/graph/outlook-share-messages-folders)。</span><span class="sxs-lookup"><span data-stu-id="7a4e3-109">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

<span data-ttu-id="7a4e3-110">由于**邮件**资源支持[扩展](/graph/extensibility-overview)，因此也可使用 `GET` 操作获取**邮件**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="7a4e3-110">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>


## <a name="permissions"></a><span data-ttu-id="7a4e3-111">权限</span><span class="sxs-lookup"><span data-stu-id="7a4e3-111">Permissions</span></span>
<span data-ttu-id="7a4e3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7a4e3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a4e3-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="7a4e3-114">Permission type</span></span>      | <span data-ttu-id="7a4e3-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7a4e3-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a4e3-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7a4e3-116">Delegated (work or school account)</span></span> | <span data-ttu-id="7a4e3-117">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="7a4e3-117">Mail.ReadBasic, Mail.Read</span></span>    |
|<span data-ttu-id="7a4e3-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7a4e3-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a4e3-119">Mail.ReadBasic、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="7a4e3-119">Mail.ReadBasic, Mail.Read</span></span>    |
|<span data-ttu-id="7a4e3-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="7a4e3-120">Application</span></span> | <span data-ttu-id="7a4e3-121">Mail.ReadBasic.All、Mail.Read</span><span class="sxs-lookup"><span data-stu-id="7a4e3-121">Mail.ReadBasic.All, Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a4e3-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7a4e3-122">HTTP request</span></span>

<span data-ttu-id="7a4e3-123">要获取指定的邮件：</span><span class="sxs-lookup"><span data-stu-id="7a4e3-123">To get the specified message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="7a4e3-124">要获取指定邮件的 MIME 内容：</span><span class="sxs-lookup"><span data-stu-id="7a4e3-124">To get the MIME content of the specified message:</span></span>
<!-- { "blockType": "ignored" } --> 
```http 
GET /me/messages/{id}/$value 
GET /users/{id | userPrincipalName}/messages/{id}/$value 
GET /me/mailFolders/{id}/messages/{id}/$value 
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/$value 
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7a4e3-125">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7a4e3-125">Optional query parameters</span></span>
<span data-ttu-id="7a4e3-126">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7a4e3-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="7a4e3-127">使用 `$value` 参数获取邮件的 MIME 内容。</span><span class="sxs-lookup"><span data-stu-id="7a4e3-127">You can use the  parameter to get the MIME content of a message.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7a4e3-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="7a4e3-128">Request headers</span></span>
| <span data-ttu-id="7a4e3-129">名称</span><span class="sxs-lookup"><span data-stu-id="7a4e3-129">Name</span></span>       | <span data-ttu-id="7a4e3-130">类型</span><span class="sxs-lookup"><span data-stu-id="7a4e3-130">Type</span></span> | <span data-ttu-id="7a4e3-131">说明</span><span class="sxs-lookup"><span data-stu-id="7a4e3-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7a4e3-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a4e3-132">Authorization</span></span>  | <span data-ttu-id="7a4e3-133">string</span><span class="sxs-lookup"><span data-stu-id="7a4e3-133">string</span></span>  | <span data-ttu-id="7a4e3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7a4e3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7a4e3-136">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="7a4e3-136">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="7a4e3-137">string</span><span class="sxs-lookup"><span data-stu-id="7a4e3-137">string</span></span> | <span data-ttu-id="7a4e3-138">要返回的 **body** 和 **uniqueBody** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="7a4e3-138">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="7a4e3-139">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="7a4e3-139">Values can be "text" or "html".</span></span> <span data-ttu-id="7a4e3-140">如果指定此 `Preference-Applied` 头，返回 `Prefer` 头作为证明。</span><span class="sxs-lookup"><span data-stu-id="7a4e3-140">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="7a4e3-141">如果未指定此头，采用 HTML 格式返回 **body** 和 **uniqueBody** 属性。</span><span class="sxs-lookup"><span data-stu-id="7a4e3-141">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="7a4e3-142">可选。</span><span class="sxs-lookup"><span data-stu-id="7a4e3-142">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7a4e3-143">请求正文</span><span class="sxs-lookup"><span data-stu-id="7a4e3-143">Request body</span></span>
<span data-ttu-id="7a4e3-144">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7a4e3-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a4e3-145">响应</span><span class="sxs-lookup"><span data-stu-id="7a4e3-145">Response</span></span>

<span data-ttu-id="7a4e3-146">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7a4e3-146">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>

<span data-ttu-id="7a4e3-147">如果指定 `$value` 参数，则返回 MIME 格式的邮件内容，而不是**邮件**资源。</span><span class="sxs-lookup"><span data-stu-id="7a4e3-147">Specifying the `$value` parameter returns the message content in MIME format, and not a **message** resource.</span></span>


## <a name="examples"></a><span data-ttu-id="7a4e3-148">示例</span><span class="sxs-lookup"><span data-stu-id="7a4e3-148">Examples</span></span>
### <a name="example-1"></a><span data-ttu-id="7a4e3-149">示例 1</span><span class="sxs-lookup"><span data-stu-id="7a4e3-149">Example 1</span></span>
#### <a name="request"></a><span data-ttu-id="7a4e3-150">请求</span><span class="sxs-lookup"><span data-stu-id="7a4e3-150">Request</span></span>
<span data-ttu-id="7a4e3-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7a4e3-151">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7a4e3-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a4e3-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhMGAAA="],
  "name": "get_message"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhMGAAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7a4e3-153">C#</span><span class="sxs-lookup"><span data-stu-id="7a4e3-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7a4e3-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a4e3-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7a4e3-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7a4e3-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7a4e3-156">Java</span><span class="sxs-lookup"><span data-stu-id="7a4e3-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="7a4e3-157">响应</span><span class="sxs-lookup"><span data-stu-id="7a4e3-157">Response</span></span>
<span data-ttu-id="7a4e3-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7a4e3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
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

### <a name="example-2"></a><span data-ttu-id="7a4e3-161">示例 2</span><span class="sxs-lookup"><span data-stu-id="7a4e3-161">Example 2</span></span>
#### <a name="request"></a><span data-ttu-id="7a4e3-162">请求</span><span class="sxs-lookup"><span data-stu-id="7a4e3-162">Request</span></span>
<span data-ttu-id="7a4e3-163">下一个示例使用 `$select` 查询参数获取邮件的 Internet 邮件标头。</span><span class="sxs-lookup"><span data-stu-id="7a4e3-163">The next example uses a `$select` query parameter to get the Internet message headers of a message.</span></span> 

# <a name="httptabhttp"></a>[<span data-ttu-id="7a4e3-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a4e3-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAAW-VPeAAA="],
  "name": "get_message_headers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhAAAW-VPeAAA=/?$select=internetMessageHeaders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7a4e3-165">C#</span><span class="sxs-lookup"><span data-stu-id="7a4e3-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7a4e3-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a4e3-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7a4e3-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7a4e3-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7a4e3-168">Java</span><span class="sxs-lookup"><span data-stu-id="7a4e3-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-headers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="7a4e3-169">响应</span><span class="sxs-lookup"><span data-stu-id="7a4e3-169">Response</span></span>
<span data-ttu-id="7a4e3-170">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7a4e3-170">Here is an example of the response.</span></span> <span data-ttu-id="7a4e3-171">注意：为简洁起见，将截断响应对象中的邮件标头集。</span><span class="sxs-lookup"><span data-stu-id="7a4e3-171">Note: The set of message headers in the response object is truncated for brevity.</span></span> <span data-ttu-id="7a4e3-172">所有标头都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7a4e3-172">All of the headers will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
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

### <a name="example-3"></a><span data-ttu-id="7a4e3-173">示例 3</span><span class="sxs-lookup"><span data-stu-id="7a4e3-173">Example 3</span></span>
#### <a name="request"></a><span data-ttu-id="7a4e3-174">请求</span><span class="sxs-lookup"><span data-stu-id="7a4e3-174">Request</span></span>

<span data-ttu-id="7a4e3-175">第三个示例介绍如何使用 `Prefer: outlook.body-content-type="text"` 标头获取采用文本格式的指定消息的 **body** 和 **uniqueBody**。</span><span class="sxs-lookup"><span data-stu-id="7a4e3-175">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** of the specified message in text format.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7a4e3-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a4e3-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message_in_text"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGI1AAAoZCfHAAA=/?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7a4e3-177">C#</span><span class="sxs-lookup"><span data-stu-id="7a4e3-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7a4e3-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a4e3-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7a4e3-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7a4e3-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7a4e3-180">Java</span><span class="sxs-lookup"><span data-stu-id="7a4e3-180">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-in-text-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7a4e3-181">响应</span><span class="sxs-lookup"><span data-stu-id="7a4e3-181">Response</span></span>

<span data-ttu-id="7a4e3-182">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7a4e3-182">Here is an example of the response.</span></span> <span data-ttu-id="7a4e3-183">注意：响应包含用于确认 `Prefer: outlook.body-content-type` 请求标头的 `Preference-Applied: outlook.body-content-type` 标头。</span><span class="sxs-lookup"><span data-stu-id="7a4e3-183">Note: The response includes a `Preference-Applied: outlook.body-content-type` header to acknowledge the `Prefer: outlook.body-content-type` request header.</span></span>
<!-- {
  "blockType": "response",
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

### <a name="example-4"></a><span data-ttu-id="7a4e3-184">示例 4</span><span class="sxs-lookup"><span data-stu-id="7a4e3-184">Example 4</span></span>
#### <a name="request"></a><span data-ttu-id="7a4e3-185">请求</span><span class="sxs-lookup"><span data-stu-id="7a4e3-185">Request</span></span>
<span data-ttu-id="7a4e3-186">第 4 个示例获取已登录用户的邮箱中邮件的 MIME 内容。</span><span class="sxs-lookup"><span data-stu-id="7a4e3-186">The fourth example gets the MIME content of a message in the signed-in user's mailbox.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/4aade2547798441eab5188a7a2436bc1/$value
```

#### <a name="response"></a><span data-ttu-id="7a4e3-187">响应</span><span class="sxs-lookup"><span data-stu-id="7a4e3-187">Response</span></span>
<span data-ttu-id="7a4e3-188">以下是答复。</span><span class="sxs-lookup"><span data-stu-id="7a4e3-188">The following is the response.</span></span> <span data-ttu-id="7a4e3-189">MIME 内容以 `MIME-Version` 标头开头。</span><span class="sxs-lookup"><span data-stu-id="7a4e3-189">The MIME content begins with the `MIME-Version` header.</span></span> 
<!-- {
  "blockType": "ignored"
} -->
```http
HTTP/1.1 200 OK

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
x-ms-publictraffictype: Emai

```http
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


## <a name="see-also"></a><span data-ttu-id="7a4e3-190">另请参阅</span><span class="sxs-lookup"><span data-stu-id="7a4e3-190">See also</span></span>

- [<span data-ttu-id="7a4e3-191">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="7a4e3-191">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="7a4e3-192">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="7a4e3-192">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
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
