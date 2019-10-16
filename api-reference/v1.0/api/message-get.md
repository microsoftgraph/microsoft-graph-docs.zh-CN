---
title: 获取邮件
description: 检索邮件对象的属性和关系。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3dfb0f3d7f6d30bb04b635330a3ceca68b6df9f0
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538831"
---
# <a name="get-message"></a><span data-ttu-id="41c38-103">获取邮件</span><span class="sxs-lookup"><span data-stu-id="41c38-103">Get message</span></span>

<span data-ttu-id="41c38-104">检索[邮件](../resources/message.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="41c38-104">Retrieve the properties and relationships of a [message](../resources/message.md) object.</span></span>

<span data-ttu-id="41c38-105">可使用 `$value` 参数来[获取邮件的 MIME 内容](/graph/outlook-get-mime-message)。</span><span class="sxs-lookup"><span data-stu-id="41c38-105">You can now use a  segment to get the MIME content of an Outlook message.</span></span>

<span data-ttu-id="41c38-106">在以下两种情况下，应用可以获取其他用户的邮件文件夹中的邮件：</span><span class="sxs-lookup"><span data-stu-id="41c38-106">There are two scenarios where an app can get a message in another user's mail folder:</span></span>

* <span data-ttu-id="41c38-107">如果该应用具有应用程序权限，或者</span><span class="sxs-lookup"><span data-stu-id="41c38-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="41c38-108">如果应用具有来自某个用户的相应委派[权限](#permissions)，而另一个用户与该用户共享了邮件文件夹，或者已为该用户授予委派的访问权限。</span><span class="sxs-lookup"><span data-stu-id="41c38-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="41c38-109">请参阅[详细信息和示例](/graph/outlook-share-messages-folders)。</span><span class="sxs-lookup"><span data-stu-id="41c38-109">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

<span data-ttu-id="41c38-110">由于**邮件**资源支持[扩展](/graph/extensibility-overview)，因此也可使用 `GET` 操作获取**邮件**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="41c38-110">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>


## <a name="permissions"></a><span data-ttu-id="41c38-111">权限</span><span class="sxs-lookup"><span data-stu-id="41c38-111">Permissions</span></span>
<span data-ttu-id="41c38-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="41c38-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41c38-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="41c38-114">Permission type</span></span>      | <span data-ttu-id="41c38-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="41c38-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41c38-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="41c38-116">Delegated (work or school account)</span></span> | <span data-ttu-id="41c38-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="41c38-117">Mail.Read</span></span>    |
|<span data-ttu-id="41c38-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="41c38-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41c38-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="41c38-119">Mail.Read</span></span>    |
|<span data-ttu-id="41c38-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="41c38-120">Application</span></span> | <span data-ttu-id="41c38-121">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="41c38-121">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="41c38-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="41c38-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="41c38-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="41c38-123">Optional query parameters</span></span>
<span data-ttu-id="41c38-124">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="41c38-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="41c38-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="41c38-125">Request headers</span></span>
| <span data-ttu-id="41c38-126">名称</span><span class="sxs-lookup"><span data-stu-id="41c38-126">Name</span></span>       | <span data-ttu-id="41c38-127">类型</span><span class="sxs-lookup"><span data-stu-id="41c38-127">Type</span></span> | <span data-ttu-id="41c38-128">说明</span><span class="sxs-lookup"><span data-stu-id="41c38-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="41c38-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="41c38-129">Authorization</span></span>  | <span data-ttu-id="41c38-130">string</span><span class="sxs-lookup"><span data-stu-id="41c38-130">string</span></span>  | <span data-ttu-id="41c38-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="41c38-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="41c38-133">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="41c38-133">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="41c38-134">string</span><span class="sxs-lookup"><span data-stu-id="41c38-134">string</span></span> | <span data-ttu-id="41c38-135">要返回的 **body** 和 **uniqueBody** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="41c38-135">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="41c38-136">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="41c38-136">Values can be "text" or "html".</span></span> <span data-ttu-id="41c38-137">如果指定此 `Preference-Applied` 头，返回 `Prefer` 头作为证明。</span><span class="sxs-lookup"><span data-stu-id="41c38-137">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="41c38-138">如果未指定此头，采用 HTML 格式返回 **body** 和 **uniqueBody** 属性。</span><span class="sxs-lookup"><span data-stu-id="41c38-138">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="41c38-139">可选。</span><span class="sxs-lookup"><span data-stu-id="41c38-139">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="41c38-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="41c38-140">Request body</span></span>
<span data-ttu-id="41c38-141">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="41c38-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41c38-142">响应</span><span class="sxs-lookup"><span data-stu-id="41c38-142">Response</span></span>

<span data-ttu-id="41c38-143">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="41c38-143">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>


## <a name="examples"></a><span data-ttu-id="41c38-144">示例</span><span class="sxs-lookup"><span data-stu-id="41c38-144">Examples</span></span>
### <a name="example-1"></a><span data-ttu-id="41c38-145">示例 1</span><span class="sxs-lookup"><span data-stu-id="41c38-145">Example 1</span></span>
#### <a name="request"></a><span data-ttu-id="41c38-146">请求</span><span class="sxs-lookup"><span data-stu-id="41c38-146">Request</span></span>
<span data-ttu-id="41c38-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="41c38-147">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="41c38-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="41c38-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhMGAAA="],
  "name": "get_message"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhMGAAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="41c38-149">C#</span><span class="sxs-lookup"><span data-stu-id="41c38-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="41c38-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41c38-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="41c38-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41c38-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="41c38-152">Java</span><span class="sxs-lookup"><span data-stu-id="41c38-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="41c38-153">响应</span><span class="sxs-lookup"><span data-stu-id="41c38-153">Response</span></span>
<span data-ttu-id="41c38-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="41c38-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-2"></a><span data-ttu-id="41c38-157">示例 2</span><span class="sxs-lookup"><span data-stu-id="41c38-157">Example 2</span></span>
#### <a name="request"></a><span data-ttu-id="41c38-158">请求</span><span class="sxs-lookup"><span data-stu-id="41c38-158">Request</span></span>
<span data-ttu-id="41c38-159">下一个示例使用 `$select` 查询参数获取邮件的 Internet 邮件标头。</span><span class="sxs-lookup"><span data-stu-id="41c38-159">The next example uses a `$select` query parameter to get the Internet message headers of a message.</span></span> 

# <a name="httptabhttp"></a>[<span data-ttu-id="41c38-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="41c38-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAAW-VPeAAA="],
  "name": "get_message_headers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhAAAW-VPeAAA=/?$select=internetMessageHeaders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="41c38-161">C#</span><span class="sxs-lookup"><span data-stu-id="41c38-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="41c38-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41c38-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="41c38-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41c38-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="41c38-164">Java</span><span class="sxs-lookup"><span data-stu-id="41c38-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-headers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="41c38-165">响应</span><span class="sxs-lookup"><span data-stu-id="41c38-165">Response</span></span>
<span data-ttu-id="41c38-166">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="41c38-166">Here is an example of the response.</span></span> <span data-ttu-id="41c38-167">注意：为简洁起见，将截断响应对象中的邮件标头集。</span><span class="sxs-lookup"><span data-stu-id="41c38-167">Note: The set of message headers in the response object is truncated for brevity.</span></span> <span data-ttu-id="41c38-168">所有标头都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="41c38-168">All of the headers will be returned from an actual call.</span></span>
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

### <a name="example-3"></a><span data-ttu-id="41c38-169">示例 3</span><span class="sxs-lookup"><span data-stu-id="41c38-169">Example 3</span></span>
#### <a name="request"></a><span data-ttu-id="41c38-170">请求</span><span class="sxs-lookup"><span data-stu-id="41c38-170">Request</span></span>

<span data-ttu-id="41c38-171">第三个示例介绍如何使用 `Prefer: outlook.body-content-type="text"` 标头获取采用文本格式的指定消息的 **body** 和 **uniqueBody**。</span><span class="sxs-lookup"><span data-stu-id="41c38-171">The second example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** property of the specified message in text format.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="41c38-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="41c38-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message_in_text"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGI1AAAoZCfHAAA=/?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="41c38-173">C#</span><span class="sxs-lookup"><span data-stu-id="41c38-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="41c38-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41c38-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="41c38-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41c38-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="41c38-176">Java</span><span class="sxs-lookup"><span data-stu-id="41c38-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-in-text-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="41c38-177">响应</span><span class="sxs-lookup"><span data-stu-id="41c38-177">Response</span></span>

<span data-ttu-id="41c38-178">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="41c38-178">Here is an example of the response.</span></span> <span data-ttu-id="41c38-179">注意：响应包含用于确认 `Prefer: outlook.body-content-type` 请求标头的 `Preference-Applied: outlook.body-content-type` 标头。</span><span class="sxs-lookup"><span data-stu-id="41c38-179">Note: The response includes a `Preference-Applied: outlook.body-content-type` header to acknowledge the `Prefer: outlook.body-content-type` request header.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="41c38-180">另请参阅</span><span class="sxs-lookup"><span data-stu-id="41c38-180">See also</span></span>

- [<span data-ttu-id="41c38-181">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="41c38-181">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="41c38-182">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="41c38-182">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
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
