---
title: 获取邮件
description: 检索邮件对象的属性和关系。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: d45342572122a256e314d7305111c3e480c48d47
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275045"
---
# <a name="get-message"></a><span data-ttu-id="6fb6d-103">获取邮件</span><span class="sxs-lookup"><span data-stu-id="6fb6d-103">Get message</span></span>

<span data-ttu-id="6fb6d-104">检索[邮件](../resources/message.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6fb6d-104">Retrieve the properties and relationships of a [message](../resources/message.md) object.</span></span>

<span data-ttu-id="6fb6d-105">目前，此操作返回纯 HTML 格式的邮件正文。</span><span class="sxs-lookup"><span data-stu-id="6fb6d-105">Currently, this operation returns message bodies in only HTML format.</span></span>

<span data-ttu-id="6fb6d-106">在以下两种情况下，应用可以获取其他用户的邮件文件夹中的邮件：</span><span class="sxs-lookup"><span data-stu-id="6fb6d-106">There are two scenarios where an app can get a message in another user's mail folder:</span></span>

* <span data-ttu-id="6fb6d-107">如果该应用具有应用程序权限，或者</span><span class="sxs-lookup"><span data-stu-id="6fb6d-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="6fb6d-108">如果应用具有来自某个用户的相应委派[权限](#permissions)，而另一个用户与该用户共享了邮件文件夹，或者已为该用户授予委派的访问权限。</span><span class="sxs-lookup"><span data-stu-id="6fb6d-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="6fb6d-109">请参阅[详细信息和示例](/graph/outlook-share-messages-folders)。</span><span class="sxs-lookup"><span data-stu-id="6fb6d-109">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

<span data-ttu-id="6fb6d-110">由于**邮件**资源支持[扩展](/graph/extensibility-overview)，因此也可使用 `GET` 操作获取**邮件**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="6fb6d-110">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>


## <a name="permissions"></a><span data-ttu-id="6fb6d-111">权限</span><span class="sxs-lookup"><span data-stu-id="6fb6d-111">Permissions</span></span>
<span data-ttu-id="6fb6d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6fb6d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fb6d-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="6fb6d-114">Permission type</span></span>      | <span data-ttu-id="6fb6d-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6fb6d-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6fb6d-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6fb6d-116">Delegated (work or school account)</span></span> | <span data-ttu-id="6fb6d-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6fb6d-117">Mail.Read</span></span>    |
|<span data-ttu-id="6fb6d-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6fb6d-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fb6d-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6fb6d-119">Mail.Read</span></span>    |
|<span data-ttu-id="6fb6d-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="6fb6d-120">Application</span></span> | <span data-ttu-id="6fb6d-121">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6fb6d-121">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="6fb6d-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6fb6d-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6fb6d-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6fb6d-123">Optional query parameters</span></span>
<span data-ttu-id="6fb6d-124">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6fb6d-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6fb6d-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="6fb6d-125">Request headers</span></span>
| <span data-ttu-id="6fb6d-126">名称</span><span class="sxs-lookup"><span data-stu-id="6fb6d-126">Name</span></span>       | <span data-ttu-id="6fb6d-127">类型</span><span class="sxs-lookup"><span data-stu-id="6fb6d-127">Type</span></span> | <span data-ttu-id="6fb6d-128">说明</span><span class="sxs-lookup"><span data-stu-id="6fb6d-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6fb6d-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="6fb6d-129">Authorization</span></span>  | <span data-ttu-id="6fb6d-130">string</span><span class="sxs-lookup"><span data-stu-id="6fb6d-130">string</span></span>  | <span data-ttu-id="6fb6d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6fb6d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6fb6d-133">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="6fb6d-133">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="6fb6d-134">string</span><span class="sxs-lookup"><span data-stu-id="6fb6d-134">string</span></span> | <span data-ttu-id="6fb6d-135">要返回的 **body** 和 **uniqueBody** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="6fb6d-135">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="6fb6d-136">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="6fb6d-136">Values can be "text" or "html".</span></span> <span data-ttu-id="6fb6d-137">如果指定此 `Preference-Applied` 头，返回 `Prefer` 头作为证明。</span><span class="sxs-lookup"><span data-stu-id="6fb6d-137">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="6fb6d-138">如果未指定此头，采用 HTML 格式返回 **body** 和 **uniqueBody** 属性。</span><span class="sxs-lookup"><span data-stu-id="6fb6d-138">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="6fb6d-139">可选。</span><span class="sxs-lookup"><span data-stu-id="6fb6d-139">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6fb6d-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="6fb6d-140">Request body</span></span>
<span data-ttu-id="6fb6d-141">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6fb6d-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6fb6d-142">响应</span><span class="sxs-lookup"><span data-stu-id="6fb6d-142">Response</span></span>

<span data-ttu-id="6fb6d-143">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6fb6d-143">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6fb6d-144">示例</span><span class="sxs-lookup"><span data-stu-id="6fb6d-144">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="6fb6d-145">请求 1</span><span class="sxs-lookup"><span data-stu-id="6fb6d-145">Request 1</span></span>
<span data-ttu-id="6fb6d-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6fb6d-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhMGAAA="],
  "name": "get_message"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhMGAAA=
```
##### <a name="response-1"></a><span data-ttu-id="6fb6d-147">响应 1</span><span class="sxs-lookup"><span data-stu-id="6fb6d-147">Response 1</span></span>
<span data-ttu-id="6fb6d-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6fb6d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="6fb6d-151">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="6fb6d-151">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6fb6d-152">C#</span><span class="sxs-lookup"><span data-stu-id="6fb6d-152">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_message-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6fb6d-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="6fb6d-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_message-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6fb6d-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6fb6d-154">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_message-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-2"></a><span data-ttu-id="6fb6d-155">请求 2</span><span class="sxs-lookup"><span data-stu-id="6fb6d-155">Request 2</span></span>
<span data-ttu-id="6fb6d-156">下一个示例使用 `$select` 查询参数获取邮件的 Internet 邮件标头。</span><span class="sxs-lookup"><span data-stu-id="6fb6d-156">The next example uses a `$select` query parameter to get the Internet message headers of a message.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAAW-VPeAAA="],
  "name": "get_message_headers"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhAAAW-VPeAAA=/?$select=internetMessageHeaders
```
##### <a name="response-2"></a><span data-ttu-id="6fb6d-157">响应 2</span><span class="sxs-lookup"><span data-stu-id="6fb6d-157">Response 2</span></span>
<span data-ttu-id="6fb6d-158">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6fb6d-158">Here is an example of the response.</span></span> <span data-ttu-id="6fb6d-159">注意：为简洁起见，将截断响应对象中的邮件标头集。</span><span class="sxs-lookup"><span data-stu-id="6fb6d-159">Note: The set of message headers in the response object is truncated for brevity.</span></span> <span data-ttu-id="6fb6d-160">所有标头都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6fb6d-160">All of the headers will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="6fb6d-161">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="6fb6d-161">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6fb6d-162">C#</span><span class="sxs-lookup"><span data-stu-id="6fb6d-162">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_message_headers-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6fb6d-163">Javascript</span><span class="sxs-lookup"><span data-stu-id="6fb6d-163">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_message_headers-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6fb6d-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6fb6d-164">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_message_headers-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


## <a name="see-also"></a><span data-ttu-id="6fb6d-165">另请参阅</span><span class="sxs-lookup"><span data-stu-id="6fb6d-165">See also</span></span>

- [<span data-ttu-id="6fb6d-166">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="6fb6d-166">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="6fb6d-167">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="6fb6d-167">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
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
    "Error: /api-reference/v1.0/api/message-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/message-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/message-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/message-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/message-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
